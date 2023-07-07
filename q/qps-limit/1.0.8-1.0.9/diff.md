# Comparing `tmp/qps_limit-1.0.8-py3-none-any.whl.zip` & `tmp/qps_limit-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5357 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jul-04 08:29 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     5742 b- defN 23-Jul-04 08:28 qps_limit/limiter.py
--rw-rw-r--  2.0 unx     5474 b- defN 23-Jul-04 04:55 qps_limit/run.py
--rw-rw-r--  2.0 unx     2552 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-04 08:29 qps_limit-1.0.8.dist-info/RECORD
-8 files, 14657 bytes uncompressed, 4273 bytes compressed:  70.8%
+Zip file size: 5418 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jul-07 07:33 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     5918 b- defN 23-Jul-07 07:34 qps_limit/limiter.py
+-rw-rw-r--  2.0 unx     5474 b- defN 23-Jul-07 07:33 qps_limit/run.py
+-rw-rw-r--  2.0 unx     2565 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/RECORD
+8 files, 14846 bytes uncompressed, 4334 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.8.dist-info/METADATA
+Filename: qps_limit-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.8.dist-info/WHEEL
+Filename: qps_limit-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.8.dist-info/top_level.txt
+Filename: qps_limit-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.8.dist-info/zip-safe
+Filename: qps_limit-1.0.9.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.0.8.dist-info/RECORD
+Filename: qps_limit-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,10 +1,10 @@
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 
-from .run import batch_run, async_batch_run
 from .limiter import Limiter
+from .run import async_batch_run, batch_run
 
 __all__ = [
     'batch_run',
     'async_batch_run',
     'Limiter'
 ]
```

## qps_limit/limiter.py

```diff
@@ -62,40 +62,45 @@
             max_coroutines=1
         )
         warmup_end_time = time.time()
         avg_worker_time = (warmup_end_time - warmup_start_time) / warmup_steps
         if self.worker_max_qps is None:
             self.max_coroutines = max_coroutines
         else:
-            self.max_coroutines = min(max_coroutines, self.worker_max_qps * math.ceil(avg_worker_time))
+            self.max_coroutines = min(max_coroutines, math.ceil(self.worker_max_qps * math.ceil(avg_worker_time)))
         if self.verbose:
             self.logger.info(
                 "avg worker time: {:.2f}s -> set coroutine num: {}".format(avg_worker_time, self.max_coroutines)
             )
 
         if self.ordered:
-            self.res_dict = multiprocessing.Manager().dict()
+            self.res_map = multiprocessing.Manager().dict()
         else:
             self.res_queue = multiprocessing.Queue()
 
         self.job_value = multiprocessing.Value('i', 0)
         self.worker_value = multiprocessing.Value('i', 0)
         self.worker_event = multiprocessing.Event()
         self.job_queue = multiprocessing.Queue()
 
+        self.run_time = multiprocessing.Value('d', 0)
+
         self.workers = []
         for mod in range(self.num_workers):
             self.workers.append(multiprocessing.Process(target=self._worker, args=(mod, )))
 
     def _progress_worker(self):
         progress_bar = tqdm(total=self.job_count, desc=self.func.__name__)
         progress_cnt = 0
         while progress_cnt < self.job_count:
             progress_bar.update(self.job_queue.get())
             progress_cnt += 1
+        progress_bar.close()
+        with self.run_time.get_lock():
+            self.run_time.value = progress_bar.last_print_t - progress_bar.start_t
 
     def _worker(self, mod: int):
         def make_worker_iterator():
             for idx, (args, kwargs) in enumerate(self.params()):
                 if idx % self.num_workers == mod:
                     yield args, kwargs
 
@@ -109,56 +114,54 @@
             job_queue=self.job_queue,
             job_value=self.job_value,
             worker_value=self.worker_value,
             worker_event=self.worker_event
         ):
             real_idx = idx * self.num_workers + mod
             if self.ordered:
-                self.res_dict[real_idx] = res
+                self.res_map[real_idx] = res
             else:
                 self.res_queue.put((real_idx, res))
 
     def __call__(self):
-        start_time = time.time()
         for worker in self.workers:
             worker.start()
 
-        if self.verbose:
-            data_bar = tqdm(desc='data')
+        data_bar = tqdm(desc='data', disable=not self.verbose)
         while True:
-            if self.verbose:
-                data_bar.update(self.job_value.value - data_bar.n)
+            data_bar.update(self.job_value.value - data_bar.n)
             if self.worker_value.value == self.num_workers:
                 break
+        data_bar.close()
         if self.verbose:
-            data_bar.close()
             self.logger.info(
                 "receive {} data from {} worker nodes".format(self.job_value.value, self.worker_value.value)
             )
 
         self.job_count = self.job_value.value
         progress_worker = multiprocessing.Process(target=self._progress_worker)
         progress_worker.start()
         self.worker_event.set()
 
         job_done = 0
         while job_done < self.job_count:
             if self.ordered:
-                while job_done not in self.res_dict:
+                while job_done not in self.res_map:
                     pass
-                yield (job_done, self.res_dict[job_done])
-                del self.res_dict[job_done]
+                yield (job_done, self.res_map[job_done])
+                del self.res_map[job_done]
             else:
                 yield self.res_queue.get()
             job_done += 1
         assert job_done == self.job_count
 
         for worker in self.workers:
             worker.join()
         progress_worker.join()
-        end_time = time.time()
+
         if self.verbose:
-            self.logger.info('elapsed time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
-                end_time - start_time,
-                self.job_count / (end_time - start_time),
+            self.logger.info('data time: {:.2f}s run time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
+                data_bar.last_print_t - data_bar.start_t,
+                self.run_time.value,
+                self.job_count / self.run_time.value,
                 self.worker_max_qps * self.num_workers if self.worker_max_qps else float("inf"))
             )
```

## Comparing `qps_limit-1.0.8.dist-info/METADATA` & `qps_limit-1.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.8
+Version: 1.0.9
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -20,15 +20,15 @@
 Requires-Dist: tqdm
 Requires-Dist: aiolimiter
 
 ## QPS Limit
 
 Run functions under any limited rate using `multiprocessing` + `asyncio`
 
-Available on Unix (i.e. Linux, MacOS) only, as the default multiprocessing start method is `fork`.
+Available on Unix (i.e. Linux, MacOS) only, as the default multiprocessing start method is `fork`
 
 ### Installation
 
 ```bash
 pip install qps-limit
 ```
 
@@ -41,26 +41,26 @@
 ```
 
 ### Usage
 
 ```python
 from qps_limit import Limiter
 
-f = Limiter(
+Limiter(
     func="an asynchronous function",
     params="a generator function yields args and kwargs",
     callback="a callback function that handles the return values of func",
     num_workers="number of processes, recommended <= number of CPUs",
     worker_max_qps="maximum qps per process, None means unlimited",
     streaming="stream data processing, useful when the memory is limited",
-    ordered="return ordered results or not"
+    ordered="return ordered results or not, the default option is False"
 )
 ```
 
-BTW: The wrapped function returns a structure `(idx, res)` consisting of an index of the data and the function return value. If `ordered=False` is set, the order of the returned values may be randomized for better performance.
+BTW: The wrapped function returns tuples `(idx, res)` consisting of the data index and the function return value. If `ordered=False` is set, the order of the returned values may be randomized for better performance.
 
 ### Example
 
 > 10 workers, each with a maximum qps of 10, to calculate the function value of `(1+1/n)^n`
 
 > Assuming that `func` is a time-consuming function, it takes 1.0 seconds to execute
```

## Comparing `qps_limit-1.0.8.dist-info/RECORD` & `qps_limit-1.0.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-qps_limit/__init__.py,sha256=C8s-LOIrzYOUt9wOS2bhMGqYmDvUEnIQ11e6XSyWqg4,165
-qps_limit/limiter.py,sha256=d2JkuvHv6jcuZiasicHS9Y4ZrkhkxQIIa_ruJcfFAiA,5742
+qps_limit/__init__.py,sha256=TiIIyCKFqcgc79sHCD1V4PDjdlKO_23qgZFvVN_uv7E,165
+qps_limit/limiter.py,sha256=Zm8rYbPeGIyDL6qa9QO2Y6IjcHBE1iCRc-odVHmww3A,5918
 qps_limit/run.py,sha256=mqmPou-88VcnDqjg4dcjn5eYYyslJUGm79gblWnmVZQ,5474
-qps_limit-1.0.8.dist-info/METADATA,sha256=t29Lf6I9XfVIJHpCnxgLGdoq6pZAX7zy5dQYk6b9rmI,2552
-qps_limit-1.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-qps_limit-1.0.8.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
-qps_limit-1.0.8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-qps_limit-1.0.8.dist-info/RECORD,,
+qps_limit-1.0.9.dist-info/METADATA,sha256=5fG9ocsnjK2G4gJn_XEVu6tSAE7lJXCh0JDO-bcx5uw,2565
+qps_limit-1.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+qps_limit-1.0.9.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
+qps_limit-1.0.9.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+qps_limit-1.0.9.dist-info/RECORD,,
```


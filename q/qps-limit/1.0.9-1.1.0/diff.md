# Comparing `tmp/qps_limit-1.0.9-py3-none-any.whl.zip` & `tmp/qps_limit-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5418 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      165 b- defN 23-Jul-07 07:33 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     5918 b- defN 23-Jul-07 07:34 qps_limit/limiter.py
+Zip file size: 5613 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jul-07 09:35 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     6926 b- defN 23-Jul-07 09:35 qps_limit/limiter.py
 -rw-rw-r--  2.0 unx     5474 b- defN 23-Jul-07 07:33 qps_limit/run.py
--rw-rw-r--  2.0 unx     2565 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-07 07:35 qps_limit-1.0.9.dist-info/RECORD
-8 files, 14846 bytes uncompressed, 4334 bytes compressed:  70.8%
+-rw-rw-r--  2.0 unx     2565 b- defN 23-Jul-07 09:35 qps_limit-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 09:35 qps_limit-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-07 09:35 qps_limit-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-07 09:35 qps_limit-1.1.0.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jul-07 09:35 qps_limit-1.1.0.dist-info/RECORD
+8 files, 15854 bytes uncompressed, 4529 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: qps_limit/limiter.py
 Comment: 
 
 Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.9.dist-info/METADATA
+Filename: qps_limit-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.9.dist-info/WHEEL
+Filename: qps_limit-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.9.dist-info/top_level.txt
+Filename: qps_limit-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.9.dist-info/zip-safe
+Filename: qps_limit-1.1.0.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-1.0.9.dist-info/RECORD
+Filename: qps_limit-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.9'
+__version__ = '1.1.0'
 
 from .limiter import Limiter
 from .run import async_batch_run, batch_run
 
 __all__ = [
     'batch_run',
     'async_batch_run',
```

## qps_limit/limiter.py

```diff
@@ -1,8 +1,9 @@
 import itertools
+import json
 import logging
 import math
 import multiprocessing
 import time
 from typing import Any, Callable, Coroutine, Optional
 
 from tqdm import tqdm
@@ -46,87 +47,89 @@
         self.params = params
         self.callback = callback
         self.num_workers = num_workers
         self.worker_max_qps = worker_max_qps
         self.streaming = streaming
         self.ordered = ordered
         self.verbose = verbose
+        self.warmup_steps = warmup_steps
+        self.max_coroutines = max_coroutines
 
         if self.verbose:
-            self.logger.info("warmup worker nodes with {} data".format(warmup_steps))
-        warmup_param_iterator = itertools.islice(self.params(), warmup_steps)
+            self.logger.info("warmup worker nodes with {} data".format(self.warmup_steps))
+        warmup_param_iterator = itertools.islice(self.params(), self.warmup_steps)
         warmup_start_time = time.time()
         batch_run(
             func=self.func,
             params=warmup_param_iterator,
             max_qps=None,
             max_coroutines=1
         )
-        warmup_end_time = time.time()
-        avg_worker_time = (warmup_end_time - warmup_start_time) / warmup_steps
+        self.warmup_worker_time = (time.time() - warmup_start_time) / self.warmup_steps
         if self.worker_max_qps is None:
-            self.max_coroutines = max_coroutines
+            self.dynamic_coroutines = self.max_coroutines
         else:
-            self.max_coroutines = min(max_coroutines, math.ceil(self.worker_max_qps * math.ceil(avg_worker_time)))
+            self.dynamic_coroutines = math.ceil(self.worker_max_qps * math.ceil(self.warmup_worker_time))
+            self.dynamic_coroutines = min(self.max_coroutines, self.dynamic_coroutines)
         if self.verbose:
-            self.logger.info(
-                "avg worker time: {:.2f}s -> set coroutine num: {}".format(avg_worker_time, self.max_coroutines)
-            )
+            self.logger.info("warmup worker time: {:.2f}s -> set dynamic coroutine num: {}".format(
+                self.warmup_worker_time, self.dynamic_coroutines
+            ))
 
         if self.ordered:
             self.res_map = multiprocessing.Manager().dict()
         else:
             self.res_queue = multiprocessing.Queue()
 
         self.job_value = multiprocessing.Value('i', 0)
         self.worker_value = multiprocessing.Value('i', 0)
         self.worker_event = multiprocessing.Event()
         self.job_queue = multiprocessing.Queue()
-
-        self.run_time = multiprocessing.Value('d', 0)
+        self.worker_time = multiprocessing.Value('d', 0)
 
         self.workers = []
         for mod in range(self.num_workers):
             self.workers.append(multiprocessing.Process(target=self._worker, args=(mod, )))
 
     def _progress_worker(self):
         progress_bar = tqdm(total=self.job_count, desc=self.func.__name__)
         progress_cnt = 0
         while progress_cnt < self.job_count:
             progress_bar.update(self.job_queue.get())
             progress_cnt += 1
         progress_bar.close()
-        with self.run_time.get_lock():
-            self.run_time.value = progress_bar.last_print_t - progress_bar.start_t
+        with self.worker_time.get_lock():
+            self.worker_time.value = progress_bar.last_print_t - progress_bar.start_t
 
     def _worker(self, mod: int):
         def make_worker_iterator():
             for idx, (args, kwargs) in enumerate(self.params()):
                 if idx % self.num_workers == mod:
                     yield args, kwargs
 
         batch_run_func = batch_run if not self.streaming else streaming_batch_run
         for idx, res in batch_run_func(
             func=self.func,
             params=make_worker_iterator(),
             callback=self.callback,
             max_qps=self.worker_max_qps,
-            max_coroutines=self.max_coroutines,
+            max_coroutines=self.dynamic_coroutines,
             job_queue=self.job_queue,
             job_value=self.job_value,
             worker_value=self.worker_value,
             worker_event=self.worker_event
         ):
             real_idx = idx * self.num_workers + mod
             if self.ordered:
                 self.res_map[real_idx] = res
             else:
                 self.res_queue.put((real_idx, res))
 
     def __call__(self):
+        start_time = time.time()
         for worker in self.workers:
             worker.start()
 
         data_bar = tqdm(desc='data', disable=not self.verbose)
         while True:
             data_bar.update(self.job_value.value - data_bar.n)
             if self.worker_value.value == self.num_workers:
@@ -155,13 +158,28 @@
         assert job_done == self.job_count
 
         for worker in self.workers:
             worker.join()
         progress_worker.join()
 
         if self.verbose:
-            self.logger.info('data time: {:.2f}s run time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
-                data_bar.last_print_t - data_bar.start_t,
-                self.run_time.value,
-                self.job_count / self.run_time.value,
-                self.worker_max_qps * self.num_workers if self.worker_max_qps else float("inf"))
-            )
+            verbose_info = {}
+            verbose_info['limiter'] = {
+                'func_name': self.func.__name__,
+                'num_workers': self.num_workers,
+                'worker_max_qps': self.worker_max_qps,
+                'streaming': self.streaming,
+                'ordered': self.ordered,
+                'warmup_steps': self.warmup_steps,
+                'max_coroutines': self.max_coroutines,
+            }
+            verbose_info['runtime'] = {
+                'warmup_worker_time': self.warmup_worker_time,
+                'dynamic_coroutines': self.dynamic_coroutines,
+                'data_count': self.job_count,
+                'data_time': data_bar.last_print_t - data_bar.start_t,
+                'worker_time': self.worker_time.value,
+                'elapsed_time': time.time() - start_time,
+                'average_qps': self.job_count / self.worker_time.value if self.worker_time.value > 0 else float("inf"),
+                'expected_qps': self.worker_max_qps * self.num_workers if self.worker_max_qps else float("inf")
+            }
+            self.logger.info(json.dumps(verbose_info, indent=4))
```

## Comparing `qps_limit-1.0.9.dist-info/METADATA` & `qps_limit-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.9
+Version: 1.1.0
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

## Comparing `qps_limit-1.0.9.dist-info/RECORD` & `qps_limit-1.1.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-qps_limit/__init__.py,sha256=TiIIyCKFqcgc79sHCD1V4PDjdlKO_23qgZFvVN_uv7E,165
-qps_limit/limiter.py,sha256=Zm8rYbPeGIyDL6qa9QO2Y6IjcHBE1iCRc-odVHmww3A,5918
+qps_limit/__init__.py,sha256=EPzWSbJqZ_QcKoo6nAWSQ7KKKMcOemNkoXpnsoo5n3g,165
+qps_limit/limiter.py,sha256=oG4f-OIV5U5TrAPD_-BlShS6IE7rKc44FB4bGDGAbLI,6926
 qps_limit/run.py,sha256=mqmPou-88VcnDqjg4dcjn5eYYyslJUGm79gblWnmVZQ,5474
-qps_limit-1.0.9.dist-info/METADATA,sha256=5fG9ocsnjK2G4gJn_XEVu6tSAE7lJXCh0JDO-bcx5uw,2565
-qps_limit-1.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-qps_limit-1.0.9.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
-qps_limit-1.0.9.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-qps_limit-1.0.9.dist-info/RECORD,,
+qps_limit-1.1.0.dist-info/METADATA,sha256=TjH98uz2JRoiq48DE5nR7xuWsd3ZuC-jf-FdYalfrIY,2565
+qps_limit-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+qps_limit-1.1.0.dist-info/top_level.txt,sha256=vH2iImlC_yaDXYqPQn3x6ZXcQ5Ec2yAe-l0lLJqu0RY,10
+qps_limit-1.1.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+qps_limit-1.1.0.dist-info/RECORD,,
```


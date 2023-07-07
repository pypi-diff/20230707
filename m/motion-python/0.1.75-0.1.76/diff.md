# Comparing `tmp/motion_python-0.1.75.tar.gz` & `tmp/motion_python-0.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.75.tar", max compression
+gzip compressed data, was "motion_python-0.1.76.tar", max compression
```

## Comparing `motion_python-0.1.75.tar` & `motion_python-0.1.76.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3344 2023-07-07 16:16:17.106696 motion_python-0.1.75/README.md
--rw-r--r--   0        0        0      344 2023-07-07 16:16:17.106696 motion_python-0.1.75/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-07 16:16:17.106696 motion_python-0.1.75/motion/cli.py
--rw-r--r--   0        0        0    23355 2023-07-07 16:16:17.106696 motion_python-0.1.75/motion/component.py
--rw-r--r--   0        0        0     3929 2023-07-07 16:16:17.106696 motion_python-0.1.75/motion/dicts.py
--rw-r--r--   0        0        0    17675 2023-07-07 16:16:17.106696 motion_python-0.1.75/motion/execute.py
--rw-r--r--   0        0        0    13900 2023-07-07 16:16:17.110696 motion_python-0.1.75/motion/instance.py
--rw-r--r--   0        0        0     4882 2023-07-07 16:16:17.110696 motion_python-0.1.75/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-07 16:16:17.110696 motion_python-0.1.75/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1153 2023-07-07 16:16:17.110696 motion_python-0.1.75/motion/route.py
--rw-r--r--   0        0        0     4833 2023-07-07 16:16:17.110696 motion_python-0.1.75/motion/server/update_task.py
--rw-r--r--   0        0        0     8591 2023-07-07 16:16:17.110696 motion_python-0.1.75/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-07 16:16:42.468628 motion_python-0.1.75/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.75/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-07 20:48:13.332358 motion_python-0.1.76/README.md
+-rw-r--r--   0        0        0      344 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/cli.py
+-rw-r--r--   0        0        0    23355 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/component.py
+-rw-r--r--   0        0        0     3929 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/dicts.py
+-rw-r--r--   0        0        0    17016 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/execute.py
+-rw-r--r--   0        0        0    13900 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/instance.py
+-rw-r--r--   0        0        0     4882 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1153 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/route.py
+-rw-r--r--   0        0        0     5018 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/server/update_task.py
+-rw-r--r--   0        0        0     8591 2023-07-07 20:48:13.336358 motion_python-0.1.76/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-07 20:48:34.092632 motion_python-0.1.76/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.76/PKG-INFO
```

### Comparing `motion_python-0.1.75/README.md` & `motion_python-0.1.76/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/motion/cli.py` & `motion_python-0.1.76/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/motion/component.py` & `motion_python-0.1.76/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/motion/dicts.py` & `motion_python-0.1.76/motion/dicts.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/motion/execute.py` & `motion_python-0.1.76/motion/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,77 +115,78 @@
             if not isinstance(initial_state, dict):
                 raise TypeError(f"{self._instance_name} init should return a dict.")
             return initial_state
 
         return {}
 
     def _build_fit_jobs(self) -> None:
-        """Builds update jobs."""
-        # Set up worker loops
-        self.worker_tasks = {}
-        # self.worker_stop_events = {}
-
+        """Builds update job."""
         rp = RedisParams()
         # self.worker_states = {}
 
+        # Set up update task
+        self.route_dict_for_fit = {}
+        self.channel_dict_for_fit = {}
+        self.queue_ids_for_fit = []
         for rkey, routes in self._update_routes.items():
             for udf_name, route in routes.items():
-                pname = f"{self._instance_name}::{rkey}::{udf_name}"
-                multiprocessing.Event()
-                self.worker_tasks[pname] = UpdateTask(
-                    self._instance_name,
-                    route,
-                    save_state_func=self._save_state_func,
-                    load_state_func=self._load_state_func,
-                    queue_identifier=self._get_queue_identifier(rkey, udf_name),
-                    channel_identifier=self._get_channel_identifier(rkey, udf_name),
-                    redis_host=rp.host,
-                    redis_port=rp.port,
-                    redis_db=rp.db,
-                    redis_password=rp.password,  # type: ignore
-                    running=self.running,
+                queue_id = self._get_queue_identifier(rkey, udf_name)
+                self.queue_ids_for_fit.append(queue_id)
+                self.route_dict_for_fit[queue_id] = route
+                self.channel_dict_for_fit[queue_id] = self._get_channel_identifier(
+                    rkey, udf_name
                 )
-                # self.worker_stop_events[pname] = worker_stop_event
-                self.worker_tasks[pname].start()
+
+        self.worker_task = UpdateTask(
+            self._instance_name,
+            routes=self.route_dict_for_fit,
+            save_state_func=self._save_state_func,
+            load_state_func=self._load_state_func,
+            queue_identifiers=self.queue_ids_for_fit,
+            channel_identifiers=self.channel_dict_for_fit,
+            redis_host=rp.host,
+            redis_port=rp.port,
+            redis_db=rp.db,
+            redis_password=rp.password,  # type: ignore
+            running=self.running,
+        )
+        self.worker_task.start()
 
         # Set up a monitor thread
         self.stop_event = threading.Event()
         self.monitor_thread = threading.Thread(
-            target=self._monitor_processes, daemon=True
+            target=self._monitor_process, daemon=True
         )
         self.monitor_thread.start()
 
-    def _monitor_processes(self) -> None:
+    def _monitor_process(self) -> None:
         rp = RedisParams()
         while not self.stop_event.is_set():
-            # Loop through processes to see if they are alive
-            for pname, process in self.worker_tasks.items():
-                if not process.is_alive():
-                    logger.debug(
-                        f"Failed to detect heartbeat for update task {pname}."
-                        + " Restarting the task in the background."
-                    )
-                    # Restart
-                    rkey = pname.split("::")[1]
-                    udf_name = pname.split("::")[2]
-                    route = self._update_routes[rkey][udf_name]
-                    self.worker_tasks[pname] = UpdateTask(
-                        self._instance_name,
-                        route,
-                        save_state_func=self._save_state_func,
-                        load_state_func=self._load_state_func,
-                        queue_identifier=self._get_queue_identifier(rkey, udf_name),
-                        channel_identifier=self._get_channel_identifier(rkey, udf_name),
-                        redis_host=rp.host,
-                        redis_port=rp.port,
-                        redis_db=rp.db,
-                        redis_password=rp.password,  # type: ignore
-                        running=self.running,
-                    )
-                    self.worker_tasks[pname].start()
+            # See if the update task is alive
+            if not self.worker_task.is_alive():
+                logger.debug(
+                    f"Failed to detect heartbeat for {self.worker_task.name}."
+                    + " Restarting the task in the background."
+                )
+
+                # Restart
+                self.worker_task = UpdateTask(
+                    self._instance_name,
+                    routes=self.route_dict_for_fit,
+                    save_state_func=self._save_state_func,
+                    load_state_func=self._load_state_func,
+                    queue_identifiers=self.queue_ids_for_fit,
+                    channel_identifiers=self.channel_dict_for_fit,
+                    redis_host=rp.host,
+                    redis_port=rp.port,
+                    redis_db=rp.db,
+                    redis_password=rp.password,  # type: ignore
+                    running=self.running,
+                )
+                self.worker_task.start()
 
             if self.stop_event.is_set():
                 break
 
             # Sleep for a minute
             self.stop_event.wait(60)
 
@@ -207,28 +208,19 @@
         if is_open:
             logger.info("Running update operations on remaining data...")
 
         # Set shutdown event
         self.stop_event.set()
         self.running.value = False
 
-        processes_to_wait_for = []
-        for process in self.worker_tasks.values():
-            if psutil.pid_exists(process.pid):
-                # os.kill(process.pid, signal.SIGUSR1)  # type:ignore
-                # Set stop event
-                # self.worker_stop_events[pname].set()
-                processes_to_wait_for.append(process)
+        if psutil.pid_exists(self.worker_task.pid):
+            self.worker_task.join()
 
         self._redis_con.close()
 
-        # Join update processes
-        for process in processes_to_wait_for:
-            process.join()
-
         self.monitor_thread.join()
 
     def _updateState(self, new_state: Dict[str, Any]) -> None:
         if not new_state:
             return
 
         if not isinstance(new_state, dict):
```

### Comparing `motion_python-0.1.75/motion/instance.py` & `motion_python-0.1.76/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/motion/migrate.py` & `motion_python-0.1.76/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.76/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/motion/route.py` & `motion_python-0.1.76/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/motion/server/update_task.py` & `motion_python-0.1.76/motion/server/update_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import asyncio
 import multiprocessing
 import traceback
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, List, Optional
 
 import cloudpickle
 import redis
 from redis.lock import Lock
 
 from motion.route import Route
 from motion.utils import loadState, logger, saveState
 
 
 class UpdateTask(multiprocessing.Process):
     def __init__(
         self,
         instance_name: str,
-        route: Route,
+        routes: Dict[str, Route],
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
-        queue_identifier: str,
-        channel_identifier: str,
+        queue_identifiers: List[str],
+        channel_identifiers: Dict[str, str],
         redis_host: str,
         redis_port: int,
         redis_db: int,
         redis_password: str,
         running: Any,
     ):
         super().__init__()
-        self.name = f"UpdateTask-{instance_name}-{route.key}-{route.udf.__name__}"
+        self.name = f"UpdateTask-{instance_name}"
         self.instance_name = instance_name
         self.save_state_func = save_state_func
         self.load_state_func = load_state_func
         self.redis_host = redis_host
         self.redis_port = redis_port
         self.redis_db = redis_db
         self.redis_password = redis_password
 
-        self.route = route
-        self.queue_identifier = queue_identifier
-        self.channel_identifier = channel_identifier
+        self.routes = routes
+        self.queue_identifiers = queue_identifiers
+        self.channel_identifiers = channel_identifiers
 
         self.running = running
         self.daemon = True
 
     def run(self) -> None:
         redis_con = redis.Redis(
             host=self.redis_host,
@@ -52,23 +52,25 @@
         )
         # Acquire a lock
         lock_timeout = 300  # Lock timeout in seconds
         lock = Lock(redis_con, self.instance_name, lock_timeout)
 
         while self.running.value:
             item: Dict[str, Any] = {}
+            queue_name = ""
             try:
                 # for _ in range(self.batch_size):
-                full_item = redis_con.blpop(self.queue_identifier, timeout=0.5)
+                full_item = redis_con.blpop(self.queue_identifiers, timeout=0.1)
                 if full_item is None:
                     if not self.running.value:
                         break  # no more items in the list
                     else:
                         continue
 
+                queue_name = full_item[0].decode("utf-8")
                 item = cloudpickle.loads(full_item[1])
                 # self.batch.append(item)
                 # if flush_update:
                 #     break
             except redis.exceptions.ConnectionError:
                 logger.error("Connection to redis lost.")
                 break
@@ -81,32 +83,34 @@
             # if not self.batch:
             #     continue
 
             exception_str = ""
             # Check if it was a no op
             if item["identifier"].startswith("NOOP_"):
                 redis_con.publish(
-                    self.channel_identifier,
+                    self.channel_identifiers[queue_name],
                     str(
                         {
                             "identifier": item["identifier"],
                             "exception": exception_str,
                         }
                     ),
                 )
                 continue
 
             # Run update op
             acquired_lock = lock.acquire(blocking=True)
             if acquired_lock:
                 try:
                     old_state = loadState(
-                        redis_con, self.instance_name, self.load_state_func
+                        redis_con,
+                        self.instance_name,
+                        self.load_state_func,
                     )
-                    state_update = self.route.run(
+                    state_update = self.routes[queue_name].run(
                         state=old_state,
                         props=item["props"],
                     )
                     # Await if state_update is a coroutine
                     if asyncio.iscoroutine(state_update):
                         state_update = asyncio.run(state_update)
 
@@ -129,15 +133,15 @@
                 finally:
                     logger.info("Releasing lock.")
                     lock.release()
             else:
                 logger.error("Lock not acquired; item lost.")
 
             redis_con.publish(
-                self.channel_identifier,
+                self.channel_identifiers[queue_name],
                 str(
                     {
                         "identifier": item["identifier"],
                         "exception": exception_str,
                     }
                 ),
             )
```

### Comparing `motion_python-0.1.75/motion/utils.py` & `motion_python-0.1.76/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.75/pyproject.toml` & `motion_python-0.1.76/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.75"
+version = "0.1.76"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.75/PKG-INFO` & `motion_python-0.1.76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.75
+Version: 0.1.76
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


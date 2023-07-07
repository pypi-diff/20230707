# Comparing `tmp/mfhpo_simulator-1.2.3-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 27265 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      560 b- defN 23-Jul-05 11:48 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     7646 b- defN 23-Jul-04 15:16 benchmark_simulator/_constants.py
--rw-rw-r--  2.0 unx    11741 b- defN 23-Jul-04 14:42 benchmark_simulator/_secure_proc.py
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-14 22:34 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx    25336 b- defN 23-Jul-05 11:47 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx     2582 b- defN 23-Jul-04 07:45 benchmark_simulator/_simulator/_base_wrapper.py
+Zip file size: 29158 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      560 b- defN 23-Jul-07 16:03 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     7711 b- defN 23-Jul-07 13:22 benchmark_simulator/_constants.py
+-rw-rw-r--  2.0 unx    12110 b- defN 23-Jul-07 15:56 benchmark_simulator/_secure_proc.py
+-rw-rw-r--  2.0 unx     5116 b- defN 23-Jul-06 23:36 benchmark_simulator/_utils.py
+-rw-rw-r--  2.0 unx    27095 b- defN 23-Jul-07 15:59 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx     2582 b- defN 23-Jul-06 18:41 benchmark_simulator/_simulator/_base_wrapper.py
 -rw-rw-r--  2.0 unx     2978 b- defN 23-Jul-04 16:11 benchmark_simulator/_simulator/_utils.py
--rw-rw-r--  2.0 unx    11647 b- defN 23-Jul-04 16:12 benchmark_simulator/_simulator/_worker.py
--rw-rw-r--  2.0 unx     3223 b- defN 23-Jul-04 10:43 benchmark_simulator/_simulator/_worker_manager.py
+-rw-rw-r--  2.0 unx    12902 b- defN 23-Jul-07 16:01 benchmark_simulator/_simulator/_worker.py
+-rw-rw-r--  2.0 unx     3249 b- defN 23-Jul-07 13:10 benchmark_simulator/_simulator/_worker_manager.py
 -rw-rw-r--  2.0 unx     8290 b- defN 23-Jul-04 16:13 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       51 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1401 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/RECORD
-15 files, 88386 bytes uncompressed, 24899 bytes compressed:  71.8%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       51 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1401 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/RECORD
+15 files, 95204 bytes uncompressed, 26792 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: benchmark_simulator/_simulator/_worker_manager.py
 Comment: 
 
 Filename: benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.3.dist-info/LICENSE
+Filename: mfhpo_simulator-1.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-1.2.3.dist-info/METADATA
+Filename: mfhpo_simulator-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-1.2.3.dist-info/WHEEL
+Filename: mfhpo_simulator-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-1.2.3.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-1.2.3.dist-info/RECORD
+Filename: mfhpo_simulator-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import AbstractAskTellOptimizer, ObjectiveFuncType
 from benchmark_simulator.simulator import ObjectiveFuncWrapper, get_multiple_wrappers
 
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## benchmark_simulator/_constants.py

```diff
@@ -33,14 +33,17 @@
     result: str
     state_cache: str
     worker_cumtime: str
     timestamp: str
     timenow: str
     config_tracker: str
 
+    def __len__(self) -> int:
+        return len(self.__dict__)
+
 
 @dataclass(frozen=True)
 class _ResultData:
     cumtime: float
     eval_config: dict[str, Any]
     results: dict[str, float]
     fidels: dict[str, int | float]
```

## benchmark_simulator/_secure_proc.py

```diff
@@ -15,15 +15,20 @@
 from benchmark_simulator._utils import _SecureLock
 
 import numpy as np
 
 import ujson as json  # type: ignore
 
 
-def _init_simulator(dir_name: str) -> None:
+def _init_simulator(dir_name: str, worker_index: int | None) -> None:
+    if worker_index is not None and worker_index != 0:  # only if worker index == 0, we initialize
+        return
+
+    # Prevent unnecessary overwrite from any other workers by making workers wait for a random fraction
+    time.sleep(np.random.random() * 1e-2)  # DO NOT REMOVE
     for fn in _SharedDataFileNames:
         path = os.path.join(dir_name, fn.value)
         with open(path, "a+") as f:
             fcntl.flock(f.fileno(), fcntl.LOCK_EX)
             f.seek(0)
             content = f.read()
             if len(content) < 2:
@@ -152,15 +157,15 @@
 def _fetch_existing_configs(path: str, lock: _SecureLock) -> dict[str, dict[str, Any]]:
     with lock.read(path) as f:
         existing_configs = json.load(f)
 
     return existing_configs
 
 
-def _fetch_proc_alloc(path: str, lock: _SecureLock) -> dict[int, int]:
+def _fetch_proc_alloc(path: str, lock: _SecureLock) -> dict[int, int]:  # pragma: no cover
     return _complete_proc_allocation(path=path, lock=lock)
 
 
 def _record_result(path: str, results: dict[str, float], lock: _SecureLock, fixed: bool = True) -> None:
     with lock.edit(path) as f:
         record = json.load(f)
         n_observations = len(record.get("cumtime", []))
@@ -192,15 +197,15 @@
     return result
 
 
 def _is_allocation_ready(path: str, n_workers: int, lock: _SecureLock) -> bool:
     with lock.read(path) as f:
         n_allocs = len(json.load(f))
 
-    if n_allocs > n_workers:
+    if n_allocs > n_workers:  # pragma: no cover
         raise ValueError(_get_timeout_message("the allocation of procs", path))
 
     return n_allocs == n_workers
 
 
 def _get_worker_id_to_idx(path: str, lock: _SecureLock) -> dict[str, int]:
     with lock.read(path) as f:
@@ -313,15 +318,15 @@
     waiting_time *= 1 + np.random.random()
     while not _is_min_cumtime(path, worker_id=worker_id, lock=lock):
         time.sleep(waiting_time)
         curtime = time.time()
         if int(curtime - start + 1) % warning_interval == 0:
             warnings.warn(
                 "Workers might be hanging. Please consider setting `max_waiting_time` (< np.inf).\n"
-                "Note that if samplers or the objective function need long time (> 10 seconds), "
-                "please ignore this warning."
+                "Note that if samplers or the objective function need long time (> 10 seconds), or \n"
+                "n_workers is large, please ignore this warning."
             )
 
         if curtime - start > max_waiting_time:
             _terminate_with_unexpected_timeout(
                 path=path, worker_id=worker_id, max_waiting_time=max_waiting_time, lock=lock
             )
```

## benchmark_simulator/_utils.py

```diff
@@ -1,20 +1,25 @@
 import fcntl
+import glob
 import hashlib
+import os
 import time
 from contextlib import contextmanager
 from dataclasses import dataclass
+from fnmatch import fnmatch
 from typing import Iterator, TextIO
 
 import numpy as np
 
 
 def _generate_time_hash() -> str:
     hash = hashlib.sha1()
-    hash.update(str(time.time()).encode("utf-8"))
+    # Try to make it as unique as possible! time.time() was not sufficient!
+    timehash_pid = str(time.time() + os.getpid() + np.random.random() * 1e9)  # DO NOT MAKE IT SIMPLE
+    hash.update(timehash_pid.encode("utf-8"))
     return hash.hexdigest()
 
 
 @dataclass(frozen=True)
 class _SecureLock:
     waiting_time: float = 1e-4
     time_limit: float = 10.0
@@ -26,15 +31,15 @@
         fetched = False
         while not fetched:
             with open(path, "r") as f:
                 try:
                     fcntl.flock(f, fcntl.LOCK_SH | fcntl.LOCK_NB)
                     yield f
                     fetched = True
-                except IOError:
+                except IOError:  # pragma: no cover
                     time.sleep(waiting_time)
                     if time.time() - start >= self.time_limit:
                         raise TimeoutError("Timeout during secure read. Try again.")
 
     @contextmanager
     def edit(self, path: str) -> Iterator[TextIO]:
         start = time.time()
@@ -43,13 +48,85 @@
         while not fetched:
             with open(path, "r+") as f:
                 try:
                     fcntl.flock(f, fcntl.LOCK_EX)
                     yield f
                     f.truncate()
                     fetched = True
-                except IOError:
+                except IOError:  # pragma: no cover
                     time.sleep(waiting_time)
                     if time.time() - start >= self.time_limit:
                         raise TimeoutError("Timeout during secure edit. Try again.")
-                finally:
+                finally:  # pragma: no cover
                     fcntl.flock(f, fcntl.LOCK_UN)
+
+
+@dataclass(frozen=True)
+class _SecureLockForDistributedSystem:  # pragma: no cover
+    """
+    If _SecureLock does not work on some environments, we should use it.
+    Although this lock still cannot guarantee that it works perfectly, better than nothing.
+    Typically, network latency causes some unexpected consequence.
+
+    This class acquires a file lock by publishing a token file.
+    If there exists a public token, this class renames it to private token and acquires the access.
+    As there is not public token in this situation, other processes cannot access.
+    Once the process finishes the access, it renames back to the public token and other processes can access.
+    As we acquire the lock directory-wise, it is much slower than with fcntl.
+    """
+
+    dir_name: str
+    private_token: str
+    public_token: str
+    token_pattern: str = "access_*.token"
+    waiting_time: float = 1e-4
+    time_limit: float = 10.0
+
+    def _validate(self) -> None:
+        private_token, public_token, token_pattern = self.private_token, self.public_token, self.token_pattern
+        if not private_token.startswith(self.dir_name) or not fnmatch(private_token, token_pattern):
+            raise ValueError(f"private_token must match the token pattern {token_pattern=}, but got {private_token=}")
+        if not public_token.startswith(self.dir_name) or not fnmatch(public_token, token_pattern):
+            raise ValueError(f"public_token must match the token pattern {token_pattern=}, but got {public_token=}")
+
+    def init_token(self) -> None:
+        self._validate()
+        token_pattern = os.path.join(self.dir_name, self.token_pattern)
+        n_tokens = len(glob.glob(token_pattern))
+        if n_tokens == 0:
+            with open(self.public_token, mode="w"):
+                pass
+        elif n_tokens > 1:  # Token from another process could exist!
+            raise FileExistsError
+
+    def _publish_token(self) -> None:
+        start = time.time()
+        waiting_time = self.waiting_time * (1 + np.random.random())
+        while True:
+            try:
+                os.rename(self.public_token, self.private_token)
+                return
+            except FileNotFoundError:
+                time.sleep(waiting_time)
+                if time.time() - start >= self.time_limit:
+                    raise TimeoutError("Timeout during token publication. Please remove token files and try again.")
+
+    def _remove_token(self) -> None:
+        os.rename(self.private_token, self.public_token)
+
+    @contextmanager
+    def read(self, path: str) -> Iterator[TextIO]:
+        self._publish_token()
+        with open(path, mode="r") as f:
+            fcntl.flock(f, fcntl.LOCK_SH | fcntl.LOCK_NB)
+            yield f
+        self._remove_token()
+
+    @contextmanager
+    def edit(self, path: str) -> Iterator[TextIO]:
+        self._publish_token()
+        with open(path, mode="r+") as f:
+            fcntl.flock(f, fcntl.LOCK_EX)
+            yield f
+            f.truncate()
+            fcntl.flock(f, fcntl.LOCK_UN)
+        self._remove_token()
```

## benchmark_simulator/simulator.py

```diff
@@ -71,15 +71,14 @@
 This file is used to consider the sampling time.
 after_sample is the latest cumtime immediately after the last sample and before_sample is before the last sample.
 """
 from __future__ import annotations
 
 import os
 from datetime import datetime
-from multiprocessing import Pool
 from typing import Any
 
 from benchmark_simulator._constants import AbstractAskTellOptimizer, DIR_NAME, ObjectiveFuncType, _WrapperVars
 from benchmark_simulator._simulator._worker import _ObjectiveFuncWorker
 from benchmark_simulator._simulator._worker_manager import _CentralWorkerManager
 from benchmark_simulator._simulator._worker_manager_for_ask_and_tell import _AskTellWorkerManager
 
@@ -196,23 +195,17 @@
         seed=seed,
         continual_max_fidel=continual_max_fidel,
         max_waiting_time=max_waiting_time,
         check_interval_time=check_interval_time,
         store_config=store_config,
         allow_parallel_sampling=allow_parallel_sampling,
         config_tracking=config_tracking,
+        _async_instantiations=False,
     )
-    pool = Pool()
-    results = []
-    for _ in range(n_workers):
-        results.append(pool.apply_async(ObjectiveFuncWrapper, kwds=wrapper_kwargs))
-
-    pool.close()
-    pool.join()
-    return [result.get() for result in results]
+    return [ObjectiveFuncWrapper(**wrapper_kwargs, worker_index=i) for i in range(n_workers)]  # type: ignore[arg-type]
 
 
 class ObjectiveFuncWrapper:
     """Objective function wrapper API for users.
 
     Please check more details at https://github.com/nabenabe0928/mfhpo-simulator/
 
@@ -264,14 +257,16 @@
         seed: int | None = None,
         continual_max_fidel: int | None = None,
         max_waiting_time: float = np.inf,
         check_interval_time: float = 1e-4,
         store_config: bool = False,
         allow_parallel_sampling: bool = False,
         config_tracking: bool = True,
+        worker_index: int | None = None,
+        _async_instantiations: bool = True,
     ):
         """The initialization of a wrapper class.
 
         Both ObjectiveFuncWorker and CentralWorkerManager have the same interface and the same set of control params.
 
         Args:
             obj_func (ObjectiveFuncType):
@@ -346,14 +341,26 @@
                 Whether sampling can happen in parallel.
                 In many cases, sampler will not be run in parallel and then allow_parallel_sampling should be False.
                 The default value is False.
             config_tracking (bool):
                 Whether to validate config_id provided from the user side.
                 It slows the simulation down when n_evals is large (> 3000),
                 but it is recommended to avoid unexpected bugs that could happen.
+            worker_index (int | None):
+                It specifies which worker index will be used for this wrapper.
+                It is typically useful when you run this wrapper from different processes in parallel.
+                If you did not specify this index, our wrapper automatically allocates worker indices,
+                but this may sometimes fail (in our environment with 0.01% of the probability for n_workers=8).
+                The failure rate might be higher especially when you use a large n_workers, so in that case,
+                probably users would like to use this option.
+                The worker indices must be unique across the parallel workers and must be in [0, n_workers - 1].
+            _async_instantiations (bool):
+                Whether each worker is instantiated asynchrously.
+                In other words, whether to wait all workers' instantiations or not.
+                This argument must not be touched by users.
         """
         curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S.%f")
         wrapper_vars = _WrapperVars(
             obj_func=obj_func,
             save_dir_name=save_dir_name if save_dir_name is not None else f"data-{curtime}",
             n_workers=n_workers,
             n_actual_evals_in_opt=n_actual_evals_in_opt,
@@ -371,27 +378,35 @@
         )
 
         self._main_wrapper: _AskTellWorkerManager | _CentralWorkerManager | _ObjectiveFuncWorker
         self._validate(
             save_dir_name=save_dir_name,
             ask_and_tell=ask_and_tell,
             launch_multiple_wrappers_from_user_side=launch_multiple_wrappers_from_user_side,
+            worker_index=worker_index,
+            n_workers=n_workers,
         )
         if ask_and_tell:
             self._main_wrapper = _AskTellWorkerManager(wrapper_vars)
         elif launch_multiple_wrappers_from_user_side:
-            self._main_wrapper = _ObjectiveFuncWorker(wrapper_vars)
+            self._main_wrapper = _ObjectiveFuncWorker(
+                wrapper_vars, worker_index=worker_index, async_instantiations=_async_instantiations
+            )
         else:
             self._main_wrapper = _CentralWorkerManager(wrapper_vars)
 
     @property
     def dir_name(self) -> str:
         return self._main_wrapper.dir_name
 
     @property
+    def result_file_path(self) -> str:
+        return self._main_wrapper._paths.result
+
+    @property
     def obj_keys(self) -> list[str]:
         return self._main_wrapper.obj_keys
 
     @property
     def runtime_key(self) -> str:
         return self._main_wrapper.runtime_key
 
@@ -408,24 +423,33 @@
         return self._main_wrapper._wrapper_vars.n_workers
 
     def _validate(
         self,
         save_dir_name: str | None,
         ask_and_tell: bool,
         launch_multiple_wrappers_from_user_side: bool,
+        n_workers: int,
+        worker_index: int | None,
     ) -> None:
         if ask_and_tell and launch_multiple_wrappers_from_user_side:
             raise ValueError(
                 "ask_and_tell and launch_multiple_wrappers_from_user_side cannot be True at the same time."
             )
         if launch_multiple_wrappers_from_user_side and save_dir_name is None:
             raise ValueError(
                 "When launch_multiple_wrappers_from_user_side is False, save_dir_name must be specified so that \n"
                 "each worker recognizes with which processes it shares the optimization results."
             )
+        if worker_index is not None and (ask_and_tell or not launch_multiple_wrappers_from_user_side):
+            raise ValueError(
+                "When launch_multiple_wrappers_from_user_side=False or ask_and_tell=True, "
+                "worker_index cannot be specified."
+            )
+        if worker_index is not None and worker_index not in list(range(n_workers)):
+            raise ValueError(f"worker_index must be in [0, {n_workers-1=}], but got {worker_index=}")
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
         config_id: int | None = None,
```

## benchmark_simulator/_simulator/_worker.py

```diff
@@ -5,14 +5,15 @@
 from typing import Any
 
 from benchmark_simulator._constants import (
     INF,
     _TIME_VALUES,
     _TimeNowDictType,
     _WorkerVars,
+    _WrapperVars,
 )
 from benchmark_simulator._secure_proc import (
     _fetch_cumtimes,
     _fetch_timenow,
     _fetch_timestamps,
     _finish_worker_timer,
     _init_simulator,
@@ -45,31 +46,57 @@
     This worker class is supposed to be instantiated for each worker.
     For example, if we use 4 workers for an optimization, then four instances should be created.
 
     Note:
         See benchmark_simulator/simulator.py to know variables shared across workers.
     """
 
+    def __init__(self, wrapper_vars: _WrapperVars, worker_index: int | None, async_instantiations: bool):
+        self._temp_worker_index = worker_index
+        self._async_inst = async_instantiations
+        super().__init__(wrapper_vars=wrapper_vars)
+
     def __repr__(self) -> str:
         return f"Worker-{self._worker_vars.worker_id}"
 
     def _init_worker(self, worker_id: str) -> None:
         os.makedirs(self.dir_name, exist_ok=True)
         self._state_tracker = _StateTracker(
             path=self._paths.state_cache, lock=self._lock, continual_max_fidel=self._wrapper_vars.continual_max_fidel
         )
         self._config_tracker = _ConfigIDTracker(path=self._paths.config_tracker, lock=self._lock)
-        _init_simulator(dir_name=self.dir_name)
+        _init_simulator(dir_name=self.dir_name, worker_index=self._temp_worker_index)
+        self._wait_till_init_simulator_finish()
         _start_worker_timer(path=self._paths.worker_cumtime, worker_id=worker_id, lock=self._lock)
 
+    def _wait_till_init_simulator_finish(self) -> None:
+        n_files = len(self._paths)
+        n_repeats = 10000
+        n_workers = self._wrapper_vars.n_workers
+        while len(os.listdir(self.dir_name)) < n_files:  # pragma: no cover
+            # In fact, below is covered by test, but not detected by pytest-cov
+            time.sleep(1e-4)
+            n_repeats -= 1
+            if n_repeats == 0:
+                msg = [
+                    "The file initialization did not finish.",
+                    "worker_index specified by users probably did not include 0.",
+                    f"worker_index must be unique and in [0, {n_workers-1=}].",
+                ]
+                raise TimeoutError("\n".join(msg))
+
     def _alloc_index(self, worker_id: str) -> int:
+        if not self._async_inst:
+            assert self._temp_worker_index is not None  # mypy redefinition
+            return self._temp_worker_index
+
         worker_id_to_index = _wait_all_workers(
             path=self._paths.worker_cumtime, n_workers=self._wrapper_vars.n_workers, lock=self._lock
         )
-        time.sleep(1e-2)  # buffer before the optimization
+        time.sleep(1e-2)  # buffer before the optimization: DO NOT REMOVE
         return worker_id_to_index[worker_id]
 
     def _init_wrapper(self) -> None:
         continual_eval = self._wrapper_vars.continual_max_fidel is not None
         worker_id = _generate_time_hash()
         self._wrapper_vars.validate()
         _validate_fidel_args(continual_eval, fidel_keys=self._fidel_keys)
```

## benchmark_simulator/_simulator/_worker_manager.py

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import os
 import threading
-from multiprocessing import Pool
 from typing import Any
 
 from benchmark_simulator._secure_proc import (
     _allocate_proc_to_worker,
     _fetch_proc_alloc,
     _is_allocation_ready,
     _wait_proc_allocation,
@@ -32,47 +31,45 @@
         self._init_workers()
         self._pid_to_index: dict[int, int] = {}
 
     def _init_workers(self) -> None:
         if os.path.exists(self.dir_name):
             raise FileExistsError(f"The directory `{self.dir_name}` already exists. Remove it first.")
 
-        pool = Pool()
-        results = []
-        for _ in range(self._wrapper_vars.n_workers):
-            results.append(pool.apply_async(_ObjectiveFuncWorker, kwds=dict(wrapper_vars=self._wrapper_vars)))
-
-        pool.close()
-        pool.join()
-        self._workers = [result.get() for result in results]
+        n_workers = self._wrapper_vars.n_workers
+        self._workers = [
+            _ObjectiveFuncWorker(wrapper_vars=self._wrapper_vars, worker_index=i, async_instantiations=False)
+            for i in range(n_workers)
+        ]
 
     def _init_alloc(self, pid: int) -> None:
         path = self._paths.proc_alloc
         if not _is_allocation_ready(path=path, n_workers=self._wrapper_vars.n_workers, lock=self._lock):
             _allocate_proc_to_worker(path=path, pid=pid, lock=self._lock)
             self._pid_to_index = _wait_proc_allocation(
                 path=path, n_workers=self._wrapper_vars.n_workers, lock=self._lock
             )
         else:
-            self._pid_to_index = _fetch_proc_alloc(path=path, lock=self._lock)
+            # This line is actually covered, but it is not visible due to multiprocessing nature
+            self._pid_to_index = _fetch_proc_alloc(path=path, lock=self._lock)  # pragma: no cover
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
         config_id: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         pid = os.getpid()
         pid = threading.get_ident() if pid == self._main_pid else pid
         if len(self._pid_to_index) != self._wrapper_vars.n_workers:
             self._init_alloc(pid)
 
-        if pid not in self._pid_to_index:
+        if pid not in self._pid_to_index:  # pragma: no cover
             raise ProcessLookupError(
                 f"An unknown process/thread with ID {pid} was specified.\n"
                 "It is likely that one of the workers crashed and a new worker was added or \n"
                 f"n_workers in ObjectiveFuncWrapper and your optimizer were incompatible.\n"
                 f"However, worker additions are not allowed in ObjectiveFuncWrapper."
             )
```

## Comparing `mfhpo_simulator-1.2.3.dist-info/LICENSE` & `mfhpo_simulator-1.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_simulator-1.2.3.dist-info/RECORD` & `mfhpo_simulator-1.2.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-benchmark_simulator/__init__.py,sha256=gcjgqYhs2r0tgv5fgrgZo8XUtjfDfS1uZ7nXTDUwabw,560
-benchmark_simulator/_constants.py,sha256=_9Whr7k-DDFxXoPHANgILWWLaYxKnfHobDkd_Ctql7o,7646
-benchmark_simulator/_secure_proc.py,sha256=Go1sN__3lsirYFUGOXm5Kgp0Lvkhc3TGd017bDoZHzI,11741
-benchmark_simulator/_utils.py,sha256=s2kwhhHIJbrT0VbNglmq-rlm0oE8OrqUBvDpCLEAsXk,1772
-benchmark_simulator/simulator.py,sha256=GkVnFY0Zepinp79s6vJOv9I_T9iXH9TVdgT8r7Z3fCk,25336
+benchmark_simulator/__init__.py,sha256=1ITNCN35fru3HBqWUJ99T3Xc1knYyL6GRuK87Qze6S4,560
+benchmark_simulator/_constants.py,sha256=exAEgiuwOzlf-Q6vn5Iey_k0lvUxz4EljM_sHHK1k10,7711
+benchmark_simulator/_secure_proc.py,sha256=U5fKC9CtvZwSrlLo2X_WFRZdoO1MF8cvVJKLem9YZT4,12110
+benchmark_simulator/_utils.py,sha256=ZA8l51dZMxpjhMZCUExO-Mg8r5ilJWdvR2P3RFipzk4,5116
+benchmark_simulator/simulator.py,sha256=XaOHO3MWtic2JzhmOPK1VNU6-qmT9z0rdRL6W3LuXx4,27095
 benchmark_simulator/_simulator/_base_wrapper.py,sha256=HvK4Iq1vjCuD1HEcphY-hl4Wo_vo1d-N_FA9PFkYukA,2582
 benchmark_simulator/_simulator/_utils.py,sha256=eVQOty1X3ZfXb4Hr8oaRjaOMWYJQHi-YPmCDB91xhO4,2978
-benchmark_simulator/_simulator/_worker.py,sha256=oE-vEJEgSu9LGNXIGE8Z7S8PCaivIGq9WWKDr8U-K-c,11647
-benchmark_simulator/_simulator/_worker_manager.py,sha256=hQXJR2GLrrKiTgCXoYDEs5bYRO1ASTF87ye37eGfKn8,3223
+benchmark_simulator/_simulator/_worker.py,sha256=SAUkMFNv1X26nYby8Rvr5qIhWkLX1snsySkoZKyeDns,12902
+benchmark_simulator/_simulator/_worker_manager.py,sha256=DTCkHst5kAS75YICG7A7edf8RD-owMF3m3tBimbAVvI,3249
 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py,sha256=l3SK3Vv5_N4KrsNyTB-yWt3CfY453VFZ3z3iE7nmDN4,8290
-mfhpo_simulator-1.2.3.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_simulator-1.2.3.dist-info/METADATA,sha256=W9-5rBtU34rEfmV_vZG60uUw93hGceRTreolOj4-now,307
-mfhpo_simulator-1.2.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_simulator-1.2.3.dist-info/top_level.txt,sha256=dkUhIqI2xJvV1NOS7bvMDWMNDJ1GGBwTnOBedLuz3OA,51
-mfhpo_simulator-1.2.3.dist-info/RECORD,,
+mfhpo_simulator-1.2.4.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_simulator-1.2.4.dist-info/METADATA,sha256=F69eigXbIaKox6XHEWwqlNh0XFt1EX8c0WF3NCcnOVM,307
+mfhpo_simulator-1.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mfhpo_simulator-1.2.4.dist-info/top_level.txt,sha256=dkUhIqI2xJvV1NOS7bvMDWMNDJ1GGBwTnOBedLuz3OA,51
+mfhpo_simulator-1.2.4.dist-info/RECORD,,
```


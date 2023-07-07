# Comparing `tmp/spaces-0.6b1.tar.gz` & `tmp/spaces-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.6b1.tar", max compression
+gzip compressed data, was "spaces-0.7.0.tar", max compression
```

## Comparing `spaces-0.6b1.tar` & `spaces-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.6b1/README.md
--rw-r--r--   0        0        0     1489 2023-06-30 16:02:24.855918 spaces-0.6b1/pyproject.toml
--rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.6b1/spaces/__init__.py
--rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.6b1/spaces/config.py
--rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.6b1/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     1839 2023-06-29 12:42:06.802062 spaces-0.6b1/spaces/gpu/client.py
--rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.6b1/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3581 2023-06-29 12:16:02.996586 spaces-0.6b1/spaces/gpu/torch.py
--rw-r--r--   0        0        0     6753 2023-06-02 18:54:45.252087 spaces-0.6b1/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.6b1/spaces/gradio.py
--rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.6b1/spaces/utils.py
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.6b1/setup.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.6b1/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.7.0/README.md
+-rw-r--r--   0        0        0     1524 2023-07-07 16:42:49.331263 spaces-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.7.0/spaces/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.7.0/spaces/config.py
+-rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.7.0/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     2224 2023-07-07 16:19:13.425611 spaces-0.7.0/spaces/gpu/client.py
+-rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.7.0/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3573 2023-07-07 16:29:17.706242 spaces-0.7.0/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     6888 2023-07-07 16:28:48.625635 spaces-0.7.0/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.7.0/spaces/gradio.py
+-rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.7.0/spaces/utils.py
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 spaces-0.7.0/setup.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 spaces-0.7.0/PKG-INFO
```

### Comparing `spaces-0.6b1/pyproject.toml` & `spaces-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "spaces"
-version = "0.6b1"
+version = "0.7.0"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psutil = "^5.9.5"
 typing-extensions = "^4.5.0"
 requests = "^2.29.0"
 pydantic = "^1.10.8"
+gradio = "^3.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-dotenv = "^0.5.2"
 pytest-mock = "^3.10.0"
 requests-mock = "^1.10.0"
 pytest-timeout = "^2.1.0"
 poethepoet = "^0.20.0"
 coverage = "^7.2.6"
 pyright = "^1.1.311"
 pytest-order = "^1.1.0"
+pynvml = "^11.5.0"
 
 [tool.poetry.group.test.dependencies]
 diffusers = "^0.16.1"
 transformers = "^4.29.1"
 accelerate = "^0.19.0"
 xformers = "^0.0.19"
```

### Comparing `spaces-0.6b1/spaces/gpu/client.py` & `spaces-0.7.0/spaces/gpu/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 """
 from __future__ import annotations
 
+import time
 from http import HTTPStatus
 
+import gradio as gr
 import requests
 from pydantic import BaseModel
 
 from .. import utils
 from ..config import Config
 
 
@@ -16,14 +18,15 @@
 
 class ScheduleParams(BaseModel):
     cgroupPath: str
 
 class ScheduleResponse(BaseModel):
     idle: bool
     nvidiaIndex: int
+    nvidiaUUID: str
 
 class ReleaseParams(BaseModel):
     cgroupPath: str
     nvidiaIndex: int
     fail: bool
 
 
@@ -33,27 +36,31 @@
 
 
 def post(path: str, params: BaseModel | None = None) -> requests.Response:
     return requests.post(base_url() + path, params=params.dict() if params else None)
 
 
 def startup_report():
-    res = post('/startup-report')
-    if res.status_code != HTTPStatus.OK: # pragma: no cover
-        raise RuntimeError("Error while initializing ZeroGPU")
+    retries, max_retries = 0, 2
+    while (status := post('/startup-report').status_code) == HTTPStatus.NOT_FOUND: # pragma: no cover
+        time.sleep(1)
+        if (retries := retries + 1) > max_retries:
+            raise RuntimeError("Error while initializing ZeroGPU: NotFound")
+    if status != HTTPStatus.OK: # pragma: no cover
+        raise RuntimeError("Error while initializing ZeroGPU: Unknown")
 
 
 def schedule() -> ScheduleResponse:
 
     res = post('/schedule', params=ScheduleParams(
         cgroupPath=CGROUP_PATH,
     ))
 
     if res.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise RuntimeError("GPU already in use")
+        raise gr.Error("No GPU is currently available")
 
     try:
         data = res.json()
     except requests.JSONDecodeError: # pragma: no cover
         data = {}
 
     if not res.ok: # pragma: no cover
@@ -71,10 +78,11 @@
     ))
 
     if not res.ok:
         try:
             data = res.json()
         except requests.JSONDecodeError: # pragma: no cover
             data = {}
+        # TODO: use future gr.Warning() if /release didn't detect GPU usage
         raise RuntimeError(f"ZeroGPU API /release error: {data.get('detail')}")
 
     return None
```

### Comparing `spaces-0.6b1/spaces/gpu/decorator.py` & `spaces-0.7.0/spaces/gpu/decorator.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6b1/spaces/gpu/torch.py` & `spaces-0.7.0/spaces/gpu/torch.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,16 +72,16 @@
 
     def _unpatch():
         torch.Tensor.to         = _tensor_to
         torch.Tensor.cuda       = _tensor_cuda
         torch._C._cuda_init     = _cuda_init
         torch.cuda.is_available = _cuda_available
 
-    def _move(nvidia_index: int):
-        os.environ['CUDA_VISIBLE_DEVICES'] = str(nvidia_index)
+    def _move(nvidia_uuid: str):
+        os.environ['CUDA_VISIBLE_DEVICES'] = nvidia_uuid
         for op in to_ops:
             tensor, parsed_args = op
             _, dtype, _, memory_format = parsed_args
             tensor.data = _tensor_to(tensor,
                 device='cuda',
                 dtype=dtype,
                 memory_format=memory_format,
@@ -100,15 +100,15 @@
         torch.Tensor.to   = _tensor_to
         torch.Tensor.cuda = _tensor_cuda
 
 else:
 
     _patch = lambda: None
     _unpatch = lambda: None
-    _move = lambda nvidia_index: None
+    _move = lambda nvidia_uuid: None
     _is_in_bad_fork = lambda: False
     _disable_cuda_intercept = lambda: None
 
 
 patch = _patch
 unpatch = _unpatch
 move = _move
```

### Comparing `spaces-0.6b1/spaces/gpu/wrappers.py` & `spaces-0.7.0/spaces/gpu/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 """
 from __future__ import annotations
 
+import gradio as gr
 import multiprocessing
 import os
 import signal
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from pickle import PicklingError
@@ -28,32 +29,33 @@
 
 Process = multiprocessing.get_context('fork').Process
 
 Arg = tuple[tuple[Any], dict[str, Any]]
 Res = TypeVar('Res')
 Param = ParamSpec('Param')
 NvidiaIndex = int
+NvidiaUUID = str
 
 
 class Worker(Generic[Res]):
     process: Process
     arg_queue: Queue[Arg]
     res_queue: Queue[Res]
     _sentinel: Thread
 
     def __init__(
         self,
-        target: Callable[[Queue[Arg], Queue[Res], NvidiaIndex, list[int]], None],
-        nvidia_index: int,
+        target: Callable[[Queue[Arg], Queue[Res], NvidiaUUID, list[int]], None],
+        nvidia_uuid: str,
     ):
         self._sentinel = Thread(target=self._close_on_exit)
         self.arg_queue = Queue()
         self.res_queue = Queue()
         fds = [c.fd for c in psutil.Process().connections()]
-        args = self.arg_queue, self.res_queue, nvidia_index, fds
+        args = self.arg_queue, self.res_queue, nvidia_uuid, fds
         if TYPE_CHECKING:
             target(*args)
         self.process = Process(
             target=target,
             args=args,
             daemon=True,
         )
@@ -72,57 +74,58 @@
 
     workers: dict[NvidiaIndex, Worker[list[Res] | Exception]] = {}
 
     def process_wrapper(*args: Param.args, **kwargs: Param.kwargs) -> Res:
 
         schedule_response = client.schedule()
         nvidia_index = schedule_response.nvidiaIndex
+        nvidia_uuid = schedule_response.nvidiaUUID
         release = partial(client.release, nvidia_index=nvidia_index)
 
         worker = workers.get(nvidia_index)
         if worker is None or not worker.process.is_alive():
-            worker = Worker(thread_wrapper, nvidia_index)
+            worker = Worker(thread_wrapper, nvidia_uuid)
             workers[nvidia_index] = worker
 
         try:
             worker.arg_queue.put((args, kwargs))
         except PicklingError:
             release(fail=True)
             raise
 
         try:
             res = worker.res_queue.get()
         except EOFError:
             release(fail=True)
-            raise RuntimeError("Operation aborted")
+            raise gr.Error("GPU task aborted")
         if isinstance(res, Exception):
             release(fail=True)
             raise res
         release()
         return res[0]
 
 
     def thread_wrapper(
         arg_queue: Queue[Arg],
         res_queue: Queue[list[Res] | Exception],
-        nvidia_index: int,
+        nvidia_uuid: str,
         fds: list[int],
     ):
         torch.unpatch()
-        torch.move(nvidia_index)
+        torch.move(nvidia_uuid)
         for fd in fds:
             os.close(fd)
         signal.signal(signal.SIGTERM, drop_params(arg_queue.close))
         while True:
             try:
                 args, kwargs = arg_queue.get()
             except OSError:
                 break
             with ThreadPoolExecutor() as executor:
-                future = executor.submit(task, *args, **kwargs)
+                future = executor.submit(task, *args, **kwargs) # type: ignore
             try:
                 res = [future.result()]
             except Exception as e:
                 traceback.print_exc()
                 res = e
             try:
                 res_queue.put(res)
@@ -139,19 +142,20 @@
 
     workers: dict[NvidiaIndex, Worker[list[Res] | Exception | None]] = {}
 
     def process_wrapper(*args: Param.args, **kwargs: Param.kwargs) -> Generator[Res, None, None]:
 
         schedule_response = client.schedule()
         nvidia_index = schedule_response.nvidiaIndex
+        nvidia_uuid = schedule_response.nvidiaUUID
         release = partial(client.release, nvidia_index=nvidia_index)
 
         worker = workers.get(nvidia_index)
         if worker is None or not worker.process.is_alive():
-            worker = Worker(thread_wrapper, nvidia_index)
+            worker = Worker(thread_wrapper, nvidia_uuid)
             workers[nvidia_index] = worker
 
         try:
             worker.arg_queue.put((args, kwargs))
         except PicklingError:
             release(fail=True)
             raise
@@ -177,30 +181,30 @@
 
         with ThreadPoolExecutor() as e:
             e.submit(fill_yield_queue, worker)
             while True:
                 try:
                     res = yield_queue.get()
                 except Exception:
-                    raise RuntimeError("Operation aborted")
+                    raise gr.Error("GPU task aborted")
                 if isinstance(res, Exception):
                     raise res
                 if res is None:
                     break
                 yield res[0]
 
 
     def thread_wrapper(
         arg_queue: Queue[Arg],
         res_queue: Queue[list[Res] | Exception | None],
-        nvidia_index: int,
+        nvidia_uuid: str,
         fds: list[int],
     ):
         torch.unpatch()
-        torch.move(nvidia_index)
+        torch.move(nvidia_uuid)
         for fd in fds:
             os.close(fd)
         signal.signal(signal.SIGTERM, drop_params(arg_queue.close))
         while True:
             try:
                 args, kwargs = arg_queue.get()
             except OSError:
```

### Comparing `spaces-0.6b1/spaces/gradio.py` & `spaces-0.7.0/spaces/gradio.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6b1/spaces/utils.py` & `spaces-0.7.0/spaces/utils.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6b1/setup.py` & `spaces-0.7.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 packages = \
 ['spaces', 'spaces.gpu']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['psutil>=5.9.5,<6.0.0',
+['gradio>=3.2,<4.0',
+ 'psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.6b1',
+    'version': '0.7.0',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.6b1/PKG-INFO` & `spaces-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.6b1
+Version: 0.7.0
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: gradio (>=3.2,<4.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/huggingface/huggingface_hub
 Description-Content-Type: text/markdown
```


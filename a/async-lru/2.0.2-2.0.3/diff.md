# Comparing `tmp/async-lru-2.0.2.tar.gz` & `tmp/async-lru-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-lru-2.0.2.tar", last modified: Mon Feb 20 16:42:49 2023, max compression
+gzip compressed data, was "async-lru-2.0.3.tar", last modified: Fri Jul  7 19:00:21 2023, max compression
```

## Comparing `async-lru-2.0.2.tar` & `async-lru-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:42:49.911354 async-lru-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-20 16:42:29.000000 async-lru-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-20 16:42:29.000000 async-lru-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-20 16:42:29.000000 async-lru-2.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-02-20 16:42:49.911354 async-lru-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-02-20 16:42:29.000000 async-lru-2.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:42:49.907353 async-lru-2.0.2/async_lru/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-02-20 16:42:29.000000 async-lru-2.0.2/async_lru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-20 16:42:29.000000 async-lru-2.0.2/async_lru/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:42:49.911354 async-lru-2.0.2/async_lru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-02-20 16:42:49.000000 async-lru-2.0.2/async_lru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-20 16:42:49.000000 async-lru-2.0.2/async_lru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 16:42:49.000000 async-lru-2.0.2/async_lru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 16:42:49.000000 async-lru-2.0.2/async_lru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-20 16:42:49.000000 async-lru-2.0.2/async_lru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-02-20 16:42:49.911354 async-lru-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-20 16:42:29.000000 async-lru-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:42:49.911354 async-lru-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_cache_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_cache_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_cache_invalidate.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_close.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_partialmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-02-20 16:42:29.000000 async-lru-2.0.2/tests/test_ttl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:00:21.228657 async-lru-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-07 18:59:59.000000 async-lru-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-07 18:59:59.000000 async-lru-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-07 18:59:59.000000 async-lru-2.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-07 19:00:21.228657 async-lru-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-07 18:59:59.000000 async-lru-2.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:00:21.228657 async-lru-2.0.3/async_lru/
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-07 18:59:59.000000 async-lru-2.0.3/async_lru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:59:59.000000 async-lru-2.0.3/async_lru/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:00:21.228657 async-lru-2.0.3/async_lru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 19:00:21.000000 async-lru-2.0.3/async_lru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-07 19:00:21.232658 async-lru-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 18:59:59.000000 async-lru-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:00:21.228657 async-lru-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_cache_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_cache_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_cache_invalidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_partialmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-07 18:59:59.000000 async-lru-2.0.3/tests/test_ttl.py
```

### Comparing `async-lru-2.0.2/LICENSE` & `async-lru-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/async_lru/__init__.py` & `async-lru-2.0.3/async_lru/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import dataclasses
+import sys
 from asyncio.coroutines import _is_coroutine  # type: ignore[attr-defined]
 from functools import _CacheInfo, _make_key, partial, partialmethod
 from typing import (
     Any,
     Callable,
     Coroutine,
     Generic,
@@ -16,18 +17,22 @@
     TypeVar,
     Union,
     cast,
     final,
     overload,
 )
 
-from typing_extensions import Self
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
 
-__version__ = "2.0.2"
+
+__version__ = "2.0.3"
 
 __all__ = ("alru_cache",)
 
 
 _T = TypeVar("_T")
 _R = TypeVar("_R")
 _Coro = Coroutine[Any, Any, _R]
@@ -131,15 +136,15 @@
 
         await asyncio.gather(*tasks, return_exceptions=True)
 
     def cache_info(self) -> _CacheInfo:
         return _CacheInfo(
             self.__hits,
             self.__misses,
-            self.__maxsize,  # type: ignore[arg-type]
+            self.__maxsize,
             len(self.__cache),
         )
 
     def cache_parameters(self) -> _CacheParameters:
         return _CacheParameters(
             maxsize=self.__maxsize,
             typed=self.__typed,
@@ -155,17 +160,17 @@
         self.__misses += 1
 
     def _task_done_callback(
         self, fut: "asyncio.Future[_R]", key: Hashable, task: "asyncio.Task[_R]"
     ) -> None:
         self.__tasks.remove(task)
 
-        if self.__ttl is not None:
+        cache_item = self.__cache.get(key)
+        if self.__ttl is not None and cache_item is not None:
             loop = asyncio.get_running_loop()
-            cache_item = self.__cache[key]
             cache_item.later_call = loop.call_later(
                 self.__ttl, self.__cache.pop, key, None
             )
 
         if task.cancelled():
             fut.cancel()
             return
@@ -175,15 +180,15 @@
             fut.set_exception(exc)
             return
 
         fut.set_result(task.result())
 
     async def __call__(self, /, *fn_args: Any, **fn_kwargs: Any) -> _R:
         if self.__closed:
-            raise RuntimeError("alru_cache is closed for {}".format(self))
+            raise RuntimeError(f"alru_cache is closed for {self}")
 
         loop = asyncio.get_running_loop()
 
         key = _make_key(fn_args, fn_kwargs, self.__typed)
 
         cache_item = self.__cache.get(key)
 
@@ -293,15 +298,15 @@
     def wrapper(fn: _CBP[_R]) -> _LRUCacheWrapper[_R]:
         origin = fn
 
         while isinstance(origin, (partial, partialmethod)):
             origin = origin.func
 
         if not asyncio.iscoroutinefunction(origin):
-            raise RuntimeError("Coroutine function is required, got {!r}".format(fn))
+            raise RuntimeError(f"Coroutine function is required, got {fn!r}")
 
         # functools.partialmethod support
         if hasattr(fn, "_make_unbound_method"):
             fn = fn._make_unbound_method()
 
         return _LRUCacheWrapper(cast(_CB[_R], fn), maxsize, typed, ttl)
 
@@ -336,8 +341,8 @@
         return _make_wrapper(maxsize, typed, ttl)
     else:
         fn = cast(_CB[_R], maxsize)
 
         if callable(fn) or hasattr(fn, "_make_unbound_method"):
             return _make_wrapper(128, False, None)(fn)
 
-        raise NotImplementedError("{!r} decorating is not supported".format(fn))
+        raise NotImplementedError(f"{fn!r} decorating is not supported")
```

### Comparing `async-lru-2.0.2/async_lru.egg-info/SOURCES.txt` & `async-lru-2.0.3/async_lru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/setup.cfg` & `async-lru-2.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [metadata]
 name = async-lru
 version = attr: async_lru.__version__
 url = https://github.com/aio-libs/async-lru
 project_urls = 
+	Chat: Matrix = https://matrix.to/#/#aio-libs:matrix.org
+	Chat: Matrix Space = https://matrix.to/#/#aio-libs-space:matrix.org
 	CI: GitHub Actions = https://github.com/aio-libs/async-lru/actions
 	GitHub: repo = https://github.com/aio-libs/async-lru
 description = Simple LRU cache for asyncio
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 maintainer = aiohttp team <team@aiohttp.org>
 maintainer_email = team@aiohttp.org
@@ -34,15 +36,15 @@
 	lru
 	lru_cache
 
 [options]
 python_requires = >=3.8
 packages = find:
 install_requires = 
-	typing_extensions>=4.0.0
+	typing_extensions>=4.0.0; python_version<"3.11"
 
 [options.package_data]
 * = 
 	py.typed
 
 [flake8]
 exclude = .git,.env,__pycache__,.eggs
```

### Comparing `async-lru-2.0.2/tests/conftest.py` & `async-lru-2.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_basic.py` & `async-lru-2.0.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_cache_info.py` & `async-lru-2.0.3/tests/test_cache_info.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_cache_invalidate.py` & `async-lru-2.0.3/tests/test_cache_invalidate.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_close.py` & `async-lru-2.0.3/tests/test_close.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_exception.py` & `async-lru-2.0.3/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_internals.py` & `async-lru-2.0.3/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_partialmethod.py` & `async-lru-2.0.3/tests/test_partialmethod.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_size.py` & `async-lru-2.0.3/tests/test_size.py`

 * *Files identical despite different names*

### Comparing `async-lru-2.0.2/tests/test_ttl.py` & `async-lru-2.0.3/tests/test_ttl.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,7 +54,16 @@
     assert await coro(1) == 1
     check_lru(coro, hits=0, misses=2, cache=1, tasks=0, maxsize=None)
 
     await asyncio.sleep(0.1)
     # cache is not cleared after ttl expires because invalidate also should clear
     # the invalidation by timeout
     check_lru(coro, hits=0, misses=2, cache=1, tasks=0, maxsize=None)
+
+
+async def test_ttl_concurrent() -> None:
+    @alru_cache(maxsize=1, ttl=1)
+    async def coro(val: int) -> int:
+        return val
+
+    results = await asyncio.gather(*(coro(i) for i in range(2)))
+    assert results == list(range(2))
```


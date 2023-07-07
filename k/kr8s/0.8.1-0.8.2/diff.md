# Comparing `tmp/kr8s-0.8.1.tar.gz` & `tmp/kr8s-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.8.1.tar", max compression
+gzip compressed data, was "kr8s-0.8.2.tar", max compression
```

## Comparing `kr8s-0.8.1.tar` & `kr8s-0.8.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1549 2023-07-06 14:11:09.419376 kr8s-0.8.1/LICENSE
--rw-r--r--   0        0        0     2587 2023-07-06 14:11:09.419376 kr8s-0.8.1/README.md
--rw-r--r--   0        0        0     1143 2023-07-06 14:11:33.199634 kr8s-0.8.1/kr8s/__init__.py
--rw-r--r--   0        0        0    14447 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/_api.py
--rw-r--r--   0        0        0     5879 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/_exceptions.py
--rw-r--r--   0        0        0     4336 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/_io.py
--rw-r--r--   0        0        0    33118 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/_objects.py
--rw-r--r--   0        0        0     8074 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/_testutils.py
--rw-r--r--   0        0        0      248 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0     1796 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/asyncio/_helpers.py
--rw-r--r--   0        0        0      827 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0      168 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5503 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/conftest.py
--rw-r--r--   0        0        0     6001 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/objects.py
--rw-r--r--   0        0        0      152 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/portforward.py
--rw-r--r--   0        0        0       78 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0       61 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0      369 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rw-r--r--   0        0        0      144 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rwxr-xr-x   0        0        0      614 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     5666 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3394 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0     1710 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    17697 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-07-06 14:11:09.439377 kr8s-0.8.1/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2556 2023-07-06 14:11:33.199634 kr8s-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3323 1970-01-01 00:00:00.000000 kr8s-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-07-07 11:06:36.660486 kr8s-0.8.2/LICENSE
+-rw-r--r--   0        0        0     2587 2023-07-07 11:06:36.660486 kr8s-0.8.2/README.md
+-rw-r--r--   0        0        0     1143 2023-07-07 11:07:02.624519 kr8s-0.8.2/kr8s/__init__.py
+-rw-r--r--   0        0        0    14608 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/_api.py
+-rw-r--r--   0        0        0     5879 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4336 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/_io.py
+-rw-r--r--   0        0        0    33118 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/_objects.py
+-rw-r--r--   0        0        0     8074 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/_testutils.py
+-rw-r--r--   0        0        0      248 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0     1681 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/asyncio/_helpers.py
+-rw-r--r--   0        0        0      827 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0      168 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5503 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     5909 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3394 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0     1710 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    17697 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-07-07 11:06:36.684486 kr8s-0.8.2/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2556 2023-07-07 11:07:02.624519 kr8s-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3323 1970-01-01 00:00:00.000000 kr8s-0.8.2/PKG-INFO
```

### Comparing `kr8s-0.8.1/LICENSE` & `kr8s-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/README.md` & `kr8s-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/__init__.py` & `kr8s-0.8.2/kr8s/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .asyncio import (
     version as _version,
 )
 from .asyncio import (
     watch as _watch,
 )
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.8.1/kr8s/_api.py` & `kr8s-0.8.2/kr8s/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,20 @@
                     auth_attempts += 1
                     await self.auth.reauthenticate()
                     await self._create_session()
                     continue
                 else:
                     raise
             except RuntimeError as e:
-                if "Event loop is closed" in str(e):
+                if any(
+                    [
+                        "Event loop is closed" in str(e),
+                        "bound to a different event loop" in str(e),
+                    ]
+                ):
                     await self._create_session()
                     continue
                 else:
                     raise
             break
 
     @contextlib.asynccontextmanager
```

### Comparing `kr8s-0.8.1/kr8s/_auth.py` & `kr8s-0.8.2/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/_data_utils.py` & `kr8s-0.8.2/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/_io.py` & `kr8s-0.8.2/kr8s/_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/_objects.py` & `kr8s-0.8.2/kr8s/_objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/_portforward.py` & `kr8s-0.8.2/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/_testutils.py` & `kr8s-0.8.2/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/asyncio/_api.py` & `kr8s-0.8.2/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/asyncio/_helpers.py` & `kr8s-0.8.2/kr8s/asyncio/_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 from typing import Dict, List, Union
 
 from kr8s._api import Api
-from kr8s._io import run_sync as _run_sync
 
 from ._api import api as _api
 
 
 async def get(
     kind: str,
     *names: List[str],
@@ -16,18 +15,15 @@
     field_selector: Union[str, Dict] = None,
     as_object: object = None,
     api=None,
     _asyncio=True,
     **kwargs,
 ):
     if api is None:
-        if _asyncio:
-            api = await _api()
-        else:
-            api = _run_sync(_api)(_asyncio=False)
+        api = await _api(_asyncio=_asyncio)
     return await api._get(
         kind,
         *names,
         namespace=namespace,
         label_selector=label_selector,
         field_selector=field_selector,
         as_object=as_object,
```

### Comparing `kr8s-0.8.1/kr8s/asyncio/objects.py` & `kr8s-0.8.2/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/conftest.py` & `kr8s-0.8.2/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/objects.py` & `kr8s-0.8.2/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/tests/scripts/envexec.py` & `kr8s-0.8.2/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/tests/test_api.py` & `kr8s-0.8.2/kr8s/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,7 +199,16 @@
     assert pods[0]._asyncio is False
 
 
 def test_sync_api_returns_sync_objects():
     api = kr8s.api()
     pods = api.get("pods", namespace=kr8s.ALL)
     assert pods[0]._asyncio is False
+
+
+def test_api_client_reuse_between_event_loops():
+    async def get_api():
+        await kr8s.asyncio.get("pods", namespace=kr8s.ALL)
+
+    asyncio.run(get_api())
+    asyncio.set_event_loop(asyncio.new_event_loop())
+    asyncio.run(get_api())
```

### Comparing `kr8s-0.8.1/kr8s/tests/test_auth.py` & `kr8s-0.8.2/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/tests/test_data_utils.py` & `kr8s-0.8.2/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/tests/test_io.py` & `kr8s-0.8.2/kr8s/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/tests/test_objects.py` & `kr8s-0.8.2/kr8s/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/kr8s/tests/test_testutils.py` & `kr8s-0.8.2/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.1/pyproject.toml` & `kr8s-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.8.1"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.8.2"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `kr8s-0.8.1/PKG-INFO` & `kr8s-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.8.1
+Version: 0.8.2
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```


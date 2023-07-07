# Comparing `tmp/ms_python_client-0.1.0.tar.gz` & `tmp/ms_python_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_python_client-0.1.0.tar", max compression
+gzip compressed data, was "ms_python_client-0.1.1.tar", max compression
```

## Comparing `ms_python_client-0.1.0.tar` & `ms_python_client-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1100 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/LICENSE
--rw-r--r--   0        0        0     5433 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/__init__.py
--rw-r--r--   0        0        0     5332 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/api_client.py
--rw-r--r--   0        0        0        0 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/components/events/__init__.py
--rw-r--r--   0        0        0     5111 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/ms_api_client.py
--rw-r--r--   0        0        0     1023 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/ms_client_interface.py
--rw-r--r--   0        0        0        0 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/utils/__init__.py
--rw-r--r--   0        0        0       97 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/utils/file_system.py
--rw-r--r--   0        0        0     1276 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/utils/init_from_env.py
--rw-r--r--   0        0        0      729 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/utils/logger.py
--rw-r--r--   0        0        0     1034 2023-07-07 15:32:03.058291 ms_python_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 ms_python_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5433 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/__init__.py
+-rw-r--r--   0        0        0     5332 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/api_client.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/components/events/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/components/events/events_component.py
+-rw-r--r--   0        0        0     5222 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/ms_api_client.py
+-rw-r--r--   0        0        0     1023 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/ms_client_interface.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/utils/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/utils/file_system.py
+-rw-r--r--   0        0        0     1276 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/utils/init_from_env.py
+-rw-r--r--   0        0        0      729 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/ms_python_client/utils/logger.py
+-rw-r--r--   0        0        0     1034 2023-07-07 15:47:34.341212 ms_python_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 ms_python_client-0.1.1/PKG-INFO
```

### Comparing `ms_python_client-0.1.0/LICENSE` & `ms_python_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.1.0/README.md` & `ms_python_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.1.0/ms_python_client/api_client.py` & `ms_python_client-0.1.1/ms_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.1.0/ms_python_client/ms_api_client.py` & `ms_python_client-0.1.1/ms_python_client/ms_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from typing import Any, Mapping, Optional
 
 import requests
 from msal import ConfidentialClientApplication, SerializableTokenCache
 
 from ms_python_client.api_client import ApiClient
+from ms_python_client.components.events.events_component import EventsComponent
 from ms_python_client.ms_client_interface import MSClientInterface
 from ms_python_client.utils import init_from_env
 
 logging.getLogger("ms_python_client").addHandler(logging.NullHandler())
 logger = logging.getLogger("ms_python_client")
 
 TypeData = Mapping[str, Any]
@@ -52,15 +53,15 @@
 
     def _write_cache(self, cache_path: str, cache: SerializableTokenCache) -> None:
         with open(cache_path, "w", encoding="utf-8") as f:
             f.write(cache.serialize())
 
     def init_components(self):
         # Add all the new components here
-        pass
+        self.events = EventsComponent(self)
 
     def __init__(
         self,
         account_id: str,
         client_id: str,
         client_secret: str,
         api_endpoint: str = "https://graph.microsoft.com/v1.0",
```

### Comparing `ms_python_client-0.1.0/ms_python_client/ms_client_interface.py` & `ms_python_client-0.1.1/ms_python_client/ms_client_interface.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.1.0/ms_python_client/utils/init_from_env.py` & `ms_python_client-0.1.1/ms_python_client/utils/init_from_env.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.1.0/ms_python_client/utils/logger.py` & `ms_python_client-0.1.1/ms_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.1.0/pyproject.toml` & `ms_python_client-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-python-client"
-version = "0.1.0"
+version = "0.1.1"
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
 description = "This package is used to interact with the microsoft graph API"
 authors = ["Samuel Guillemet <samuel.guillemet@telecom-sudparis.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ms_python_client"}]
```

### Comparing `ms_python_client-0.1.0/PKG-INFO` & `ms_python_client-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-python-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package is used to interact with the microsoft graph API
 License: MIT
 Author: Samuel Guillemet
 Author-email: samuel.guillemet@telecom-sudparis.eu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


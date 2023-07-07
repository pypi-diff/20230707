# Comparing `tmp/dalpha-0.1.3.tar.gz` & `tmp/dalpha-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.1.3.tar", max compression
+gzip compressed data, was "dalpha-0.1.4.tar", max compression
```

## Comparing `dalpha-0.1.3.tar` & `dalpha-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      459 2023-05-27 07:33:56.211092 dalpha-0.1.3/README.md
--rw-r--r--   0        0        0     6455 2023-07-07 11:54:23.808631 dalpha-0.1.3/dalpha/__init__.py
--rw-r--r--   0        0        0      745 2023-07-07 11:53:39.519356 dalpha-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 dalpha-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      459 2023-05-27 07:33:56.211092 dalpha-0.1.4/README.md
+-rw-r--r--   0        0        0     6468 2023-07-07 12:13:08.221508 dalpha-0.1.4/dalpha/__init__.py
+-rw-r--r--   0        0        0      800 2023-07-07 12:13:34.068442 dalpha-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 dalpha-0.1.4/PKG-INFO
```

### Comparing `dalpha-0.1.3/dalpha/__init__.py` & `dalpha-0.1.4/dalpha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import requests, json, boto3, io, logging, sys, os
+import time
+
 class Agent:
     def __init__(self, api_id, use_sqs = False, dev_server=False):
         self.cfg_path = os.path.join(sys.path[0],'.dalphacfg')
         self.__load_config(self.cfg_path)
         self.token = os.environ['TOKEN']
         if dev_server:
             self.base_url = os.environ['DEV_BASE_URL']
```

### Comparing `dalpha-0.1.3/pyproject.toml` & `dalpha-0.1.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.26.137"
 requests = "^2.30.0"
 build = "^0.10.0"
 
+[tool.poetry.group.dev.dependencies]
+twine = "^4.0.2"
+
 [project]
 name = "dalpha"
 version = "0.1.2"
 authors = [
   { name="Beomseok", email="beomseok.lee@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
```

### Comparing `dalpha-0.1.3/PKG-INFO` & `dalpha-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


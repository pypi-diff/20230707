# Comparing `tmp/python_openobserve-0.1.0.tar.gz` & `tmp/python_openobserve-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_openobserve-0.1.0.tar", max compression
+gzip compressed data, was "python_openobserve-0.1.1.tar", max compression
```

## Comparing `python_openobserve-0.1.0.tar` & `python_openobserve-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-07-07 07:42:34.442507 python_openobserve-0.1.0/LICENSE
--rw-r--r--   0        0        0     1078 2023-07-07 09:09:16.563406 python_openobserve-0.1.0/README.md
--rw-r--r--   0        0        0      714 2023-07-07 07:59:35.986551 python_openobserve-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 07:43:49.510022 python_openobserve-0.1.0/python_openobserve/__init__.py
--rw-r--r--   0        0        0     3564 2023-07-07 09:04:56.149357 python_openobserve-0.1.0/python_openobserve/openobserve.py
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 python_openobserve-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-07 07:42:34.442507 python_openobserve-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1180 2023-07-07 09:13:16.438280 python_openobserve-0.1.1/README.md
+-rw-r--r--   0        0        0      714 2023-07-07 09:13:31.258166 python_openobserve-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 07:43:49.510022 python_openobserve-0.1.1/python_openobserve/__init__.py
+-rw-r--r--   0        0        0     3564 2023-07-07 09:04:56.149357 python_openobserve-0.1.1/python_openobserve/openobserve.py
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 python_openobserve-0.1.1/PKG-INFO
```

### Comparing `python_openobserve-0.1.0/LICENSE` & `python_openobserve-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_openobserve-0.1.0/README.md` & `python_openobserve-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # python-openobserve
 A python connector to submit information to OpenObserve (https://github.com/openobserve/openobserve)
 
 The idea is to have a similar python connector to the "Elasticsearch" package, which allows a 1:1 replacement of the "Elasticsearch" package with the "OpenObserve" package.
 
 OpenObserve is way more lightweight than Elasticsearch, and it is open source, like everything should be.
 
+## install
+
+`pip install python-openobserve`
+
 ## usage
 
 see [example.ipynb](example.ipynb) for a full example
 
 ```python
+from python_openobserve.openobserve import OpenObserve
+
 OO = OpenObserve(user = "root@example.com", password = "Complexpass#123")
 
 from datetime import datetime
 from random import random
 from pprint import pprint
 document = {
     "@timestamp" : datetime.utcnow(),
```

### Comparing `python_openobserve-0.1.0/pyproject.toml` & `python_openobserve-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-openobserve"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Justin Guese <guese.justin@gmail.com>"]
 license = "GNUv3"
 readme = "README.md"
 homepage = "https://github.com/JustinGuese/python-openobserve"
 repository = "https://github.com/JustinGuese/python-openobserve"
 keywords = ["openobserve", "elasticsearch", "logging", "unstructured data"]
```

### Comparing `python_openobserve-0.1.0/python_openobserve/openobserve.py` & `python_openobserve-0.1.1/python_openobserve/openobserve.py`

 * *Files identical despite different names*

### Comparing `python_openobserve-0.1.0/PKG-INFO` & `python_openobserve-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-openobserve
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/JustinGuese/python-openobserve
 License: GNUv3
 Keywords: openobserve,elasticsearch,logging,unstructured data
 Author: Justin Guese
 Author-email: guese.justin@gmail.com
 Requires-Python: >3.9
@@ -21,19 +21,25 @@
 # python-openobserve
 A python connector to submit information to OpenObserve (https://github.com/openobserve/openobserve)
 
 The idea is to have a similar python connector to the "Elasticsearch" package, which allows a 1:1 replacement of the "Elasticsearch" package with the "OpenObserve" package.
 
 OpenObserve is way more lightweight than Elasticsearch, and it is open source, like everything should be.
 
+## install
+
+`pip install python-openobserve`
+
 ## usage
 
 see [example.ipynb](example.ipynb) for a full example
 
 ```python
+from python_openobserve.openobserve import OpenObserve
+
 OO = OpenObserve(user = "root@example.com", password = "Complexpass#123")
 
 from datetime import datetime
 from random import random
 from pprint import pprint
 document = {
     "@timestamp" : datetime.utcnow(),
```


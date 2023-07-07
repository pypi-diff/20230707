# Comparing `tmp/Ruster-1.0.7.tar.gz` & `tmp/Ruster-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ruster-1.0.7.tar", last modified: Fri Jul  7 17:21:21 2023, max compression
+gzip compressed data, was "Ruster-2.0.0.tar", last modified: Fri Jul  7 17:26:26 2023, max compression
```

## Comparing `Ruster-1.0.7.tar` & `Ruster-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:21:21.302455 Ruster-1.0.7/
--rw-rw-rw-   0        0        0      904 2023-07-07 17:21:21.302455 Ruster-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 17:21:21.128911 Ruster-1.0.7/Ruster/
--rw-rw-rw-   0        0        0      122 2023-07-07 17:17:23.000000 Ruster-1.0.7/Ruster/__init__.py
--rw-rw-rw-   0        0        0    13107 2023-07-06 20:18:13.000000 Ruster-1.0.7/Ruster/app.py
--rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-1.0.7/Ruster/blueprints.py
--rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-1.0.7/Ruster/exceptions.py
--rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-1.0.7/Ruster/hasher.py
--rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-1.0.7/Ruster/jwt.py
--rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-1.0.7/Ruster/limiter.py
--rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-1.0.7/Ruster/mailer.py
--rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-1.0.7/Ruster/sanitizer.py
--rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-1.0.7/Ruster/session.py
--rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-1.0.7/Ruster/wtf.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:21:21.294438 Ruster-1.0.7/Ruster.egg-info/
--rw-rw-rw-   0        0        0      904 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 17:21:20.000000 Ruster-1.0.7/Ruster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 17:21:21.302455 Ruster-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-07-07 17:21:10.000000 Ruster-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:26.566744 Ruster-2.0.0/
+-rw-rw-rw-   0        0        0      904 2023-07-07 17:26:26.566744 Ruster-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:26.454893 Ruster-2.0.0/Ruster/
+-rw-rw-rw-   0        0        0       20 2023-07-07 17:25:59.000000 Ruster-2.0.0/Ruster/__init__.py
+-rw-rw-rw-   0        0        0    13111 2023-07-07 17:25:53.000000 Ruster-2.0.0/Ruster/app.py
+-rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-2.0.0/Ruster/blueprints.py
+-rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-2.0.0/Ruster/exceptions.py
+-rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-2.0.0/Ruster/hasher.py
+-rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-2.0.0/Ruster/jwt.py
+-rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-2.0.0/Ruster/limiter.py
+-rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-2.0.0/Ruster/mailer.py
+-rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-2.0.0/Ruster/sanitizer.py
+-rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-2.0.0/Ruster/session.py
+-rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-2.0.0/Ruster/wtf.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:26:26.558743 Ruster-2.0.0/Ruster.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 17:26:26.000000 Ruster-2.0.0/Ruster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:26:26.566744 Ruster-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-07-07 17:26:14.000000 Ruster-2.0.0/setup.py
```

### Comparing `Ruster-1.0.7/PKG-INFO` & `Ruster-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.7
+Version: 2.0.0
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ruster-1.0.7/Ruster/app.py` & `Ruster-2.0.0/Ruster/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 import asyncio
 from werkzeug.wrappers import Request, Response
 from werkzeug.routing import Map, Rule
 from jinja2 import Environment, FileSystemLoader
-from exceptions import HTTPException
-from blueprints import Blueprint
+from .exceptions import HTTPException
+from .blueprints import Blueprint
 from werkzeug.exceptions import NotFound, MethodNotAllowed, BadRequest, Unauthorized, Forbidden
 from werkzeug.middleware.dispatcher import DispatcherMiddleware
 from itsdangerous import URLSafeTimedSerializer, BadSignature
 from werkzeug.serving import run_simple
 from werkzeug.urls import url_encode
 import asyncio
-from session import session_manager
-from limiter import Limiter
+from .session import session_manager
+from .limiter import Limiter
 import traceback
 import os
 import importlib.util
 
 class Rust:
     def __init__(self):
         self.url_map = Map()
```

### Comparing `Ruster-1.0.7/Ruster/blueprints.py` & `Ruster-2.0.0/Ruster/blueprints.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.7/Ruster/hasher.py` & `Ruster-2.0.0/Ruster/hasher.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.7/Ruster/jwt.py` & `Ruster-2.0.0/Ruster/jwt.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.7/Ruster/limiter.py` & `Ruster-2.0.0/Ruster/limiter.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.7/Ruster/mailer.py` & `Ruster-2.0.0/Ruster/mailer.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.7/Ruster/sanitizer.py` & `Ruster-2.0.0/Ruster/sanitizer.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.7/Ruster/session.py` & `Ruster-2.0.0/Ruster/session.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.7/Ruster/wtf.py` & `Ruster-2.0.0/Ruster/wtf.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.7/Ruster.egg-info/PKG-INFO` & `Ruster-2.0.0/Ruster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.7
+Version: 2.0.0
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ruster-1.0.7/setup.py` & `Ruster-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Ruster",
-    version="1.0.7",
+    version="2.0.0",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/ruster",
```


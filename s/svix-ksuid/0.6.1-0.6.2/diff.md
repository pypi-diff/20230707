# Comparing `tmp/svix-ksuid-0.6.1.tar.gz` & `tmp/svix-ksuid-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svix-ksuid-0.6.1.tar", last modified: Thu May 25 12:47:09 2023, max compression
+gzip compressed data, was "svix-ksuid-0.6.2.tar", last modified: Fri Jul  7 09:18:08 2023, max compression
```

## Comparing `svix-ksuid-0.6.1.tar` & `svix-ksuid-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/
--rw-r--r--   0 tom       (1000) tom       (1000)     1087 2021-07-12 10:31:00.000000 svix-ksuid-0.6.1/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     5318 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     4226 2023-05-25 12:26:03.000000 svix-ksuid-0.6.1/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/ksuid/
--rw-r--r--   0 tom       (1000) tom       (1000)      120 2021-08-17 15:19:24.000000 svix-ksuid-0.6.1/ksuid/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4033 2023-05-25 12:26:03.000000 svix-ksuid-0.6.1/ksuid/ksuid.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2021-07-12 10:31:15.000000 svix-ksuid-0.6.1/ksuid/py.typed
--rw-r--r--   0 tom       (1000) tom       (1000)      196 2021-07-12 10:31:00.000000 svix-ksuid-0.6.1/pyproject.toml
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1850 2023-05-25 12:26:36.000000 svix-ksuid-0.6.1/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/svix_ksuid.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     5318 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      311 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-07-12 10:31:15.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/not-zip-safe
--rw-r--r--   0 tom       (1000) tom       (1000)       16 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        6 2023-05-25 12:47:09.000000 svix-ksuid-0.6.1/svix_ksuid.egg-info/top_level.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-25 12:47:09.827973 svix-ksuid-0.6.1/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     4980 2022-01-29 11:28:54.000000 svix-ksuid-0.6.1/tests/test_ksuid.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-07 09:18:08.469986 svix-ksuid-0.6.2/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1087 2021-07-12 10:31:00.000000 svix-ksuid-0.6.2/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     5318 2023-07-07 09:18:08.469986 svix-ksuid-0.6.2/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     4226 2023-05-25 12:26:03.000000 svix-ksuid-0.6.2/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-07 09:18:08.469986 svix-ksuid-0.6.2/ksuid/
+-rw-r--r--   0 tom       (1000) tom       (1000)      120 2021-08-17 15:19:24.000000 svix-ksuid-0.6.2/ksuid/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4049 2023-07-07 09:16:10.000000 svix-ksuid-0.6.2/ksuid/ksuid.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2021-07-12 10:31:15.000000 svix-ksuid-0.6.2/ksuid/py.typed
+-rw-r--r--   0 tom       (1000) tom       (1000)      196 2021-07-12 10:31:00.000000 svix-ksuid-0.6.2/pyproject.toml
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-07-07 09:18:08.469986 svix-ksuid-0.6.2/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1850 2023-07-07 09:17:43.000000 svix-ksuid-0.6.2/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-07 09:18:08.469986 svix-ksuid-0.6.2/svix_ksuid.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5318 2023-07-07 09:18:08.000000 svix-ksuid-0.6.2/svix_ksuid.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      311 2023-07-07 09:18:08.000000 svix-ksuid-0.6.2/svix_ksuid.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-07-07 09:18:08.000000 svix-ksuid-0.6.2/svix_ksuid.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2021-07-12 10:31:15.000000 svix-ksuid-0.6.2/svix_ksuid.egg-info/not-zip-safe
+-rw-r--r--   0 tom       (1000) tom       (1000)       16 2023-07-07 09:18:08.000000 svix-ksuid-0.6.2/svix_ksuid.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        6 2023-07-07 09:18:08.000000 svix-ksuid-0.6.2/svix_ksuid.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-07 09:18:08.469986 svix-ksuid-0.6.2/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4980 2022-01-29 11:28:54.000000 svix-ksuid-0.6.2/tests/test_ksuid.py
```

### Comparing `svix-ksuid-0.6.1/LICENSE` & `svix-ksuid-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `svix-ksuid-0.6.1/PKG-INFO` & `svix-ksuid-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svix-ksuid
-Version: 0.6.1
+Version: 0.6.2
 Summary:  A pure-Python KSUID implementation
 Home-page: https://github.com/svixhq/python-ksuid/
 Author: Svix
 Author-email: development@svix.com
 License: MIT
 Keywords: svix,ksuid
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: svix-ksuid Version: 0.6.1 Summary: A pure-Python
+Metadata-Version: 2.1 Name: svix-ksuid Version: 0.6.2 Summary: A pure-Python
 KSUID implementation Home-page: https://github.com/svixhq/python-ksuid/ Author:
 Svix Author-email: development@svix.com License: MIT Keywords: svix,ksuid
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Classifier: Topic :: Software Development :: Libraries
```

### Comparing `svix-ksuid-0.6.1/README.md` & `svix-ksuid-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `svix-ksuid-0.6.1/ksuid/ksuid.py` & `svix-ksuid-0.6.2/ksuid/ksuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         _payload = secrets.token_bytes(self.PAYLOAD_LENGTH_IN_BYTES) if payload is None else payload
         datetime = datetime.astimezone(timezone.utc) if datetime is not None else datetime_lib.now(tz=timezone.utc)
         self._uid = self._inner_init(datetime, _payload)
 
     def __str__(self) -> str:
         """Creates a base62 string representation"""
 
-        return base62.encode(int.from_bytes(bytes(self), "big")).zfill(27)
+        return base62.encode(int.from_bytes(bytes(self), "big")).zfill(self.BASE62_LENGTH)
 
     def __repr__(self) -> str:
         return str(self)
 
     def __bytes__(self) -> bytes:
         return self._uid
```

### Comparing `svix-ksuid-0.6.1/setup.py` & `svix-ksuid-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import find_packages, setup  # noqa: H301
 
 NAME = "svix-ksuid"
-VERSION = "0.6.1"
+VERSION = "0.6.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `svix-ksuid-0.6.1/svix_ksuid.egg-info/PKG-INFO` & `svix-ksuid-0.6.2/svix_ksuid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svix-ksuid
-Version: 0.6.1
+Version: 0.6.2
 Summary:  A pure-Python KSUID implementation
 Home-page: https://github.com/svixhq/python-ksuid/
 Author: Svix
 Author-email: development@svix.com
 License: MIT
 Keywords: svix,ksuid
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: svix-ksuid Version: 0.6.1 Summary: A pure-Python
+Metadata-Version: 2.1 Name: svix-ksuid Version: 0.6.2 Summary: A pure-Python
 KSUID implementation Home-page: https://github.com/svixhq/python-ksuid/ Author:
 Svix Author-email: development@svix.com License: MIT Keywords: svix,ksuid
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Classifier: Topic :: Software Development :: Libraries
```

### Comparing `svix-ksuid-0.6.1/tests/test_ksuid.py` & `svix-ksuid-0.6.2/tests/test_ksuid.py`

 * *Files identical despite different names*


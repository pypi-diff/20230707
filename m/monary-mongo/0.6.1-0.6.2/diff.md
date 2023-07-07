# Comparing `tmp/monary_mongo-0.6.1.tar.gz` & `tmp/monary_mongo-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monary_mongo-0.6.1.tar", max compression
+gzip compressed data, was "monary_mongo-0.6.2.tar", max compression
```

## Comparing `monary_mongo-0.6.1.tar` & `monary_mongo-0.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    10850 2022-12-18 00:47:34.611553 monary_mongo-0.6.1/LICENSE.TXT
--rw-r--r--   0        0        0     3037 2022-12-18 05:17:48.308193 monary_mongo-0.6.1/build.py
--rw-r--r--   0        0        0      452 2022-12-18 05:09:53.578618 monary_mongo-0.6.1/monary_mongo/__init__.py
--rw-r--r--   0        0        0    46111 2022-12-18 04:56:37.774527 monary_mongo-0.6.1/monary_mongo/cmonary.c
--rw-r--r--   0        0        0     2018 2022-12-18 04:51:59.516624 monary_mongo-0.6.1/monary_mongo/datehelper.py
--rw-r--r--   0        0        0      452 2022-12-18 05:10:00.188565 monary_mongo-0.6.1/monary_mongo/main.py
--rw-r--r--   0        0        0    36991 2022-12-18 05:09:12.928944 monary_mongo-0.6.1/monary_mongo/monary_mongo.py
--rw-r--r--   0        0        0     4509 2022-12-18 05:10:03.411873 monary_mongo-0.6.1/monary_mongo/monary_param.py
--rw-r--r--   0        0        0     8936 2022-12-18 04:51:59.516624 monary_mongo-0.6.1/monary_mongo/ordereddict.py
--rw-r--r--   0        0        0     2880 2022-12-18 05:10:16.621767 monary_mongo-0.6.1/monary_mongo/write_concern.py
--rw-r--r--   0        0        0      822 2022-12-18 07:02:50.941219 monary_mongo-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 monary_mongo-0.6.1/setup.py
--rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 monary_mongo-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10850 2023-07-07 18:16:26.237632 monary_mongo-0.6.2/LICENSE.TXT
+-rw-r--r--   0        0        0     3037 2023-07-07 18:16:26.237632 monary_mongo-0.6.2/build.py
+-rw-r--r--   0        0        0      452 2023-07-07 18:16:26.237632 monary_mongo-0.6.2/monary_mongo/__init__.py
+-rw-r--r--   0        0        0    46111 2023-07-07 18:16:26.237632 monary_mongo-0.6.2/monary_mongo/cmonary.c
+-rw-r--r--   0        0        0     2018 2023-07-07 18:16:26.237632 monary_mongo-0.6.2/monary_mongo/datehelper.py
+-rw-r--r--   0        0        0      452 2023-07-07 18:16:26.237632 monary_mongo-0.6.2/monary_mongo/main.py
+-rw-r--r--   0        0        0    37008 2023-07-07 18:17:39.354570 monary_mongo-0.6.2/monary_mongo/monary_mongo.py
+-rw-r--r--   0        0        0     4509 2023-07-07 18:16:26.240965 monary_mongo-0.6.2/monary_mongo/monary_param.py
+-rw-r--r--   0        0        0     8936 2023-07-07 18:16:26.240965 monary_mongo-0.6.2/monary_mongo/ordereddict.py
+-rw-r--r--   0        0        0     2880 2023-07-07 18:16:26.240965 monary_mongo-0.6.2/monary_mongo/write_concern.py
+-rw-r--r--   0        0        0      822 2023-07-07 18:46:22.975563 monary_mongo-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 monary_mongo-0.6.2/setup.py
+-rw-r--r--   0        0        0      925 1970-01-01 00:00:00.000000 monary_mongo-0.6.2/PKG-INFO
```

### Comparing `monary_mongo-0.6.1/LICENSE.TXT` & `monary_mongo-0.6.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `monary_mongo-0.6.1/build.py` & `monary_mongo-0.6.2/build.py`

 * *Files identical despite different names*

### Comparing `monary_mongo-0.6.1/monary_mongo/cmonary.c` & `monary_mongo-0.6.2/monary_mongo/cmonary.c`

 * *Files identical despite different names*

### Comparing `monary_mongo-0.6.1/monary_mongo/datehelper.py` & `monary_mongo-0.6.2/monary_mongo/datehelper.py`

 * *Files identical despite different names*

### Comparing `monary_mongo-0.6.1/monary_mongo/monary_mongo.py` & `monary_mongo-0.6.2/monary_mongo/monary_mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 cmonary.monary_init()
 atexit.register(cmonary.monary_cleanup)
 
 # Table of type names and conversions between cmonary and numpy types.
 MONARY_TYPES = {
     # "common_name": (cmonary_type_code, numpy_type_object)
     "id":        (1, numpy.dtype("<V12")),
-    "bool":      (2, numpy.bool),
+    "bool":      (2, bool),
     "int8":      (3, numpy.int8),
     "int16":     (4, numpy.int16),
     "int32":     (5, numpy.int32),
     "int64":     (6, numpy.int64),
     "uint8":     (7, numpy.uint8),
     "uint16":    (8, numpy.uint16),
     "uint32":    (9, numpy.uint32),
@@ -412,18 +412,18 @@
                     uri.append("%s@" % username)
                 else:
                     uri.append("%s:%s@" % (username, password))
             elif password is not None:
                 raise ValueError("You cannot have a password with no"
                                  " username.")
 
-            uri.append("%s:%d" % (host, port))
+            uri.append("%s:%d/" % (host, port))
 
             if database is not None:
-                uri.append("/%s" % database)
+                uri.append("%s" % database)
             if options is not None:
                 uri.append("?%s" % urlencode(options))
             uri = "".join(uri)
 
         if sys.version >= "3":
             p_file = bytes(p_file, "ascii") if p_file is not None else None
             pem_pwd = bytes(pem_pwd, "ascii") if pem_pwd is not None else None
@@ -439,14 +439,15 @@
             ctypes.c_char_p(pem_pwd),
             ctypes.c_char_p(ca_file),
             ctypes.c_char_p(ca_dir),
             ctypes.c_char_p(c_file),
             ctypes.c_bool(weak_cert_validation),
             ctypes.byref(err))
         if self._connection is None:
+            print(uri)
             raise MonaryError(err.message)
 
     def _make_column_data(self, fields, types, count):
         """Builds the 'column data' structure used by the underlying cmonary
         code to populate the arrays.  This code must allocate the array
         objects, and provide their corresponding storage pointers and sizes
         to cmonary.
```

### Comparing `monary_mongo-0.6.1/monary_mongo/monary_param.py` & `monary_mongo-0.6.2/monary_mongo/monary_param.py`

 * *Files identical despite different names*

### Comparing `monary_mongo-0.6.1/monary_mongo/ordereddict.py` & `monary_mongo-0.6.2/monary_mongo/ordereddict.py`

 * *Files identical despite different names*

### Comparing `monary_mongo-0.6.1/monary_mongo/write_concern.py` & `monary_mongo-0.6.2/monary_mongo/write_concern.py`

 * *Files identical despite different names*

### Comparing `monary_mongo-0.6.1/pyproject.toml` & `monary_mongo-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monary_mongo"
-version = "0.6.1"
+version = "0.6.2"
 description = "Monary performs high-performance column queries on MongoDB"
 authors = ["Andrew Gigena <mail@andrewgigena.dev>", "David J. C. Beach <info@djcinnovations.com>"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: Unix",
     "Environment :: Console",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `monary_mongo-0.6.1/setup.py` & `monary_mongo-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy']
 
 setup_kwargs = {
     'name': 'monary-mongo',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'Monary performs high-performance column queries on MongoDB',
     'long_description': 'None',
     'author': 'Andrew Gigena',
     'author_email': 'mail@andrewgigena.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/andrewgigena/monary_mongo',
```

### Comparing `monary_mongo-0.6.1/PKG-INFO` & `monary_mongo-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monary-mongo
-Version: 0.6.1
+Version: 0.6.2
 Summary: Monary performs high-performance column queries on MongoDB
 Home-page: https://github.com/andrewgigena/monary_mongo
 Keywords: monary,pymongo,mongo,mongodb,numpy,array
 Author: Andrew Gigena
 Author-email: mail@andrewgigena.dev
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
```


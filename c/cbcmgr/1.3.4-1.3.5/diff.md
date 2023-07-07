# Comparing `tmp/cbcmgr-1.3.4.tar.gz` & `tmp/cbcmgr-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.3.4.tar", last modified: Fri Jul  7 19:46:30 2023, max compression
+gzip compressed data, was "cbcmgr-1.3.5.tar", last modified: Fri Jul  7 20:01:18 2023, max compression
```

## Comparing `cbcmgr-1.3.4.tar` & `cbcmgr-1.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:46:30.191239 cbcmgr-1.3.4/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.4/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 19:46:30.191106 cbcmgr-1.3.4/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.4/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:46:30.152408 cbcmgr-1.3.4/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.4/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.4/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    25554 2023-07-07 19:44:21.000000 cbcmgr-1.3.4/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 19:40:32.000000 cbcmgr-1.3.4/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.4/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.4/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.4/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.4/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.4/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.4/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:46:30.190872 cbcmgr-1.3.4/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 19:46:30.191283 cbcmgr-1.3.4/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 19:30:15.000000 cbcmgr-1.3.4/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:01:18.439053 cbcmgr-1.3.5/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.5/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 20:01:18.438920 cbcmgr-1.3.5/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.5/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:01:18.425428 cbcmgr-1.3.5/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.5/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.5/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    25568 2023-07-07 19:57:58.000000 cbcmgr-1.3.5/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 19:40:32.000000 cbcmgr-1.3.5/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.5/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.5/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.5/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.5/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.5/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.5/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:01:18.438694 cbcmgr-1.3.5/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 20:01:18.439101 cbcmgr-1.3.5/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 20:01:13.000000 cbcmgr-1.3.5/setup.py
```

### Comparing `cbcmgr-1.3.4/LICENSE.txt` & `cbcmgr-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/PKG-INFO` & `cbcmgr-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.4
+Version: 1.3.5
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.4/README.md` & `cbcmgr-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr/cb_connect.py` & `cbcmgr-1.3.5/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr/cb_management.py` & `cbcmgr-1.3.5/cbcmgr/cb_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
         else:
             raise PathMapUpsertError(f"cb_map_upsert: JSON or XML input data is required")
 
         def _cb_upsert(collection, meta_id, doc_data):
             try:
                 upsert_options = UpsertOptions(timeout=timedelta(seconds=timeout))
                 _collection = self._scope.collection(collection)
-                result = _collection.upsert(meta_id, doc_data, upsert_options)
+                result = retry_inline(_collection.upsert, meta_id, doc_data, upsert_options)
                 logger.debug(f"upsert -> {collection}: {meta_id}: cas {result.cas}")
                 return result.cas
             except Exception as error:
                 raise CollectionUpsertError(f"upsert error: {error}")
 
         for c in config.paths:
             logger.debug(f"cb_map_upsert: processing key {c.path} name {c.name}")
```

### Comparing `cbcmgr-1.3.4/cbcmgr/cb_session.py` & `cbcmgr-1.3.5/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr/config.py` & `cbcmgr-1.3.5/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr/exceptions.py` & `cbcmgr-1.3.5/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.3.5/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr/retry.py` & `cbcmgr-1.3.5/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr/schema.py` & `cbcmgr-1.3.5/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr/util.py` & `cbcmgr-1.3.5/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.4/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.3.5/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.4
+Version: 1.3.5
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.4/setup.py` & `cbcmgr-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.3.4',
+    version='1.3.5',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```


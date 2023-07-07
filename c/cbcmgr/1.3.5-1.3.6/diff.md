# Comparing `tmp/cbcmgr-1.3.5.tar.gz` & `tmp/cbcmgr-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.3.5.tar", last modified: Fri Jul  7 20:01:18 2023, max compression
+gzip compressed data, was "cbcmgr-1.3.6.tar", last modified: Fri Jul  7 20:37:01 2023, max compression
```

## Comparing `cbcmgr-1.3.5.tar` & `cbcmgr-1.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:01:18.439053 cbcmgr-1.3.5/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.5/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 20:01:18.438920 cbcmgr-1.3.5/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.5/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:01:18.425428 cbcmgr-1.3.5/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.5/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.5/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    25568 2023-07-07 19:57:58.000000 cbcmgr-1.3.5/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 19:40:32.000000 cbcmgr-1.3.5/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.5/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.5/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.5/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.5/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.5/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.5/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:01:18.438694 cbcmgr-1.3.5/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 20:01:18.000000 cbcmgr-1.3.5/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 20:01:18.439101 cbcmgr-1.3.5/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 20:01:13.000000 cbcmgr-1.3.5/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:37:01.794421 cbcmgr-1.3.6/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.6/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 20:37:01.794245 cbcmgr-1.3.6/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.6/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:37:01.726436 cbcmgr-1.3.6/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.6/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.6/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    26442 2023-07-07 20:36:57.000000 cbcmgr-1.3.6/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 19:40:32.000000 cbcmgr-1.3.6/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.6/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.6/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.6/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.6/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.6/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.6/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 20:37:01.793880 cbcmgr-1.3.6/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 20:37:01.000000 cbcmgr-1.3.6/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 20:37:01.794482 cbcmgr-1.3.6/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 20:33:10.000000 cbcmgr-1.3.6/setup.py
```

### Comparing `cbcmgr-1.3.5/LICENSE.txt` & `cbcmgr-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/PKG-INFO` & `cbcmgr-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.5
+Version: 1.3.6
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.5/README.md` & `cbcmgr-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr/cb_connect.py` & `cbcmgr-1.3.6/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr/cb_management.py` & `cbcmgr-1.3.6/cbcmgr/cb_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def create_bucket(self, name, quota: int = 256, replicas: int = 0):
         if not name:
             raise BucketCreateException(f"bucket name can not be null")
+        self._cluster.wait_until_ready(timedelta(seconds=5), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
         logger.debug(f"create_bucket: create bucket {name}")
         try:
             bm = self._cluster.buckets()
             bm.create_bucket(CreateBucketSettings(name=name,
                                                   bucket_type=BucketType.COUCHBASE,
                                                   storage_backend=StorageBackend.COUCHSTORE,
                                                   num_replicas=replicas,
@@ -89,33 +90,34 @@
             bm.drop_bucket(name)
         except (BucketNotFoundException, BucketDoesNotExistException):
             pass
 
     def create_scope(self, name):
         if not name:
             raise ScopeCreateException(f"scope name can not be null")
+        self._cluster.wait_until_ready(timedelta(seconds=5), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
         logger.debug(f"create_scope: create scope {name}")
         try:
             if name != "_default":
                 cm = self._bucket.collections()
                 cm.create_scope(name, CreateScopeOptions(timeout=timedelta(seconds=25)))
         except ScopeAlreadyExistsException:
             pass
         self.scope(name)
 
     def create_collection(self, name):
         if not name:
             raise CollectionCreateException(f"collection name can not be null")
+        self._cluster.wait_until_ready(timedelta(seconds=5), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
         logger.debug(f"create_collection: create collection {name}")
         try:
             if name != "_default":
                 collection_spec = CollectionSpec(name, scope_name=self._scope.name)
                 cm = self._bucket.collections()
                 cm.create_collection(collection_spec, CreateCollectionOptions(timeout=timedelta(seconds=25)))
-                self._cluster.wait_until_ready(timedelta(seconds=5), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
                 retry_inline(self.get_collection, cm, name)
         except CollectionAlreadyExistsException:
             pass
         self.collection(name)
 
     def get_bucket(self, name: str) -> Optional[BucketSettings]:
         try:
@@ -499,15 +501,15 @@
     def cb_map_upsert(self,
                       prefix: str,
                       config: UpsertMapConfig,
                       json_file: str = None,
                       xml_file: str = None,
                       json_data: str = None,
                       xml_data: str = None,
-                      timeout=10):
+                      timeout=5):
         tasks = set()
         executor = concurrent.futures.ThreadPoolExecutor()
 
         if json_file:
             with open(json_file, mode="r") as json_xml:
                 data = json.load(json_xml)
         elif xml_file:
@@ -527,28 +529,42 @@
                 _collection = self._scope.collection(collection)
                 result = retry_inline(_collection.upsert, meta_id, doc_data, upsert_options)
                 logger.debug(f"upsert -> {collection}: {meta_id}: cas {result.cas}")
                 return result.cas
             except Exception as error:
                 raise CollectionUpsertError(f"upsert error: {error}")
 
+        def _create_collection(c_name):
+            try:
+                collection_spec = CollectionSpec(c_name, scope_name=self._scope.name)
+                cm = self._bucket.collections()
+                cm.create_collection(collection_spec, CreateCollectionOptions(timeout=timedelta(seconds=10)))
+            except CollectionAlreadyExistsException:
+                pass
+            except Exception as error:
+                raise CollectionCreateException(f"collection create error: {error}")
+
+        for c in config.paths:
+            if c.collection:
+                logger.debug(f"cb_map_upsert: creating collection {c.name}")
+                retry_inline(_create_collection, c.name)
+
         for c in config.paths:
             logger.debug(f"cb_map_upsert: processing key {c.path} name {c.name}")
 
             subset = copy_path(c.path, data)
 
             if not subset or len(subset) == 0:
                 if c.optional:
                     continue
                 else:
                     raise PathMapUpsertError(f"path {c.path} not found in source data")
 
             if c.collection:
                 collection_name = c.name
-                self.create_collection(collection_name)
             else:
                 collection_name = self._collection.name
 
             if c.exclude:
                 logger.debug(f"cb_map_upsert: excluding {','.join(c.exclude)}")
                 subset = omit_path(subset, c.exclude)
```

### Comparing `cbcmgr-1.3.5/cbcmgr/cb_session.py` & `cbcmgr-1.3.6/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr/config.py` & `cbcmgr-1.3.6/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr/exceptions.py` & `cbcmgr-1.3.6/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.3.6/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr/retry.py` & `cbcmgr-1.3.6/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr/schema.py` & `cbcmgr-1.3.6/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr/util.py` & `cbcmgr-1.3.6/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.5/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.3.6/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.5
+Version: 1.3.6
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.5/setup.py` & `cbcmgr-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.3.5',
+    version='1.3.6',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```


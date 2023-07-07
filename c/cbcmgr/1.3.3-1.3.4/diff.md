# Comparing `tmp/cbcmgr-1.3.3.tar.gz` & `tmp/cbcmgr-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.3.3.tar", last modified: Fri Jul  7 19:04:37 2023, max compression
+gzip compressed data, was "cbcmgr-1.3.4.tar", last modified: Fri Jul  7 19:46:30 2023, max compression
```

## Comparing `cbcmgr-1.3.3.tar` & `cbcmgr-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:04:37.240563 cbcmgr-1.3.3/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.3/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 19:04:37.240410 cbcmgr-1.3.3/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.3/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:04:37.190570 cbcmgr-1.3.3/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.3/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.3/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    25276 2023-07-07 19:01:23.000000 cbcmgr-1.3.3/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 00:37:37.000000 cbcmgr-1.3.3/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.3/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.3/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.3/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.3/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.3/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.3/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:04:37.240124 cbcmgr-1.3.3/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 19:04:37.240616 cbcmgr-1.3.3/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 19:01:23.000000 cbcmgr-1.3.3/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:46:30.191239 cbcmgr-1.3.4/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.4/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 19:46:30.191106 cbcmgr-1.3.4/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.4/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:46:30.152408 cbcmgr-1.3.4/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.4/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.4/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    25554 2023-07-07 19:44:21.000000 cbcmgr-1.3.4/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 19:40:32.000000 cbcmgr-1.3.4/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.4/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.4/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.4/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.4/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.4/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.4/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:46:30.190872 cbcmgr-1.3.4/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 19:46:30.000000 cbcmgr-1.3.4/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 19:46:30.191283 cbcmgr-1.3.4/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 19:30:15.000000 cbcmgr-1.3.4/setup.py
```

### Comparing `cbcmgr-1.3.3/LICENSE.txt` & `cbcmgr-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/PKG-INFO` & `cbcmgr-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.3
+Version: 1.3.4
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.3/README.md` & `cbcmgr-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/cbcmgr/cb_connect.py` & `cbcmgr-1.3.4/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/cbcmgr/cb_management.py` & `cbcmgr-1.3.4/cbcmgr/cb_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from couchbase.diagnostics import ServiceType, PingState
 from couchbase.management.buckets import CreateBucketSettings, BucketType, StorageBackend, BucketSettings
 from couchbase.management.collections import CollectionSpec
 from couchbase.exceptions import (QueryIndexNotFoundException, QueryIndexAlreadyExistsException, BucketAlreadyExistsException, BucketNotFoundException, BucketDoesNotExistException,
                                   WatchQueryIndexTimeoutException, ScopeAlreadyExistsException, CollectionAlreadyExistsException, CollectionNotFoundException)
 from couchbase.management.queries import (CreateQueryIndexOptions, CreatePrimaryQueryIndexOptions, WatchQueryIndexOptions, DropPrimaryQueryIndexOptions, DropQueryIndexOptions)
 from couchbase.management.options import CreateBucketOptions, CreateScopeOptions, CreateCollectionOptions, GetAllQueryIndexOptions
-from couchbase.options import WaitUntilReadyOptions
+from couchbase.options import WaitUntilReadyOptions, UpsertOptions
 
 logger = logging.getLogger('cbutil.manager')
 logger.addHandler(logging.NullHandler())
 
 
 @attr.s
 class CBQueryIndex(Protocol):
@@ -107,14 +107,15 @@
             raise CollectionCreateException(f"collection name can not be null")
         logger.debug(f"create_collection: create collection {name}")
         try:
             if name != "_default":
                 collection_spec = CollectionSpec(name, scope_name=self._scope.name)
                 cm = self._bucket.collections()
                 cm.create_collection(collection_spec, CreateCollectionOptions(timeout=timedelta(seconds=25)))
+                self._cluster.wait_until_ready(timedelta(seconds=5), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
                 retry_inline(self.get_collection, cm, name)
         except CollectionAlreadyExistsException:
             pass
         self.collection(name)
 
     def get_bucket(self, name: str) -> Optional[BucketSettings]:
         try:
@@ -497,15 +498,16 @@
 
     def cb_map_upsert(self,
                       prefix: str,
                       config: UpsertMapConfig,
                       json_file: str = None,
                       xml_file: str = None,
                       json_data: str = None,
-                      xml_data: str = None):
+                      xml_data: str = None,
+                      timeout=10):
         tasks = set()
         executor = concurrent.futures.ThreadPoolExecutor()
 
         if json_file:
             with open(json_file, mode="r") as json_xml:
                 data = json.load(json_xml)
         elif xml_file:
@@ -517,16 +519,17 @@
         elif xml_data:
             data = xmltodict.parse(xml_data)
         else:
             raise PathMapUpsertError(f"cb_map_upsert: JSON or XML input data is required")
 
         def _cb_upsert(collection, meta_id, doc_data):
             try:
+                upsert_options = UpsertOptions(timeout=timedelta(seconds=timeout))
                 _collection = self._scope.collection(collection)
-                result = _collection.upsert(meta_id, doc_data)
+                result = _collection.upsert(meta_id, doc_data, upsert_options)
                 logger.debug(f"upsert -> {collection}: {meta_id}: cas {result.cas}")
                 return result.cas
             except Exception as error:
                 raise CollectionUpsertError(f"upsert error: {error}")
 
         for c in config.paths:
             logger.debug(f"cb_map_upsert: processing key {c.path} name {c.name}")
```

### Comparing `cbcmgr-1.3.3/cbcmgr/cb_session.py` & `cbcmgr-1.3.4/cbcmgr/cb_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,19 +45,19 @@
         self.node_cycle = None
         self.cluster_info = None
         self.sw_version = None
         self.memory_quota = None
         self.cluster_services = []
         self.auth = PasswordAuthenticator(self.username, self.password)
         self.timeouts = ClusterTimeoutOptions(query_timeout=timedelta(seconds=60),
-                                              kv_timeout=timedelta(seconds=4),
-                                              bootstrap_timeout=timedelta(seconds=4),
-                                              resolve_timeout=timedelta(seconds=4),
-                                              connect_timeout=timedelta(seconds=4),
-                                              management_timeout=timedelta(seconds=4))
+                                              kv_timeout=timedelta(seconds=5),
+                                              bootstrap_timeout=timedelta(seconds=5),
+                                              resolve_timeout=timedelta(seconds=5),
+                                              connect_timeout=timedelta(seconds=5),
+                                              management_timeout=timedelta(seconds=5))
 
         if self.ssl:
             self.prefix = "https://"
             self.cb_prefix = "couchbases://"
             self.srv_prefix = "_couchbases._tcp."
             self.admin_port = "18091"
             self.node_port = "19102"
```

### Comparing `cbcmgr-1.3.3/cbcmgr/config.py` & `cbcmgr-1.3.4/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/cbcmgr/exceptions.py` & `cbcmgr-1.3.4/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.3.4/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/cbcmgr/retry.py` & `cbcmgr-1.3.4/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/cbcmgr/schema.py` & `cbcmgr-1.3.4/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/cbcmgr/util.py` & `cbcmgr-1.3.4/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.3/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.3.4/cbcmgr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.3
+Version: 1.3.4
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.3/setup.py` & `cbcmgr-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.3.3',
+    version='1.3.4',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```


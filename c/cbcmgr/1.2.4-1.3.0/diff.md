# Comparing `tmp/cbcmgr-1.2.4.tar.gz` & `tmp/cbcmgr-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.2.4.tar", last modified: Mon Jun 12 14:43:06 2023, max compression
+gzip compressed data, was "cbcmgr-1.3.0.tar", last modified: Fri Jul  7 00:46:37 2023, max compression
```

## Comparing `cbcmgr-1.2.4.tar` & `cbcmgr-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:43:06.391038 cbcmgr-1.2.4/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.2.4/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-06-12 14:43:06.390906 cbcmgr-1.2.4/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.2.4/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:43:06.378163 cbcmgr-1.2.4/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.2.4/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.2.4/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.2.4/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.2.4/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     4197 2023-06-12 14:40:15.000000 cbcmgr-1.2.4/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.2.4/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.2.4/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.2.4/cbcmgr/schema.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:43:06.390664 cbcmgr-1.2.4/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      343 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       57 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-12 14:43:06.391085 cbcmgr-1.2.4/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      705 2023-06-12 14:43:01.000000 cbcmgr-1.2.4/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 00:46:37.648951 cbcmgr-1.3.0/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.0/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-07-07 00:46:37.648679 cbcmgr-1.3.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.0/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 00:46:37.429793 cbcmgr-1.3.0/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.0/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.0/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    21613 2023-07-07 00:36:53.000000 cbcmgr-1.3.0/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 00:37:37.000000 cbcmgr-1.3.0/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     1781 2023-07-07 00:05:02.000000 cbcmgr-1.3.0/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.0/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.0/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.0/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.0/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)      502 2023-07-07 00:16:42.000000 cbcmgr-1.3.0/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 00:46:37.647825 cbcmgr-1.3.0/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       57 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 00:46:37.649042 cbcmgr-1.3.0/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      705 2023-07-07 00:39:27.000000 cbcmgr-1.3.0/setup.py
```

### Comparing `cbcmgr-1.2.4/LICENSE.txt` & `cbcmgr-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.4/PKG-INFO` & `cbcmgr-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.2.4
+Version: 1.3.0
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.2.4/README.md` & `cbcmgr-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.4/cbcmgr/cb_connect.py` & `cbcmgr-1.3.0/cbcmgr/cb_connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 from .exceptions import (CollectionNameNotFound, IndexExistsError, QueryArgumentsError, QueryEmptyException, ClusterNotConnected, BucketNotConnected,
                          ScopeNotConnected, CollectionSubdocUpsertError, BucketWaitException, BucketStatsError, CollectionCountException, CollectionCountError)
 from .retry import retry, retry_inline
 from .cb_session import CBSession
 from .httpsessionmgr import APISession
 from datetime import timedelta
 from typing import Union, Dict, Any, List
+import logging
 import concurrent.futures
 from couchbase.cluster import Cluster
 import couchbase.subdocument as SD
-from couchbase.exceptions import (CouchbaseException, QueryIndexNotFoundException, DocumentNotFoundException, DocumentExistsException, QueryIndexAlreadyExistsException)
+from couchbase.exceptions import (CouchbaseException, QueryIndexNotFoundException, DocumentNotFoundException, DocumentExistsException, QueryIndexAlreadyExistsException,
+                                  PathNotFoundException)
 from couchbase.options import (QueryOptions, LockMode, ClusterOptions, TLSVerifyMode, WaitUntilReadyOptions)
 from couchbase.management.options import GetAllQueryIndexOptions
 from couchbase.management.queries import CreatePrimaryQueryIndexOptions, DropPrimaryQueryIndexOptions
 from couchbase.diagnostics import ServiceType
 
+logger = logging.getLogger('cbutil.connect')
+logger.addHandler(logging.NullHandler())
 JSONType = Union[str, int, float, bool, None, Dict[str, Any], List[Any]]
 
 
 class CBConnect(CBSession):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -32,42 +36,42 @@
                                               lockmode=LockMode.WAIT)
         if self.use_external_network:
             self.cluster_options.update(network="external")
         else:
             self.cluster_options.update(network="default")
 
     def connect(self, bucket: str = None, scope: str = "_default", collection: str = "_default"):
-        self.logger.debug(f"connect: connect string {self.cb_connect_string}")
+        logger.debug(f"connect: connect string {self.cb_connect_string}")
         self._cluster = Cluster.connect(self.cb_connect_string, self.cluster_options)
         self._cluster.wait_until_ready(timedelta(seconds=4), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue, ServiceType.Management]))
         if bucket:
             self.bucket(bucket)
             self.scope(scope)
             self.collection(collection)
         return self
 
     def bucket(self, name: str):
-        self.logger.debug(f"bucket: connecting bucket {name}")
+        logger.debug(f"bucket: connecting bucket {name}")
         if self._cluster:
             self._bucket = retry_inline(self._cluster.bucket, name)
         else:
             raise ClusterNotConnected("no cluster connected")
 
     def scope(self, name: str = "_default"):
         if self._bucket:
-            self.logger.debug(f"scope: connecting scope {name}")
+            logger.debug(f"scope: connecting scope {name}")
             self._cluster.wait_until_ready(timedelta(seconds=4), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
             self._scope = self._bucket.scope(name)
             self._scope_name = name
         else:
             raise BucketNotConnected("bucket not connected")
 
     def collection(self, name: str = "_default"):
         if self._scope:
-            self.logger.debug(f"collection: connecting collection {name}")
+            logger.debug(f"collection: connecting collection {name}")
             self._cluster.wait_until_ready(timedelta(seconds=4), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
             self._collection = self._scope.collection(name)
             self._collection_name = name
         else:
             raise ScopeNotConnected("scope not connected")
 
     @retry()
@@ -139,37 +143,62 @@
             return False
 
     @retry()
     def cb_get(self, key: Union[int, str]):
         try:
             document_id = self.construct_key(key)
             result = self._collection.get(document_id)
-            self.logger.debug(f"cb_get: {document_id}: cas {result.cas}")
+            logger.debug(f"cb_get: {document_id}: cas {result.cas}")
             return result.content_as[dict]
         except DocumentNotFoundException:
             return None
 
     @retry()
     def cb_upsert(self, key: Union[int, str], document: JSONType):
         try:
-            self.logger.debug(f"cb_upsert: key {key}")
+            logger.debug(f"cb_upsert: key {key}")
             document_id = self.construct_key(key)
             result = self._collection.upsert(document_id, document)
-            self.logger.debug(f"cb_upsert: {document_id}: cas {result.cas}")
+            logger.debug(f"cb_upsert: {document_id}: cas {result.cas}")
             return result
         except DocumentExistsException:
             return None
 
     @retry()
     def cb_subdoc_upsert(self, key: Union[int, str], field: str, value: JSONType):
         document_id = self.construct_key(key)
         result = self._collection.mutate_in(document_id, [SD.upsert(field, value)])
-        self.logger.debug(f"cb_subdoc_upsert: {document_id}: cas {result.cas}")
+        logger.debug(f"cb_subdoc_upsert: {document_id}: cas {result.cas}")
         return result.content_as[dict]
 
+    def cb_path_upsert(self, doc_id: str, path: str, data: JSONType):
+        root = False
+        path_v = path.split('.')
+        if len(path_v[0]) == 0:
+            root = True
+
+        while True:
+            try:
+                if root:
+                    self._collection.upsert(doc_id, data)
+                else:
+                    self._collection.mutate_in(doc_id, (SD.upsert(path, data),))
+                break
+            except DocumentNotFoundException:
+                self._collection.upsert(doc_id, {})
+            except PathNotFoundException:
+                for n in range(len(path_v)):
+                    p_path = '.'.join(path_v[:n + 1])
+                    r = self._collection.lookup_in(doc_id, (SD.exists(p_path),))
+                    if not r.exists(0):
+                        self._collection.mutate_in(doc_id, (SD.upsert(p_path, {}),))
+            except Exception as err:
+                print(f"Error: {err}")
+                break
+
     @retry()
     def cb_subdoc_multi_upsert(self, key_list: list, field: str, value_list: list):
         tasks = set()
         executor = concurrent.futures.ThreadPoolExecutor()
         for n in range(len(key_list)):
             tasks.add(executor.submit(self.cb_subdoc_upsert, key_list[n], field, value_list[n]))
         while tasks:
@@ -194,15 +223,15 @@
     @retry(
         always_raise_list=(CollectionNameNotFound, QueryArgumentsError, IndexExistsError, QueryIndexNotFoundException))
     def cb_query(self, field: str = None, where: str = None, value: str = None, sql: str = None, empty_retry: bool = False):
         query = self.query_sql_constructor(field, where, value, sql)
         contents = []
         try:
             self._cluster.wait_until_ready(timedelta(seconds=4), WaitUntilReadyOptions(service_types=[ServiceType.Query]))
-            self.logger.debug(f"cb_query: running query: {query}")
+            logger.debug(f"cb_query: running query: {query}")
             result = self._cluster.query(query, QueryOptions(metrics=False, adhoc=True))
             for item in result:
                 contents.append(item)
             if empty_retry:
                 if len(contents) == 0:
                     raise QueryEmptyException(f"query did not return any results")
             return contents
```

### Comparing `cbcmgr-1.2.4/cbcmgr/cb_management.py` & `cbcmgr-1.3.0/cbcmgr/cb_management.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 ##
 ##
 
-from .exceptions import (IndexNotReady, IndexNotFoundError, CollectionNameNotFound, IndexStatError, ClusterHealthCheckError)
+from .exceptions import (IndexNotReady, IndexNotFoundError, CollectionNameNotFound, IndexStatError, ClusterHealthCheckError, PathMapUpsertError)
 from .retry import retry, retry_inline
 from .cb_connect import CBConnect
+from .util import r_getattr, omit_path
+from .config import UpsertMapConfig, MapUpsertType
 from datetime import timedelta
 import attr
 import hashlib
+import logging
 from attr.validators import instance_of as io, optional
-from typing import Protocol, Iterable, Optional
+from typing import Protocol, Iterable, Optional, Any
 from couchbase.cluster import Cluster
 from couchbase.options import QueryOptions
 from couchbase.diagnostics import ServiceType, PingState
 from couchbase.management.buckets import CreateBucketSettings, BucketType, StorageBackend, BucketSettings
 from couchbase.management.collections import CollectionSpec
 from couchbase.exceptions import (QueryIndexNotFoundException, QueryIndexAlreadyExistsException, BucketAlreadyExistsException, BucketNotFoundException, BucketDoesNotExistException,
                                   WatchQueryIndexTimeoutException, ScopeAlreadyExistsException, CollectionAlreadyExistsException, CollectionNotFoundException)
 from couchbase.management.queries import (CreateQueryIndexOptions, CreatePrimaryQueryIndexOptions, WatchQueryIndexOptions, DropPrimaryQueryIndexOptions, DropQueryIndexOptions)
 from couchbase.management.options import CreateBucketOptions, CreateScopeOptions, CreateCollectionOptions, GetAllQueryIndexOptions
 from couchbase.options import WaitUntilReadyOptions
 
+logger = logging.getLogger('cbutil.manager')
+logger.addHandler(logging.NullHandler())
+
 
 @attr.s
 class CBQueryIndex(Protocol):
     name = attr.ib(validator=io(str))
     is_primary = attr.ib(validator=io(bool))
     state = attr.ib(validator=io(str))
     namespace = attr.ib(validator=io(str))
@@ -53,47 +59,47 @@
 
 class CBManager(CBConnect):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def create_bucket(self, name, quota: int = 256, replicas: int = 0):
-        self.logger.debug(f"create_bucket: create bucket {name}")
+        logger.debug(f"create_bucket: create bucket {name}")
         try:
             bm = self._cluster.buckets()
             bm.create_bucket(CreateBucketSettings(name=name,
                                                   bucket_type=BucketType.COUCHBASE,
                                                   storage_backend=StorageBackend.COUCHSTORE,
                                                   num_replicas=replicas,
                                                   ram_quota_mb=quota),
                              CreateBucketOptions(timeout=timedelta(seconds=25)))
         except BucketAlreadyExistsException:
             pass
         self.bucket(name)
 
     def drop_bucket(self, name):
-        self.logger.debug(f"drop_bucket: drop bucket {name}")
+        logger.debug(f"drop_bucket: drop bucket {name}")
         try:
             bm = self._cluster.buckets()
             bm.drop_bucket(name)
         except (BucketNotFoundException, BucketDoesNotExistException):
             pass
 
     def create_scope(self, name):
-        self.logger.debug(f"create_scope: create scope {name}")
+        logger.debug(f"create_scope: create scope {name}")
         try:
             if name != "_default":
                 cm = self._bucket.collections()
                 cm.create_scope(name, CreateScopeOptions(timeout=timedelta(seconds=25)))
         except ScopeAlreadyExistsException:
             pass
         self.scope(name)
 
     def create_collection(self, name):
-        self.logger.debug(f"create_collection: create collection {name}")
+        logger.debug(f"create_collection: create collection {name}")
         try:
             if name != "_default":
                 collection_spec = CollectionSpec(name, scope_name=self._scope.name)
                 cm = self._bucket.collections()
                 cm.create_collection(collection_spec, CreateCollectionOptions(timeout=timedelta(seconds=25)))
                 retry_inline(self.get_collection, cm, name)
         except CollectionAlreadyExistsException:
@@ -119,15 +125,15 @@
         if not collection:
             raise CollectionNameNotFound(f"collection {collection_name} not found")
         else:
             return collection
 
     @retry()
     def drop_collection(self, name):
-        self.logger.debug(f"drop_collection: drop collection {name}")
+        logger.debug(f"drop_collection: drop collection {name}")
         try:
             collection_spec = CollectionSpec(name, scope_name=self._scope.name)
             cm = self._bucket.collections()
             cm.drop_collection(collection_spec)
         except CollectionNotFoundException:
             pass
 
@@ -211,27 +217,27 @@
                         {
                             "name": b.name,
                             "scopes": []
                         }
                     ]
                 }
             }
-            self.logger.debug(f"scanning bucket {b.name}")
+            logger.debug(f"scanning bucket {b.name}")
             bucket = cluster.bucket(b.name)
             cm = bucket.collections()
             scopes = cm.get_all_scopes()
             for s in scopes:
                 schema_scope = {
                     "name": s.name,
                     "collections": []
                 }
-                self.logger.debug(f"scanning scope {s.name}")
+                logger.debug(f"scanning scope {s.name}")
                 collections = s.collections
                 for c in collections:
-                    self.logger.debug(f"scanning collection {c.name}")
+                    logger.debug(f"scanning collection {c.name}")
                     primary_index = False
                     index_get_options = GetAllQueryIndexOptions(scope_name=s.name, collection_name=c.name)
                     indexes = qim.get_all_indexes(b.name, index_get_options)
                     index_names = list(map(lambda i: i.name, [index for index in indexes]))
                     index_keys_lists = list(map(lambda i: i.index_key, [index for index in indexes]))
                     index_keys = [item.strip('`') for sublist in index_keys_lists for item in sublist]
                     if '#primary' in index_names:
@@ -269,15 +275,15 @@
                                                            num_replicas=replica,
                                                            collection_name=self._collection.name,
                                                            scope_name=self._scope.name)
         else:
             index_options = CreatePrimaryQueryIndexOptions(deferred=False,
                                                            timeout=timedelta(seconds=timeout),
                                                            num_replicas=replica)
-        self.logger.debug(
+        logger.debug(
             f"cb_create_primary_index: creating primary index on {self._collection.name}")
         try:
             qim = self._cluster.query_indexes()
             qim.create_primary_index(self._bucket.name, index_options)
         except QueryIndexAlreadyExistsException:
             pass
 
@@ -292,30 +298,30 @@
         else:
             index_options = CreateQueryIndexOptions(deferred=False,
                                                     timeout=timedelta(seconds=timeout),
                                                     num_replicas=replica)
         try:
             index_name = self.index_name(fields)
             qim = self._cluster.query_indexes()
-            self.logger.debug(
+            logger.debug(
                 f"creating index {index_name} on {','.join(fields)} for {self.keyspace}")
             qim.create_index(self._bucket.name, index_name, fields, index_options)
             return index_name
         except QueryIndexAlreadyExistsException:
             pass
 
     @retry()
     def cb_drop_primary_index(self, timeout: int = 120):
         if self._collection_name != '_default':
             index_options = DropPrimaryQueryIndexOptions(timeout=timedelta(seconds=timeout),
                                                          collection_name=self._collection.name,
                                                          scope_name=self._scope.name)
         else:
             index_options = DropPrimaryQueryIndexOptions(timeout=timedelta(seconds=timeout))
-        self.logger.debug(f"cb_drop_primary_index: dropping primary index on {self.collection_name}")
+        logger.debug(f"cb_drop_primary_index: dropping primary index on {self.collection_name}")
         try:
             qim = self._cluster.query_indexes()
             qim.drop_primary_index(self._bucket.name, index_options)
         except QueryIndexNotFoundException:
             pass
 
     @retry()
@@ -323,15 +329,15 @@
         if self._collection_name != '_default':
             index_options = DropQueryIndexOptions(timeout=timedelta(seconds=timeout),
                                                   collection_name=self._collection.name,
                                                   scope_name=self._scope.name)
         else:
             index_options = DropQueryIndexOptions(timeout=timedelta(seconds=timeout))
         try:
-            self.logger.debug(f"cb_drop_index: drop index {name}")
+            logger.debug(f"cb_drop_index: drop index {name}")
             qim = self._cluster.query_indexes()
             qim.drop_index(self._bucket.name, name, index_options)
         except QueryIndexNotFoundException:
             pass
 
     @retry()
     def index_list_all(self):
@@ -432,7 +438,49 @@
         except Exception as err:
             raise IndexNotReady(f"index_list: bucket {self._bucket.name} error: {err}")
 
     @retry(factor=0.5, allow_list=(IndexNotReady,))
     def delete_wait(self, index_name: str = None):
         if self.is_index(index_name=index_name):
             raise IndexNotReady(f"delete_wait: index still exists")
+
+    def cb_map_upsert(self, prefix: str, config: UpsertMapConfig, attr_obj: Any):
+        primitive = (int, str, bool, list, dict)
+        value = None
+        for c in config.paths:
+            logger.debug(f"cb_map_upsert: processing key {c.path} name {c.name}")
+            try:
+                subset = r_getattr(attr_obj, c.path)
+                if isinstance(subset, list):
+                    if not any(isinstance(item, primitive) for item in subset):
+                        value = []
+                        for item in subset:
+                            value.append(item.as_dict)
+                elif isinstance(subset, primitive) or not subset:
+                    value = subset
+                else:
+                    value = subset.as_dict
+
+                if c.collection:
+                    self.create_collection(c.name)
+
+                if c.exclude:
+                    logger.debug(f"cb_map_upsert: excluding {','.join(c.exclude)}")
+                    value = omit_path(value, c.exclude)
+
+                if c.p_type == MapUpsertType.DOCUMENT:
+                    doc_id = self.key_format(c.id, value, text=prefix)
+                    logger.debug(f"cb_map_upsert: processing doc ID {doc_id}")
+                    self._collection.upsert(doc_id, {c.name: value})
+                elif c.p_type == MapUpsertType.LIST:
+                    logger.debug(f"cb_map_upsert: processing list")
+                    if not isinstance(value, list):
+                        raise PathMapUpsertError(f"cb_map_upsert: path {c.path} type {type(value)} incompatible with list mode")
+                    for doc in value:
+                        doc_id = self.key_format(c.id, doc, text=prefix, id_key=c.id_key)
+                        self._collection.upsert(doc_id, doc)
+
+            except AttributeError:
+                raise PathMapUpsertError(f"cb_map_upsert: key {c.path} not found")
+
+            except Exception as err:
+                raise PathMapUpsertError(f"cb_map_upsert: error {err}")
```

### Comparing `cbcmgr-1.2.4/cbcmgr/cb_session.py` & `cbcmgr-1.3.0/cbcmgr/cb_session.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 ##
 ##
 
-from .exceptions import (DNSLookupTimeout, NodeUnreachable, NodeConnectionTimeout, NodeConnectionError, NodeConnectionFailed, ClusterHealthCheckError)
+from .exceptions import (DNSLookupTimeout, NodeUnreachable, NodeConnectionTimeout, NodeConnectionError, NodeConnectionFailed, ClusterHealthCheckError, KeyFormatError)
 from .retry import retry
 from .httpsessionmgr import APISession
+from .config import KeyStyle
 import logging
 import socket
 import dns.resolver
+import uuid
+from typing import Union
 from datetime import timedelta
 from couchbase.auth import PasswordAuthenticator
 from couchbase.options import ClusterTimeoutOptions, ClusterOptions, LockMode
 from couchbase.cluster import Cluster
 from couchbase.diagnostics import ServiceType, PingState
 
+logger = logging.getLogger('cbutil.session')
+logger.addHandler(logging.NullHandler())
+
 
 class CBSession(object):
 
     def __init__(self, hostname: str, username: str, password: str, ssl=False, external=False):
         self.cluster_node_count = None
-        self.logger = logging.getLogger(self.__class__.__name__)
         self._cluster = None
         self._bucket = None
         self._scope = None
         self._collection = None
         self._scope_name = "_default"
         self._collection_name = "_default"
         self.username = username
@@ -85,24 +90,24 @@
             return self._bucket.name
         else:
             return self._collection_name
 
     @property
     def cb_connect_string(self):
         connect_string = self.cb_prefix + self.rally_host_name
-        self.logger.debug(f"Connect string: {connect_string}")
+        logger.debug(f"Connect string: {connect_string}")
         return connect_string
 
     @retry(retry_count=5)
     def is_reachable(self):
         resolver = dns.resolver.Resolver()
         resolver.timeout = 5
         resolver.lifetime = 10
 
-        self.logger.debug(f"checking if rally node is reachable: {self.rally_host_name}")
+        logger.debug(f"checking if rally node is reachable: {self.rally_host_name}")
         try:
             answer = resolver.resolve(self.srv_prefix + self.rally_host_name, "SRV")
             for srv in answer:
                 record = {'hostname': str(srv.target).rstrip('.')}
                 host_answer = resolver.resolve(record['hostname'], 'A')
                 record['address'] = host_answer[0].address
                 self.srv_host_list.append(record)
@@ -113,15 +118,15 @@
         except dns.exception.Timeout:
             raise DNSLookupTimeout(f"{self.srv_prefix + self.rally_host_name} lookup timeout")
         except Exception:
             raise
 
         if self.rally_dns_domain:
             self.rally_cluster_node = self.rally_host_name = self.srv_host_list[0]['hostname']
-            self.logger.debug(f"Rewriting rally node as {self.rally_cluster_node}")
+            logger.debug(f"Rewriting rally node as {self.rally_cluster_node}")
 
         try:
             self.check_node_connectivity(self.rally_cluster_node, self.admin_port)
         except (NodeConnectionTimeout, NodeConnectionError, NodeConnectionFailed) as err:
             raise NodeUnreachable(f"can not connect to node {self.rally_cluster_node}: {err}")
 
         return True
@@ -132,29 +137,29 @@
         self.cluster_info = s.api_get('/pools/default').json()
         self.process_cluster_data()
 
     def process_cluster_data(self):
         rally_ip = socket.gethostbyname(self.rally_host_name)
 
         if not self.cluster_info:
-            self.logger.debug("process_cluster_data: no cluster info")
+            logger.debug("process_cluster_data: no cluster info")
             return
 
         self.cluster_node_count = range(len(self.cluster_info['nodes']))
         self.sw_version = self.cluster_info['nodes'][0]['version']
 
         for node in self.cluster_info['nodes']:
             node_name = node.get("configuredHostname").split(':')[0]
             alternate_address = node.get("alternateAddresses", {}).get("external", {}).get("hostname")
             self.node_list.append(node_name)
             if alternate_address:
                 self.external_list.append(alternate_address)
                 external_ip = socket.gethostbyname(alternate_address)
                 if rally_ip == external_ip:
-                    self.logger.debug(f"external address {rally_ip} detected")
+                    logger.debug(f"external address {rally_ip} detected")
                     self.use_external_network = True
 
     @retry(retry_count=5)
     def check_node_connectivity(self, hostname, port):
         try:
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             sock.settimeout(1)
@@ -172,26 +177,26 @@
 
     @retry(factor=0.5)
     def wait_until_ready(self):
         nodes = []
         cluster = Cluster(self.cb_connect_string, ClusterOptions(self.auth,
                                                                  timeout_options=self.timeouts,
                                                                  lockmode=LockMode.WAIT))
-        self.logger.debug(f"cluster {self.cb_connect_string} ping")
+        logger.debug(f"cluster {self.cb_connect_string} ping")
         ping_result = cluster.ping()
         endpoint: ServiceType
         for endpoint, reports in ping_result.endpoints.items():
             for report in reports:
                 remote = report.remote.split(":")[0]
                 nodes.append(remote)
                 if not report.state == PingState.OK:
                     raise ClusterHealthCheckError(f"service {endpoint.value} not ok")
 
         node_set = set(nodes)
-        self.logger.debug("ping complete")
+        logger.debug("ping complete")
         return list(node_set)
 
     def print_host_map(self):
         if self.rally_dns_domain:
             print("Name %s is a domain with SRV records:" % self.rally_host_name)
             for record in self.srv_host_list:
                 print(" => %s (%s)" % (record['hostname'], record['address']))
@@ -211,7 +216,54 @@
             print(" [%02d] %s" % (i + 1, host_name), end=' ')
             if ext_host_name:
                 print("[external]> %s" % ext_host_name, end=' ')
             if ext_port_list:
                 for key in ext_port_list:
                     print("%s:%s" % (key, ext_port_list[key]), end=' ')
             print("[Services] %s [version] %s [platform] %s" % (services, version, ostype))
+
+    def key_format(self,
+                   style: KeyStyle,
+                   document: dict,
+                   doc_num: int = 1,
+                   id_key: str = "record_id",
+                   separator: str = "::",
+                   text: Union[str, None] = None,
+                   path: Union[str, None] = None,
+                   field: Union[str, None] = None):
+        if style.value == 0:
+            return f"{self.keyspace}{separator}{doc_num}"
+        elif style.value == 1:
+            if not document.get('type'):
+                raise KeyFormatError(f"Key style type requested: document does not have type field")
+            if document.get(id_key):
+                number = document.get(id_key)
+            else:
+                number = doc_num
+            return f"{document['type']}{separator}{number}"
+        elif style.value == 2:
+            return uuid.uuid4()
+        elif style.value == 3:
+            if not field:
+                raise KeyFormatError(f"Key field name style requested: field parameter is null")
+            return f"{field}{separator}{doc_num}"
+        elif style.value == 4:
+            return f"{self.keyspace}{separator}{doc_num}"
+        elif style.value == 5:
+            if not field:
+                raise KeyFormatError(f"Key compound name style requested: field parameter is null")
+            return f"{self.keyspace}{separator}{field}{separator}{doc_num}"
+        elif style.value == 6:
+            if not path or not text:
+                raise KeyFormatError(f"Key path style parameters not provided")
+            return f"{text}{separator}{path}"
+        elif style.value == 7:
+            if not text:
+                raise KeyFormatError(f"Key text style parameter not provided")
+            return f"{text}"
+        elif style.value == 8:
+            if not text:
+                raise KeyFormatError(f"Key text style parameter not provided")
+            number = document.get(id_key, 1)
+            return f"{text}{separator}{id_key}{separator}{number}"
+        else:
+            raise KeyFormatError(f"Unknown key style {style.name}")
```

### Comparing `cbcmgr-1.2.4/cbcmgr/exceptions.py` & `cbcmgr-1.3.0/cbcmgr/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,7 +308,15 @@
 
 class CollectionNotConnected(CBException):
     pass
 
 
 class SchemaFileError(CBException):
     pass
+
+
+class KeyFormatError(CBException):
+    pass
+
+
+class PathMapUpsertError(CBException):
+    pass
```

### Comparing `cbcmgr-1.2.4/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.3.0/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.4/cbcmgr/retry.py` & `cbcmgr-1.3.0/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.4/cbcmgr/schema.py` & `cbcmgr-1.3.0/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.4/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.3.0/cbcmgr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.2.4
+Version: 1.3.0
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.2.4/setup.py` & `cbcmgr-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.2.4',
+    version='1.3.0',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```


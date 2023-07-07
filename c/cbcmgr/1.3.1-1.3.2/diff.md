# Comparing `tmp/cbcmgr-1.3.1.tar.gz` & `tmp/cbcmgr-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.3.1.tar", last modified: Fri Jul  7 16:50:14 2023, max compression
+gzip compressed data, was "cbcmgr-1.3.2.tar", last modified: Fri Jul  7 18:12:16 2023, max compression
```

## Comparing `cbcmgr-1.3.1.tar` & `cbcmgr-1.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 16:50:14.748003 cbcmgr-1.3.1/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.1/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-07-07 16:50:14.747884 cbcmgr-1.3.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.1/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 16:50:14.735967 cbcmgr-1.3.1/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.1/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.1/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    24565 2023-07-07 16:30:04.000000 cbcmgr-1.3.1/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 00:37:37.000000 cbcmgr-1.3.1/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     1862 2023-07-07 16:40:09.000000 cbcmgr-1.3.1/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.1/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.1/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.1/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.1/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.1/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 16:50:14.747678 cbcmgr-1.3.1/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 16:50:14.748043 cbcmgr-1.3.1/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      726 2023-07-07 16:44:25.000000 cbcmgr-1.3.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 18:12:16.870164 cbcmgr-1.3.2/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.2/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 18:12:16.870024 cbcmgr-1.3.2/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.2/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 18:12:16.835739 cbcmgr-1.3.2/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.2/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.2/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    24947 2023-07-07 18:03:28.000000 cbcmgr-1.3.2/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 00:37:37.000000 cbcmgr-1.3.2/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     1862 2023-07-07 16:40:09.000000 cbcmgr-1.3.2/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.2/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.2/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.2/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.2/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.2/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 18:12:16.869762 cbcmgr-1.3.2/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 18:12:16.870217 cbcmgr-1.3.2/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 18:11:57.000000 cbcmgr-1.3.2/setup.py
```

### Comparing `cbcmgr-1.3.1/LICENSE.txt` & `cbcmgr-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/README.md` & `cbcmgr-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/cbcmgr/cb_connect.py` & `cbcmgr-1.3.2/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/cbcmgr/cb_management.py` & `cbcmgr-1.3.2/cbcmgr/cb_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ##
 ##
 
-from .exceptions import (IndexNotReady, IndexNotFoundError, CollectionNameNotFound, IndexStatError, ClusterHealthCheckError, PathMapUpsertError, CollectionUpsertError)
+from .exceptions import (IndexNotReady, IndexNotFoundError, CollectionNameNotFound, IndexStatError, ClusterHealthCheckError, PathMapUpsertError, CollectionUpsertError,
+                         ScopeCreateException, BucketCreateException, CollectionCreateException)
 from .retry import retry, retry_inline
 from .cb_connect import CBConnect
 from .util import r_getattr, omit_path, copy_path
 from .config import UpsertMapConfig, MapUpsertType
 from datetime import timedelta
 import attr
 import hashlib
@@ -62,14 +63,16 @@
 
 class CBManager(CBConnect):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def create_bucket(self, name, quota: int = 256, replicas: int = 0):
+        if not name:
+            raise BucketCreateException(f"bucket name can not be null")
         logger.debug(f"create_bucket: create bucket {name}")
         try:
             bm = self._cluster.buckets()
             bm.create_bucket(CreateBucketSettings(name=name,
                                                   bucket_type=BucketType.COUCHBASE,
                                                   storage_backend=StorageBackend.COUCHSTORE,
                                                   num_replicas=replicas,
@@ -84,24 +87,28 @@
         try:
             bm = self._cluster.buckets()
             bm.drop_bucket(name)
         except (BucketNotFoundException, BucketDoesNotExistException):
             pass
 
     def create_scope(self, name):
+        if not name:
+            raise ScopeCreateException(f"scope name can not be null")
         logger.debug(f"create_scope: create scope {name}")
         try:
             if name != "_default":
                 cm = self._bucket.collections()
                 cm.create_scope(name, CreateScopeOptions(timeout=timedelta(seconds=25)))
         except ScopeAlreadyExistsException:
             pass
         self.scope(name)
 
     def create_collection(self, name):
+        if not name:
+            raise CollectionCreateException(f"collection name can not be null")
         logger.debug(f"create_collection: create collection {name}")
         try:
             if name != "_default":
                 collection_spec = CollectionSpec(name, scope_name=self._scope.name)
                 cm = self._bucket.collections()
                 cm.create_collection(collection_spec, CreateCollectionOptions(timeout=timedelta(seconds=25)))
                 retry_inline(self.get_collection, cm, name)
```

### Comparing `cbcmgr-1.3.1/cbcmgr/cb_session.py` & `cbcmgr-1.3.2/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/cbcmgr/config.py` & `cbcmgr-1.3.2/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/cbcmgr/exceptions.py` & `cbcmgr-1.3.2/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.3.2/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/cbcmgr/retry.py` & `cbcmgr-1.3.2/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/cbcmgr/schema.py` & `cbcmgr-1.3.2/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.1/cbcmgr/util.py` & `cbcmgr-1.3.2/cbcmgr/util.py`

 * *Files identical despite different names*


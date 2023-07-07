# Comparing `tmp/cbcmgr-1.3.0.tar.gz` & `tmp/cbcmgr-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.3.0.tar", last modified: Fri Jul  7 00:46:37 2023, max compression
+gzip compressed data, was "cbcmgr-1.3.1.tar", last modified: Fri Jul  7 16:50:14 2023, max compression
```

## Comparing `cbcmgr-1.3.0.tar` & `cbcmgr-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 00:46:37.648951 cbcmgr-1.3.0/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.0/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-07-07 00:46:37.648679 cbcmgr-1.3.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 00:46:37.429793 cbcmgr-1.3.0/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.0/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.0/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    21613 2023-07-07 00:36:53.000000 cbcmgr-1.3.0/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 00:37:37.000000 cbcmgr-1.3.0/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     1781 2023-07-07 00:05:02.000000 cbcmgr-1.3.0/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.0/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.0/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.0/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.0/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)      502 2023-07-07 00:16:42.000000 cbcmgr-1.3.0/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 00:46:37.647825 cbcmgr-1.3.0/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       57 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 00:46:37.000000 cbcmgr-1.3.0/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 00:46:37.649042 cbcmgr-1.3.0/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      705 2023-07-07 00:39:27.000000 cbcmgr-1.3.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 16:50:14.748003 cbcmgr-1.3.1/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.1/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-07-07 16:50:14.747884 cbcmgr-1.3.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 16:50:14.735967 cbcmgr-1.3.1/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.1/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.1/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    24565 2023-07-07 16:30:04.000000 cbcmgr-1.3.1/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 00:37:37.000000 cbcmgr-1.3.1/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     1862 2023-07-07 16:40:09.000000 cbcmgr-1.3.1/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.1/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.1/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.1/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.1/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.1/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 16:50:14.747678 cbcmgr-1.3.1/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 16:50:14.000000 cbcmgr-1.3.1/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 16:50:14.748043 cbcmgr-1.3.1/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      726 2023-07-07 16:44:25.000000 cbcmgr-1.3.1/setup.py
```

### Comparing `cbcmgr-1.3.0/LICENSE.txt` & `cbcmgr-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.0/PKG-INFO` & `cbcmgr-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.0
+Version: 1.3.1
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.3.0/README.md` & `cbcmgr-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.0/cbcmgr/cb_connect.py` & `cbcmgr-1.3.1/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.0/cbcmgr/cb_management.py` & `cbcmgr-1.3.1/cbcmgr/cb_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 ##
 ##
 
-from .exceptions import (IndexNotReady, IndexNotFoundError, CollectionNameNotFound, IndexStatError, ClusterHealthCheckError, PathMapUpsertError)
+from .exceptions import (IndexNotReady, IndexNotFoundError, CollectionNameNotFound, IndexStatError, ClusterHealthCheckError, PathMapUpsertError, CollectionUpsertError)
 from .retry import retry, retry_inline
 from .cb_connect import CBConnect
-from .util import r_getattr, omit_path
+from .util import r_getattr, omit_path, copy_path
 from .config import UpsertMapConfig, MapUpsertType
 from datetime import timedelta
 import attr
 import hashlib
 import logging
+import json
+import xmltodict
+import concurrent.futures
 from attr.validators import instance_of as io, optional
 from typing import Protocol, Iterable, Optional, Any
 from couchbase.cluster import Cluster
 from couchbase.options import QueryOptions
 from couchbase.diagnostics import ServiceType, PingState
 from couchbase.management.buckets import CreateBucketSettings, BucketType, StorageBackend, BucketSettings
 from couchbase.management.collections import CollectionSpec
@@ -439,15 +442,15 @@
             raise IndexNotReady(f"index_list: bucket {self._bucket.name} error: {err}")
 
     @retry(factor=0.5, allow_list=(IndexNotReady,))
     def delete_wait(self, index_name: str = None):
         if self.is_index(index_name=index_name):
             raise IndexNotReady(f"delete_wait: index still exists")
 
-    def cb_map_upsert(self, prefix: str, config: UpsertMapConfig, attr_obj: Any):
+    def cb_map_upsert_attr(self, prefix: str, config: UpsertMapConfig, attr_obj: Any):
         primitive = (int, str, bool, list, dict)
         value = None
         for c in config.paths:
             logger.debug(f"cb_map_upsert: processing key {c.path} name {c.name}")
             try:
                 subset = r_getattr(attr_obj, c.path)
                 if isinstance(subset, list):
@@ -480,7 +483,74 @@
                         self._collection.upsert(doc_id, doc)
 
             except AttributeError:
                 raise PathMapUpsertError(f"cb_map_upsert: key {c.path} not found")
 
             except Exception as err:
                 raise PathMapUpsertError(f"cb_map_upsert: error {err}")
+
+    def cb_map_upsert(self,
+                      prefix: str,
+                      config: UpsertMapConfig,
+                      json_file: str = None,
+                      xml_file: str = None,
+                      json_data: str = None,
+                      xml_data: str = None):
+        tasks = set()
+        executor = concurrent.futures.ThreadPoolExecutor()
+
+        if json_file:
+            with open(json_file, mode="r") as json_xml:
+                data = json.load(json_xml)
+        elif xml_file:
+            with open(xml_file, mode="rb") as input_xml:
+                contents = input_xml.read()
+                data = xmltodict.parse(contents)
+        elif json_data:
+            data = json.loads(json_data)
+        elif xml_data:
+            data = xmltodict.parse(xml_data)
+        else:
+            raise PathMapUpsertError(f"cb_map_upsert: JSON or XML input data is required")
+
+        def _cb_upsert(meta_id, doc_data):
+            try:
+                result = self._collection.upsert(meta_id, doc_data)
+                logger.debug(f"cb_upsert: {meta_id}: cas {result.cas}")
+                return result.cas
+            except Exception as error:
+                raise CollectionUpsertError(f"upsert error: {error}")
+
+        for c in config.paths:
+            logger.debug(f"cb_map_upsert: processing key {c.path} name {c.name}")
+
+            subset = copy_path(c.path, data)
+
+            if not subset or len(subset) == 0:
+                raise PathMapUpsertError(f"path {c.path} not found in source data")
+
+            if c.collection:
+                self.create_collection(c.name)
+
+            if c.exclude:
+                logger.debug(f"cb_map_upsert: excluding {','.join(c.exclude)}")
+                subset = omit_path(subset, c.exclude)
+
+            if c.p_type == MapUpsertType.DOCUMENT:
+                doc_id = self.key_format(c.id, subset, text=prefix)
+                logger.debug(f"cb_map_upsert: processing doc ID {doc_id}")
+                tasks.add(executor.submit(_cb_upsert, doc_id, {c.name: subset}))
+            elif c.p_type == MapUpsertType.LIST:
+                logger.debug(f"cb_map_upsert: processing list")
+                if not isinstance(subset, list):
+                    raise PathMapUpsertError(f"cb_map_upsert: path {c.path} type {type(subset)} incompatible with list mode")
+                for doc in subset:
+                    doc_id = self.key_format(c.id, doc, text=prefix, id_key=c.id_key)
+                    tasks.add(executor.submit(_cb_upsert, doc_id, doc))
+
+        while tasks:
+            done, tasks = concurrent.futures.wait(tasks, return_when=concurrent.futures.FIRST_COMPLETED)
+            for task in done:
+                try:
+                    task.result()
+                except Exception as err:
+                    raise PathMapUpsertError(f"cb_map_upsert: {err}")
```

### Comparing `cbcmgr-1.3.0/cbcmgr/cb_session.py` & `cbcmgr-1.3.1/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.0/cbcmgr/config.py` & `cbcmgr-1.3.1/cbcmgr/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,20 @@
     LIST = 1
 
 
 @attr.s
 class UpsertMapConfig:
     paths: List[UpsertMapPathConfig] = attr.ib(default=[])
 
+    @classmethod
+    def new(cls):
+        return cls(
+            []
+        )
+
     def add(self,
             path: str,
             p_type: MapUpsertType = MapUpsertType.DOCUMENT,
             collection: bool = False,
             exclude: list[str] = None,
             doc_id: KeyStyle = KeyStyle.TEXT,
             id_key: str = "record_id"):
```

### Comparing `cbcmgr-1.3.0/cbcmgr/exceptions.py` & `cbcmgr-1.3.1/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.0/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.3.1/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.0/cbcmgr/retry.py` & `cbcmgr-1.3.1/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.0/cbcmgr/schema.py` & `cbcmgr-1.3.1/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.0/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.3.1/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.0
+Version: 1.3.1
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.3.0/setup.py` & `cbcmgr-1.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.3.0',
+    version='1.3.1',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
         'couchbase',
         'dnspython',
         'docker',
         'pytest',
         'requests',
-        'urllib3'
+        'urllib3',
+        'xmltodict'
     ],
     author_email='info@unix.us.com',
     description='Couchbase connection manager',
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```


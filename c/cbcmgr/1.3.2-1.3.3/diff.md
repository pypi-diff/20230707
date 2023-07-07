# Comparing `tmp/cbcmgr-1.3.2.tar.gz` & `tmp/cbcmgr-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.3.2.tar", last modified: Fri Jul  7 18:12:16 2023, max compression
+gzip compressed data, was "cbcmgr-1.3.3.tar", last modified: Fri Jul  7 19:04:37 2023, max compression
```

## Comparing `cbcmgr-1.3.2.tar` & `cbcmgr-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 18:12:16.870164 cbcmgr-1.3.2/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.2/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 18:12:16.870024 cbcmgr-1.3.2/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.2/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 18:12:16.835739 cbcmgr-1.3.2/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.2/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.2/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    24947 2023-07-07 18:03:28.000000 cbcmgr-1.3.2/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 00:37:37.000000 cbcmgr-1.3.2/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     1862 2023-07-07 16:40:09.000000 cbcmgr-1.3.2/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.2/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.2/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.2/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.2/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.2/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 18:12:16.869762 cbcmgr-1.3.2/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 18:12:16.000000 cbcmgr-1.3.2/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 18:12:16.870217 cbcmgr-1.3.2/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 18:11:57.000000 cbcmgr-1.3.2/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:04:37.240563 cbcmgr-1.3.3/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.3/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 19:04:37.240410 cbcmgr-1.3.3/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.3/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:04:37.190570 cbcmgr-1.3.3/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.3/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11085 2023-07-07 00:32:48.000000 cbcmgr-1.3.3/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    25276 2023-07-07 19:01:23.000000 cbcmgr-1.3.3/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)    11254 2023-07-07 00:37:37.000000 cbcmgr-1.3.3/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.3/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.3/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.3/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.3.3/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.3/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.3/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 19:04:37.240124 cbcmgr-1.3.3/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 19:04:37.000000 cbcmgr-1.3.3/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 19:04:37.240616 cbcmgr-1.3.3/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 19:01:23.000000 cbcmgr-1.3.3/setup.py
```

### Comparing `cbcmgr-1.3.2/LICENSE.txt` & `cbcmgr-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/PKG-INFO` & `cbcmgr-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.2
+Version: 1.3.3
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.2/README.md` & `cbcmgr-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/cbcmgr/cb_connect.py` & `cbcmgr-1.3.3/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/cbcmgr/cb_management.py` & `cbcmgr-1.3.3/cbcmgr/cb_management.py`

 * *Files 5% similar despite different names*

```diff
@@ -515,48 +515,55 @@
         elif json_data:
             data = json.loads(json_data)
         elif xml_data:
             data = xmltodict.parse(xml_data)
         else:
             raise PathMapUpsertError(f"cb_map_upsert: JSON or XML input data is required")
 
-        def _cb_upsert(meta_id, doc_data):
+        def _cb_upsert(collection, meta_id, doc_data):
             try:
-                result = self._collection.upsert(meta_id, doc_data)
-                logger.debug(f"cb_upsert: {meta_id}: cas {result.cas}")
+                _collection = self._scope.collection(collection)
+                result = _collection.upsert(meta_id, doc_data)
+                logger.debug(f"upsert -> {collection}: {meta_id}: cas {result.cas}")
                 return result.cas
             except Exception as error:
                 raise CollectionUpsertError(f"upsert error: {error}")
 
         for c in config.paths:
             logger.debug(f"cb_map_upsert: processing key {c.path} name {c.name}")
 
             subset = copy_path(c.path, data)
 
             if not subset or len(subset) == 0:
-                raise PathMapUpsertError(f"path {c.path} not found in source data")
+                if c.optional:
+                    continue
+                else:
+                    raise PathMapUpsertError(f"path {c.path} not found in source data")
 
             if c.collection:
-                self.create_collection(c.name)
+                collection_name = c.name
+                self.create_collection(collection_name)
+            else:
+                collection_name = self._collection.name
 
             if c.exclude:
                 logger.debug(f"cb_map_upsert: excluding {','.join(c.exclude)}")
                 subset = omit_path(subset, c.exclude)
 
             if c.p_type == MapUpsertType.DOCUMENT:
                 doc_id = self.key_format(c.id, subset, text=prefix)
                 logger.debug(f"cb_map_upsert: processing doc ID {doc_id}")
-                tasks.add(executor.submit(_cb_upsert, doc_id, {c.name: subset}))
+                tasks.add(executor.submit(_cb_upsert, collection_name, doc_id, {c.name: subset}))
             elif c.p_type == MapUpsertType.LIST:
                 logger.debug(f"cb_map_upsert: processing list")
                 if not isinstance(subset, list):
                     raise PathMapUpsertError(f"cb_map_upsert: path {c.path} type {type(subset)} incompatible with list mode")
                 for doc in subset:
                     doc_id = self.key_format(c.id, doc, text=prefix, id_key=c.id_key)
-                    tasks.add(executor.submit(_cb_upsert, doc_id, doc))
+                    tasks.add(executor.submit(_cb_upsert, collection_name, doc_id, doc))
 
         while tasks:
             done, tasks = concurrent.futures.wait(tasks, return_when=concurrent.futures.FIRST_COMPLETED)
             for task in done:
                 try:
                     task.result()
                 except Exception as err:
```

### Comparing `cbcmgr-1.3.2/cbcmgr/cb_session.py` & `cbcmgr-1.3.3/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/cbcmgr/config.py` & `cbcmgr-1.3.3/cbcmgr/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,23 +36,25 @@
 
     def add(self,
             path: str,
             p_type: MapUpsertType = MapUpsertType.DOCUMENT,
             collection: bool = False,
             exclude: list[str] = None,
             doc_id: KeyStyle = KeyStyle.TEXT,
-            id_key: str = "record_id"):
+            id_key: str = "record_id",
+            optional: bool = False):
         self.paths.append(
             UpsertMapPathConfig.create(
                 path,
                 p_type,
                 collection,
                 exclude,
                 doc_id,
-                id_key
+                id_key,
+                optional
             )
         )
 
     def get(self) -> list[UpsertMapPathConfig]:
         return self.__dict__['paths']
 
 
@@ -60,28 +62,31 @@
 class UpsertMapPathConfig:
     path: str = attr.ib()
     p_type: MapUpsertType = attr.ib(default=MapUpsertType.DOCUMENT)
     collection: bool = attr.ib(default=False)
     exclude: list[str] = attr.ib(default=None)
     id: KeyStyle = attr.ib(default=KeyStyle.TEXT)
     id_key: str = attr.ib(default="record_id")
+    optional: bool = attr.ib(default=False)
 
     @classmethod
     def create(cls,
                path: str,
                p_type: MapUpsertType,
                collection: bool,
                exclude: list[str],
                doc_id: KeyStyle,
-               id_key: str):
+               id_key: str,
+               optional: bool):
         return cls(
             path,
             p_type,
             collection,
             exclude,
             doc_id,
-            id_key
+            id_key,
+            optional
         )
 
     @property
     def name(self):
         return self.path.split('.')[-1]
```

### Comparing `cbcmgr-1.3.2/cbcmgr/exceptions.py` & `cbcmgr-1.3.3/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.3.3/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/cbcmgr/retry.py` & `cbcmgr-1.3.3/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/cbcmgr/schema.py` & `cbcmgr-1.3.3/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/cbcmgr/util.py` & `cbcmgr-1.3.3/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.2/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.3.3/cbcmgr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.2
+Version: 1.3.3
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.2/setup.py` & `cbcmgr-1.3.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.3.2',
+    version='1.3.3',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```


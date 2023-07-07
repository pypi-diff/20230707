# Comparing `tmp/orbit_database-1.0.3.tar.gz` & `tmp/orbit_database-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database-1.0.3.tar", max compression
+gzip compressed data, was "orbit_database-1.0.4.tar", max compression
```

## Comparing `orbit_database-1.0.3.tar` & `orbit_database-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0     1087 2023-06-09 10:34:34.878082 orbit_database-1.0.3/LICENSE
--rw-r--r--   0        0        0     4506 2023-06-09 10:34:34.878082 orbit_database-1.0.3/README.md
--rw-r--r--   0        0        0       46 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/README.md
--rwxr-xr-x   0        0        0     1932 2023-06-28 12:55:48.033037 orbit_database-1.0.3/orbit_database/__init__.py
--rw-r--r--   0        0        0     6369 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/audit.py
--rwxr-xr-x   0        0        0     2473 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/bitmap.py
--rw-r--r--   0        0        0     3653 2023-06-17 15:47:18.989970 orbit_database-1.0.3/orbit_database/catalog.py
--rwxr-xr-x   0        0        0    10513 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/compression.py
--rwxr-xr-x   0        0        0     1880 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/cursor.py
--rwxr-xr-x   0        0        0    15912 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/database.py
--rwxr-xr-x   0        0        0     5360 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/decorators.py
--rwxr-xr-x   0        0        0    10044 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/doc.py
--rwxr-xr-x   0        0        0     1104 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/exceptions.py
--rwxr-xr-x   0        0        0     3322 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/filterresult.py
--rwxr-xr-x   0        0        0    10506 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/index.py
--rwxr-xr-x   0        0        0    15546 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/invertedwordindex.py
--rwxr-xr-x   0        0        0     2924 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/manager.py
--rwxr-xr-x   0        0        0    14240 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/metadata.py
--rwxr-xr-x   0        0        0     4432 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/objectid.py
--rwxr-xr-x   0        0        0     6864 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/serialiser.py
--rwxr-xr-x   0        0        0    42013 2023-06-09 11:19:48.579067 orbit_database-1.0.3/orbit_database/table.py
--rwxr-xr-x   0        0        0      387 2023-06-09 10:34:34.882082 orbit_database-1.0.3/orbit_database/types_.py
--rw-r--r--   0        0        0     1586 2023-06-28 12:55:48.029037 orbit_database-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5525 1970-01-01 00:00:00.000000 orbit_database-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1087 2023-06-09 10:34:34.878082 orbit_database-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4506 2023-06-09 10:34:34.878082 orbit_database-1.0.4/README.md
+-rw-r--r--   0        0        0       46 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/README.md
+-rwxr-xr-x   0        0        0     1932 2023-07-07 15:16:48.812179 orbit_database-1.0.4/orbit_database/__init__.py
+-rw-r--r--   0        0        0     5978 2023-07-06 11:48:41.818031 orbit_database-1.0.4/orbit_database/audit.py
+-rwxr-xr-x   0        0        0     2473 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/bitmap.py
+-rw-r--r--   0        0        0     3653 2023-06-17 15:47:18.989970 orbit_database-1.0.4/orbit_database/catalog.py
+-rwxr-xr-x   0        0        0    10513 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/compression.py
+-rwxr-xr-x   0        0        0     1880 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/cursor.py
+-rwxr-xr-x   0        0        0    15912 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/database.py
+-rwxr-xr-x   0        0        0     5360 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/decorators.py
+-rwxr-xr-x   0        0        0    10044 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/doc.py
+-rwxr-xr-x   0        0        0     1104 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/exceptions.py
+-rwxr-xr-x   0        0        0     3322 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/filterresult.py
+-rwxr-xr-x   0        0        0    10506 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/index.py
+-rwxr-xr-x   0        0        0    15546 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/invertedwordindex.py
+-rwxr-xr-x   0        0        0     2924 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/manager.py
+-rwxr-xr-x   0        0        0    14240 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/metadata.py
+-rwxr-xr-x   0        0        0     4432 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/objectid.py
+-rwxr-xr-x   0        0        0     6864 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/serialiser.py
+-rwxr-xr-x   0        0        0    42032 2023-06-28 13:30:21.439050 orbit_database-1.0.4/orbit_database/table.py
+-rwxr-xr-x   0        0        0      387 2023-06-09 10:34:34.882082 orbit_database-1.0.4/orbit_database/types_.py
+-rw-r--r--   0        0        0     1586 2023-07-07 15:16:48.808180 orbit_database-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5525 1970-01-01 00:00:00.000000 orbit_database-1.0.4/PKG-INFO
```

### Comparing `orbit_database-1.0.3/LICENSE` & `orbit_database-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/README.md` & `orbit_database-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/__init__.py` & `orbit_database-1.0.4/orbit_database/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #####################################################################################
 #
 #  Copyright (c) 2020 - Mad Penguin Consulting Ltd
 #
 #####################################################################################
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from orbit_database.manager import Manager
 from orbit_database.database import Database
 from orbit_database.table import Table
 from orbit_database.filterresult import FilterResult, MatchResult
 from orbit_database.index import Index
 from orbit_database.doc import Doc, JournalType
```

### Comparing `orbit_database-1.0.3/orbit_database/audit.py` & `orbit_database-1.0.4/orbit_database/audit.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,23 +43,14 @@
         self._semaphore = None
         self._handlers = {}
         self._finished = False
         self._auditing = False
         self._tasks = []
 
     def open(self, auditing=False):
-        # doc = self._database.meta.fetch_key(self.UUID_KEY)
-        # if doc:
-        #     self._uuid = doc._uuid
-        # else:
-        #     self._uuid = f'{getuser()}_{self._database._name}'
-        #     self._database.meta.store_key(self.UUID_KEY, Doc({'uuid': self._uuid}))
-        #
-        #   Needs to be unique based on path + user ... metadata is an overcomplication
-        #
         hObj = hashlib.new('sha1')
         hObj.update(str(self._database._path).encode())
         self._uuid = hObj.hexdigest()
         if self._database.index_version == 1:
             audit_table_name = '__audit_table__'
         elif self._database.index_version == 2:
             audit_table_name = '@@audit_table@@'
```

### Comparing `orbit_database-1.0.3/orbit_database/bitmap.py` & `orbit_database-1.0.4/orbit_database/bitmap.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/catalog.py` & `orbit_database-1.0.4/orbit_database/catalog.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/compression.py` & `orbit_database-1.0.4/orbit_database/compression.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/cursor.py` & `orbit_database-1.0.4/orbit_database/cursor.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/database.py` & `orbit_database-1.0.4/orbit_database/database.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/decorators.py` & `orbit_database-1.0.4/orbit_database/decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/doc.py` & `orbit_database-1.0.4/orbit_database/doc.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/exceptions.py` & `orbit_database-1.0.4/orbit_database/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/filterresult.py` & `orbit_database-1.0.4/orbit_database/filterresult.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/index.py` & `orbit_database-1.0.4/orbit_database/index.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/invertedwordindex.py` & `orbit_database-1.0.4/orbit_database/invertedwordindex.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/manager.py` & `orbit_database-1.0.4/orbit_database/manager.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/metadata.py` & `orbit_database-1.0.4/orbit_database/metadata.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/objectid.py` & `orbit_database-1.0.4/orbit_database/objectid.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/serialiser.py` & `orbit_database-1.0.4/orbit_database/serialiser.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.3/orbit_database/table.py` & `orbit_database-1.0.4/orbit_database/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         self.integerkey = integerkey
         self._auditing = auditing
 
         if not self.name.startswith('@@') and self._database.index_version == 2:
             self._oid = name = self._database._cat.get_table_id(self.name, txn)
         else:
             self._oid = self.name
-
+            
         try:
             self._db = self.env.open_db(
                 # self.name.encode() if isinstance(self.name, str) else self.name,
                 self._oid.encode(),
                 create=False,
                 integerkey=integerkey,
                 txn=transaction)
@@ -201,15 +201,15 @@
                 # self.name.encode(),
                 self._oid.encode(),
                 integerkey=integerkey,
                 txn=transaction)
         except IncompatibleError as e:
             log.error(f'{self.name} => {self._oid}:: {str(e)}')
             return self
-
+       
         try:
             Serialiser.__init__(self, codec, txn=transaction)
             if not self._meta:
                 return self
             for index_name in self.indexes(txn=transaction):
                 if index_name in self.data:
                     # means the index is open so we're doing a 're-open'
```

### Comparing `orbit_database-1.0.3/pyproject.toml` & `orbit_database-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit_database"
-version = "1.0.3"
+version = "1.0.4"
 description = "Database library for Python based on LMDB storage engine"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `orbit_database-1.0.3/PKG-INFO` & `orbit_database-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-database
-Version: 1.0.3
+Version: 1.0.4
 Summary: Database library for Python based on LMDB storage engine
 Home-page: https://gitlab.com/madpenguin/orbit-database
 Keywords: database,nosql,lmdb
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
```


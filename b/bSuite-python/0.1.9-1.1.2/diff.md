# Comparing `tmp/bSuite-python-0.1.9.tar.gz` & `tmp/bSuite-python-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bSuite-python-0.1.9.tar", last modified: Wed Jul  5 23:45:21 2023, max compression
+gzip compressed data, was "bSuite-python-1.1.2.tar", last modified: Fri Jul  7 20:54:24 2023, max compression
```

## Comparing `bSuite-python-0.1.9.tar` & `bSuite-python-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,31 @@
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.824023 bSuite-python-0.1.9/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-0.1.9/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-05 23:45:21.823843 bSuite-python-0.1.9/PKG-INFO
--rw-r--r--   0 birdwell   (501) staff       (20)       16 2023-07-05 15:45:08.000000 bSuite-python-0.1.9/README.md
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.821370 bSuite-python-0.1.9/bSuite_auth/
--rw-r--r--   0 birdwell   (501) staff       (20)      497 2023-07-05 23:36:57.000000 bSuite-python-0.1.9/bSuite_auth/pyproject.toml
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.820193 bSuite-python-0.1.9/bSuite_auth/src/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.820237 bSuite-python-0.1.9/bSuite_auth/src/bSuite/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.821856 bSuite-python-0.1.9/bSuite_auth/src/bSuite/auth/
--rw-r--r--   0 birdwell   (501) staff       (20)       58 2023-07-05 17:22:59.000000 bSuite-python-0.1.9/bSuite_auth/src/bSuite/auth/__init__.py
--rw-r--r--   0 birdwell   (501) staff       (20)     4864 2023-07-05 17:22:59.000000 bSuite-python-0.1.9/bSuite_auth/src/bSuite/auth/client.py
--rw-r--r--   0 birdwell   (501) staff       (20)      504 2023-07-05 17:22:59.000000 bSuite-python-0.1.9/bSuite_auth/src/bSuite/auth/etc.py
--rw-r--r--   0 birdwell   (501) staff       (20)     3272 2023-07-05 17:22:59.000000 bSuite-python-0.1.9/bSuite_auth/src/bSuite/auth/middleware.py
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.822118 bSuite-python-0.1.9/bSuite_configure/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-0.1.9/bSuite_configure/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)      372 2023-07-05 02:23:50.000000 bSuite-python-0.1.9/bSuite_configure/pyproject.toml
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.820400 bSuite-python-0.1.9/bSuite_configure/src/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.820442 bSuite-python-0.1.9/bSuite_configure/src/bSuite/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.822334 bSuite-python-0.1.9/bSuite_configure/src/bSuite/configure/
--rw-r--r--   0 birdwell   (501) staff       (20)       52 2023-07-05 01:59:36.000000 bSuite-python-0.1.9/bSuite_configure/src/bSuite/configure/__init__.py
--rw-r--r--   0 birdwell   (501) staff       (20)     1233 2023-07-05 01:05:11.000000 bSuite-python-0.1.9/bSuite_configure/src/bSuite/configure/configure.py
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.822573 bSuite-python-0.1.9/bSuite_database/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-0.1.9/bSuite_database/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)      490 2023-07-05 02:26:14.000000 bSuite-python-0.1.9/bSuite_database/pyproject.toml
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.820603 bSuite-python-0.1.9/bSuite_database/src/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.820649 bSuite-python-0.1.9/bSuite_database/src/bSuite/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.823001 bSuite-python-0.1.9/bSuite_database/src/bSuite/database/
--rw-r--r--   0 birdwell   (501) staff       (20)      112 2023-07-04 23:38:47.000000 bSuite-python-0.1.9/bSuite_database/src/bSuite/database/__init__.py
--rw-r--r--   0 birdwell   (501) staff       (20)     7835 2023-07-05 00:07:10.000000 bSuite-python-0.1.9/bSuite_database/src/bSuite/database/base.py
--rw-r--r--   0 birdwell   (501) staff       (20)     2850 2023-07-04 23:52:38.000000 bSuite-python-0.1.9/bSuite_database/src/bSuite/database/crypto.py
--rw-r--r--   0 birdwell   (501) staff       (20)     1904 2023-07-05 00:21:09.000000 bSuite-python-0.1.9/bSuite_database/src/bSuite/database/mapped.py
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-05 23:45:21.823549 bSuite-python-0.1.9/bSuite_python.egg-info/
--rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-05 23:45:21.000000 bSuite-python-0.1.9/bSuite_python.egg-info/PKG-INFO
--rw-r--r--   0 birdwell   (501) staff       (20)      804 2023-07-05 23:45:21.000000 bSuite-python-0.1.9/bSuite_python.egg-info/SOURCES.txt
--rw-r--r--   0 birdwell   (501) staff       (20)        1 2023-07-05 23:45:21.000000 bSuite-python-0.1.9/bSuite_python.egg-info/dependency_links.txt
--rw-r--r--   0 birdwell   (501) staff       (20)       23 2023-07-05 23:45:21.000000 bSuite-python-0.1.9/bSuite_python.egg-info/requires.txt
--rw-r--r--   0 birdwell   (501) staff       (20)        7 2023-07-05 23:45:21.000000 bSuite-python-0.1.9/bSuite_python.egg-info/top_level.txt
--rw-r--r--   0 birdwell   (501) staff       (20)      753 2023-07-05 23:45:14.000000 bSuite-python-0.1.9/pyproject.toml
--rw-r--r--   0 birdwell   (501) staff       (20)       38 2023-07-05 23:45:21.824057 bSuite-python-0.1.9/setup.cfg
--rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-05 00:44:00.000000 bSuite-python-0.1.9/setup.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.519953 bSuite-python-1.1.2/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.2/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-07 20:54:24.519763 bSuite-python-1.1.2/PKG-INFO
+-rw-r--r--   0 birdwell   (501) staff       (20)       16 2023-07-05 15:45:08.000000 bSuite-python-1.1.2/README.md
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.512819 bSuite-python-1.1.2/bSuite_configure/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.2/bSuite_configure/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)      372 2023-07-05 02:23:50.000000 bSuite-python-1.1.2/bSuite_configure/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.511242 bSuite-python-1.1.2/bSuite_configure/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.511287 bSuite-python-1.1.2/bSuite_configure/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.513509 bSuite-python-1.1.2/bSuite_configure/src/bSuite/configure/
+-rw-r--r--   0 birdwell   (501) staff       (20)       52 2023-07-05 01:59:36.000000 bSuite-python-1.1.2/bSuite_configure/src/bSuite/configure/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     1233 2023-07-05 01:05:11.000000 bSuite-python-1.1.2/bSuite_configure/src/bSuite/configure/configure.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.513988 bSuite-python-1.1.2/bSuite_database/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.2/bSuite_database/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)      490 2023-07-05 02:26:14.000000 bSuite-python-1.1.2/bSuite_database/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.511452 bSuite-python-1.1.2/bSuite_database/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.511493 bSuite-python-1.1.2/bSuite_database/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.515222 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/
+-rw-r--r--   0 birdwell   (501) staff       (20)      112 2023-07-04 23:38:47.000000 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     8187 2023-07-07 20:47:35.000000 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/base.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     2851 2023-07-06 00:12:17.000000 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/crypto.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     2629 2023-07-07 20:26:55.000000 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/mapped.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.519412 bSuite-python-1.1.2/bSuite_python.egg-info/
+-rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/PKG-INFO
+-rw-r--r--   0 birdwell   (501) staff       (20)      622 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)        1 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/requires.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)        7 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/top_level.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)      788 2023-07-07 20:53:35.000000 bSuite-python-1.1.2/pyproject.toml
+-rw-r--r--   0 birdwell   (501) staff       (20)       38 2023-07-07 20:54:24.519993 bSuite-python-1.1.2/setup.cfg
+-rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-05 00:44:00.000000 bSuite-python-1.1.2/setup.py
```

### Comparing `bSuite-python-0.1.9/LICENSE` & `bSuite-python-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-0.1.9/PKG-INFO` & `bSuite-python-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bSuite-python
-Version: 0.1.9
+Version: 1.1.2
 Summary: advanced helper modules. python edition
 Author-email: John Birdwell <j.c.birdwell@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bSuite-python-0.1.9/bSuite_configure/LICENSE` & `bSuite-python-1.1.2/bSuite_configure/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-0.1.9/bSuite_configure/src/bSuite/configure/configure.py` & `bSuite-python-1.1.2/bSuite_configure/src/bSuite/configure/configure.py`

 * *Files identical despite different names*

### Comparing `bSuite-python-0.1.9/bSuite_database/LICENSE` & `bSuite-python-1.1.2/bSuite_database/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-0.1.9/bSuite_database/src/bSuite/database/base.py` & `bSuite-python-1.1.2/bSuite_database/src/bSuite/database/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 from contextlib import contextmanager
 from typing import Generator
 from psycopg2.extensions import cursor
 from psycopg2.pool import ThreadedConnectionPool
 
 
+def get_comparator(v) -> str | tuple:
+    if isinstance(v, str):
+        if 'null' in v:
+            return ('is not', None) if 'not' in v else ('is', None)
+        return 'like'
+    elif isinstance(v, int):
+        return '='
+
+    return 'is'
+
+
 class CoreDatabase:
     """
     Base interface for postgres database, includes methods for
     querying, selection, insertion, and deletion
     """
 
     def __init__(self, cxn_config: dict):
         # parse connection parameters from ini file and merge
         # with overrides if provided
         self.db = None
         self._tables = None
         self.config = cxn_config
         self.pool = ThreadedConnectionPool(1, 5, **self.config)
+        self.__post_init__()
 
     def __post_init__(self):
         self.db = self.query('SELECT current_database()', as_tuple=True)[0]
 
     @contextmanager
     def cursor(self) -> Generator[cursor, None, None]:
         """
@@ -133,15 +145,18 @@
         # set where params
         passed_vars = []
         if not where:
             where = ''
         else:
             conditions = []
             for k, v in where.items():
-                comparator = 'like' if isinstance(v, str) else 'is'
+                comparator = get_comparator(v)
+                if isinstance(comparator, tuple):
+                    comparator, v = comparator
+
                 conditions.append(f'{k} {comparator} %s')
                 passed_vars.append(v)
             where = f" where {' and '.join(conditions)}"
 
         # prepare parameterized values to be passed to query when present
         passed_vars = None if not passed_vars else tuple(passed_vars)
```

### Comparing `bSuite-python-0.1.9/bSuite_database/src/bSuite/database/crypto.py` & `bSuite-python-1.1.2/bSuite_database/src/bSuite/database/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from base import CoreDatabase
+from .base import CoreDatabase
 from cryptography.fernet import Fernet
 from typing import Optional, Union
 from os import environ as env
 
 
 class AutoEncodeFernet(Fernet):
     def decrypt(self,
```

### Comparing `bSuite-python-0.1.9/bSuite_database/src/bSuite/database/mapped.py` & `bSuite-python-1.1.2/bSuite_database/src/bSuite/database/mapped.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,79 @@
 import json
+import pickle as pk
 from typing import Any, Generator
 
 from .base import CoreDatabase
 from collections.abc import MutableMapping
 
 
 class MappedDatabase(CoreDatabase, MutableMapping):
     """
     Interface that allows for a database table to be interacted with as if it were a dictionary object.
     """
     # TODO: add a mode selector pickle v json
-    def __init__(self, cxn_config, table):
-        super().__init__(cxn_config)
+    def __init__(self, cxn_config: dict, table: str, pickle=False):
         self.bound_table = table
-        self.__post_init__()
+        self._pickle = pickle
+        if self._pickle:
+            print('WARNING: Pickle mode is active. Not for use in production. Learn more about pickle '
+                  'vulnerabilities here: https://docs.python.org/3/library/pickle.html')
+        self._vk = 'val_p' if self._pickle else 'val'
+        super().__init__(cxn_config)
 
     def __repr__(self):
         return f'Mutable mapping interface bound to table "{self.bound_table}" of database "{self.db}".'
 
     def __post_init__(self):
         super().__post_init__()
         print(f'ensuring {self.bound_table} in database:', self.tables)
         if self.bound_table not in self.tables:
             print('generating table')
             tq = f"""
             create table {self.bound_table} (
                 var varchar(255) primary key,
                 val jsonb,
+                val_p bytea,
                 ts timestamp default current_timestamp
             );
             """
 
             # add table
             self.query(tq, no_resp=True)
 
             # clear cached table names
             self._tables = None
 
+    def dumps(self, v) -> bytes | str:
+        if self._pickle:
+            return pk.dumps(v)
+        return json.dumps(v)
+
+    @staticmethod
+    def loads(v) -> Any:
+        if isinstance(v, memoryview):
+            return pk.loads(v)
+        return v
+
     def __setitem__(self, __k: Any, __v: Any) -> None:
-        self.insert(self.bound_table, {'var': __k, 'val': json.dumps(__v)}, upsert_on='var')
+        self.insert(self.bound_table, {'var': __k, self._vk: self.dumps(__v)}, upsert_on='var')
 
     def __delitem__(self, __v: Any) -> None:
         self.delete(self.bound_table, {'var': __v})
 
     def __getitem__(self, __k: Any) -> Any:
-        resp = self.select(self.bound_table, 'val', where={'var': __k}, limit=1)
+        resp = self.select(self.bound_table, self._vk, where={'var': __k}, limit=1)
+
+        # throw missing
         if not resp:
             raise KeyError(f'{__k} not present.')
-        return resp[0]
+
+        # enable de-pickling via parse
+        return self.loads(resp[0])
 
     def __len__(self) -> int:
-        resp = self.select(self.bound_table, 'count(*)')
+        resp = self.select(self.bound_table, f'count({self._vk})')
         return resp[0] if resp else 0
 
     def __iter__(self) -> Generator:
-        for x in self.select(self.bound_table, 'var'):
+        for x in self.select(self.bound_table, 'var', where={self._vk: 'not null'}):
             yield x
```

### Comparing `bSuite-python-0.1.9/bSuite_python.egg-info/PKG-INFO` & `bSuite-python-1.1.2/bSuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bSuite-python
-Version: 0.1.9
+Version: 1.1.2
 Summary: advanced helper modules. python edition
 Author-email: John Birdwell <j.c.birdwell@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bSuite-python-0.1.9/bSuite_python.egg-info/SOURCES.txt` & `bSuite-python-1.1.2/bSuite_python.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-bSuite_auth/pyproject.toml
-bSuite_auth/src/bSuite/auth/__init__.py
-bSuite_auth/src/bSuite/auth/client.py
-bSuite_auth/src/bSuite/auth/etc.py
-bSuite_auth/src/bSuite/auth/middleware.py
 bSuite_configure/LICENSE
 bSuite_configure/pyproject.toml
 bSuite_configure/src/bSuite/configure/__init__.py
 bSuite_configure/src/bSuite/configure/configure.py
 bSuite_database/LICENSE
 bSuite_database/pyproject.toml
 bSuite_database/src/bSuite/database/__init__.py
```

### Comparing `bSuite-python-0.1.9/pyproject.toml` & `bSuite-python-1.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name='bSuite-python'
-version='0.1.9'
+version='1.1.2'
 description='advanced helper modules. python edition'
 authors = [{name = "John Birdwell", email = "j.c.birdwell@gmail.com"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
 keywords = ["helpers", "utilities", "database", "postgres", ".ini"]
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
     "Development Status :: 3 - Alpha"
 ]
+dependencies = ["psycopg2-binary"]
 
 
 [project.optional-dependencies]
 CRYPTO = ["cryptography"]
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
```


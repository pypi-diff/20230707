# Comparing `tmp/aio-databases-0.9.0.tar.gz` & `tmp/aio-databases-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-databases-0.9.0.tar", last modified: Fri Sep 17 14:11:14 2021, max compression
+gzip compressed data, was "aio-databases-0.9.1.tar", last modified: Fri Sep 17 14:15:55 2021, max compression
```

## Comparing `aio-databases-0.9.0.tar` & `aio-databases-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 14:11:14.294347 aio-databases-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     5968 2021-09-17 14:11:14.294347 aio-databases-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4749 2021-09-17 14:11:11.000000 aio-databases-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 14:11:14.290347 aio-databases-0.9.0/aio_databases/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 14:11:14.294347 aio-databases-0.9.0/aio_databases/backends/
--rw-r--r--   0 runner    (1001) docker     (121)     8353 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/_aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/_aioodbc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/_aiopg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/_aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)     4210 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/_asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/_dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/_trio_mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     4608 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/_triopg.py
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/backends/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-09-17 14:11:11.000000 aio-databases-0.9.0/aio_databases/record.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 14:11:14.294347 aio-databases-0.9.0/aio_databases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5968 2021-09-17 14:11:14.000000 aio-databases-0.9.0/aio_databases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-09-17 14:11:14.000000 aio-databases-0.9.0/aio_databases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-17 14:11:14.000000 aio-databases-0.9.0/aio_databases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-09-17 14:11:14.000000 aio-databases-0.9.0/aio_databases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-17 14:11:14.000000 aio-databases-0.9.0/aio_databases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2021-09-17 14:11:14.294347 aio-databases-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-09-17 14:11:11.000000 aio-databases-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 14:15:55.535634 aio-databases-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     5968 2021-09-17 14:15:55.535634 aio-databases-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4749 2021-09-17 14:15:52.000000 aio-databases-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 14:15:55.535634 aio-databases-0.9.1/aio_databases/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 14:15:55.535634 aio-databases-0.9.1/aio_databases/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)     8353 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/_aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/_aioodbc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/_aiopg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/_aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4210 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/_asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/_trio_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4608 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/_triopg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/backends/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-09-17 14:15:52.000000 aio-databases-0.9.1/aio_databases/record.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 14:15:55.535634 aio-databases-0.9.1/aio_databases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5968 2021-09-17 14:15:55.000000 aio-databases-0.9.1/aio_databases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2021-09-17 14:15:55.000000 aio-databases-0.9.1/aio_databases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-17 14:15:55.000000 aio-databases-0.9.1/aio_databases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2021-09-17 14:15:55.000000 aio-databases-0.9.1/aio_databases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-17 14:15:55.000000 aio-databases-0.9.1/aio_databases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2021-09-17 14:15:55.539634 aio-databases-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-09-17 14:15:52.000000 aio-databases-0.9.1/setup.py
```

### Comparing `aio-databases-0.9.0/PKG-INFO` & `aio-databases-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-databases
-Version: 0.9.0
+Version: 0.9.1
 Summary: Async Support for various databases
 Home-page: https://github.com/klen/aio-databases
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/klen/aio-databases
 Project-URL: Source code, https://github.com/klen/aio-databases
```

### Comparing `aio-databases-0.9.0/README.md` & `aio-databases-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/__init__.py` & `aio-databases-0.9.1/aio_databases/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/_aiomysql.py` & `aio-databases-0.9.1/aio_databases/backends/_aiomysql.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/_aioodbc.py` & `aio-databases-0.9.1/aio_databases/backends/_aioodbc.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,33 +24,42 @@
 
     pool: t.Optional[aioodbc.Pool] = None
     db_type = 'odbc'
 
     def __init__(self, *args, db_type: str = None, **kwargs):
         self.db_type = db_type or self.db_type  # type: ignore
         super(Backend, self).__init__(*args, **kwargs)
+        self.pool_options = {
+            name: self.options.pop(name)
+            for name in ('minsize', 'maxsize', 'pool_recycle')
+            if name in self.options
+        }
 
     def __convert_sql__(self, sql: t.Any) -> str:
         sql = str(sql)
         if self.convert_params:
             sql = RE_PARAM.sub(r'\1?', sql)
         return sql
 
     async def connect(self) -> None:
-        self.pool = await aioodbc.create_pool(**self.options)
+        self.pool = await aioodbc.create_pool(**self.options, **self.pool_options)
 
     async def disconnect(self) -> None:
         pool = self.pool
         assert pool is not None, "Database is not connected"
         self.pool = None
         pool.close()
         await pool.wait_closed()
 
     async def acquire(self) -> aioodbc.Connection:
         pool = self.pool
-        assert pool is not None, "Database is not connected"
+        if pool is None:
+            return aioodbc.connect(**self.options)
+
         return await pool.acquire()
 
     async def release(self, conn: aioodbc.Connection):
         pool = self.pool
-        assert pool is not None, "Database is not connected"
-        await pool.release(conn)
+        if pool is None:
+            await conn.close()
+        else:
+            await pool.release(conn)
```

### Comparing `aio-databases-0.9.0/aio_databases/backends/_aiopg.py` & `aio-databases-0.9.1/aio_databases/backends/_aiopg.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/_aiosqlite.py` & `aio-databases-0.9.1/aio_databases/backends/_aiosqlite.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/_asyncpg.py` & `aio-databases-0.9.1/aio_databases/backends/_asyncpg.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/_dummy.py` & `aio-databases-0.9.1/aio_databases/backends/_dummy.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/_trio_mysql.py` & `aio-databases-0.9.1/aio_databases/backends/_trio_mysql.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/_triopg.py` & `aio-databases-0.9.1/aio_databases/backends/_triopg.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/backends/common.py` & `aio-databases-0.9.1/aio_databases/backends/common.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/database.py` & `aio-databases-0.9.1/aio_databases/database.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases/record.py` & `aio-databases-0.9.1/aio_databases/record.py`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/aio_databases.egg-info/PKG-INFO` & `aio-databases-0.9.1/aio_databases.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-databases
-Version: 0.9.0
+Version: 0.9.1
 Summary: Async Support for various databases
 Home-page: https://github.com/klen/aio-databases
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/klen/aio-databases
 Project-URL: Source code, https://github.com/klen/aio-databases
```

### Comparing `aio-databases-0.9.0/aio_databases.egg-info/SOURCES.txt` & `aio-databases-0.9.1/aio_databases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio-databases-0.9.0/setup.cfg` & `aio-databases-0.9.1/setup.cfg`

 * *Files identical despite different names*


# Comparing `tmp/peewee_aio-1.5.7.tar.gz` & `tmp/peewee_aio-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_aio-1.5.7.tar", max compression
+gzip compressed data, was "peewee_aio-1.6.0.tar", max compression
```

## Comparing `peewee_aio-1.5.7.tar` & `peewee_aio-1.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4681 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/README.md
--rw-r--r--   0        0        0      132 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/__init__.py
--rw-r--r--   0        0        0     1210 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/databases.py
--rw-r--r--   0        0        0    17336 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/fields.py
--rw-r--r--   0        0        0    15580 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/manager.py
--rw-r--r--   0        0        0    17014 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/model.py
--rw-r--r--   0        0        0        0 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/py.typed
--rw-r--r--   0        0        0      268 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/peewee_aio/types.py
--rw-r--r--   0        0        0     2622 2023-07-03 11:40:52.347069 peewee_aio-1.5.7/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     4681 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/README.md
+-rw-r--r--   0        0        0      132 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/__init__.py
+-rw-r--r--   0        0        0     1210 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/databases.py
+-rw-r--r--   0        0        0    17336 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/fields.py
+-rw-r--r--   0        0        0    15918 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/manager.py
+-rw-r--r--   0        0        0    17014 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/model.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/py.typed
+-rw-r--r--   0        0        0      268 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/types.py
+-rw-r--r--   0        0        0     2622 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.6.0/PKG-INFO
```

### Comparing `peewee_aio-1.5.7/README.md` & `peewee_aio-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.7/peewee_aio/databases.py` & `peewee_aio-1.6.0/peewee_aio/databases.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.7/peewee_aio/fields.py` & `peewee_aio-1.6.0/peewee_aio/fields.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.7/peewee_aio/manager.py` & `peewee_aio-1.6.0/peewee_aio/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 from functools import cached_property
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Callable,
     Coroutine,
@@ -59,14 +59,24 @@
     """Manage database and models."""
 
     pw_database: PWDatabase
     models: "WeakSet[Type[PWModel]]"
 
     def __init__(self, url: str, **backend_options):
         """Initialize dialect and database."""
+        if url.startswith(("sqlite://", "aiosqlite://")):
+            import peewee as pw
+
+            backend_options.setdefault("functions", ())
+            backend_options["functions"] = (
+                *backend_options["functions"],
+                ("date_part", 2, pw._sqlite_date_part),  # type: ignore[]
+                ("date_trunc", 2, pw._sqlite_date_trunc),  # type: ignore[]
+            )
+
         backend_options.setdefault("convert_params", True)
         super().__init__(url, logger=logger, **backend_options)
 
         self.models = WeakSet()
         self.pw_database = get_db(self)
 
     @cached_property
@@ -239,19 +249,16 @@
 
             # Create table
             ctx = schema._create_table(safe=safe, **opts)  # type: ignore[]
             await self.execute(ctx)
 
             # Create indexes
             for query in schema._create_indexes(safe=safe):  # type: ignore[]
-                try:
+                with suppress(OperationalError):
                     await self.execute(query)
-                except OperationalError:
-                    if not safe:
-                        raise
 
     async def drop_tables(self, *models_cls: Type[PWModel], **opts):
         """Drop tables for the given models or all registered with the manager."""
         models_cls = models_cls or tuple(self.models)
         for model_cls in reversed(sort_models(models_cls)):
             schema: SchemaManager = model_cls._schema
             ctx = schema._drop_table(**opts)  # type: ignore[]
```

### Comparing `peewee_aio-1.5.7/peewee_aio/model.py` & `peewee_aio-1.6.0/peewee_aio/model.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.5.7/pyproject.toml` & `peewee_aio-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-aio"
-version = "1.5.7"
+version = "1.6.0"
 description = "Async support for Peewee ORM"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/klen/peewee-aio"
 repository = "https://github.com/klen/peewee-aio"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["peewee", "asyncio", "trio", "orm"]
```

### Comparing `peewee_aio-1.5.7/PKG-INFO` & `peewee_aio-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-aio
-Version: 1.5.7
+Version: 1.6.0
 Summary: Async support for Peewee ORM
 Home-page: https://github.com/klen/peewee-aio
 License: MIT
 Keywords: peewee,asyncio,trio,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```


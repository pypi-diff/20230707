# Comparing `tmp/eventsourcing-mongodb-3.0.0.tar.gz` & `tmp/eventsourcing-mongodb-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventsourcing-mongodb-3.0.0.tar", last modified: Fri Jul  7 15:17:06 2023, max compression
+gzip compressed data, was "eventsourcing-mongodb-3.0.2.tar", last modified: Fri Jul  7 19:06:12 2023, max compression
```

## Comparing `eventsourcing-mongodb-3.0.0.tar` & `eventsourcing-mongodb-3.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/
--rw-r--r--   0 luca      (1000) luca      (1001)     1062 2022-07-18 14:29:26.000000 eventsourcing-mongodb-3.0.0/LICENSE
--rw-r--r--   0 luca      (1000) luca      (1001)     5600 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1001)     3820 2023-07-07 15:13:48.000000 eventsourcing-mongodb-3.0.0/README.md
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/
--rw-r--r--   0 luca      (1000) luca      (1001)       29 2022-07-19 00:25:05.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1001)     1146 2022-07-19 08:36:58.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/datastore.py
--rw-r--r--   0 luca      (1000) luca      (1001)     2123 2023-07-07 15:12:57.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/factory.py
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/
--rw-r--r--   0 luca      (1000) luca      (1001)      144 2022-07-18 22:11:10.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1001)     2789 2023-07-07 15:05:19.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/aggregate.py
--rw-r--r--   0 luca      (1000) luca      (1001)     1831 2023-07-07 15:11:14.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/application.py
--rw-r--r--   0 luca      (1000) luca      (1001)     1056 2023-07-07 15:11:14.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/process.py
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/
--rw-r--r--   0 luca      (1000) luca      (1001)     5600 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1001)      603 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 luca      (1000) luca      (1001)        1 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 luca      (1000) luca      (1001)       43 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/requires.txt
--rw-r--r--   0 luca      (1000) luca      (1001)       22 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/top_level.txt
--rw-r--r--   0 luca      (1000) luca      (1001)      770 2023-07-07 15:14:56.000000 eventsourcing-mongodb-3.0.0/pyproject.toml
--rw-r--r--   0 luca      (1000) luca      (1001)       38 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/setup.cfg
--rw-r--r--   0 luca      (1000) luca      (1001)       38 2022-07-19 02:00:30.000000 eventsourcing-mongodb-3.0.0/setup.py
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/tests/
--rw-r--r--   0 luca      (1000) luca      (1001)      295 2022-07-19 09:04:23.000000 eventsourcing-mongodb-3.0.0/tests/test_aggregate_recorder.py
--rw-r--r--   0 luca      (1000) luca      (1001)     1347 2022-07-19 08:46:06.000000 eventsourcing-mongodb-3.0.0/tests/test_datastore.py
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 19:06:12.178029 eventsourcing-mongodb-3.0.2/
+-rw-r--r--   0 luca      (1000) luca      (1001)     1062 2022-07-18 14:29:26.000000 eventsourcing-mongodb-3.0.2/LICENSE
+-rw-r--r--   0 luca      (1000) luca      (1001)     5600 2023-07-07 19:06:12.178029 eventsourcing-mongodb-3.0.2/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1001)     3820 2023-07-07 15:13:48.000000 eventsourcing-mongodb-3.0.2/README.md
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 19:06:12.178029 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/
+-rw-r--r--   0 luca      (1000) luca      (1001)       29 2022-07-19 00:25:05.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     1146 2022-07-19 08:36:58.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/datastore.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     2123 2023-07-07 15:12:57.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/factory.py
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 19:06:12.178029 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/recorders/
+-rw-r--r--   0 luca      (1000) luca      (1001)      144 2022-07-18 22:11:10.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/recorders/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     2789 2023-07-07 15:05:19.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/recorders/aggregate.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     1884 2023-07-07 19:02:18.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/recorders/application.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     1056 2023-07-07 15:11:14.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/recorders/process.py
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 19:06:12.178029 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb.egg-info/
+-rw-r--r--   0 luca      (1000) luca      (1001)     5600 2023-07-07 19:06:12.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1001)      603 2023-07-07 19:06:12.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 luca      (1000) luca      (1001)        1 2023-07-07 19:06:12.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 luca      (1000) luca      (1001)       43 2023-07-07 19:06:12.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb.egg-info/requires.txt
+-rw-r--r--   0 luca      (1000) luca      (1001)       22 2023-07-07 19:06:12.000000 eventsourcing-mongodb-3.0.2/eventsourcing_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 luca      (1000) luca      (1001)      770 2023-07-07 19:05:10.000000 eventsourcing-mongodb-3.0.2/pyproject.toml
+-rw-r--r--   0 luca      (1000) luca      (1001)       38 2023-07-07 19:06:12.178029 eventsourcing-mongodb-3.0.2/setup.cfg
+-rw-r--r--   0 luca      (1000) luca      (1001)       38 2022-07-19 02:00:30.000000 eventsourcing-mongodb-3.0.2/setup.py
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 19:06:12.178029 eventsourcing-mongodb-3.0.2/tests/
+-rw-r--r--   0 luca      (1000) luca      (1001)      295 2022-07-19 09:04:23.000000 eventsourcing-mongodb-3.0.2/tests/test_aggregate_recorder.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     1347 2022-07-19 08:46:06.000000 eventsourcing-mongodb-3.0.2/tests/test_datastore.py
```

### Comparing `eventsourcing-mongodb-3.0.0/LICENSE` & `eventsourcing-mongodb-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-3.0.0/PKG-INFO` & `eventsourcing-mongodb-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventsourcing-mongodb
-Version: 3.0.0
+Version: 3.0.2
 Summary: An extension package for the Python Eventsourcing library that provides a persistence module for MongoDB.
 Author: Luxaaa
 License: MIT License
         
         Copyright (c) 2022 Luxaaa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `eventsourcing-mongodb-3.0.0/README.md` & `eventsourcing-mongodb-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/datastore.py` & `eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/datastore.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/factory.py` & `eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/factory.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/aggregate.py` & `eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/recorders/aggregate.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/application.py` & `eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/recorders/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,17 @@
         cursor = col.find(self._build_select_notifications_query(start, stop=stop, topics=topics)).sort('position', 1)
         if limit:
             cursor.limit(limit)
         documents = list(cursor)
         notifications = self._documents_to_notifications(documents)
         return notifications
 
+    def max_notification_id(self):
+        return 0
+
     @classmethod
     def _build_select_notifications_query(cls, start: int, stop: Optional[int] = None,
                                           topics: Sequence[str] = ()) -> dict:
         query = {'originator_version': {'$gte': start}}
         if stop:
             query['originator_version']['$lte'] = stop
         if topics:
```

### Comparing `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/process.py` & `eventsourcing-mongodb-3.0.2/eventsourcing_mongodb/recorders/process.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/PKG-INFO` & `eventsourcing-mongodb-3.0.2/eventsourcing_mongodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventsourcing-mongodb
-Version: 3.0.0
+Version: 3.0.2
 Summary: An extension package for the Python Eventsourcing library that provides a persistence module for MongoDB.
 Author: Luxaaa
 License: MIT License
         
         Copyright (c) 2022 Luxaaa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/SOURCES.txt` & `eventsourcing-mongodb-3.0.2/eventsourcing_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-3.0.0/pyproject.toml` & `eventsourcing-mongodb-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eventsourcing-mongodb"
-version = "3.0.0"
+version = "3.0.2"
 description = "An extension package for the Python Eventsourcing library that provides a persistence module for MongoDB."
 readme = "README.md"
 authors = [{ name = "Luxaaa"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `eventsourcing-mongodb-3.0.0/tests/test_datastore.py` & `eventsourcing-mongodb-3.0.2/tests/test_datastore.py`

 * *Files identical despite different names*


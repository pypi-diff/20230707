# Comparing `tmp/eventsourcing-mongodb-2.0.1.tar.gz` & `tmp/eventsourcing-mongodb-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventsourcing-mongodb-2.0.1.tar", last modified: Mon Sep  5 16:50:10 2022, max compression
+gzip compressed data, was "eventsourcing-mongodb-3.0.0.tar", last modified: Fri Jul  7 15:17:06 2023, max compression
```

## Comparing `eventsourcing-mongodb-2.0.1.tar` & `eventsourcing-mongodb-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2022-09-05 16:50:10.136073 eventsourcing-mongodb-2.0.1/
--rw-r--r--   0 luca      (1000) luca      (1001)     1062 2022-07-18 14:29:26.000000 eventsourcing-mongodb-2.0.1/LICENSE
--rw-r--r--   0 luca      (1000) luca      (1001)     5787 2022-09-05 16:50:10.136073 eventsourcing-mongodb-2.0.1/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1001)     4007 2022-08-08 13:06:49.000000 eventsourcing-mongodb-2.0.1/README.md
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2022-09-05 16:50:10.136073 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/
--rw-r--r--   0 luca      (1000) luca      (1001)       29 2022-07-19 00:25:05.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1001)     1146 2022-07-19 08:36:58.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/datastore.py
--rw-r--r--   0 luca      (1000) luca      (1001)     2632 2022-08-08 13:06:49.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/factory.py
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2022-09-05 16:50:10.136073 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/recorders/
--rw-r--r--   0 luca      (1000) luca      (1001)      144 2022-07-18 22:11:10.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/recorders/__init__.py
--rw-r--r--   0 luca      (1000) luca      (1001)     3362 2022-09-05 16:48:14.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/recorders/aggregate.py
--rw-r--r--   0 luca      (1000) luca      (1001)     2173 2022-07-18 23:55:50.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/recorders/application.py
--rw-r--r--   0 luca      (1000) luca      (1001)     2114 2022-07-18 23:50:54.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/recorders/process.py
-drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2022-09-05 16:50:10.136073 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb.egg-info/
--rw-r--r--   0 luca      (1000) luca      (1001)     5787 2022-09-05 16:50:10.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 luca      (1000) luca      (1001)      546 2022-09-05 16:50:10.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 luca      (1000) luca      (1001)        1 2022-09-05 16:50:10.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 luca      (1000) luca      (1001)       43 2022-09-05 16:50:10.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb.egg-info/requires.txt
--rw-r--r--   0 luca      (1000) luca      (1001)       22 2022-09-05 16:50:10.000000 eventsourcing-mongodb-2.0.1/eventsourcing_mongodb.egg-info/top_level.txt
--rw-r--r--   0 luca      (1000) luca      (1001)      770 2022-09-05 16:48:38.000000 eventsourcing-mongodb-2.0.1/pyproject.toml
--rw-r--r--   0 luca      (1000) luca      (1001)       38 2022-09-05 16:50:10.136073 eventsourcing-mongodb-2.0.1/setup.cfg
--rw-r--r--   0 luca      (1000) luca      (1001)       38 2022-07-19 02:00:30.000000 eventsourcing-mongodb-2.0.1/setup.py
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/
+-rw-r--r--   0 luca      (1000) luca      (1001)     1062 2022-07-18 14:29:26.000000 eventsourcing-mongodb-3.0.0/LICENSE
+-rw-r--r--   0 luca      (1000) luca      (1001)     5600 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1001)     3820 2023-07-07 15:13:48.000000 eventsourcing-mongodb-3.0.0/README.md
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/
+-rw-r--r--   0 luca      (1000) luca      (1001)       29 2022-07-19 00:25:05.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     1146 2022-07-19 08:36:58.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/datastore.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     2123 2023-07-07 15:12:57.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/factory.py
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/
+-rw-r--r--   0 luca      (1000) luca      (1001)      144 2022-07-18 22:11:10.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/__init__.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     2789 2023-07-07 15:05:19.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/aggregate.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     1831 2023-07-07 15:11:14.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/application.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     1056 2023-07-07 15:11:14.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/process.py
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/
+-rw-r--r--   0 luca      (1000) luca      (1001)     5600 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 luca      (1000) luca      (1001)      603 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 luca      (1000) luca      (1001)        1 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 luca      (1000) luca      (1001)       43 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/requires.txt
+-rw-r--r--   0 luca      (1000) luca      (1001)       22 2023-07-07 15:17:06.000000 eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 luca      (1000) luca      (1001)      770 2023-07-07 15:14:56.000000 eventsourcing-mongodb-3.0.0/pyproject.toml
+-rw-r--r--   0 luca      (1000) luca      (1001)       38 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/setup.cfg
+-rw-r--r--   0 luca      (1000) luca      (1001)       38 2022-07-19 02:00:30.000000 eventsourcing-mongodb-3.0.0/setup.py
+drwxr-xr-x   0 luca      (1000) luca      (1001)        0 2023-07-07 15:17:06.194930 eventsourcing-mongodb-3.0.0/tests/
+-rw-r--r--   0 luca      (1000) luca      (1001)      295 2022-07-19 09:04:23.000000 eventsourcing-mongodb-3.0.0/tests/test_aggregate_recorder.py
+-rw-r--r--   0 luca      (1000) luca      (1001)     1347 2022-07-19 08:46:06.000000 eventsourcing-mongodb-3.0.0/tests/test_datastore.py
```

### Comparing `eventsourcing-mongodb-2.0.1/LICENSE` & `eventsourcing-mongodb-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-2.0.1/PKG-INFO` & `eventsourcing-mongodb-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventsourcing-mongodb
-Version: 2.0.1
+Version: 3.0.0
 Summary: An extension package for the Python Eventsourcing library that provides a persistence module for MongoDB.
 Author: Luxaaa
 License: MIT License
         
         Copyright (c) 2022 Luxaaa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -125,11 +125,10 @@
 
 | Variable | Type / Possible values | Required | Description |
 | --- | --- | --- | --- |
 | `PERSISTENCE_MODULE` | `'eventsourcing_mongodb'` | `true` | configures the application to use this module for persistence. 
 | `MONGO_CONNECTION_STRING` | string | `true` | MongoDB Connection String. Please refer to the [MongoDB Documentation](https://www.mongodb.com/docs/manual/reference/connection-string/) to learn more about connection strings.
 | `MONGO_DB_NAME` | string | `true` | Name of the Database the data sould be stored in
 | `MONGO_COL_PREFIX` | string | `false` | Prefix for the MongoDB Collections for events, snapshots and trackings. The default is an empty String.
-| `MONGO_COUNTTRACK_COL_NAME` | string | `false` | Name of the MongoDB Collection for count trakcings. The default is CountTracking. (You can use the same name for multiple applications)
```

### Comparing `eventsourcing-mongodb-2.0.1/README.md` & `eventsourcing-mongodb-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -89,11 +89,10 @@
 
 | Variable | Type / Possible values | Required | Description |
 | --- | --- | --- | --- |
 | `PERSISTENCE_MODULE` | `'eventsourcing_mongodb'` | `true` | configures the application to use this module for persistence. 
 | `MONGO_CONNECTION_STRING` | string | `true` | MongoDB Connection String. Please refer to the [MongoDB Documentation](https://www.mongodb.com/docs/manual/reference/connection-string/) to learn more about connection strings.
 | `MONGO_DB_NAME` | string | `true` | Name of the Database the data sould be stored in
 | `MONGO_COL_PREFIX` | string | `false` | Prefix for the MongoDB Collections for events, snapshots and trackings. The default is an empty String.
-| `MONGO_COUNTTRACK_COL_NAME` | string | `false` | Name of the MongoDB Collection for count trakcings. The default is CountTracking. (You can use the same name for multiple applications)
```

### Comparing `eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/datastore.py` & `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/datastore.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/factory.py` & `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from eventsourcing_mongodb.recorders import MongoDBAggregateRecorder, MongoDBApplicationRecorder, MongoDBProcessRecorder
 
 
 class Factory(InfrastructureFactory):
     MONGO_CONNECTION_STRING = 'MONGO_CONNECTION_STRING'
     MONGO_DB_NAME = 'MONGO_DB_NAME'
     MONGO_COL_PREFIX = 'MONGO_COL_PREFIX'
-    MONGO_COUNTTRACK_COL_NAME = 'MONGO_COUNTTRACK_COL_NAME'
 
     def __init__(self, env: Environment):
         super().__init__(env)
         conn_str = self.env.get(self.MONGO_CONNECTION_STRING)
         if not conn_str:
             keys = self.env.create_keys(self.MONGO_CONNECTION_STRING)
             raise EnvironmentError(f'MongoDB connection string not found in environment with keys: {", ".join(keys)}')
@@ -20,31 +19,25 @@
         if not db_name:
             keys = self.env.create_keys(self.MONGO_DB_NAME)
             raise EnvironmentError(f'MongoDB database name not found in environment with keys: {", ".join(keys)}')
 
         self.datastore = MongoDataStore(conn_str, db_name)
 
     def aggregate_recorder(self, purpose: str = "events") -> AggregateRecorder:
-        recorder = MongoDBAggregateRecorder(self.datastore, self._events_collection_name(purpose),
-                                            count_track_collection_name=self._count_track_collection_name())
+        recorder = MongoDBAggregateRecorder(self.datastore, self._events_collection_name(purpose))
         return recorder
 
     def application_recorder(self) -> ApplicationRecorder:
-        recorder = MongoDBApplicationRecorder(self.datastore, self._events_collection_name('events'),
-                                              count_track_collection_name=self._count_track_collection_name())
+        recorder = MongoDBApplicationRecorder(self.datastore, self._events_collection_name('events'))
         return recorder
 
     def process_recorder(self) -> ProcessRecorder:
         recorder = MongoDBProcessRecorder(self.datastore, self._events_collection_name('events'),
-                                          count_track_collection_name=self._count_track_collection_name(),
                                           trackings_collection_name=self._trackings_collection_name()
                                           )
         return recorder
 
     def _events_collection_name(self, purpose: str):
         return self.env.get(self.MONGO_COL_PREFIX, '') + purpose.capitalize()
 
-    def _count_track_collection_name(self):
-        return self.env.get(self.MONGO_COUNTTRACK_COL_NAME, 'CountTracking')
-
     def _trackings_collection_name(self):
         return self.env.get(self.MONGO_COL_PREFIX, 'Trackings')
```

### Comparing `eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/recorders/aggregate.py` & `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/aggregate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from eventsourcing.persistence import AggregateRecorder, StoredEvent
 from eventsourcing_mongodb.datastore import MongoDataStore
 import pymongo
-from uuid import UUID
+from uuid import UUID, uuid4
 from typing import List, Optional, Sequence, Dict, Any
 
 
 class MongoDBAggregateRecorder(AggregateRecorder):
-    def __init__(self, datastore: MongoDataStore, events_collection_name: str,
-                 count_track_collection_name='EventCountTrackers'):
+    def __init__(self, datastore: MongoDataStore, events_collection_name: str):
         self.datastore = datastore
         self.events_col_name = events_collection_name
-        self.count_track_col_name = count_track_collection_name
 
-    def insert_events(self, stored_events: List[StoredEvent], **kwargs: Any) -> Optional[Sequence[int]]:
+    def insert_events(self, stored_events: List[StoredEvent], **kwargs: Any) -> Optional[Sequence[Any]]:
         documents = self._stored_events_to_documents(stored_events)
         collection = self.datastore.get_collection(self.events_col_name)  # database collection
         collection.insert_many(documents)
         return [doc['_id'] for doc in documents]
 
     def select_events(
             self,
@@ -31,24 +29,18 @@
         cursor = collection.find(query)
         cursor = cursor.sort('originator_version', pymongo.DESCENDING if desc else pymongo.ASCENDING)
         if limit:
             cursor = cursor.limit(limit)
         documents = list(cursor)
         return self._documents_to_stored_events(documents)
 
-    def _get_next_doc_id_and_update_counter(self, col_name: str, amount_of_docs: int):
-        col = self.datastore.get_collection(self.count_track_col_name)
-        counter_doc = col.find_one_and_update({'_id': col_name}, {'$inc': {'counter': amount_of_docs}}, upsert=True)
-        return counter_doc['counter'] + 1 if counter_doc else 1
-
     def _stored_events_to_documents(self, stored_events: List[StoredEvent]) -> List[Dict[str, Any]]:
         """ converts a list of stored events into dicts which can be inserted into mongodb. """
-        start_id = self._get_next_doc_id_and_update_counter(self.events_col_name, len(stored_events))
         return [{
-            '_id': start_id + idx,
+            '_id': uuid4(),
             'originator_id': e.originator_id,
             'originator_version': e.originator_version,
             'topic': e.topic,
             'state': e.state
         } for idx, e in enumerate(stored_events)]
 
     @classmethod
```

### Comparing `eventsourcing-mongodb-2.0.1/eventsourcing_mongodb/recorders/application.py` & `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb/recorders/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from eventsourcing.persistence import ApplicationRecorder, Notification
 
 from eventsourcing_mongodb.datastore import MongoDataStore
 from eventsourcing_mongodb.recorders.aggregate import MongoDBAggregateRecorder
 
 
 class MongoDBApplicationRecorder(MongoDBAggregateRecorder, ApplicationRecorder):
-    def __init__(self, datastore: MongoDataStore, events_collection_name: str,
-                 count_track_collection_name='EventCountTrackers'):
-        super().__init__(datastore, events_collection_name, count_track_collection_name=count_track_collection_name)
+    def __init__(self, datastore: MongoDataStore, events_collection_name: str):
+        super().__init__(datastore, events_collection_name)
 
     def select_notifications(
             self,
             start: int,
             limit: int,
             stop: Optional[int] = None,
             topics: Sequence[str] = (),
@@ -22,25 +21,20 @@
         cursor = col.find(self._build_select_notifications_query(start, stop=stop, topics=topics)).sort('position', 1)
         if limit:
             cursor.limit(limit)
         documents = list(cursor)
         notifications = self._documents_to_notifications(documents)
         return notifications
 
-    def max_notification_id(self) -> int:
-        collection = self.datastore.get_collection(self.count_track_col_name)
-        count_doc = collection.find_one({'_id': self.events_col_name})
-        return count_doc['counter'] if count_doc else 0
-
     @classmethod
     def _build_select_notifications_query(cls, start: int, stop: Optional[int] = None,
                                           topics: Sequence[str] = ()) -> dict:
-        query = {'_id': {'$gte': start}}
+        query = {'originator_version': {'$gte': start}}
         if stop:
-            query['_id']['$lte'] = stop
+            query['originator_version']['$lte'] = stop
         if topics:
             query['topic'] = {'$in': topics}
         return query
 
     @classmethod
     def _documents_to_notifications(cls, documents: List[Dict[str, Any]]) -> List[Notification]:
         return [Notification(
```

### Comparing `eventsourcing-mongodb-2.0.1/eventsourcing_mongodb.egg-info/PKG-INFO` & `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventsourcing-mongodb
-Version: 2.0.1
+Version: 3.0.0
 Summary: An extension package for the Python Eventsourcing library that provides a persistence module for MongoDB.
 Author: Luxaaa
 License: MIT License
         
         Copyright (c) 2022 Luxaaa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -125,11 +125,10 @@
 
 | Variable | Type / Possible values | Required | Description |
 | --- | --- | --- | --- |
 | `PERSISTENCE_MODULE` | `'eventsourcing_mongodb'` | `true` | configures the application to use this module for persistence. 
 | `MONGO_CONNECTION_STRING` | string | `true` | MongoDB Connection String. Please refer to the [MongoDB Documentation](https://www.mongodb.com/docs/manual/reference/connection-string/) to learn more about connection strings.
 | `MONGO_DB_NAME` | string | `true` | Name of the Database the data sould be stored in
 | `MONGO_COL_PREFIX` | string | `false` | Prefix for the MongoDB Collections for events, snapshots and trackings. The default is an empty String.
-| `MONGO_COUNTTRACK_COL_NAME` | string | `false` | Name of the MongoDB Collection for count trakcings. The default is CountTracking. (You can use the same name for multiple applications)
```

### Comparing `eventsourcing-mongodb-2.0.1/eventsourcing_mongodb.egg-info/SOURCES.txt` & `eventsourcing-mongodb-3.0.0/eventsourcing_mongodb.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -9,8 +9,10 @@
 eventsourcing_mongodb.egg-info/SOURCES.txt
 eventsourcing_mongodb.egg-info/dependency_links.txt
 eventsourcing_mongodb.egg-info/requires.txt
 eventsourcing_mongodb.egg-info/top_level.txt
 eventsourcing_mongodb/recorders/__init__.py
 eventsourcing_mongodb/recorders/aggregate.py
 eventsourcing_mongodb/recorders/application.py
-eventsourcing_mongodb/recorders/process.py
+eventsourcing_mongodb/recorders/process.py
+tests/test_aggregate_recorder.py
+tests/test_datastore.py
```

### Comparing `eventsourcing-mongodb-2.0.1/pyproject.toml` & `eventsourcing-mongodb-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eventsourcing-mongodb"
-version = "2.0.1"
+version = "3.0.0"
 description = "An extension package for the Python Eventsourcing library that provides a persistence module for MongoDB."
 readme = "README.md"
 authors = [{ name = "Luxaaa"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```


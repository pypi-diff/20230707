# Comparing `tmp/lib310_lite-0.1.0.dev3.tar.gz` & `tmp/lib310_lite-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.1.0.dev3.tar", max compression
+gzip compressed data, was "lib310_lite-0.1.0.dev4.tar", max compression
```

## Comparing `lib310_lite-0.1.0.dev3.tar` & `lib310_lite-0.1.0.dev4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev3/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev3/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev3/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev3/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0    11752 2023-07-06 12:50:42.285615 lib310_lite-0.1.0.dev3/lib310_lite/laser/laser.py
--rw-r--r--   0        0        0      778 2023-07-06 12:51:21.380002 lib310_lite-0.1.0.dev3/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev3/setup.py
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev4/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev4/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev4/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev4/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0    13106 2023-07-07 12:31:58.113908 lib310_lite-0.1.0.dev4/lib310_lite/laser/laser.py
+-rw-r--r--   0        0        0      778 2023-07-07 12:32:03.228499 lib310_lite-0.1.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev4/setup.py
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev4/PKG-INFO
```

### Comparing `lib310_lite-0.1.0.dev3/lib310_lite/bigquery/client.py` & `lib310_lite-0.1.0.dev4/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev3/lib310_lite/bigquery/constants.py` & `lib310_lite-0.1.0.dev4/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev3/lib310_lite/laser/laser.py` & `lib310_lite-0.1.0.dev4/lib310_lite/laser/laser.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 from queue import Queue
 from threading import Thread, Event
 from bounded_pool_executor import BoundedThreadPoolExecutor
 
 import pandas as pd
 import time
 
+
 class Laser:
 
     instances = 0
     instances_limit = 5
 
-    def __init__(self, db_config: dict, cache_size: int = 50, num_threads: int = 10):
+    def __init__(self, db_config: dict, cache_size: int = 30, num_threads: int = 10):
         if Laser.instances >= Laser.instances_limit:
             raise Exception('Too many instances of Laser')
         if db_config is None:
             raise Exception('db_config must be provided')
         Laser.instances += 1
 
         # Constants
@@ -52,14 +53,41 @@
         # response queue (only works with buffering technique)
         self.response_queue = Queue(self.cache_size)
         # Thread that fill the response queue
         self.fill_response_queue_thread = None
         # Signal to stop the fill_response_queue_thread
         self.kill_fill_response_queue_thread = Event()
 
+    def get_cached_queries(self):
+        """
+        Get the cached query
+        :return: cached query
+        """
+        cnx = None
+        cursor = None
+        try:
+            # Establish a connection to the database
+            cnx = MySQLdb.connect(**self.db_config, )
+            cursor = cnx.cursor(cursorclass=MySQLdb.cursors.DictCursor)
+            # check if the query is already in the database
+            cursor.execute(f"SELECT * FROM {self.CACHED_TABLE_NAME}")
+            result = cursor.fetchall()
+            if result is None:
+                return None
+            else:
+                return result
+        except Exception as e:
+            print(e)
+            return None
+        finally:
+            if cursor is not None:
+                cursor.close()
+            if cnx is not None:
+                cnx.close()
+
     def create_pool(self, query: str = None, force_update: bool = False):
         """
         Create a pool of row_id's from the database
         :param query: The query to be executed and cached to create the pool
         :param force_update: ignore cache and force update
         :return:
             hit is True if the query was already in the database, False otherwise (even in force update is False)
@@ -69,28 +97,31 @@
         cnx = None
         cursor = None
         result = None
         try:
             # pool hash is using MD5
             h = hashlib.md5(query.encode()).hexdigest()
             # Establish a connection to the database
-            cnx = MySQLdb.connect(**self.db_config)
+            cnx = MySQLdb.connect(**self.db_config, cnnect_timeout=1200)
             cursor = cnx.cursor()
             query = query.strip()
 
             # check if the query is already in the database
             cursor.execute("SELECT * FROM cached WHERE hash = %s", (h,))
             result = cursor.fetchone()
 
             if result is None or force_update:
                 hit = False
                 cursor.execute("DROP TABLE IF EXISTS pool_{}".format(h))
-                print("Dropped table pool_{}".format(h))
+                print("Dropped If table Exists pool_{}".format(h))
                 # Create a table pool_{hash} with the query
+                print("Start creating table pool_{}".format(h))
                 cursor.execute("CREATE TABLE pool_{} AS {}".format(h, query))
+                print("Commit pool_{}".format(h))
+                cursor.commit()
                 print("Created table pool_{}".format(h))
                 if result is None:
                     # Create a row in the table cached
                     cursor.execute(f"INSERT INTO {self.CACHED_TABLE_NAME} (query, hash) VALUES (%s, %s)", (query, h,))
                     print(f"Inserted query {query} in {self.CACHED_TABLE_NAME}")
                 else:
                     # Update the row in the table cached
@@ -105,15 +136,15 @@
             # If the query is already in the database, check if it is valid
             if cursor is not None:
                 cursor.close()
             if cnx is not None:
                 cnx.close()
             return {"hit": hit, "result": result}
 
-    def get_pool(self, query: str = None, hashed: str = None, collate_fn: callable = None):
+    def get_pool(self, query: str = None, hashed: str = None, collate_fn: callable = None, num_parts: int = 1, part: int = 0):
         """
         Get the pool of row_id's from the database
         :param query: the query we want it's pool
         :param hashed: the hashed of the query we want it's pool
         :param collate_fn: how to reach extract data from pool in the database to only row_id's
         :return: pool of row_id's
         """
@@ -152,18 +183,24 @@
         finally:
             if cursor is not None:
                 cursor.close()
             if cnx is not None:
                 cnx.close()
             if self.pool is None:
                 return None
-            if collate_fn is None:
+            if collate_fn is not None:
+                self.pool = collate_fn(self.pool)
+            else:
                 self.pool = [t[0] for t in self.pool]
-                return self.pool
-            self.pool = collate_fn(self.pool)
+
+            pool_len = len(self.pool)
+            if num_parts > 1:
+                # If distributed, split the pool into num_parts parts and return the part with index part
+                self.pool = [self.pool[j:j + pool_len // num_parts] for j in range(0, pool_len, pool_len // num_parts)][part]
+
             return self.pool
 
     def start_buffering(self, sample_number: int, short_nap: int = 2, starting_batch_number: int = 0) -> None:
         """
         Start buffering technique
         :param sample_number: the number of row_id's in each chunk
         :param short_nap: the time to sleep at begging of starting the buffering to let buffer fill
```

### Comparing `lib310_lite-0.1.0.dev3/pyproject.toml` & `lib310_lite-0.1.0.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.1.0.dev3"
+version = "0.1.0.dev4"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.1.0.dev3/setup.py` & `lib310_lite-0.1.0.dev4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'mysqlclient>=2.0.0',
  'numpy<1.23.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.1.0.dev3',
+    'version': '0.1.0.dev4',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.1.0.dev3/PKG-INFO` & `lib310_lite-0.1.0.dev4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```


# Comparing `tmp/lib310_lite-0.1.0.dev4.tar.gz` & `tmp/lib310_lite-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.1.0.dev4.tar", max compression
+gzip compressed data, was "lib310_lite-0.1.0.dev5.tar", max compression
```

## Comparing `lib310_lite-0.1.0.dev4.tar` & `lib310_lite-0.1.0.dev5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev4/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev4/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev4/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev4/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0    13106 2023-07-07 12:31:58.113908 lib310_lite-0.1.0.dev4/lib310_lite/laser/laser.py
--rw-r--r--   0        0        0      778 2023-07-07 12:32:03.228499 lib310_lite-0.1.0.dev4/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev4/setup.py
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0      253 2023-07-06 11:48:04.613198 lib310_lite-0.1.0.dev5/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.1.0.dev5/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.1.0.dev5/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.1.0.dev5/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0    13107 2023-07-07 12:45:49.101315 lib310_lite-0.1.0.dev5/lib310_lite/laser/laser.py
+-rw-r--r--   0        0        0      778 2023-07-07 12:45:58.538799 lib310_lite-0.1.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev5/setup.py
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 lib310_lite-0.1.0.dev5/PKG-INFO
```

### Comparing `lib310_lite-0.1.0.dev4/lib310_lite/bigquery/client.py` & `lib310_lite-0.1.0.dev5/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev4/lib310_lite/bigquery/constants.py` & `lib310_lite-0.1.0.dev5/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.1.0.dev4/lib310_lite/laser/laser.py` & `lib310_lite-0.1.0.dev5/lib310_lite/laser/laser.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         cnx = None
         cursor = None
         result = None
         try:
             # pool hash is using MD5
             h = hashlib.md5(query.encode()).hexdigest()
             # Establish a connection to the database
-            cnx = MySQLdb.connect(**self.db_config, cnnect_timeout=1200)
+            cnx = MySQLdb.connect(**self.db_config, connect_timeout=1200)
             cursor = cnx.cursor()
             query = query.strip()
 
             # check if the query is already in the database
             cursor.execute("SELECT * FROM cached WHERE hash = %s", (h,))
             result = cursor.fetchone()
```

### Comparing `lib310_lite-0.1.0.dev4/pyproject.toml` & `lib310_lite-0.1.0.dev5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.1.0.dev4"
+version = "0.1.0.dev5"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.1.0.dev4/setup.py` & `lib310_lite-0.1.0.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'mysqlclient>=2.0.0',
  'numpy<1.23.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.1.0.dev4',
+    'version': '0.1.0.dev5',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.1.0.dev4/PKG-INFO` & `lib310_lite-0.1.0.dev5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```


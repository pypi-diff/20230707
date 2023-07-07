# Comparing `tmp/logger-local-0.0.7.tar.gz` & `tmp/logger-local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-local-0.0.7.tar", last modified: Fri Jul  7 07:15:01 2023, max compression
+gzip compressed data, was "logger-local-0.0.8.tar", last modified: Fri Jul  7 07:40:42 2023, max compression
```

## Comparing `logger-local-0.0.7.tar` & `logger-local-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:15:01.504119 logger-local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 07:14:46.000000 logger-local-0.0.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:15:01.504119 logger-local-0.0.7/LoggerLocalPythonPackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-07 07:14:46.000000 logger-local-0.0.7/LoggerLocalPythonPackage/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-07 07:14:46.000000 logger-local-0.0.7/LoggerLocalPythonPackage/LoggerServiceSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 07:14:46.000000 logger-local-0.0.7/LoggerLocalPythonPackage/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-07 07:14:46.000000 logger-local-0.0.7/LoggerLocalPythonPackage/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:14:46.000000 logger-local-0.0.7/LoggerLocalPythonPackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 07:15:01.504119 logger-local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-07 07:14:46.000000 logger-local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:15:01.504119 logger-local-0.0.7/logger_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 07:15:01.000000 logger-local-0.0.7/logger_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 07:15:01.000000 logger-local-0.0.7/logger_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:15:01.000000 logger-local-0.0.7/logger_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 07:15:01.000000 logger-local-0.0.7/logger_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:15:01.504119 logger-local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-07 07:14:46.000000 logger-local-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:15:01.504119 logger-local-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-07 07:14:46.000000 logger-local-0.0.7/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:42.025340 logger-local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 07:40:32.000000 logger-local-0.0.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:42.025340 logger-local-0.0.8/LoggerLocalPythonPackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/LoggerServiceSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:32.000000 logger-local-0.0.8/LoggerLocalPythonPackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 07:40:42.025340 logger-local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-07 07:40:32.000000 logger-local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:42.025340 logger-local-0.0.8/logger_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 07:40:42.000000 logger-local-0.0.8/logger_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 07:40:42.000000 logger-local-0.0.8/logger_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:40:42.000000 logger-local-0.0.8/logger_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 07:40:42.000000 logger-local-0.0.8/logger_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:40:42.029341 logger-local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-07 07:40:32.000000 logger-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:40:42.025340 logger-local-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-07 07:40:32.000000 logger-local-0.0.8/tests/test_writer.py
```

### Comparing `logger-local-0.0.7/LICENSE` & `logger-local-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.7/LoggerLocalPythonPackage/LoggerService.py` & `logger-local-0.0.8/LoggerLocalPythonPackage/LoggerService.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.7/LoggerLocalPythonPackage/Writer.py` & `logger-local-0.0.8/LoggerLocalPythonPackage/Writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import pymysql
 import os
 from dotenv import load_dotenv
 load_dotenv()
 
+debug = os.getenv('DEBUG')
+
 class Writer:
 
     # TODO: We need to replace this with the database package
     def get_connection(self) -> pymysql.connections.Connection:
-        return pymysql.connect(
+        if (debug): print ("get_connection")
+        result = pymysql.connect(
             user=os.getenv('RDS_USERNAME'),
             password=os.getenv('RDS_PASSWORD'),
             host=os.getenv('RDS_HOSTNAME'),
             database='logger' # os.getenv('RDS_DB_NAME')
         )
+        if (debug): print(result)
+        return result
 
     def add(self, **kwargs):
 
         try:
             params_to_insert = kwargs['object']
             # creating connection
             connection = self.get_connection()
@@ -51,22 +56,22 @@
             print("catched " + str(e))
         finally:
             connection.commit()
             cursor.close()
             connection.close()
 
     def add_message(self, message, log_level):
-
+        if (debug): print ("add_message" + message+ ' ' + log_level)
         try:
             # creating connection
             connection = self.get_connection()
             # connection = self._pool.get_connection()
             cursor = connection.cursor()
-            sql = f"INSERT INTO logger_table (payload, severity_id) VALUES ('{message}', {log_level})"
+            sql = f"INSERT INTO logger.logger_table (payload, severity_id) VALUES ('{message}', {log_level})"
             cursor.execute(sql)
 
         except Exception as e:
-            print("catched" + str(e))
+            print("Writer.py Writer.add_message catched" + str(e))
         finally:
             connection.commit()
             cursor.close()
             connection.close()
```

### Comparing `logger-local-0.0.7/PKG-INFO` & `logger-local-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.7/README.md` & `logger-local-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.7/logger_local.egg-info/PKG-INFO` & `logger-local-0.0.8/logger_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.7/setup.py` & `logger-local-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='logger-local',
-    version='0.0.7',
+    version='0.0.8',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Logger Python Local",
     long_description="This is a package for sharing common Logger function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles-zone/logger-local-python-package",
     packages=setuptools.find_packages(),
```

### Comparing `logger-local-0.0.7/tests/test_writer.py` & `logger-local-0.0.8/tests/test_writer.py`

 * *Files identical despite different names*


# Comparing `tmp/simple-redis-helper-0.1.3.tar.gz` & `tmp/simple-redis-helper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-redis-helper-0.1.3.tar", last modified: Thu Jul  6 23:17:43 2023, max compression
+gzip compressed data, was "simple-redis-helper-0.1.4.tar", last modified: Thu Jul  6 23:43:17 2023, max compression
```

## Comparing `simple-redis-helper-0.1.3.tar` & `simple-redis-helper-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      443 2023-07-06 23:16:13.000000 simple-redis-helper-0.1.3/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      116 2021-09-14 00:46:54.000000 simple-redis-helper-0.1.3/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:54.000000 simple-redis-helper-0.1.3/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1302 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6466 2023-07-06 23:16:13.000000 simple-redis-helper-0.1.3/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1304 2023-07-06 23:17:14.000000 simple-redis-helper-0.1.3/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/src/simple_redis_helper/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:45:09.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2994 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/broadcast.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     4185 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/listen.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2174 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/load.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2479 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/save.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1159 2023-07-06 23:12:45.000000 simple-redis-helper-0.1.3/src/simple_redis_helper/utils.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:17:43.416156 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1302 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      546 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      213 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       20 2023-07-06 23:17:43.000000 simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:43:17.863657 simple-redis-helper-0.1.4/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      509 2023-07-06 23:42:35.000000 simple-redis-helper-0.1.4/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      116 2021-09-14 00:46:54.000000 simple-redis-helper-0.1.4/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:43:54.000000 simple-redis-helper-0.1.4/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1416 2023-07-06 23:43:17.863657 simple-redis-helper-0.1.4/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6466 2023-07-06 23:16:13.000000 simple-redis-helper-0.1.4/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-06 23:43:17.863657 simple-redis-helper-0.1.4/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1304 2023-07-06 23:42:35.000000 simple-redis-helper-0.1.4/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:43:17.859657 simple-redis-helper-0.1.4/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:43:17.863657 simple-redis-helper-0.1.4/src/simple_redis_helper/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2021-08-14 06:45:09.000000 simple-redis-helper-0.1.4/src/simple_redis_helper/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2994 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.4/src/simple_redis_helper/broadcast.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4185 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.4/src/simple_redis_helper/listen.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2174 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.4/src/simple_redis_helper/load.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2479 2023-07-06 23:14:03.000000 simple-redis-helper-0.1.4/src/simple_redis_helper/save.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1123 2023-07-06 23:40:55.000000 simple-redis-helper-0.1.4/src/simple_redis_helper/utils.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:43:17.863657 simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1416 2023-07-06 23:43:17.000000 simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      546 2023-07-06 23:43:17.000000 simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-06 23:43:17.000000 simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      213 2023-07-06 23:43:17.000000 simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2023-07-06 23:43:17.000000 simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       20 2023-07-06 23:43:17.000000 simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/top_level.txt
```

### Comparing `simple-redis-helper-0.1.3/PKG-INFO` & `simple-redis-helper-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 1.1
 Name: simple-redis-helper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Command-line utilities to for sending/receiving data to/from a Redis backend.
 Home-page: https://github.com/fracpete/redis_helper
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Little command-line library to send/receive data to/from a Redis backend.
         
         https://github.com/fracpete/redis_helper
         
         Changelog
         =========
         
+        0.1.4 (2023-07-07)
+        ------------------
+        
+        - fixed password support
+        
+        
         0.1.3 (2023-07-07)
         ------------------
         
         - added support for supplying a password for connecting to the Redis server (`--password` or `--password_env`)
         
         
         0.1.2 (2021-10-01)
```

### Comparing `simple-redis-helper-0.1.3/README.md` & `simple-redis-helper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `simple-redis-helper-0.1.3/setup.py` & `simple-redis-helper-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     license='MIT License',
     package_dir={
         '': 'src'
     },
     packages=[
       'simple_redis_helper',
     ],
-    version="0.1.3",
+    version="0.1.4",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     install_requires=[
         "redis",
     ],
     entry_points={
         "console_scripts": [
```

### Comparing `simple-redis-helper-0.1.3/src/simple_redis_helper/broadcast.py` & `simple-redis-helper-0.1.4/src/simple_redis_helper/broadcast.py`

 * *Files identical despite different names*

### Comparing `simple-redis-helper-0.1.3/src/simple_redis_helper/listen.py` & `simple-redis-helper-0.1.4/src/simple_redis_helper/listen.py`

 * *Files identical despite different names*

### Comparing `simple-redis-helper-0.1.3/src/simple_redis_helper/load.py` & `simple-redis-helper-0.1.4/src/simple_redis_helper/load.py`

 * *Files identical despite different names*

### Comparing `simple-redis-helper-0.1.3/src/simple_redis_helper/save.py` & `simple-redis-helper-0.1.4/src/simple_redis_helper/save.py`

 * *Files identical despite different names*

### Comparing `simple-redis-helper-0.1.3/src/simple_redis_helper/utils.py` & `simple-redis-helper-0.1.4/src/simple_redis_helper/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     Direct password takes precedence over environment variable.
 
     :param ns: the namespace to check
     :return: True if a password has been supplied
     :rtype: bool
     """
     if hasattr(ns, "password"):
-        if ns.redis_password is not None:
+        if ns.password is not None:
             return True
 
     if hasattr(ns, "password_env"):
-        if os.getenv(ns.redis_password_env) is not None:
+        if os.getenv(ns.password_env) is not None:
             return True
 
     return False
 
 
 def get_password(ns):
     """
@@ -27,15 +27,15 @@
     Direct password takes precedence over environment variable.
 
     :param ns: the namespace to use
     :return: the password if one has been supplied, otherwise None
     :rtype: str
     """
     if hasattr(ns, "password"):
-        if ns.redis_password is not None:
-            return ns.redis_password
+        if ns.password is not None:
+            return ns.password
 
     if hasattr(ns, "password_env"):
-        if os.getenv(ns.redis_password_env) is not None:
-            return os.getenv(ns.redis_password_env)
+        if os.getenv(ns.password_env) is not None:
+            return os.getenv(ns.password_env)
 
     return None
```

### Comparing `simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/PKG-INFO` & `simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 1.1
 Name: simple-redis-helper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Command-line utilities to for sending/receiving data to/from a Redis backend.
 Home-page: https://github.com/fracpete/redis_helper
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Little command-line library to send/receive data to/from a Redis backend.
         
         https://github.com/fracpete/redis_helper
         
         Changelog
         =========
         
+        0.1.4 (2023-07-07)
+        ------------------
+        
+        - fixed password support
+        
+        
         0.1.3 (2023-07-07)
         ------------------
         
         - added support for supplying a password for connecting to the Redis server (`--password` or `--password_env`)
         
         
         0.1.2 (2021-10-01)
```

### Comparing `simple-redis-helper-0.1.3/src/simple_redis_helper.egg-info/SOURCES.txt` & `simple-redis-helper-0.1.4/src/simple_redis_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*


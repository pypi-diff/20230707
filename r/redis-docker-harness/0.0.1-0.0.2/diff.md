# Comparing `tmp/redis-docker-harness-0.0.1.tar.gz` & `tmp/redis-docker-harness-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-docker-harness-0.0.1.tar", last modified: Tue Sep 21 23:39:51 2021, max compression
+gzip compressed data, was "redis-docker-harness-0.0.2.tar", last modified: Thu Jul  6 23:23:40 2023, max compression
```

## Comparing `redis-docker-harness-0.0.1.tar` & `redis-docker-harness-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2021-09-21 23:39:51.885113 redis-docker-harness-0.0.1/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       78 2021-09-21 23:38:13.000000 redis-docker-harness-0.0.1/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      125 2021-09-21 22:04:15.000000 redis-docker-harness-0.0.1/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 redis-docker-harness-0.0.1/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      851 2021-09-21 23:39:51.885113 redis-docker-harness-0.0.1/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2021-09-21 23:31:38.000000 redis-docker-harness-0.0.1/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2021-09-21 23:39:51.885113 redis-docker-harness-0.0.1/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1114 2021-09-21 22:07:18.000000 redis-docker-harness-0.0.1/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2021-09-21 23:39:51.885113 redis-docker-harness-0.0.1/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2021-09-21 23:39:51.885113 redis-docker-harness-0.0.1/src/rdh/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      157 2021-09-21 23:03:29.000000 redis-docker-harness-0.0.1/src/rdh/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1651 2021-09-21 22:24:45.000000 redis-docker-harness-0.0.1/src/rdh/_argparse.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      203 2021-09-21 22:33:02.000000 redis-docker-harness-0.0.1/src/rdh/_log.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2455 2021-09-21 23:03:29.000000 redis-docker-harness-0.0.1/src/rdh/_redis.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2021-09-21 23:39:51.885113 redis-docker-harness-0.0.1/src/redis_docker_harness.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      851 2021-09-21 23:39:51.000000 redis-docker-harness-0.0.1/src/redis_docker_harness.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      372 2021-09-21 23:39:51.000000 redis-docker-harness-0.0.1/src/redis_docker_harness.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2021-09-21 23:39:51.000000 redis-docker-harness-0.0.1/src/redis_docker_harness.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2021-09-21 23:39:51.000000 redis-docker-harness-0.0.1/src/redis_docker_harness.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2021-09-21 23:39:51.000000 redis-docker-harness-0.0.1/src/redis_docker_harness.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      220 2023-07-06 23:22:44.000000 redis-docker-harness-0.0.2/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      125 2021-09-21 22:04:15.000000 redis-docker-harness-0.0.2/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 redis-docker-harness-0.0.2/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1041 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2021-09-21 23:31:38.000000 redis-docker-harness-0.0.2/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1045 2023-07-06 23:22:44.000000 redis-docker-harness-0.0.2/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/src/rdh/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      185 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.2/src/rdh/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3280 2023-07-06 23:08:51.000000 redis-docker-harness-0.0.2/src/rdh/_argparse.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      203 2021-09-21 22:33:02.000000 redis-docker-harness-0.0.2/src/rdh/_log.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2502 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.2/src/rdh/_redis.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1041 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      372 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/top_level.txt
```

### Comparing `redis-docker-harness-0.0.1/PKG-INFO` & `redis-docker-harness-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 1.1
 Name: redis-docker-harness
-Version: 0.0.1
+Version: 0.0.2
 Summary: Classes and methods for integrating code inside a docker image into a processing pipeline, using redis for exchanging data.
 Home-page: https://github.com/waikato-datamining/redis-docker-harness
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Classes and methods for integrating code inside a docker image into a processing pipeline, using redis for exchanging data.
         
         
         Changelog
         =========
         
+        0.0.2 (2023-07-07)
+        ------------------
+        
+        - added support for supplying a password to use for the Redis connection (--password/--password_env)
+        
+        
         0.0.1 (2021-09-22)
         ------------------
         
         - initial release
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `redis-docker-harness-0.0.1/setup.py` & `redis-docker-harness-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# setup.py
-# Copyright (C) 2021 University of Waikato, Hamilton, NZ
-
 from setuptools import setup
 
 
 def _read(f):
     """
     Reads in the content of the file.
     :param f: the file to read
@@ -34,11 +31,11 @@
     },
     packages=[
         "rdh",
     ],
     install_requires=[
         "redis",
     ],
-    version="0.0.1",
+    version="0.0.2",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
 )
```

### Comparing `redis-docker-harness-0.0.1/src/rdh/_redis.py` & `redis-docker-harness-0.0.2/src/rdh/_redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import redis
-import threading
+
+from ._argparse import get_password
 
 
 class Container(object):
     """
     Ancestor for containers.
     """
     pass
@@ -52,15 +53,15 @@
     :param ns: the parsed argparse namespace
     :type ns: argparse.Namespace
     :param config: additional parameters to make available via the "config" attribute in the returned container, eg a subclass of Container
     :return: the parameter container with the redis parts filled in
     :rtype: ParameterContainer
     """
     result = ParameterContainer()
-    result.redis = redis.Redis(host=ns.redis_host, port=ns.redis_port, db=ns.redis_db)
+    result.redis = redis.Redis(host=ns.redis_host, port=ns.redis_port, db=ns.redis_db, password=get_password(ns))
     result.pubsub = result.redis.pubsub()
     result.channel_in = ns.redis_in
     result.channel_out = ns.redis_out
     if config is not None:
         result.config = config
     return result
```

### Comparing `redis-docker-harness-0.0.1/src/redis_docker_harness.egg-info/PKG-INFO` & `redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 1.1
 Name: redis-docker-harness
-Version: 0.0.1
+Version: 0.0.2
 Summary: Classes and methods for integrating code inside a docker image into a processing pipeline, using redis for exchanging data.
 Home-page: https://github.com/waikato-datamining/redis-docker-harness
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT License
 Description: Classes and methods for integrating code inside a docker image into a processing pipeline, using redis for exchanging data.
         
         
         Changelog
         =========
         
+        0.0.2 (2023-07-07)
+        ------------------
+        
+        - added support for supplying a password to use for the Redis connection (--password/--password_env)
+        
+        
         0.0.1 (2021-09-22)
         ------------------
         
         - initial release
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```


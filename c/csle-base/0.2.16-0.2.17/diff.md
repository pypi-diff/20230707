# Comparing `tmp/csle_base-0.2.16.tar.gz` & `tmp/csle_base-0.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_base-0.2.16.tar", last modified: Fri Jul  7 11:00:12 2023, max compression
+gzip compressed data, was "csle_base-0.2.17.tar", last modified: Fri Jul  7 11:28:01 2023, max compression
```

## Comparing `csle_base-0.2.16.tar` & `csle_base-0.2.17.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 11:00:12.060485 csle_base-0.2.16/
--rw-r--r--   0 kimham     (501) staff       (20)      664 2023-07-07 11:00:12.060630 csle_base-0.2.16/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3391 2023-06-28 07:40:45.000000 csle_base-0.2.16/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      670 2023-06-11 13:17:52.000000 csle_base-0.2.16/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1222 2023-07-07 11:00:12.061237 csle_base-0.2.16/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2023-06-11 13:17:52.000000 csle_base-0.2.16/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 11:00:12.054209 csle_base-0.2.16/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 11:00:12.058110 csle_base-0.2.16/src/csle_base/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2023-06-11 13:17:52.000000 csle_base-0.2.16/src/csle_base/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       23 2023-07-07 11:00:01.000000 csle_base-0.2.16/src/csle_base/__version__.py
--rw-r--r--   0 kimham     (501) staff       (20)      574 2023-06-16 06:45:51.000000 csle_base-0.2.16/src/csle_base/grpc_serializable.py
--rw-r--r--   0 kimham     (501) staff       (20)     1537 2023-06-11 13:17:52.000000 csle_base-0.2.16/src/csle_base/json_serializable.py
--rw-r--r--   0 kimham     (501) staff       (20)      713 2023-06-16 06:45:51.000000 csle_base-0.2.16/src/csle_base/kafka_serializable.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 11:00:12.060231 csle_base-0.2.16/src/csle_base.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      664 2023-07-07 11:00:11.000000 csle_base-0.2.16/src/csle_base.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      424 2023-07-07 11:00:12.000000 csle_base-0.2.16/src/csle_base.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-07-07 11:00:11.000000 csle_base-0.2.16/src/csle_base.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-07-07 09:36:52.000000 csle_base-0.2.16/src/csle_base.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      204 2023-07-07 11:00:11.000000 csle_base-0.2.16/src/csle_base.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       10 2023-07-07 11:00:11.000000 csle_base-0.2.16/src/csle_base.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 11:28:01.408560 csle_base-0.2.17/
+-rw-r--r--   0 kimham     (501) staff       (20)      664 2023-07-07 11:28:01.408723 csle_base-0.2.17/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     3391 2023-06-28 07:40:45.000000 csle_base-0.2.17/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      670 2023-06-11 13:17:52.000000 csle_base-0.2.17/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1222 2023-07-07 11:28:01.409661 csle_base-0.2.17/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2023-06-11 13:17:52.000000 csle_base-0.2.17/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 11:28:01.402106 csle_base-0.2.17/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 11:28:01.405612 csle_base-0.2.17/src/csle_base/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2023-06-11 13:17:52.000000 csle_base-0.2.17/src/csle_base/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       23 2023-07-07 11:27:52.000000 csle_base-0.2.17/src/csle_base/__version__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      574 2023-06-16 06:45:51.000000 csle_base-0.2.17/src/csle_base/grpc_serializable.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1537 2023-06-11 13:17:52.000000 csle_base-0.2.17/src/csle_base/json_serializable.py
+-rw-r--r--   0 kimham     (501) staff       (20)      713 2023-06-16 06:45:51.000000 csle_base-0.2.17/src/csle_base/kafka_serializable.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 11:28:01.408132 csle_base-0.2.17/src/csle_base.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      664 2023-07-07 11:28:00.000000 csle_base-0.2.17/src/csle_base.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      424 2023-07-07 11:28:01.000000 csle_base-0.2.17/src/csle_base.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-07-07 11:28:00.000000 csle_base-0.2.17/src/csle_base.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-07-07 09:36:52.000000 csle_base-0.2.17/src/csle_base.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      204 2023-07-07 11:28:01.000000 csle_base-0.2.17/src/csle_base.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       10 2023-07-07 11:28:01.000000 csle_base-0.2.17/src/csle_base.egg-info/top_level.txt
```

### Comparing `csle_base-0.2.16/PKG-INFO` & `csle_base-0.2.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_base
-Version: 0.2.16
+Version: 0.2.17
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_base-0.2.16/README.md` & `csle_base-0.2.17/README.md`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.16/pyproject.toml` & `csle_base-0.2.17/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.16/setup.cfg` & `csle_base-0.2.17/setup.cfg`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.16/src/csle_base/grpc_serializable.py` & `csle_base-0.2.17/src/csle_base/grpc_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.16/src/csle_base/json_serializable.py` & `csle_base-0.2.17/src/csle_base/json_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.16/src/csle_base/kafka_serializable.py` & `csle_base-0.2.17/src/csle_base/kafka_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.16/src/csle_base.egg-info/PKG-INFO` & `csle_base-0.2.17/src/csle_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-base
-Version: 0.2.16
+Version: 0.2.17
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```


# Comparing `tmp/reliableGPT-0.2.975.tar.gz` & `tmp/reliableGPT-0.2.976.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.975.tar", last modified: Fri Jul  7 01:41:49 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.976.tar", last modified: Fri Jul  7 01:47:02 2023, max compression
```

## Comparing `reliableGPT-0.2.975.tar` & `reliableGPT-0.2.976.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:41:49.763665 reliableGPT-0.2.975/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.975/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-07 01:41:49.763552 reliableGPT-0.2.975/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8271 2023-07-03 21:43:04.000000 reliableGPT-0.2.975/README.md
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.975/pyproject.toml
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:41:49.760801 reliableGPT-0.2.975/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      514 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       54 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-07 01:41:49.000000 reliableGPT-0.2.975/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:41:49.763203 reliableGPT-0.2.975/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4210 2023-06-28 20:45:06.000000 reliableGPT-0.2.975/reliablegpt/APICallHandler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3284 2023-07-07 00:13:35.000000 reliableGPT-0.2.975/reliablegpt/Alerting.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4407 2023-06-28 20:45:06.000000 reliableGPT-0.2.975/reliablegpt/CustomQueue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    18148 2023-07-07 01:39:23.000000 reliableGPT-0.2.975/reliablegpt/IndividualRequest.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.975/reliablegpt/Model.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5170 2023-07-02 02:49:46.000000 reliableGPT-0.2.975/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7483 2023-07-06 16:11:58.000000 reliableGPT-0.2.975/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      375 2023-07-06 16:14:08.000000 reliableGPT-0.2.975/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5167 2023-07-07 01:37:33.000000 reliableGPT-0.2.975/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2363 2023-07-03 21:42:46.000000 reliableGPT-0.2.975/reliablegpt/reliableQuery.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-07 01:41:49.763701 reliableGPT-0.2.975/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      398 2023-07-07 01:41:30.000000 reliableGPT-0.2.975/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:47:02.624580 reliableGPT-0.2.976/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.976/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-07 01:47:02.624462 reliableGPT-0.2.976/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8271 2023-07-03 21:43:04.000000 reliableGPT-0.2.976/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.976/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:47:02.621805 reliableGPT-0.2.976/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-07 01:47:02.000000 reliableGPT-0.2.976/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      514 2023-07-07 01:47:02.000000 reliableGPT-0.2.976/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-07 01:47:02.000000 reliableGPT-0.2.976/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       54 2023-07-07 01:47:02.000000 reliableGPT-0.2.976/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-07 01:47:02.000000 reliableGPT-0.2.976/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-07 01:47:02.624118 reliableGPT-0.2.976/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4210 2023-06-28 20:45:06.000000 reliableGPT-0.2.976/reliablegpt/APICallHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3284 2023-07-07 00:13:35.000000 reliableGPT-0.2.976/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4407 2023-06-28 20:45:06.000000 reliableGPT-0.2.976/reliablegpt/CustomQueue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    18148 2023-07-07 01:39:23.000000 reliableGPT-0.2.976/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.976/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5170 2023-07-02 02:49:46.000000 reliableGPT-0.2.976/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7483 2023-07-06 16:11:58.000000 reliableGPT-0.2.976/reliablegpt/ReliableDataLoaders.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      375 2023-07-06 16:14:08.000000 reliableGPT-0.2.976/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5167 2023-07-07 01:46:38.000000 reliableGPT-0.2.976/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2363 2023-07-03 21:42:46.000000 reliableGPT-0.2.976/reliablegpt/reliableQuery.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-07 01:47:02.624618 reliableGPT-0.2.976/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      398 2023-07-07 01:46:44.000000 reliableGPT-0.2.976/setup.py
```

### Comparing `reliableGPT-0.2.975/LICENSE` & `reliableGPT-0.2.976/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/README.md` & `reliableGPT-0.2.976/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliableGPT.egg-info/SOURCES.txt` & `reliableGPT-0.2.976/reliableGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.976/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliablegpt/Alerting.py` & `reliableGPT-0.2.976/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.976/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.976/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliablegpt/Model.py` & `reliableGPT-0.2.976/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.976/reliablegpt/RateLimitHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliablegpt/ReliableDataLoaders.py` & `reliableGPT-0.2.976/reliablegpt/ReliableDataLoaders.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.975/reliablegpt/main.py` & `reliableGPT-0.2.976/reliablegpt/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # # Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
 from reliablegpt.RateLimitHandler import RateLimitHandler
 from reliablegpt.Model import Model
-from reliablegpt.alerting import Alerting
+from reliablegpt.Alerting import Alerting
 from reliablegpt.reliableQuery import reliable_query
 import requests
 
 # # Dev Imports
 # from IndividualRequest import IndividualRequest
 # from Model import Model
 # from Alerting import Alerting
```

### Comparing `reliableGPT-0.2.975/reliablegpt/reliableQuery.py` & `reliableGPT-0.2.976/reliablegpt/reliableQuery.py`

 * *Files identical despite different names*


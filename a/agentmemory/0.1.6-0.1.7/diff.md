# Comparing `tmp/agentmemory-0.1.6.tar.gz` & `tmp/agentmemory-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.1.6.tar", last modified: Fri Jul  7 00:05:04 2023, max compression
+gzip compressed data, was "agentmemory-0.1.7.tar", last modified: Fri Jul  7 00:07:33 2023, max compression
```

## Comparing `agentmemory-0.1.6.tar` & `agentmemory-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:05:04.679733 agentmemory-0.1.6/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.6/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     3141 2023-07-07 00:05:04.679578 agentmemory-0.1.6/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     2506 2023-07-07 00:03:00.000000 agentmemory-0.1.6/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:05:04.678468 agentmemory-0.1.6/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)      222 2023-07-07 00:05:01.000000 agentmemory-0.1.6/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5118 2023-07-06 23:03:16.000000 agentmemory-0.1.6/agentmemory/memory.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     2438 2023-07-06 23:01:34.000000 agentmemory-0.1.6/agentmemory/memory_test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:05:04.679345 agentmemory-0.1.6/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     3141 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      273 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 00:05:04.679783 agentmemory-0.1.6/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)      942 2023-07-07 00:05:01.000000 agentmemory-0.1.6/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:07:33.084228 agentmemory-0.1.7/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.7/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3109 2023-07-07 00:07:33.083983 agentmemory-0.1.7/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2506 2023-07-07 00:03:00.000000 agentmemory-0.1.7/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:07:33.080520 agentmemory-0.1.7/agentmemory/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      222 2023-07-07 00:07:29.000000 agentmemory-0.1.7/agentmemory/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5118 2023-07-06 23:03:16.000000 agentmemory-0.1.7/agentmemory/memory.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2438 2023-07-06 23:01:34.000000 agentmemory-0.1.7/agentmemory/memory_test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:07:33.083691 agentmemory-0.1.7/agentmemory.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3109 2023-07-07 00:07:33.000000 agentmemory-0.1.7/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      273 2023-07-07 00:07:33.000000 agentmemory-0.1.7/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 00:07:33.000000 agentmemory-0.1.7/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 00:07:33.000000 agentmemory-0.1.7/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-07 00:07:33.000000 agentmemory-0.1.7/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 00:07:33.084309 agentmemory-0.1.7/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-07 00:07:29.000000 agentmemory-0.1.7/setup.py
```

### Comparing `agentmemory-0.1.6/LICENSE` & `agentmemory-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.6/PKG-INFO` & `agentmemory-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # agentmemory
 
 Easy-to-use agent memory, powered by chromadb
 
-<img src="resources/image.jpg">
 
 # Installation
 
 ```bash
 pip install agentmemory
 ```
```

### Comparing `agentmemory-0.1.6/README.md` & `agentmemory-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.6/agentmemory/memory.py` & `agentmemory-0.1.7/agentmemory/memory.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.6/agentmemory/memory_test.py` & `agentmemory-0.1.7/agentmemory/memory_test.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.6/agentmemory.egg-info/PKG-INFO` & `agentmemory-0.1.7/agentmemory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # agentmemory
 
 Easy-to-use agent memory, powered by chromadb
 
-<img src="resources/image.jpg">
 
 # Installation
 
 ```bash
 pip install agentmemory
 ```
```


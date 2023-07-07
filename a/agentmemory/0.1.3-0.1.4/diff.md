# Comparing `tmp/agentmemory-0.1.3.tar.gz` & `tmp/agentmemory-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.1.3.tar", last modified: Fri Jul  7 00:00:00 2023, max compression
+gzip compressed data, was "agentmemory-0.1.4.tar", last modified: Fri Jul  7 00:00:29 2023, max compression
```

## Comparing `agentmemory-0.1.3.tar` & `agentmemory-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:00:00.110520 agentmemory-0.1.3/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.3/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)      594 2023-07-07 00:00:00.110356 agentmemory-0.1.3/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     2509 2023-07-06 23:56:31.000000 agentmemory-0.1.3/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:00:00.109340 agentmemory-0.1.3/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)      222 2023-07-06 23:59:56.000000 agentmemory-0.1.3/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5118 2023-07-06 23:03:16.000000 agentmemory-0.1.3/agentmemory/memory.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     2438 2023-07-06 23:01:34.000000 agentmemory-0.1.3/agentmemory/memory_test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:00:00.110117 agentmemory-0.1.3/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)      594 2023-07-07 00:00:00.000000 agentmemory-0.1.3/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      273 2023-07-07 00:00:00.000000 agentmemory-0.1.3/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 00:00:00.000000 agentmemory-0.1.3/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 00:00:00.000000 agentmemory-0.1.3/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-07 00:00:00.000000 agentmemory-0.1.3/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 00:00:00.110569 agentmemory-0.1.3/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)      747 2023-07-06 23:59:56.000000 agentmemory-0.1.3/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:00:29.114821 agentmemory-0.1.4/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.4/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)      594 2023-07-07 00:00:29.114659 agentmemory-0.1.4/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2509 2023-07-06 23:56:31.000000 agentmemory-0.1.4/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:00:29.113376 agentmemory-0.1.4/agentmemory/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      222 2023-07-07 00:00:25.000000 agentmemory-0.1.4/agentmemory/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5118 2023-07-06 23:03:16.000000 agentmemory-0.1.4/agentmemory/memory.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2438 2023-07-06 23:01:34.000000 agentmemory-0.1.4/agentmemory/memory_test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:00:29.114411 agentmemory-0.1.4/agentmemory.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      594 2023-07-07 00:00:29.000000 agentmemory-0.1.4/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      273 2023-07-07 00:00:29.000000 agentmemory-0.1.4/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 00:00:29.000000 agentmemory-0.1.4/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 00:00:29.000000 agentmemory-0.1.4/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-07 00:00:29.000000 agentmemory-0.1.4/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 00:00:29.114872 agentmemory-0.1.4/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)      747 2023-07-07 00:00:25.000000 agentmemory-0.1.4/setup.py
```

### Comparing `agentmemory-0.1.3/LICENSE` & `agentmemory-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.3/PKG-INFO` & `agentmemory-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dead simple agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentmemory-0.1.3/README.md` & `agentmemory-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.3/agentmemory/memory.py` & `agentmemory-0.1.4/agentmemory/memory.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.3/agentmemory/memory_test.py` & `agentmemory-0.1.4/agentmemory/memory_test.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.3/agentmemory.egg-info/PKG-INFO` & `agentmemory-0.1.4/agentmemory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dead simple agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentmemory-0.1.3/setup.py` & `agentmemory-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='agentmemory',
-    version='0.1.3',
+    version='0.1.4',
     description='Dead simple agent memory, powered by chromadb',
     url='https://github.com/lalalune/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
     packages=['agentmemory'],
     install_requires=['chromadb'],
```


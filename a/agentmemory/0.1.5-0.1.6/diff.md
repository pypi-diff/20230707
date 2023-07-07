# Comparing `tmp/agentmemory-0.1.5.tar.gz` & `tmp/agentmemory-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.1.5.tar", last modified: Fri Jul  7 00:03:42 2023, max compression
+gzip compressed data, was "agentmemory-0.1.6.tar", last modified: Fri Jul  7 00:05:04 2023, max compression
```

## Comparing `agentmemory-0.1.5.tar` & `agentmemory-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:03:42.297228 agentmemory-0.1.5/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.5/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)      594 2023-07-07 00:03:42.297073 agentmemory-0.1.5/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     2506 2023-07-07 00:03:00.000000 agentmemory-0.1.5/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:03:42.296105 agentmemory-0.1.5/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)      222 2023-07-07 00:03:38.000000 agentmemory-0.1.5/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5118 2023-07-06 23:03:16.000000 agentmemory-0.1.5/agentmemory/memory.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     2438 2023-07-06 23:01:34.000000 agentmemory-0.1.5/agentmemory/memory_test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:03:42.296843 agentmemory-0.1.5/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)      594 2023-07-07 00:03:42.000000 agentmemory-0.1.5/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      273 2023-07-07 00:03:42.000000 agentmemory-0.1.5/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 00:03:42.000000 agentmemory-0.1.5/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 00:03:42.000000 agentmemory-0.1.5/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-07 00:03:42.000000 agentmemory-0.1.5/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 00:03:42.297285 agentmemory-0.1.5/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)      942 2023-07-07 00:03:38.000000 agentmemory-0.1.5/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:05:04.679733 agentmemory-0.1.6/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.6/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3141 2023-07-07 00:05:04.679578 agentmemory-0.1.6/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2506 2023-07-07 00:03:00.000000 agentmemory-0.1.6/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:05:04.678468 agentmemory-0.1.6/agentmemory/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      222 2023-07-07 00:05:01.000000 agentmemory-0.1.6/agentmemory/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5118 2023-07-06 23:03:16.000000 agentmemory-0.1.6/agentmemory/memory.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     2438 2023-07-06 23:01:34.000000 agentmemory-0.1.6/agentmemory/memory_test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-07 00:05:04.679345 agentmemory-0.1.6/agentmemory.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3141 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      273 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-07 00:05:04.000000 agentmemory-0.1.6/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-07 00:05:04.679783 agentmemory-0.1.6/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)      942 2023-07-07 00:05:01.000000 agentmemory-0.1.6/setup.py
```

### Comparing `agentmemory-0.1.5/LICENSE` & `agentmemory-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.5/README.md` & `agentmemory-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.5/agentmemory/memory.py` & `agentmemory-0.1.6/agentmemory/memory.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.5/agentmemory/memory_test.py` & `agentmemory-0.1.6/agentmemory/memory_test.py`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.5/setup.py` & `agentmemory-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-    long_description=long_description,  # added this line
-    long_description_content_type="text/markdown",  # and this line
 
 setup(
     name='agentmemory',
-    version='0.1.5',
+    version='0.1.6',
     description='Easy-to-use agent memory, powered by chromadb',
+    long_description=long_description,  # added this line
+    long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
     packages=['agentmemory'],
     install_requires=['chromadb'],
     readme = "README.md",
```


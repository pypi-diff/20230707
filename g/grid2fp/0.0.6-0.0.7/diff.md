# Comparing `tmp/grid2fp-0.0.6.tar.gz` & `tmp/grid2fp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2fp-0.0.6.tar", last modified: Tue May 30 19:21:42 2023, max compression
+gzip compressed data, was "grid2fp-0.0.7.tar", last modified: Fri Jul  7 03:09:27 2023, max compression
```

## Comparing `grid2fp-0.0.6.tar` & `grid2fp-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:21:42.169627 grid2fp-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 19:21:16.000000 grid2fp-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-30 19:21:42.169627 grid2fp-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-30 19:21:16.000000 grid2fp-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:21:42.165627 grid2fp-0.0.6/grid2fp/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 19:21:16.000000 grid2fp-0.0.6/grid2fp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-30 19:21:16.000000 grid2fp-0.0.6/grid2fp/grid2fp.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 19:21:16.000000 grid2fp-0.0.6/grid2fp/grid_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:21:42.169627 grid2fp-0.0.6/grid2fp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 19:21:42.000000 grid2fp-0.0.6/grid2fp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:21:42.169627 grid2fp-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-30 19:21:16.000000 grid2fp-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:21:42.169627 grid2fp-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 19:21:16.000000 grid2fp-0.0.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-30 19:21:16.000000 grid2fp-0.0.6/test/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:09:27.920999 grid2fp-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 03:08:54.000000 grid2fp-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-07 03:09:27.920999 grid2fp-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-07 03:08:54.000000 grid2fp-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:09:27.920999 grid2fp-0.0.7/grid2fp/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 03:08:54.000000 grid2fp-0.0.7/grid2fp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-07 03:08:54.000000 grid2fp-0.0.7/grid2fp/grid2fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-07 03:08:54.000000 grid2fp-0.0.7/grid2fp/grid_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:09:27.920999 grid2fp-0.0.7/grid2fp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-07 03:09:27.000000 grid2fp-0.0.7/grid2fp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-07 03:09:27.000000 grid2fp-0.0.7/grid2fp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:09:27.000000 grid2fp-0.0.7/grid2fp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 03:09:27.000000 grid2fp-0.0.7/grid2fp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 03:09:27.000000 grid2fp-0.0.7/grid2fp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 03:09:27.920999 grid2fp-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-07 03:08:54.000000 grid2fp-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:09:27.920999 grid2fp-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 03:08:54.000000 grid2fp-0.0.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-07 03:08:54.000000 grid2fp-0.0.7/test/test_integration.py
```

### Comparing `grid2fp-0.0.6/LICENSE` & `grid2fp-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.6/PKG-INFO` & `grid2fp-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
-Author: Casey Duckering
+Author: Joe Starr
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: IPython
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `grid2fp-0.0.6/README.md` & `grid2fp-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.6/grid2fp/grid2fp.py` & `grid2fp-0.0.7/grid2fp/grid2fp.py`

 * *Files identical despite different names*

### Comparing `grid2fp-0.0.6/grid2fp.egg-info/PKG-INFO` & `grid2fp-0.0.7/grid2fp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grid2fp
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to eat grid diagrams and generate its front projection.
 Home-page: https://github.com/Joecstarr/grid2fp
-Author: Casey Duckering
+Author: Joe Starr
 Keywords: topology,Legendrian,Grid Diagram,knot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: IPython
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `grid2fp-0.0.6/setup.py` & `grid2fp-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import logging
 
 logger = logging.getLogger(__name__)
 
-version = "0.0.6"
+version = "0.0.7"
 
 try:
     with open("README.md", "r") as f:
         long_desc = f.read()
 except:
     logger.warning("Could not open README.md.  long_description will be set to None.")
     long_desc = None
@@ -15,15 +15,15 @@
 setup(
     name="grid2fp",
     packages=find_packages(),
     version=version,
     description="A tool to eat grid diagrams and generate its front projection.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
-    author="Casey Duckering",
+    author="Joe Starr",
     # author_email = '',
     url="https://github.com/Joecstarr/grid2fp",
     keywords=["topology", "Legendrian", "Grid Diagram","knot"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
```

### Comparing `grid2fp-0.0.6/test/test_integration.py` & `grid2fp-0.0.7/test/test_integration.py`

 * *Files identical despite different names*


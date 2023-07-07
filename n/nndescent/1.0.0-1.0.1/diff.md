# Comparing `tmp/nndescent-1.0.0.tar.gz` & `tmp/nndescent-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nndescent-1.0.0.tar", last modified: Fri Jul  7 12:30:13 2023, max compression
+gzip compressed data, was "dist/nndescent-1.0.1.tar", last modified: Fri Jul  7 13:20:56 2023, max compression
```

## Comparing `nndescent-1.0.0.tar` & `nndescent-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 12:30:13.000000 nndescent-1.0.0/
--rw-r--r--   0 minknow   (1000) minknow   (1000)     1300 2023-06-01 12:23:37.000000 nndescent-1.0.0/LICENSE
--rw-rw-r--   0 minknow   (1000) minknow   (1000)      158 2023-07-07 12:30:13.000000 nndescent-1.0.0/PKG-INFO
--rw-r--r--   0 minknow   (1000) minknow   (1000)     6765 2023-07-06 19:11:49.000000 nndescent-1.0.0/README.md
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 12:30:13.000000 nndescent-1.0.0/nndescent.egg-info/
--rw-rw-r--   0 minknow   (1000) minknow   (1000)      158 2023-07-07 12:30:12.000000 nndescent-1.0.0/nndescent.egg-info/PKG-INFO
--rw-rw-r--   0 minknow   (1000) minknow   (1000)      333 2023-07-07 12:30:12.000000 nndescent-1.0.0/nndescent.egg-info/SOURCES.txt
--rw-rw-r--   0 minknow   (1000) minknow   (1000)        1 2023-07-07 12:30:12.000000 nndescent-1.0.0/nndescent.egg-info/dependency_links.txt
--rw-rw-r--   0 minknow   (1000) minknow   (1000)       64 2023-07-07 12:30:12.000000 nndescent-1.0.0/nndescent.egg-info/requires.txt
--rw-rw-r--   0 minknow   (1000) minknow   (1000)       10 2023-07-07 12:30:12.000000 nndescent-1.0.0/nndescent.egg-info/top_level.txt
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 12:30:13.000000 nndescent-1.0.0/pybindings/
--rw-r--r--   0 minknow   (1000) minknow   (1000)    12951 2023-07-07 05:56:42.000000 nndescent-1.0.0/pybindings/pybind11ings.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)      148 2023-05-27 21:21:15.000000 nndescent-1.0.0/pyproject.toml
--rw-rw-r--   0 minknow   (1000) minknow   (1000)       38 2023-07-07 12:30:13.000000 nndescent-1.0.0/setup.cfg
--rw-r--r--   0 minknow   (1000) minknow   (1000)     1523 2023-07-02 09:31:11.000000 nndescent-1.0.0/setup.py
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 12:30:13.000000 nndescent-1.0.0/src/
--rw-r--r--   0 minknow   (1000) minknow   (1000)      138 2023-07-02 07:23:54.000000 nndescent-1.0.0/src/distances.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)     1812 2023-07-04 13:39:18.000000 nndescent-1.0.0/src/dtypes.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)    27254 2023-07-07 06:54:11.000000 nndescent-1.0.0/src/nnd.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)    17734 2023-07-05 06:36:04.000000 nndescent-1.0.0/src/rp_trees.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)     1871 2023-07-05 06:36:33.000000 nndescent-1.0.0/src/utils.cpp
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 12:30:13.000000 nndescent-1.0.0/tests/
--rw-r--r--   0 minknow   (1000) minknow   (1000)     3768 2023-07-06 09:08:44.000000 nndescent-1.0.0/tests/test_distances.py
+drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:20:56.000000 nndescent-1.0.1/
+-rw-r--r--   0 minknow   (1000) minknow   (1000)     1300 2023-06-01 12:23:37.000000 nndescent-1.0.1/LICENSE
+-rw-rw-r--   0 minknow   (1000) minknow   (1000)      158 2023-07-07 13:20:56.000000 nndescent-1.0.1/PKG-INFO
+-rw-r--r--   0 minknow   (1000) minknow   (1000)     6765 2023-07-06 19:11:49.000000 nndescent-1.0.1/README.md
+drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:20:56.000000 nndescent-1.0.1/nndescent.egg-info/
+-rw-rw-r--   0 minknow   (1000) minknow   (1000)      158 2023-07-07 13:20:56.000000 nndescent-1.0.1/nndescent.egg-info/PKG-INFO
+-rw-rw-r--   0 minknow   (1000) minknow   (1000)      333 2023-07-07 13:20:56.000000 nndescent-1.0.1/nndescent.egg-info/SOURCES.txt
+-rw-rw-r--   0 minknow   (1000) minknow   (1000)        1 2023-07-07 13:20:56.000000 nndescent-1.0.1/nndescent.egg-info/dependency_links.txt
+-rw-rw-r--   0 minknow   (1000) minknow   (1000)       64 2023-07-07 13:20:56.000000 nndescent-1.0.1/nndescent.egg-info/requires.txt
+-rw-rw-r--   0 minknow   (1000) minknow   (1000)       10 2023-07-07 13:20:56.000000 nndescent-1.0.1/nndescent.egg-info/top_level.txt
+drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:20:56.000000 nndescent-1.0.1/pybindings/
+-rw-r--r--   0 minknow   (1000) minknow   (1000)    12951 2023-07-07 05:56:42.000000 nndescent-1.0.1/pybindings/pybind11ings.cpp
+-rw-r--r--   0 minknow   (1000) minknow   (1000)      148 2023-05-27 21:21:15.000000 nndescent-1.0.1/pyproject.toml
+-rw-rw-r--   0 minknow   (1000) minknow   (1000)       38 2023-07-07 13:20:56.000000 nndescent-1.0.1/setup.cfg
+-rw-r--r--   0 minknow   (1000) minknow   (1000)     1476 2023-07-07 13:07:40.000000 nndescent-1.0.1/setup.py
+drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:20:56.000000 nndescent-1.0.1/src/
+-rw-r--r--   0 minknow   (1000) minknow   (1000)      138 2023-07-02 07:23:54.000000 nndescent-1.0.1/src/distances.cpp
+-rw-r--r--   0 minknow   (1000) minknow   (1000)     1812 2023-07-04 13:39:18.000000 nndescent-1.0.1/src/dtypes.cpp
+-rw-r--r--   0 minknow   (1000) minknow   (1000)    27254 2023-07-07 06:54:11.000000 nndescent-1.0.1/src/nnd.cpp
+-rw-r--r--   0 minknow   (1000) minknow   (1000)    17734 2023-07-05 06:36:04.000000 nndescent-1.0.1/src/rp_trees.cpp
+-rw-r--r--   0 minknow   (1000) minknow   (1000)     1871 2023-07-05 06:36:33.000000 nndescent-1.0.1/src/utils.cpp
+drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:20:56.000000 nndescent-1.0.1/tests/
+-rw-r--r--   0 minknow   (1000) minknow   (1000)     3768 2023-07-06 09:08:44.000000 nndescent-1.0.1/tests/test_distances.py
```

### Comparing `nndescent-1.0.0/LICENSE` & `nndescent-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.0/README.md` & `nndescent-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.0/pybindings/pybind11ings.cpp` & `nndescent-1.0.1/pybindings/pybind11ings.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.0/setup.py` & `nndescent-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from setuptools import Extension, setup
+import glob
 import numpy as np
 import re
 import pybind11
 
 
 def get_version_string():
     """Extracts version number from source code."""
@@ -16,22 +17,15 @@
 include_dirs = [
     pybind11.get_include(),
     np.get_include(),
 ]
 
 module = Extension(
     name="nndescent",
-    sources=[
-        "pybindings/pybind11ings.cpp",
-        "src/dtypes.cpp",
-        "src/nnd.cpp",
-        "src/rp_trees.cpp",
-        "src/utils.cpp",
-        "src/distances.cpp",
-    ],
+    sources=glob.glob("pybindings/*.cpp") + glob.glob("src/*.cpp"),
     include_dirs=include_dirs,
     extra_compile_args=[
         "-Ofast",
         "-flto",
         "-DALL_METRICS",
         "-fno-math-errno",
         "-fopenmp",
@@ -65,8 +59,9 @@
             "pynndescent",
             "scipy",
             "seaborn",
             "sklearn",
         ],
     },
     ext_modules=[module],
+    headers=glob.glob("pybindings/*.h") + glob.glob("src/*.h"),
 )
```

### Comparing `nndescent-1.0.0/src/dtypes.cpp` & `nndescent-1.0.1/src/dtypes.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.0/src/nnd.cpp` & `nndescent-1.0.1/src/nnd.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.0/src/rp_trees.cpp` & `nndescent-1.0.1/src/rp_trees.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.0/src/utils.cpp` & `nndescent-1.0.1/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.0/tests/test_distances.py` & `nndescent-1.0.1/tests/test_distances.py`

 * *Files identical despite different names*


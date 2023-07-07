# Comparing `tmp/nndescent-1.0.2.tar.gz` & `tmp/nndescent-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nndescent-1.0.2.tar", last modified: Fri Jul  7 13:51:28 2023, max compression
+gzip compressed data, was "nndescent-1.0.3.tar", last modified: Fri Jul  7 19:13:06 2023, max compression
```

## Comparing `nndescent-1.0.2.tar` & `nndescent-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:51:28.000000 nndescent-1.0.2/
--rw-r--r--   0 minknow   (1000) minknow   (1000)     1300 2023-06-01 12:23:37.000000 nndescent-1.0.2/LICENSE
--rw-rw-r--   0 minknow   (1000) minknow   (1000)       16 2023-07-07 13:47:36.000000 nndescent-1.0.2/MANIFEST.in
--rw-rw-r--   0 minknow   (1000) minknow   (1000)      158 2023-07-07 13:51:28.000000 nndescent-1.0.2/PKG-INFO
--rw-r--r--   0 minknow   (1000) minknow   (1000)     6765 2023-07-06 19:11:49.000000 nndescent-1.0.2/README.md
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:51:28.000000 nndescent-1.0.2/nndescent.egg-info/
--rw-rw-r--   0 minknow   (1000) minknow   (1000)      158 2023-07-07 13:51:27.000000 nndescent-1.0.2/nndescent.egg-info/PKG-INFO
--rw-rw-r--   0 minknow   (1000) minknow   (1000)      411 2023-07-07 13:51:27.000000 nndescent-1.0.2/nndescent.egg-info/SOURCES.txt
--rw-rw-r--   0 minknow   (1000) minknow   (1000)        1 2023-07-07 13:51:27.000000 nndescent-1.0.2/nndescent.egg-info/dependency_links.txt
--rw-rw-r--   0 minknow   (1000) minknow   (1000)       64 2023-07-07 13:51:27.000000 nndescent-1.0.2/nndescent.egg-info/requires.txt
--rw-rw-r--   0 minknow   (1000) minknow   (1000)       10 2023-07-07 13:51:27.000000 nndescent-1.0.2/nndescent.egg-info/top_level.txt
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:51:28.000000 nndescent-1.0.2/pybindings/
--rw-r--r--   0 minknow   (1000) minknow   (1000)    12951 2023-07-07 05:56:42.000000 nndescent-1.0.2/pybindings/pybind11ings.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)      148 2023-05-27 21:21:15.000000 nndescent-1.0.2/pyproject.toml
--rw-rw-r--   0 minknow   (1000) minknow   (1000)       38 2023-07-07 13:51:28.000000 nndescent-1.0.2/setup.cfg
--rw-r--r--   0 minknow   (1000) minknow   (1000)     1412 2023-07-07 13:47:07.000000 nndescent-1.0.2/setup.py
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:51:28.000000 nndescent-1.0.2/src/
--rw-r--r--   0 minknow   (1000) minknow   (1000)      138 2023-07-02 07:23:54.000000 nndescent-1.0.2/src/distances.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)    84644 2023-07-07 06:00:46.000000 nndescent-1.0.2/src/distances.h
--rw-r--r--   0 minknow   (1000) minknow   (1000)     1812 2023-07-04 13:39:18.000000 nndescent-1.0.2/src/dtypes.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)    32723 2023-07-07 06:08:44.000000 nndescent-1.0.2/src/dtypes.h
--rw-r--r--   0 minknow   (1000) minknow   (1000)    27254 2023-07-07 06:54:11.000000 nndescent-1.0.2/src/nnd.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)    27219 2023-07-07 13:49:06.000000 nndescent-1.0.2/src/nnd.h
--rw-r--r--   0 minknow   (1000) minknow   (1000)    17734 2023-07-05 06:36:04.000000 nndescent-1.0.2/src/rp_trees.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)    18575 2023-07-07 06:52:01.000000 nndescent-1.0.2/src/rp_trees.h
--rw-r--r--   0 minknow   (1000) minknow   (1000)     1871 2023-07-05 06:36:33.000000 nndescent-1.0.2/src/utils.cpp
--rw-r--r--   0 minknow   (1000) minknow   (1000)     5890 2023-07-05 06:39:50.000000 nndescent-1.0.2/src/utils.h
-drwxrwxr-x   0 minknow   (1000) minknow   (1000)        0 2023-07-07 13:51:28.000000 nndescent-1.0.2/tests/
--rw-r--r--   0 minknow   (1000) minknow   (1000)     3768 2023-07-06 09:08:44.000000 nndescent-1.0.2/tests/test_distances.py
+drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-07 19:13:06.405541 nndescent-1.0.3/
+-rw-r--r--   0 dr_b      (1000) dr_b      (1000)     1300 2023-06-01 12:23:37.000000 nndescent-1.0.3/LICENSE
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      236 2023-07-07 19:07:46.000000 nndescent-1.0.3/MANIFEST.in
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7825 2023-07-07 19:13:06.405541 nndescent-1.0.3/PKG-INFO
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7075 2023-07-07 19:07:46.000000 nndescent-1.0.3/README.md
+drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-07 19:13:06.401541 nndescent-1.0.3/nndescent.egg-info/
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7825 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/PKG-INFO
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      387 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/SOURCES.txt
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)        1 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/dependency_links.txt
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       64 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/requires.txt
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       10 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/top_level.txt
+drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-07 19:13:06.401541 nndescent-1.0.3/pybindings/
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    12951 2023-07-07 19:07:46.000000 nndescent-1.0.3/pybindings/pybind11ings.cpp
+-rw-r--r--   0 dr_b      (1000) dr_b      (1000)      148 2023-05-27 21:21:15.000000 nndescent-1.0.3/pyproject.toml
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       38 2023-07-07 19:13:06.405541 nndescent-1.0.3/setup.cfg
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     2347 2023-07-07 19:07:46.000000 nndescent-1.0.3/setup.py
+drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-07 19:13:06.405541 nndescent-1.0.3/src/
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      138 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/distances.cpp
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    84644 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/distances.h
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     1812 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/dtypes.cpp
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    32723 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/dtypes.h
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    27254 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/nnd.cpp
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    27219 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/nnd.h
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    17734 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/rp_trees.cpp
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    18575 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/rp_trees.h
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     1871 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/utils.cpp
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     5890 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/utils.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nndescent-1.0.2/LICENSE` & `nndescent-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/README.md` & `nndescent-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,38 @@
     - Yule
 
 Please note that not all distances have undergone thorough testing. Therefore, it is advised to use them with caution and at your own discretion.
 
 
 ## Installation
 
+### From PyPI
+
+You can install nndescent directly from PyPI using pip:
+
+```sh
+pip install nndescent
+```
+
+If you want to run the examples in `tests`, additional packages are needed. You can install them manually or install nndescent with the full option:
+
+```sh
+pip install nndescent[full]
+```
+
+### From Source
+
 1. Clone the repository:
 
 ```sh
 git clone https://github.com/brj0/nndescent.git
 cd nndescent
 ```
 
-2. The project can by build with:
+2. Build and install the package:
 
 ```sh
 pip install .
 ```
 
 If you want to run the examples in `tests`, additional packages are needed. You can install them manually or install nndescent with the full option:
 
@@ -67,15 +83,14 @@
 
 3. To run the examples in `tests` you must first download the datasets:
 
 ```sh
 python tests/make_test_data.py
 ```
 
-
 ## Usage
 
 In Python you can utilize the nndescent library in the following way:
 
 ```python
 import numpy as np
 import nndescent
```

### Comparing `nndescent-1.0.2/pybindings/pybind11ings.cpp` & `nndescent-1.0.3/pybindings/pybind11ings.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/src/distances.h` & `nndescent-1.0.3/src/distances.h`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/src/dtypes.cpp` & `nndescent-1.0.3/src/dtypes.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/src/dtypes.h` & `nndescent-1.0.3/src/dtypes.h`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/src/nnd.cpp` & `nndescent-1.0.3/src/nnd.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/src/nnd.h` & `nndescent-1.0.3/src/nnd.h`

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
 
 namespace nndescent
 {
 
 
 /**
- * @version 1.0.2
+ * @version 1.0.3
  */
-const std::string PROJECT_VERSION = "1.0.2";
+const std::string PROJECT_VERSION = "1.0.3";
 
 
 // Constants
 const char OLD = '0';
 const char NEW = '1';
 const int MAX_INT = std::numeric_limits<int>::max();
 const int DEFAULT_K = 10;
```

### Comparing `nndescent-1.0.2/src/rp_trees.cpp` & `nndescent-1.0.3/src/rp_trees.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/src/rp_trees.h` & `nndescent-1.0.3/src/rp_trees.h`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/src/utils.cpp` & `nndescent-1.0.3/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.2/src/utils.h` & `nndescent-1.0.3/src/utils.h`

 * *Files identical despite different names*


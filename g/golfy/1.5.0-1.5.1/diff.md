# Comparing `tmp/golfy-1.5.0.tar.gz` & `tmp/golfy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.5.0.tar", last modified: Fri Jul  7 14:33:51 2023, max compression
+gzip compressed data, was "golfy-1.5.1.tar", last modified: Fri Jul  7 15:59:15 2023, max compression
```

## Comparing `golfy-1.5.0.tar` & `golfy-1.5.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 14:33:51.494099 golfy-1.5.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.5.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-07 14:33:51.493914 golfy-1.5.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.5.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 14:33:51.490654 golfy-1.5.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      366 2023-07-07 14:30:48.000000 golfy-1.5.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     5492 2023-07-06 20:50:21.000000 golfy-1.5.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     8479 2023-07-07 14:29:26.000000 golfy-1.5.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     8453 2023-07-07 14:00:59.000000 golfy-1.5.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-07 14:00:08.000000 golfy-1.5.0/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.5.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.5.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.5.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 14:33:51.491129 golfy-1.5.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-07 14:33:51.000000 golfy-1.5.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      370 2023-07-07 14:33:51.000000 golfy-1.5.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-07 14:33:51.000000 golfy-1.5.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 14:33:51.000000 golfy-1.5.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      734 2023-07-07 14:30:55.000000 golfy-1.5.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-07 14:33:51.494142 golfy-1.5.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 14:33:51.493615 golfy-1.5.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.5.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.5.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.5.0/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 15:59:15.653431 golfy-1.5.1/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.5.1/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-07 15:59:15.653286 golfy-1.5.1/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1317 2023-07-06 20:51:05.000000 golfy-1.5.1/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 15:59:15.651398 golfy-1.5.1/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      357 2023-07-07 15:58:21.000000 golfy-1.5.1/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5492 2023-07-06 20:50:21.000000 golfy-1.5.1/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8479 2023-07-07 14:29:26.000000 golfy-1.5.1/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8453 2023-07-07 14:00:59.000000 golfy-1.5.1/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     4089 2023-07-07 14:00:08.000000 golfy-1.5.1/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.5.1/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-1.5.1/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.5.1/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 15:59:15.651938 golfy-1.5.1/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     2043 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      415 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:59:15.000000 golfy-1.5.1/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-07 15:56:30.000000 golfy-1.5.1/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-1.5.1/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-07 15:59:15.653468 golfy-1.5.1/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-07 15:59:15.652892 golfy-1.5.1/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.5.1/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1660 2023-07-07 14:04:35.000000 golfy-1.5.1/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.5.1/tests/test_optimize.py
```

### Comparing `golfy-1.5.0/LICENSE` & `golfy-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/PKG-INFO` & `golfy-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.5.0/README.md` & `golfy-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/golfy/deconvolution.py` & `golfy-1.5.1/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/golfy/initialization.py` & `golfy-1.5.1/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/golfy/optimization.py` & `golfy-1.5.1/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/golfy/solution.py` & `golfy-1.5.1/golfy/solution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/golfy/util.py` & `golfy-1.5.1/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/golfy/validity.py` & `golfy-1.5.1/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/golfy.egg-info/PKG-INFO` & `golfy-1.5.1/golfy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-1.5.0/pyproject.toml` & `golfy-1.5.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,19 @@
     'Environment :: Console',
     'Operating System :: OS Independent',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: Apache Software License',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 readme = "README.md"
-version = "1.5.0"  
+dynamic = ["version", "dependencies"]
+
+[tool.setuptools.dynamic]
+version = {attr = "golfy.__version__"}
+dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools]
 packages = ["golfy"]
 
 [project.urls]
 "Homepage" = "https://github.com/pirl-unc/golfy"
 "Bug Tracker" = "https://github.com/pirl-unc/golfy"
```

### Comparing `golfy-1.5.0/tests/test_deconvolution.py` & `golfy-1.5.1/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-1.5.0/tests/test_init.py` & `golfy-1.5.1/tests/test_init.py`

 * *Files identical despite different names*


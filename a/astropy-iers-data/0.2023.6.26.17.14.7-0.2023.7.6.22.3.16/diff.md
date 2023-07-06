# Comparing `tmp/astropy-iers-data-0.2023.6.26.17.14.7.tar.gz` & `tmp/astropy-iers-data-0.2023.7.6.22.3.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astropy-iers-data-0.2023.6.26.17.14.7.tar", last modified: Mon Jun 26 17:15:12 2023, max compression
+gzip compressed data, was "astropy-iers-data-0.2023.7.6.22.3.16.tar", last modified: Thu Jul  6 22:04:19 2023, max compression
```

## Comparing `astropy-iers-data-0.2023.6.26.17.14.7.tar` & `astropy-iers-data-0.2023.7.6.22.3.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:15:12.528513 astropy-iers-data-0.2023.6.26.17.14.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-26 17:15:12.528513 astropy-iers-data-0.2023.6.26.17.14.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:15:12.516512 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-26 17:15:12.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:15:12.524513 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/Leap_Second.dat
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/ReadMe.eopc04
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/ReadMe.finals2000A
--rw-r--r--   0 runner    (1001) docker     (123)  4912027 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/eopc04.1962-now
--rw-r--r--   0 runner    (1001) docker     (123)  3545116 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/finals2000A.all
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:15:12.528513 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:15:12.520513 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-26 17:15:12.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-26 17:15:12.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:15:12.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 17:15:12.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 17:15:12.000000 astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:15:12.528513 astropy-iers-data-0.2023.6.26.17.14.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-26 17:14:52.000000 astropy-iers-data-0.2023.6.26.17.14.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:04:19.164902 astropy-iers-data-0.2023.7.6.22.3.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-06 22:04:19.164902 astropy-iers-data-0.2023.7.6.22.3.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:04:19.152902 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-06 22:04:19.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:04:19.160902 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/Leap_Second.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/ReadMe.eopc04
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/ReadMe.finals2000A
+-rw-r--r--   0 runner    (1001) docker     (123)  4912027 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/eopc04.1962-now
+-rw-r--r--   0 runner    (1001) docker     (123)  3545116 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/finals2000A.all
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:04:19.160902 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:04:19.152902 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-06 22:04:19.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-06 22:04:19.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:04:19.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 22:04:19.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 22:04:19.000000 astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:04:19.164902 astropy-iers-data-0.2023.7.6.22.3.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-06 22:04:03.000000 astropy-iers-data-0.2023.7.6.22.3.16/tox.ini
```

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/LICENSE.rst` & `astropy-iers-data-0.2023.7.6.22.3.16/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/PKG-INFO` & `astropy-iers-data-0.2023.7.6.22.3.16/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropy-iers-data
-Version: 0.2023.6.26.17.14.7
+Version: 0.2023.7.6.22.3.16
 Summary: IERS Earth Rotation and Leap Second tables for the astropy core package
 Author-email: Astropy Developers <astropy.team@gmail.com>
 License: Copyright (c) 2023, Astropy Developers
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
@@ -43,14 +43,17 @@
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 IERS Earth Rotation and Leap Second tables for the astropy core package
 -----------------------------------------------------------------------
 
+.. image:: https://zenodo.org/badge/644894042.svg
+   :target: https://zenodo.org/badge/latestdoi/644894042
+
 **Note:** This package is not currently meant to be used directly by users, and only
 meant to be used from the core astropy package.
 
 https://docs.astropy.org/en/latest/utils/iers.html
 
 License
 -------
```

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/README.rst` & `astropy-iers-data-0.2023.7.6.22.3.16/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 IERS Earth Rotation and Leap Second tables for the astropy core package
 -----------------------------------------------------------------------
 
+.. image:: https://zenodo.org/badge/644894042.svg
+   :target: https://zenodo.org/badge/latestdoi/644894042
+
 **Note:** This package is not currently meant to be used directly by users, and only
 meant to be used from the core astropy package.
 
 https://docs.astropy.org/en/latest/utils/iers.html
 
 License
 -------
```

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/__init__.py` & `astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/__init__.py`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/Leap_Second.dat` & `astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/Leap_Second.dat`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/ReadMe.eopc04` & `astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/ReadMe.eopc04`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/ReadMe.finals2000A` & `astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/ReadMe.finals2000A`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/eopc04.1962-now` & `astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/eopc04.1962-now`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data/data/finals2000A.all` & `astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data/data/finals2000A.all`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data.egg-info/PKG-INFO` & `astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropy-iers-data
-Version: 0.2023.6.26.17.14.7
+Version: 0.2023.7.6.22.3.16
 Summary: IERS Earth Rotation and Leap Second tables for the astropy core package
 Author-email: Astropy Developers <astropy.team@gmail.com>
 License: Copyright (c) 2023, Astropy Developers
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
@@ -43,14 +43,17 @@
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.rst
 
 IERS Earth Rotation and Leap Second tables for the astropy core package
 -----------------------------------------------------------------------
 
+.. image:: https://zenodo.org/badge/644894042.svg
+   :target: https://zenodo.org/badge/latestdoi/644894042
+
 **Note:** This package is not currently meant to be used directly by users, and only
 meant to be used from the core astropy package.
 
 https://docs.astropy.org/en/latest/utils/iers.html
 
 License
 -------
```

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/astropy_iers_data.egg-info/SOURCES.txt` & `astropy-iers-data-0.2023.7.6.22.3.16/astropy_iers_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/pyproject.toml` & `astropy-iers-data-0.2023.7.6.22.3.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astropy-iers-data-0.2023.6.26.17.14.7/tox.ini` & `astropy-iers-data-0.2023.7.6.22.3.16/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     # TMP: should be changed once changes are in astropy
     git+https://github.com/astrofrog/astropy@iers-package
 extras =
     test
 
 commands =
     pip freeze
-    pytest --pyargs astropy.coordinates {posargs}
-    pytest --pyargs astropy.time {posargs}
-    pytest --pyargs astropy.utils.iers {posargs}
+    pytest --pyargs astropy.coordinates -m "not hypothesis" {posargs}
+    pytest --pyargs astropy.time -m "not hypothesis" {posargs}
+    pytest --pyargs astropy.utils.iers -m "not hypothesis" {posargs}
 
 [testenv:build_docs]
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
 extras = docs
 commands =
     pip freeze
```


# Comparing `tmp/desy-mento-0.1.1.tar.gz` & `tmp/desy-mento-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desy-mento-0.1.1.tar", last modified: Fri Jun 30 15:02:48 2023, max compression
+gzip compressed data, was "desy-mento-0.1.2.tar", last modified: Fri Jul  7 13:39:49 2023, max compression
```

## Comparing `desy-mento-0.1.1.tar` & `desy-mento-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.536481 desy-mento-0.1.1/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     7747 2023-06-30 15:02:48.536481 desy-mento-0.1.1/PKG-INFO
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     6809 2023-06-28 15:09:51.000000 desy-mento-0.1.1/README.rst
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     1190 2023-06-30 15:00:43.000000 desy-mento-0.1.1/pyproject.toml
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)       38 2023-06-30 15:02:48.536481 desy-mento-0.1.1/setup.cfg
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)      238 2023-06-30 14:45:08.000000 desy-mento-0.1.1/setup.py
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.535481 desy-mento-0.1.1/src/
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.535481 desy-mento-0.1.1/src/desy_mento.egg-info/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     7747 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/PKG-INFO
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)      372 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/SOURCES.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)        1 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/dependency_links.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)       47 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/requires.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)        6 2023-06-30 15:02:48.000000 desy-mento-0.1.1/src/desy_mento.egg-info/top_level.txt
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.536481 desy-mento-0.1.1/src/mento/
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)      420 2022-06-27 12:44:38.000000 desy-mento-0.1.1/src/mento/__init__.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11594 2023-06-28 12:35:53.000000 desy-mento-0.1.1/src/mento/metadata.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11937 2023-06-28 12:35:53.000000 desy-mento-0.1.1/src/mento/trigger.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     9696 2023-06-28 12:35:53.000000 desy-mento-0.1.1/src/mento/utils.py
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-06-30 15:02:48.536481 desy-mento-0.1.1/tests/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     8285 2023-06-28 12:35:53.000000 desy-mento-0.1.1/tests/test_metadata.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     5242 2023-06-28 12:35:53.000000 desy-mento-0.1.1/tests/test_trigger.py
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)     3684 2022-06-27 12:44:38.000000 desy-mento-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.224818 desy-mento-0.1.2/
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)      664 2023-07-07 13:39:49.224818 desy-mento-0.1.2/PKG-INFO
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     6809 2023-06-28 15:09:51.000000 desy-mento-0.1.2/README.rst
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)      168 2023-07-07 13:39:49.224818 desy-mento-0.1.2/setup.cfg
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     1075 2023-07-07 13:38:26.000000 desy-mento-0.1.2/setup.py
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.221818 desy-mento-0.1.2/src/
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.223818 desy-mento-0.1.2/src/desy_mento.egg-info/
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)      664 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/PKG-INFO
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)      367 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/SOURCES.txt
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)        1 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/dependency_links.txt
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)       34 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/requires.txt
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)        6 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/top_level.txt
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.223818 desy-mento-0.1.2/src/mento/
+-rw-rw-r--   0 kartikv   (1000) kartikv   (1000)      420 2022-06-27 12:44:38.000000 desy-mento-0.1.2/src/mento/__init__.py
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11594 2023-06-28 12:35:53.000000 desy-mento-0.1.2/src/mento/metadata.py
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11937 2023-06-28 12:35:53.000000 desy-mento-0.1.2/src/mento/trigger.py
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     9696 2023-06-28 12:35:53.000000 desy-mento-0.1.2/src/mento/utils.py
+drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.223818 desy-mento-0.1.2/tests/
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     8285 2023-06-28 12:35:53.000000 desy-mento-0.1.2/tests/test_metadata.py
+-rw-r--r--   0 kartikv   (1000) kartikv   (1000)     5242 2023-06-28 12:35:53.000000 desy-mento-0.1.2/tests/test_trigger.py
+-rw-rw-r--   0 kartikv   (1000) kartikv   (1000)     3684 2022-06-27 12:44:38.000000 desy-mento-0.1.2/tests/test_utils.py
```

### Comparing `desy-mento-0.1.1/PKG-INFO` & `desy-mento-0.1.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: desy-mento
-Version: 0.1.1
-Summary: A Python (3.7+ only) package for PETRA-III beamlines at DESY for automatically triggering online data processing jobs like remote data analysis, and local visualization tasks.
-Author-email: Vijay Kartik <vijay.kartik@desy.de>
-Project-URL: Repository, https://gitlab.desy.de/fs-sc/mento
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: lint
-
 .. SPDX-FileCopyrightText: 2021 S. Vijay Kartik <vijay.kartik@desy.de>, DESY
 ..
 .. SPDX-License-Identifier: CC-BY-4.0
 
 .. |oa| replace:: ``MENTO``
 .. _examples: /examples
 .. _docs: /docs
```

### Comparing `desy-mento-0.1.1/src/mento/metadata.py` & `desy-mento-0.1.2/src/mento/metadata.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.1/src/mento/trigger.py` & `desy-mento-0.1.2/src/mento/trigger.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.1/src/mento/utils.py` & `desy-mento-0.1.2/src/mento/utils.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.1/tests/test_metadata.py` & `desy-mento-0.1.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.1/tests/test_trigger.py` & `desy-mento-0.1.2/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.1/tests/test_utils.py` & `desy-mento-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*


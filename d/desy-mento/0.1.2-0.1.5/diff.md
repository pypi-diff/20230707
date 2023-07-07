# Comparing `tmp/desy-mento-0.1.2.tar.gz` & `tmp/desy-mento-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desy-mento-0.1.2.tar", last modified: Fri Jul  7 13:39:49 2023, max compression
+gzip compressed data, was "/builds/fs-sc/mento/dist/.tmp-_hbgyh0f/desy-mento-0.1.5.tar", last modified: Fri Jul  7 14:36:52 2023, max compression
```

## Comparing `desy-mento-0.1.2.tar` & `desy-mento-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.224818 desy-mento-0.1.2/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)      664 2023-07-07 13:39:49.224818 desy-mento-0.1.2/PKG-INFO
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     6809 2023-06-28 15:09:51.000000 desy-mento-0.1.2/README.rst
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)      168 2023-07-07 13:39:49.224818 desy-mento-0.1.2/setup.cfg
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     1075 2023-07-07 13:38:26.000000 desy-mento-0.1.2/setup.py
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.221818 desy-mento-0.1.2/src/
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.223818 desy-mento-0.1.2/src/desy_mento.egg-info/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)      664 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/PKG-INFO
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)      367 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/SOURCES.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)        1 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/dependency_links.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)       34 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/requires.txt
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)        6 2023-07-07 13:39:49.000000 desy-mento-0.1.2/src/desy_mento.egg-info/top_level.txt
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.223818 desy-mento-0.1.2/src/mento/
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)      420 2022-06-27 12:44:38.000000 desy-mento-0.1.2/src/mento/__init__.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11594 2023-06-28 12:35:53.000000 desy-mento-0.1.2/src/mento/metadata.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)    11937 2023-06-28 12:35:53.000000 desy-mento-0.1.2/src/mento/trigger.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     9696 2023-06-28 12:35:53.000000 desy-mento-0.1.2/src/mento/utils.py
-drwxr-xr-x   0 kartikv   (1000) kartikv   (1000)        0 2023-07-07 13:39:49.223818 desy-mento-0.1.2/tests/
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     8285 2023-06-28 12:35:53.000000 desy-mento-0.1.2/tests/test_metadata.py
--rw-r--r--   0 kartikv   (1000) kartikv   (1000)     5242 2023-06-28 12:35:53.000000 desy-mento-0.1.2/tests/test_trigger.py
--rw-rw-r--   0 kartikv   (1000) kartikv   (1000)     3684 2022-06-27 12:44:38.000000 desy-mento-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)      664 2023-07-07 14:36:52.000000 desy-mento-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6809 2023-07-07 14:36:33.000000 desy-mento-0.1.5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-07 14:36:52.000000 desy-mento-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-07-07 14:36:33.000000 desy-mento-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      664 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/desy_mento.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/src/mento/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-07 14:36:33.000000 desy-mento-0.1.5/src/mento/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11594 2023-07-07 14:36:33.000000 desy-mento-0.1.5/src/mento/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11937 2023-07-07 14:36:33.000000 desy-mento-0.1.5/src/mento/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)     9696 2023-07-07 14:36:33.000000 desy-mento-0.1.5/src/mento/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:36:52.000000 desy-mento-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     8285 2023-07-07 14:36:33.000000 desy-mento-0.1.5/tests/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5242 2023-07-07 14:36:33.000000 desy-mento-0.1.5/tests/test_trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3684 2023-07-07 14:36:33.000000 desy-mento-0.1.5/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `desy-mento-0.1.2/PKG-INFO` & `desy-mento-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desy-mento
-Version: 0.1.2
+Version: 0.1.5
 Home-page: https://gitlab.desy.de/fs-sc/mento/
 Author: Vijay Kartik
 Author-email: vijay.kartik@desy.de
 License: GPLv3
 Keywords: photon science data processing analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `desy-mento-0.1.2/README.rst` & `desy-mento-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.2/setup.py` & `desy-mento-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-FileCopyrightText: 2021 S. Vijay Kartik <vijay.kartik@desy.de>, DESY
 #
 # SPDX-License-Identifier: CC0-1.0
 
 from setuptools import find_packages, setup
 
 name = 'desy-mento'
-version = '0.1.2'
+version = '0.1.5'
 
 setup(
     name=name,
     version=version,
     author='Vijay Kartik',
     author_email='vijay.kartik@desy.de',
     url='https://gitlab.desy.de/fs-sc/mento/',
```

### Comparing `desy-mento-0.1.2/src/desy_mento.egg-info/PKG-INFO` & `desy-mento-0.1.5/src/desy_mento.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desy-mento
-Version: 0.1.2
+Version: 0.1.5
 Home-page: https://gitlab.desy.de/fs-sc/mento/
 Author: Vijay Kartik
 Author-email: vijay.kartik@desy.de
 License: GPLv3
 Keywords: photon science data processing analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `desy-mento-0.1.2/src/mento/metadata.py` & `desy-mento-0.1.5/src/mento/metadata.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.2/src/mento/trigger.py` & `desy-mento-0.1.5/src/mento/trigger.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.2/src/mento/utils.py` & `desy-mento-0.1.5/src/mento/utils.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.2/tests/test_metadata.py` & `desy-mento-0.1.5/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.2/tests/test_trigger.py` & `desy-mento-0.1.5/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `desy-mento-0.1.2/tests/test_utils.py` & `desy-mento-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*


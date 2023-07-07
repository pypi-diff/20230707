# Comparing `tmp/taxOrder-0.2.6.tar.gz` & `tmp/taxOrder-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxOrder-0.2.6.tar", last modified: Fri Jul  7 10:02:56 2023, max compression
+gzip compressed data, was "taxOrder-0.2.7.tar", last modified: Fri Jul  7 10:04:26 2023, max compression
```

## Comparing `taxOrder-0.2.6.tar` & `taxOrder-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-07-07 10:02:56.515267 taxOrder-0.2.6/
--rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.6/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)     1484 2023-07-07 10:02:56.513270 taxOrder-0.2.6/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      948 2023-06-01 11:02:50.000000 taxOrder-0.2.6/README.md
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-07-07 10:02:56.516266 taxOrder-0.2.6/setup.cfg
--rw-r--r--   0 felixl   (10024) users      (501)     1028 2023-07-07 10:02:43.000000 taxOrder-0.2.6/setup.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-07-07 10:02:56.491267 taxOrder-0.2.6/taxOrder/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.6/taxOrder/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     1932 2023-07-07 10:01:17.000000 taxOrder-0.2.6/taxOrder/cmdline_taxOrder.py
--rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.6/taxOrder/requirements.txt
--rw-r--r--   0 felixl   (10024) users      (501)     1121 2023-06-01 11:03:23.000000 taxOrder-0.2.6/taxOrder/taxOrder.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-07-07 10:02:56.510265 taxOrder-0.2.6/taxOrder.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     1484 2023-07-07 10:02:56.000000 taxOrder-0.2.6/taxOrder.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      317 2023-07-07 10:02:56.000000 taxOrder-0.2.6/taxOrder.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-07-07 10:02:56.000000 taxOrder-0.2.6/taxOrder.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)       60 2023-07-07 10:02:56.000000 taxOrder-0.2.6/taxOrder.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       15 2023-07-07 10:02:56.000000 taxOrder-0.2.6/taxOrder.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        9 2023-07-07 10:02:56.000000 taxOrder-0.2.6/taxOrder.egg-info/top_level.txt
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-07-07 10:04:26.926382 taxOrder-0.2.7/
+-rw-r--r--   0 felixl   (10024) users      (501)    35148 2022-12-01 14:14:30.000000 taxOrder-0.2.7/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)     1484 2023-07-07 10:04:26.925375 taxOrder-0.2.7/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      948 2023-06-01 11:02:50.000000 taxOrder-0.2.7/README.md
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-07-07 10:04:26.927377 taxOrder-0.2.7/setup.cfg
+-rw-r--r--   0 felixl   (10024) users      (501)     1028 2023-07-07 10:04:17.000000 taxOrder-0.2.7/setup.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-07-07 10:04:26.897390 taxOrder-0.2.7/taxOrder/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2022-12-01 13:23:00.000000 taxOrder-0.2.7/taxOrder/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1941 2023-07-07 10:04:05.000000 taxOrder-0.2.7/taxOrder/cmdline_taxOrder.py
+-rw-r--r--   0 felixl   (10024) users      (501)       14 2022-12-01 13:28:58.000000 taxOrder-0.2.7/taxOrder/requirements.txt
+-rw-r--r--   0 felixl   (10024) users      (501)     1121 2023-06-01 11:03:23.000000 taxOrder-0.2.7/taxOrder/taxOrder.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-07-07 10:04:26.921380 taxOrder-0.2.7/taxOrder.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     1484 2023-07-07 10:04:26.000000 taxOrder-0.2.7/taxOrder.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      317 2023-07-07 10:04:26.000000 taxOrder-0.2.7/taxOrder.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-07-07 10:04:26.000000 taxOrder-0.2.7/taxOrder.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       60 2023-07-07 10:04:26.000000 taxOrder-0.2.7/taxOrder.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       15 2023-07-07 10:04:26.000000 taxOrder-0.2.7/taxOrder.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        9 2023-07-07 10:04:26.000000 taxOrder-0.2.7/taxOrder.egg-info/top_level.txt
```

### Comparing `taxOrder-0.2.6/LICENSE` & `taxOrder-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.6/PKG-INFO` & `taxOrder-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.6
+Version: 0.2.7
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `taxOrder-0.2.6/README.md` & `taxOrder-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.6/setup.py` & `taxOrder-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="taxOrder",
-    version="0.2.6",
+    version="0.2.7",
     #python_requires='>=3.7.0',
     description="Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(include=['taxOrder', 'taxOrder.*']),
```

### Comparing `taxOrder-0.2.6/taxOrder/cmdline_taxOrder.py` & `taxOrder-0.2.7/taxOrder/cmdline_taxOrder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import os
-from taxOrder import order_taxa
+from taxOrder.taxOrder import order_taxa
 
 
 
 def check_file(f):
     if not os.path.isfile(f):
         raise ValueError(f'File not found at: {f}')
```

### Comparing `taxOrder-0.2.6/taxOrder/taxOrder.py` & `taxOrder-0.2.7/taxOrder/taxOrder.py`

 * *Files identical despite different names*

### Comparing `taxOrder-0.2.6/taxOrder.egg-info/PKG-INFO` & `taxOrder-0.2.7/taxOrder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxOrder
-Version: 0.2.6
+Version: 0.2.7
 Summary: Returns list of species in a phylogenetic tree ordered by increasing taxonomic distance to a reference species
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```


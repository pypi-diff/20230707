# Comparing `tmp/micomputing-1.1.42.tar.gz` & `tmp/micomputing-1.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micomputing-1.1.42.tar", last modified: Thu Jul  6 16:12:43 2023, max compression
+gzip compressed data, was "micomputing-1.1.43.tar", last modified: Thu Jul  6 16:43:40 2023, max compression
```

## Comparing `micomputing-1.1.42.tar` & `micomputing-1.1.43.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:12:43.333509 micomputing-1.1.42/
--rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-06 16:12:43.000000 micomputing-1.1.42/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 16:12:43.333359 micomputing-1.1.42/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 16:12:43.000000 micomputing-1.1.42/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:12:43.331188 micomputing-1.1.42/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2360 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    38302 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/metrics.py
--rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/micfunctions.so
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98918 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:12:43.332524 micomputing-1.1.42/micomputing/zxhtools/
--rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/zxhtools/TRS.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:12:43.333120 micomputing-1.1.42/micomputing/zxhtools/__pycache__/
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/zxhtools/exec.py
--rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/zxhtools/image2.AFF
--rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing/zxhtools/image2.FFD
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:12:43.331979 micomputing-1.1.42/micomputing.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-06 16:12:43.000000 micomputing-1.1.42/micomputing.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 16:12:43.333562 micomputing-1.1.42/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-06 16:12:43.000000 micomputing-1.1.42/setup_micomputing.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:43:40.405617 micomputing-1.1.43/
+-rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-06 16:43:40.000000 micomputing-1.1.43/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 16:43:40.405456 micomputing-1.1.43/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 16:43:40.000000 micomputing-1.1.43/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:43:40.402778 micomputing-1.1.43/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2360 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    38302 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/metrics.py
+-rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/micfunctions.so
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98918 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:43:40.404178 micomputing-1.1.43/micomputing/zxhtools/
+-rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/zxhtools/TRS.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:43:40.405146 micomputing-1.1.43/micomputing/zxhtools/__pycache__/
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/zxhtools/exec.py
+-rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/zxhtools/image2.AFF
+-rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing/zxhtools/image2.FFD
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 16:43:40.403616 micomputing-1.1.43/micomputing.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       72 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-06 16:43:40.000000 micomputing-1.1.43/micomputing.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 16:43:40.405726 micomputing-1.1.43/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1482 2023-07-06 16:43:40.000000 micomputing-1.1.43/setup_micomputing.py
```

### Comparing `micomputing-1.1.42/PKG-INFO` & `micomputing-1.1.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.42
+Version: 1.1.43
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.42/README.md` & `micomputing-1.1.43/README.md`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/__init__.py` & `micomputing-1.1.43/micomputing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.41',
+    version = '1.1.42',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
-    update = '2023-07-06 23:33:19',
+    update = '2023-07-07 00:12:43',
     package_data = True
 ).check()
 
 from . import plot as plt
 from .stdio import IMG, dcm2nii, nii2dcm #*
 from .data import Info, Subject, ImageObject, Dataset, MedicalDataset #*
 from .network import U_Net, CNN, FCN
```

### Comparing `micomputing-1.1.42/micomputing/data.py` & `micomputing-1.1.43/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/funcs.py` & `micomputing-1.1.43/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/metrics.py` & `micomputing-1.1.43/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/micfunctions.so` & `micomputing-1.1.43/micomputing/micfunctions.so`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/network.py` & `micomputing-1.1.43/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/plot.py` & `micomputing-1.1.43/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/stdio.py` & `micomputing-1.1.43/micomputing/stdio.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/test.py` & `micomputing-1.1.43/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/trans.py` & `micomputing-1.1.43/micomputing/trans.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/zxhtools/TRS.py` & `micomputing-1.1.43/micomputing/zxhtools/TRS.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc` & `micomputing-1.1.43/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc` & `micomputing-1.1.43/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc` & `micomputing-1.1.43/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc` & `micomputing-1.1.43/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/zxhtools/exec.py` & `micomputing-1.1.43/micomputing/zxhtools/exec.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing/zxhtools/image2.FFD` & `micomputing-1.1.43/micomputing/zxhtools/image2.FFD`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/micomputing.egg-info/PKG-INFO` & `micomputing-1.1.43/micomputing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.42
+Version: 1.1.43
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.42/micomputing.egg-info/SOURCES.txt` & `micomputing-1.1.43/micomputing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.42/setup_micomputing.py` & `micomputing-1.1.43/setup_micomputing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'micomputing',
-	version = '1.1.42',
+	version = '1.1.43',
 	keywords = ['pip', 'pymyc', 'micomputing', 'medical image', 'image registration', 'image similarities'],
 	description = "'micomputing' is a package for medical image computing. ",
 	long_description = '# MIComputing\n\n## Introduction\n\nPackage [`micomputing`](https://github.com/Bertie97/pycamia/tree/main/micomputing) is the medical image processing package under project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It handles medical image read write, image interpolation, transformation, registration and so on. This package works under `PyCAMIA` and use `batorch.Tensor` as its basic data format. \n\n## Installation\n\nThis package can be installed by `pip install micomputing` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/micomputing/)). \n\n```shell\npip install micomputing\n```\n\n\n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer\n',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/micomputing',
 	author = 'Yuncheng Zhou',
```


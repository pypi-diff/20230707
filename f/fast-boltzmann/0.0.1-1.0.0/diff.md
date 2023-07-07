# Comparing `tmp/fast_boltzmann-0.0.1.tar.gz` & `tmp/fast_boltzmann-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_boltzmann-0.0.1.tar", last modified: Fri Jul  7 16:52:04 2023, max compression
+gzip compressed data, was "fast_boltzmann-1.0.0.tar", last modified: Fri Jul  7 17:06:54 2023, max compression
```

## Comparing `fast_boltzmann-0.0.1.tar` & `fast_boltzmann-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yonniye    (501) staff       (20)        0 2023-07-07 16:52:04.682874 fast_boltzmann-0.0.1/
--rwxr-xr-x   0 yonniye    (501) staff       (20)     1066 2023-07-07 13:21:24.000000 fast_boltzmann-0.0.1/LICENSE
--rw-r--r--   0 yonniye    (501) staff       (20)     4159 2023-07-07 16:52:04.682712 fast_boltzmann-0.0.1/PKG-INFO
--rwxr-xr-x   0 yonniye    (501) staff       (20)     3040 2023-07-07 16:46:27.000000 fast_boltzmann-0.0.1/README.md
-drwxr-xr-x   0 yonniye    (501) staff       (20)        0 2023-07-07 16:52:04.681498 fast_boltzmann-0.0.1/fast_boltzmann.egg-info/
--rw-r--r--   0 yonniye    (501) staff       (20)     4159 2023-07-07 16:52:04.000000 fast_boltzmann-0.0.1/fast_boltzmann.egg-info/PKG-INFO
--rw-r--r--   0 yonniye    (501) staff       (20)      311 2023-07-07 16:52:04.000000 fast_boltzmann-0.0.1/fast_boltzmann.egg-info/SOURCES.txt
--rw-r--r--   0 yonniye    (501) staff       (20)        1 2023-07-07 16:52:04.000000 fast_boltzmann-0.0.1/fast_boltzmann.egg-info/dependency_links.txt
--rw-r--r--   0 yonniye    (501) staff       (20)       14 2023-07-07 16:52:04.000000 fast_boltzmann-0.0.1/fast_boltzmann.egg-info/requires.txt
--rw-r--r--   0 yonniye    (501) staff       (20)       15 2023-07-07 16:52:04.000000 fast_boltzmann-0.0.1/fast_boltzmann.egg-info/top_level.txt
--rw-r--r--   0 yonniye    (501) staff       (20)       38 2023-07-07 16:52:04.682931 fast_boltzmann-0.0.1/setup.cfg
--rw-r--r--   0 yonniye    (501) staff       (20)     1508 2023-07-07 16:51:47.000000 fast_boltzmann-0.0.1/setup.py
-drwxr-xr-x   0 yonniye    (501) staff       (20)        0 2023-07-07 16:52:04.679981 fast_boltzmann-0.0.1/src/
-drwxr-xr-x   0 yonniye    (501) staff       (20)        0 2023-07-07 16:52:04.682326 fast_boltzmann-0.0.1/src/fast_boltzmann/
--rw-r--r--   0 yonniye    (501) staff       (20)      395 2023-07-07 16:11:29.000000 fast_boltzmann-0.0.1/src/fast_boltzmann/__init__.py
--rw-r--r--   0 yonniye    (501) staff       (20)    14254 2023-07-07 16:03:26.000000 fast_boltzmann-0.0.1/src/fast_boltzmann/fast_boltzmann.py
--rwxr-xr-x   0 yonniye    (501) staff       (20)     2199 2023-07-07 14:03:38.000000 fast_boltzmann-0.0.1/src/fast_boltzmann/utils.py
+drwxr-xr-x   0 yonniye    (501) staff       (20)        0 2023-07-07 17:06:54.986207 fast_boltzmann-1.0.0/
+-rwxr-xr-x   0 yonniye    (501) staff       (20)     1066 2023-07-07 13:21:24.000000 fast_boltzmann-1.0.0/LICENSE
+-rw-r--r--   0 yonniye    (501) staff       (20)     4159 2023-07-07 17:06:54.985998 fast_boltzmann-1.0.0/PKG-INFO
+-rwxr-xr-x   0 yonniye    (501) staff       (20)     3040 2023-07-07 16:46:27.000000 fast_boltzmann-1.0.0/README.md
+drwxr-xr-x   0 yonniye    (501) staff       (20)        0 2023-07-07 17:06:54.985097 fast_boltzmann-1.0.0/fast_boltzmann.egg-info/
+-rw-r--r--   0 yonniye    (501) staff       (20)     4159 2023-07-07 17:06:54.000000 fast_boltzmann-1.0.0/fast_boltzmann.egg-info/PKG-INFO
+-rw-r--r--   0 yonniye    (501) staff       (20)      311 2023-07-07 17:06:54.000000 fast_boltzmann-1.0.0/fast_boltzmann.egg-info/SOURCES.txt
+-rw-r--r--   0 yonniye    (501) staff       (20)        1 2023-07-07 17:06:54.000000 fast_boltzmann-1.0.0/fast_boltzmann.egg-info/dependency_links.txt
+-rw-r--r--   0 yonniye    (501) staff       (20)       14 2023-07-07 17:06:54.000000 fast_boltzmann-1.0.0/fast_boltzmann.egg-info/requires.txt
+-rw-r--r--   0 yonniye    (501) staff       (20)       15 2023-07-07 17:06:54.000000 fast_boltzmann-1.0.0/fast_boltzmann.egg-info/top_level.txt
+-rw-r--r--   0 yonniye    (501) staff       (20)       38 2023-07-07 17:06:54.986274 fast_boltzmann-1.0.0/setup.cfg
+-rw-r--r--   0 yonniye    (501) staff       (20)     1508 2023-07-07 17:05:40.000000 fast_boltzmann-1.0.0/setup.py
+drwxr-xr-x   0 yonniye    (501) staff       (20)        0 2023-07-07 17:06:54.983714 fast_boltzmann-1.0.0/src/
+drwxr-xr-x   0 yonniye    (501) staff       (20)        0 2023-07-07 17:06:54.985536 fast_boltzmann-1.0.0/src/fast_boltzmann/
+-rw-r--r--   0 yonniye    (501) staff       (20)      395 2023-07-07 17:06:10.000000 fast_boltzmann-1.0.0/src/fast_boltzmann/__init__.py
+-rw-r--r--   0 yonniye    (501) staff       (20)    14255 2023-07-07 17:06:18.000000 fast_boltzmann-1.0.0/src/fast_boltzmann/fast_boltzmann.py
+-rwxr-xr-x   0 yonniye    (501) staff       (20)     2199 2023-07-07 14:03:38.000000 fast_boltzmann-1.0.0/src/fast_boltzmann/utils.py
```

### Comparing `fast_boltzmann-0.0.1/LICENSE` & `fast_boltzmann-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_boltzmann-0.0.1/PKG-INFO` & `fast_boltzmann-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_boltzmann
-Version: 0.0.1
+Version: 1.0.0
 Summary: `fast_boltzmann` is a Python package developed for the fast computation of the Boltzmann Entropy (also known as configurational entropy) for a two-dimensional numerical or nominal data array.
 Home-page: https://github.com/geoye/fast_boltzmann
 Author: Yuxuan YE<yuxuanye145@gmail.com>, Xinghua Cheng<cxh9791156936@gmail.com>
 Author-email: yuxuanye145@gmail.com, cxh9791156936@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/geoye/fast_boltzmann
 Project-URL: Bug Tracker, https://github.com/geoye/fast_boltzmann/issues
```

### Comparing `fast_boltzmann-0.0.1/README.md` & `fast_boltzmann-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fast_boltzmann-0.0.1/fast_boltzmann.egg-info/PKG-INFO` & `fast_boltzmann-1.0.0/fast_boltzmann.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-boltzmann
-Version: 0.0.1
+Version: 1.0.0
 Summary: `fast_boltzmann` is a Python package developed for the fast computation of the Boltzmann Entropy (also known as configurational entropy) for a two-dimensional numerical or nominal data array.
 Home-page: https://github.com/geoye/fast_boltzmann
 Author: Yuxuan YE<yuxuanye145@gmail.com>, Xinghua Cheng<cxh9791156936@gmail.com>
 Author-email: yuxuanye145@gmail.com, cxh9791156936@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/geoye/fast_boltzmann
 Project-URL: Bug Tracker, https://github.com/geoye/fast_boltzmann/issues
```

### Comparing `fast_boltzmann-0.0.1/setup.py` & `fast_boltzmann-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='fast_boltzmann',
-    version='0.0.1',
+    version='1.0.0',
     url='https://github.com/geoye/fast_boltzmann',
     license='MIT',
     author='Yuxuan YE<yuxuanye145@gmail.com>, Xinghua Cheng<cxh9791156936@gmail.com>',
     author_email='yuxuanye145@gmail.com, cxh9791156936@gmail.com',
     description='`fast_boltzmann` is a Python package developed for the fast computation of the Boltzmann Entropy '
                 '(also known as configurational entropy) for a two-dimensional numerical or nominal data array.',
     long_description=long_description,
```

### Comparing `fast_boltzmann-0.0.1/src/fast_boltzmann/fast_boltzmann.py` & `fast_boltzmann-1.0.0/src/fast_boltzmann/fast_boltzmann.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Fast computation of the Boltzmann Entropy of a numerical or nominal 2-D data array.
 Author: Yuxuan YE, Xinghua Cheng
-Date: 2023/07/07
-Version: 0.0.1
+Date: 2023/07/08
+Version: 1.0.0
 Email: yuxuanye145@gmail.com, cxh9791156936@gmail.com
 """
 
 import numpy as np
 import math
 import warnings
-from utils import map_d, map_n, initial_check
+from .utils import map_d, map_n, initial_check
 
 
 class BoltzNumerical:
     """
     Fast calculation of the Boltzmann Entropy of a 2-D numerical (raster) data array.
 
     Reference:
```

### Comparing `fast_boltzmann-0.0.1/src/fast_boltzmann/utils.py` & `fast_boltzmann-1.0.0/src/fast_boltzmann/utils.py`

 * *Files identical despite different names*


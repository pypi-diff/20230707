# Comparing `tmp/bombaysoftwares-pysupp-1.0.2.tar.gz` & `tmp/bombaysoftwares-pysupp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bombaysoftwares-pysupp-1.0.2.tar", last modified: Thu Jul  6 12:37:54 2023, max compression
+gzip compressed data, was "bombaysoftwares-pysupp-1.0.3.tar", last modified: Fri Jul  7 07:36:57 2023, max compression
```

## Comparing `bombaysoftwares-pysupp-1.0.2.tar` & `bombaysoftwares-pysupp-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-06 12:37:54.526139 bombaysoftwares-pysupp-1.0.2/
--rw-rw-r--   0 divy      (1000) divy      (1000)     1073 2023-07-05 06:20:56.000000 bombaysoftwares-pysupp-1.0.2/LICENSE
--rw-rw-r--   0 divy      (1000) divy      (1000)       33 2023-07-05 06:20:36.000000 bombaysoftwares-pysupp-1.0.2/MANIFEST.in
--rw-rw-r--   0 divy      (1000) divy      (1000)     4662 2023-07-06 12:37:54.526139 bombaysoftwares-pysupp-1.0.2/PKG-INFO
--rw-rw-r--   0 divy      (1000) divy      (1000)     2760 2023-07-06 12:00:30.000000 bombaysoftwares-pysupp-1.0.2/README.md
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-06 12:37:54.526139 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp/
--rw-rw-r--   0 divy      (1000) divy      (1000)      661 2023-07-06 11:35:00.000000 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp/__init__.py
--rw-rw-r--   0 divy      (1000) divy      (1000)    30127 2023-07-06 12:34:50.000000 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp/utils.py
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-06 12:37:54.526139 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp.egg-info/
--rw-rw-r--   0 divy      (1000) divy      (1000)     4662 2023-07-06 12:37:54.000000 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp.egg-info/PKG-INFO
--rw-rw-r--   0 divy      (1000) divy      (1000)      334 2023-07-06 12:37:54.000000 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp.egg-info/SOURCES.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-06 12:37:54.000000 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp.egg-info/dependency_links.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)       14 2023-07-06 12:37:54.000000 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp.egg-info/requires.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)       23 2023-07-06 12:37:54.000000 bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp.egg-info/top_level.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)       38 2023-07-06 12:37:54.526139 bombaysoftwares-pysupp-1.0.2/setup.cfg
--rw-rw-r--   0 divy      (1000) divy      (1000)     1419 2023-07-06 12:29:11.000000 bombaysoftwares-pysupp-1.0.2/setup.py
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-07 07:36:57.765308 bombaysoftwares-pysupp-1.0.3/
+-rw-rw-r--   0 divy      (1000) divy      (1000)     1073 2023-07-05 06:20:56.000000 bombaysoftwares-pysupp-1.0.3/LICENSE
+-rw-rw-r--   0 divy      (1000) divy      (1000)       33 2023-07-05 06:20:36.000000 bombaysoftwares-pysupp-1.0.3/MANIFEST.in
+-rw-rw-r--   0 divy      (1000) divy      (1000)     4662 2023-07-07 07:36:57.765308 bombaysoftwares-pysupp-1.0.3/PKG-INFO
+-rw-rw-r--   0 divy      (1000) divy      (1000)     2760 2023-07-06 12:00:30.000000 bombaysoftwares-pysupp-1.0.3/README.md
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-07 07:36:57.765308 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp/
+-rw-rw-r--   0 divy      (1000) divy      (1000)      661 2023-07-06 11:35:00.000000 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp/__init__.py
+-rw-rw-r--   0 divy      (1000) divy      (1000)    30127 2023-07-07 04:03:29.000000 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp/utils.py
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-07 07:36:57.765308 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp.egg-info/
+-rw-rw-r--   0 divy      (1000) divy      (1000)     4662 2023-07-07 07:36:57.000000 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp.egg-info/PKG-INFO
+-rw-rw-r--   0 divy      (1000) divy      (1000)      334 2023-07-07 07:36:57.000000 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp.egg-info/SOURCES.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-07 07:36:57.000000 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp.egg-info/dependency_links.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)       69 2023-07-07 07:36:57.000000 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp.egg-info/requires.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)       23 2023-07-07 07:36:57.000000 bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp.egg-info/top_level.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)       38 2023-07-07 07:36:57.765308 bombaysoftwares-pysupp-1.0.3/setup.cfg
+-rw-rw-r--   0 divy      (1000) divy      (1000)     1489 2023-07-07 07:15:22.000000 bombaysoftwares-pysupp-1.0.3/setup.py
```

### Comparing `bombaysoftwares-pysupp-1.0.2/LICENSE` & `bombaysoftwares-pysupp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bombaysoftwares-pysupp-1.0.2/PKG-INFO` & `bombaysoftwares-pysupp-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bombaysoftwares-pysupp
-Version: 1.0.2
+Version: 1.0.3
 Summary: The bombaysoftwares_pysupp package provides a comprehensive set of utility functions for various operations in Python. These functions simplify common tasks such as date formatting, timestamp conversion, manipulating strings. This package is designed to enhance the functionality of various operations in your Python projects.
 Home-page: UNKNOWN
 Author: Bombay Softwares
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Edugem-Technologies/bombaysoftwares-pysupp/issues
 Project-URL: Source Code, https://github.com/Edugem-Technologies/bombaysoftwares-pysupp
 Project-URL: Documentation, https://github.com/Edugem-Technologies/bombaysoftwares-pysupp#readme
```

### Comparing `bombaysoftwares-pysupp-1.0.2/README.md` & `bombaysoftwares-pysupp-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp/__init__.py` & `bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp/__init__.py`

 * *Files identical despite different names*

### Comparing `bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp/utils.py` & `bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp/utils.py`

 * *Files identical despite different names*

### Comparing `bombaysoftwares-pysupp-1.0.2/bombaysoftwares_pysupp.egg-info/PKG-INFO` & `bombaysoftwares-pysupp-1.0.3/bombaysoftwares_pysupp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bombaysoftwares-pysupp
-Version: 1.0.2
+Version: 1.0.3
 Summary: The bombaysoftwares_pysupp package provides a comprehensive set of utility functions for various operations in Python. These functions simplify common tasks such as date formatting, timestamp conversion, manipulating strings. This package is designed to enhance the functionality of various operations in your Python projects.
 Home-page: UNKNOWN
 Author: Bombay Softwares
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Edugem-Technologies/bombaysoftwares-pysupp/issues
 Project-URL: Source Code, https://github.com/Edugem-Technologies/bombaysoftwares-pysupp
 Project-URL: Documentation, https://github.com/Edugem-Technologies/bombaysoftwares-pysupp#readme
```

### Comparing `bombaysoftwares-pysupp-1.0.2/setup.py` & `bombaysoftwares-pysupp-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name='bombaysoftwares-pysupp',
-    version='1.0.2',
+    version='1.0.3',
     description='The bombaysoftwares_pysupp package provides a comprehensive set of utility functions for various operations in Python. These functions simplify common tasks such as date formatting, timestamp conversion, manipulating strings. This package is designed to enhance the functionality of various operations in your Python projects.',
     author='Bombay Softwares',
     packages=["bombaysoftwares_pysupp"],
-    install_requires=["PyJWT", "hashids"],
+    install_requires=["PyJWT", "hashids", "python-dateutil", "python-slugify", "six", "text-unidecode", "pytz"],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     project_urls={
         "Bug Tracker": "https://github.com/Edugem-Technologies/bombaysoftwares-pysupp/issues",
         "Source Code": "https://github.com/Edugem-Technologies/bombaysoftwares-pysupp",
         "Documentation": "https://github.com/Edugem-Technologies/bombaysoftwares-pysupp#readme"
```


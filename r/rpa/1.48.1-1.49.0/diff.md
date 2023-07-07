# Comparing `tmp/rpa-1.48.1.tar.gz` & `tmp/rpa-1.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rpa-1.48.1.tar", last modified: Thu Jun 30 01:22:32 2022, max compression
+gzip compressed data, was "dist/rpa-1.49.0.tar", last modified: Fri Jul  7 01:37:32 2023, max compression
```

## Comparing `rpa-1.48.1.tar` & `rpa-1.49.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kensoh     (501) staff       (20)        0 2022-06-30 01:22:32.000000 rpa-1.48.1/
--rw-r--r--   0 kensoh     (501) staff       (20)     1518 2022-06-30 01:22:32.000000 rpa-1.48.1/PKG-INFO
--rw-r--r--   0 kensoh     (501) staff       (20)      361 2022-06-30 01:20:19.000000 rpa-1.48.1/rpa.py
-drwxr-xr-x   0 kensoh     (501) staff       (20)        0 2022-06-30 01:22:32.000000 rpa-1.48.1/rpa.egg-info/
--rw-r--r--   0 kensoh     (501) staff       (20)     1518 2022-06-30 01:22:32.000000 rpa-1.48.1/rpa.egg-info/PKG-INFO
--rw-r--r--   0 kensoh     (501) staff       (20)      173 2022-06-30 01:22:32.000000 rpa-1.48.1/rpa.egg-info/SOURCES.txt
--rw-r--r--   0 kensoh     (501) staff       (20)       14 2022-06-30 01:22:32.000000 rpa-1.48.1/rpa.egg-info/requires.txt
--rw-r--r--   0 kensoh     (501) staff       (20)        4 2022-06-30 01:22:32.000000 rpa-1.48.1/rpa.egg-info/top_level.txt
--rw-r--r--   0 kensoh     (501) staff       (20)        1 2022-06-30 01:22:32.000000 rpa-1.48.1/rpa.egg-info/dependency_links.txt
--rw-r--r--   0 kensoh     (501) staff       (20)       20 2020-01-21 11:34:51.000000 rpa-1.48.1/MANIFEST.in
--rw-r--r--   0 kensoh     (501) staff       (20)     1614 2022-06-30 01:20:12.000000 rpa-1.48.1/setup.py
--rw-r--r--   0 kensoh     (501) staff       (20)       38 2022-06-30 01:22:32.000000 rpa-1.48.1/setup.cfg
--rw-r--r--   0 kensoh     (501) staff       (20)    11364 2021-05-07 17:11:25.000000 rpa-1.48.1/LICENSE.txt
+drwxr-xr-x   0 kensoh     (501) staff       (20)        0 2023-07-07 01:37:32.000000 rpa-1.49.0/
+-rw-r--r--   0 kensoh     (501) staff       (20)     1518 2023-07-07 01:37:32.000000 rpa-1.49.0/PKG-INFO
+-rw-r--r--   0 kensoh     (501) staff       (20)      361 2023-07-07 00:32:41.000000 rpa-1.49.0/rpa.py
+drwxr-xr-x   0 kensoh     (501) staff       (20)        0 2023-07-07 01:37:32.000000 rpa-1.49.0/rpa.egg-info/
+-rw-r--r--   0 kensoh     (501) staff       (20)     1518 2023-07-07 01:37:32.000000 rpa-1.49.0/rpa.egg-info/PKG-INFO
+-rw-r--r--   0 kensoh     (501) staff       (20)      173 2023-07-07 01:37:32.000000 rpa-1.49.0/rpa.egg-info/SOURCES.txt
+-rw-r--r--   0 kensoh     (501) staff       (20)       14 2023-07-07 01:37:32.000000 rpa-1.49.0/rpa.egg-info/requires.txt
+-rw-r--r--   0 kensoh     (501) staff       (20)        4 2023-07-07 01:37:32.000000 rpa-1.49.0/rpa.egg-info/top_level.txt
+-rw-r--r--   0 kensoh     (501) staff       (20)        1 2023-07-07 01:37:32.000000 rpa-1.49.0/rpa.egg-info/dependency_links.txt
+-rw-r--r--   0 kensoh     (501) staff       (20)       20 2020-01-21 11:34:51.000000 rpa-1.49.0/MANIFEST.in
+-rw-r--r--   0 kensoh     (501) staff       (20)     1614 2023-07-07 00:31:54.000000 rpa-1.49.0/setup.py
+-rw-r--r--   0 kensoh     (501) staff       (20)       38 2023-07-07 01:37:32.000000 rpa-1.49.0/setup.cfg
+-rw-r--r--   0 kensoh     (501) staff       (20)    11364 2021-05-07 17:11:25.000000 rpa-1.49.0/LICENSE.txt
```

### Comparing `rpa-1.48.1/PKG-INFO` & `rpa-1.49.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rpa
-Version: 1.48.1
+Version: 1.49.0
 Summary: RPA for Python is a Python package for RPA (robotic process automation)
 Home-page: https://github.com/tebelorg/RPA-Python
 Author: Ken Soh
 Author-email: opensource@tebel.org
 License: Apache License 2.0
 Description: RPA for Python's simple and powerful API makes robotic process automation fun! You can use it to quickly automate away repetitive time-consuming tasks on websites, desktop applications, or the command line.
```

### Comparing `rpa-1.48.1/rpa.egg-info/PKG-INFO` & `rpa-1.49.0/rpa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rpa
-Version: 1.48.1
+Version: 1.49.0
 Summary: RPA for Python is a Python package for RPA (robotic process automation)
 Home-page: https://github.com/tebelorg/RPA-Python
 Author: Ken Soh
 Author-email: opensource@tebel.org
 License: Apache License 2.0
 Description: RPA for Python's simple and powerful API makes robotic process automation fun! You can use it to quickly automate away repetitive time-consuming tasks on websites, desktop applications, or the command line.
```

### Comparing `rpa-1.48.1/setup.py` & `rpa-1.49.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='rpa',
-    version='1.48.1',
-    py_modules=['rpa'], install_requires=['tagui>=1.48.1'],
+    version='1.49.0',
+    py_modules=['rpa'], install_requires=['tagui>=1.49.0'],
     author='Ken Soh',
     author_email='opensource@tebel.org',
     license='Apache License 2.0',
     url='https://github.com/tebelorg/RPA-Python',
     description='RPA for Python is a Python package for RPA (robotic process automation)',
     long_description='RPA for Python\'s simple and powerful API makes robotic process automation fun! You can use it to quickly automate away repetitive time-consuming tasks on websites, desktop applications, or the command line.\n\nBuilt on AI Singapore\'s TagUI open-source RPA tool, RPA capabilities out-of-the-box for this package include website automation, computer vision automation, optical character recognition, keyboard & mouse automation.\n\nTables can\'t be displayed here, please refer to RPA for Python homepage for full API - https://github.com/tebelorg/RPA-Python',
     classifiers=[
```

### Comparing `rpa-1.48.1/LICENSE.txt` & `rpa-1.49.0/LICENSE.txt`

 * *Files identical despite different names*


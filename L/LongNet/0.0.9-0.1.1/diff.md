# Comparing `tmp/LongNet-0.0.9.tar.gz` & `tmp/LongNet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.0.9.tar", last modified: Fri Jul  7 17:48:16 2023, max compression
+gzip compressed data, was "LongNet-0.1.1.tar", last modified: Fri Jul  7 18:00:09 2023, max compression
```

## Comparing `LongNet-0.0.9.tar` & `LongNet-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:48:16.591555 LongNet-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 17:48:04.000000 LongNet-0.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:48:16.587556 LongNet-0.0.9/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 17:48:04.000000 LongNet-0.0.9/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 17:48:05.000000 LongNet-0.0.9/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-07 17:48:05.000000 LongNet-0.0.9/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-07 17:48:05.000000 LongNet-0.0.9/LongNet/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23041 2023-07-07 17:48:05.000000 LongNet-0.0.9/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 17:48:05.000000 LongNet-0.0.9/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:48:16.591555 LongNet-0.0.9/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 17:48:16.000000 LongNet-0.0.9/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 17:48:16.000000 LongNet-0.0.9/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:48:16.000000 LongNet-0.0.9/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 17:48:16.000000 LongNet-0.0.9/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 17:48:16.000000 LongNet-0.0.9/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 17:48:16.591555 LongNet-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-07-07 17:48:05.000000 LongNet-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:48:16.591555 LongNet-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 17:48:05.000000 LongNet-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:48:16.591555 LongNet-0.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-07 17:48:05.000000 LongNet-0.0.9/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:00:09.404963 LongNet-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 17:59:57.000000 LongNet-0.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:00:09.400962 LongNet-0.1.1/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 17:59:57.000000 LongNet-0.1.1/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 17:59:57.000000 LongNet-0.1.1/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-07 17:59:57.000000 LongNet-0.1.1/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-07 17:59:57.000000 LongNet-0.1.1/LongNet/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23041 2023-07-07 17:59:57.000000 LongNet-0.1.1/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 17:59:57.000000 LongNet-0.1.1/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:00:09.404963 LongNet-0.1.1/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 18:00:09.000000 LongNet-0.1.1/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 18:00:09.000000 LongNet-0.1.1/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:00:09.000000 LongNet-0.1.1/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 18:00:09.000000 LongNet-0.1.1/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 18:00:09.000000 LongNet-0.1.1/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 18:00:09.404963 LongNet-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-07-07 17:59:57.000000 LongNet-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:00:09.404963 LongNet-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 17:59:57.000000 LongNet-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:00:09.404963 LongNet-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-07 17:59:57.000000 LongNet-0.1.1/test/test.py
```

### Comparing `LongNet-0.0.9/LICENSE` & `LongNet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.9/LongNet/attention.py` & `LongNet-0.1.1/LongNet/attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.9/LongNet/model.py` & `LongNet-0.1.1/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.9/LongNet/model_test.py` & `LongNet-0.1.1/LongNet/model_test.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.9/LongNet/training.py` & `LongNet-0.1.1/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.9/LongNet/utils.py` & `LongNet-0.1.1/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.9/LongNet.egg-info/PKG-INFO` & `LongNet-0.1.1/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.0.9
+Version: 0.1.1
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.0.9/PKG-INFO` & `LongNet-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.0.9
+Version: 0.1.1
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.0.9/README.md` & `LongNet-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.9/setup.py` & `LongNet-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.0.9',
+  version = '0.1.1',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.0.9/test/test.py` & `LongNet-0.1.1/test/test.py`

 * *Files identical despite different names*


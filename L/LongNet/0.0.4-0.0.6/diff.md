# Comparing `tmp/LongNet-0.0.4.tar.gz` & `tmp/LongNet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.0.4.tar", last modified: Fri Jul  7 12:11:16 2023, max compression
+gzip compressed data, was "LongNet-0.0.6.tar", last modified: Fri Jul  7 12:16:23 2023, max compression
```

## Comparing `LongNet-0.0.4.tar` & `LongNet-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:11:16.483978 LongNet-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 12:11:02.000000 LongNet-0.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:11:16.483978 LongNet-0.0.4/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:11:16.483978 LongNet-0.0.4/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 12:11:16.483978 LongNet-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-07 12:11:02.000000 LongNet-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:11:16.483978 LongNet-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 12:11:02.000000 LongNet-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:11:16.483978 LongNet-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 12:11:02.000000 LongNet-0.0.4/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:16:23.357909 LongNet-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 12:16:07.000000 LongNet-0.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:16:23.357909 LongNet-0.0.6/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-07 12:16:07.000000 LongNet-0.0.6/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-07 12:16:07.000000 LongNet-0.0.6/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-07 12:16:07.000000 LongNet-0.0.6/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-07 12:16:07.000000 LongNet-0.0.6/LongNet/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-07-07 12:16:07.000000 LongNet-0.0.6/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 12:16:07.000000 LongNet-0.0.6/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:16:23.357909 LongNet-0.0.6/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 12:16:23.000000 LongNet-0.0.6/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 12:16:23.000000 LongNet-0.0.6/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:16:23.000000 LongNet-0.0.6/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 12:16:23.000000 LongNet-0.0.6/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 12:16:23.000000 LongNet-0.0.6/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 12:16:23.357909 LongNet-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-07 12:16:07.000000 LongNet-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:16:23.357909 LongNet-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 12:16:07.000000 LongNet-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:16:23.357909 LongNet-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 12:16:07.000000 LongNet-0.0.6/test/test.py
```

### Comparing `LongNet-0.0.4/LICENSE` & `LongNet-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.4/LongNet/attention.py` & `LongNet-0.0.6/LongNet/attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.4/LongNet/model.py` & `LongNet-0.0.6/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.4/LongNet/model_test.py` & `LongNet-0.0.6/LongNet/model_test.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.4/LongNet/training.py` & `LongNet-0.0.6/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.4/LongNet/utils.py` & `LongNet-0.0.6/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.4/LongNet.egg-info/PKG-INFO` & `LongNet-0.0.6/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.0.4
+Version: 0.0.6
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.0.4/PKG-INFO` & `LongNet-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.0.4
+Version: 0.0.6
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.0.4/README.md` & `LongNet-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.4/setup.py` & `LongNet-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.6',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
@@ -18,15 +18,18 @@
     "Prompt Engineering"
   ],
     install_requires=[
         'torch',
         'einops',
         'flash-attn',
         'accelerate',
-        'bitsandbytes'
+        'bitsandbytes',
+        'fairscale',
+        'timm',
+        'flamingo-pytorch'
     ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `LongNet-0.0.4/test/test.py` & `LongNet-0.0.6/test/test.py`

 * *Files identical despite different names*


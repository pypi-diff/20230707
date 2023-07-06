# Comparing `tmp/fundus_lesions_toolkit-0.1.0a0.tar.gz` & `tmp/fundus_lesions_toolkit-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundus_lesions_toolkit-0.1.0a0.tar", last modified: Thu Jul  6 21:12:55 2023, max compression
+gzip compressed data, was "fundus_lesions_toolkit-0.1.0b0.tar", last modified: Thu Jul  6 22:12:55 2023, max compression
```

## Comparing `fundus_lesions_toolkit-0.1.0a0.tar` & `fundus_lesions_toolkit-0.1.0b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-07-06 21:12:55.807654 fundus_lesions_toolkit-0.1.0a0/
--rw-rw-r--   0 clement   (1000) clement   (1000)     1067 2023-07-05 13:24:50.000000 fundus_lesions_toolkit-0.1.0a0/LICENSE
--rw-rw-r--   0 clement   (1000) clement   (1000)      719 2023-07-06 21:12:55.807654 fundus_lesions_toolkit-0.1.0a0/PKG-INFO
--rw-rw-r--   0 clement   (1000) clement   (1000)      407 2023-07-06 17:52:58.000000 fundus_lesions_toolkit-0.1.0a0/README.md
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-07-06 21:12:55.807654 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit/
--rw-rw-r--   0 clement   (1000) clement   (1000)      108 2023-07-06 21:00:43.000000 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      623 2023-07-06 09:35:01.000000 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit/constants.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-07-06 21:12:55.807654 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit.egg-info/
--rw-rw-r--   0 clement   (1000) clement   (1000)      719 2023-07-06 21:12:55.000000 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 clement   (1000) clement   (1000)      336 2023-07-06 21:12:55.000000 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)        1 2023-07-06 21:12:55.000000 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)       57 2023-07-06 21:12:55.000000 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit.egg-info/requires.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)       23 2023-07-06 21:12:55.000000 fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)       79 2023-07-06 21:12:55.807654 fundus_lesions_toolkit-0.1.0a0/setup.cfg
--rw-rw-r--   0 clement   (1000) clement   (1000)     1024 2023-07-06 21:12:50.000000 fundus_lesions_toolkit-0.1.0a0/setup.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-07-06 22:12:55.734766 fundus_lesions_toolkit-0.1.0b0/
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1067 2023-07-05 13:24:50.000000 fundus_lesions_toolkit-0.1.0b0/LICENSE
+-rw-rw-r--   0 clement   (1000) clement   (1000)      718 2023-07-06 22:12:55.734766 fundus_lesions_toolkit-0.1.0b0/PKG-INFO
+-rw-rw-r--   0 clement   (1000) clement   (1000)      407 2023-07-06 17:52:58.000000 fundus_lesions_toolkit-0.1.0b0/README.md
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-07-06 22:12:55.734766 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit/
+-rw-rw-r--   0 clement   (1000) clement   (1000)       15 2023-07-06 22:09:40.000000 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      623 2023-07-06 09:35:01.000000 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit/constants.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-07-06 22:12:55.734766 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit.egg-info/
+-rw-rw-r--   0 clement   (1000) clement   (1000)      718 2023-07-06 22:12:55.000000 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 clement   (1000) clement   (1000)      336 2023-07-06 22:12:55.000000 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)        1 2023-07-06 22:12:55.000000 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)       57 2023-07-06 22:12:55.000000 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)       23 2023-07-06 22:12:55.000000 fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)       79 2023-07-06 22:12:55.734766 fundus_lesions_toolkit-0.1.0b0/setup.cfg
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1022 2023-07-06 22:12:49.000000 fundus_lesions_toolkit-0.1.0b0/setup.py
```

### Comparing `fundus_lesions_toolkit-0.1.0a0/LICENSE` & `fundus_lesions_toolkit-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `fundus_lesions_toolkit-0.1.0a0/PKG-INFO` & `fundus_lesions_toolkit-0.1.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fundus_lesions_toolkit
-Version: 0.1.0a0
+Version: 0.1.0b0
 Summary: Tools Lesions Segmentation in Fundus
 Home-page: https://github.com/ClementPla/fundus-lesions-toolkit/tree/main
-Download-URL: https://github.com/ClementPla/fundus-lesions-toolkit/archive/refs/tags/v0.1.0-alpha.tar.gz
+Download-URL: https://github.com/ClementPla/fundus-lesions-toolkit/archive/refs/tags/v0.1.0-beta.tar.gz
 Author: Clement Playout
 Author-email: clement.playout@polymtl.ca
 License: MIT
 Keywords: Segmentation,Fundus,CNN,Neural Networks,PyTorch,Models,Semantic,Lesions
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit/constants.py` & `fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `fundus_lesions_toolkit-0.1.0a0/fundus_lesions_toolkit.egg-info/PKG-INFO` & `fundus_lesions_toolkit-0.1.0b0/fundus_lesions_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fundus-lesions-toolkit
-Version: 0.1.0a0
+Version: 0.1.0b0
 Summary: Tools Lesions Segmentation in Fundus
 Home-page: https://github.com/ClementPla/fundus-lesions-toolkit/tree/main
-Download-URL: https://github.com/ClementPla/fundus-lesions-toolkit/archive/refs/tags/v0.1.0-alpha.tar.gz
+Download-URL: https://github.com/ClementPla/fundus-lesions-toolkit/archive/refs/tags/v0.1.0-beta.tar.gz
 Author: Clement Playout
 Author-email: clement.playout@polymtl.ca
 License: MIT
 Keywords: Segmentation,Fundus,CNN,Neural Networks,PyTorch,Models,Semantic,Lesions
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fundus_lesions_toolkit-0.1.0a0/setup.py` & `fundus_lesions_toolkit-0.1.0b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'fundus_lesions_toolkit',        
   packages = ['fundus_lesions_toolkit'],  
-  version = '0.1.0-alpha',
+  version = '0.1.0-beta',
   license = 'MIT', 
   description = 'Tools Lesions Segmentation in Fundus', 
   author = 'Clement Playout',                   
   author_email = 'clement.playout@polymtl.ca', 
   url = 'https://github.com/ClementPla/fundus-lesions-toolkit/tree/main',   
-  download_url = 'https://github.com/ClementPla/fundus-lesions-toolkit/archive/refs/tags/v0.1.0-alpha.tar.gz',   
+  download_url = 'https://github.com/ClementPla/fundus-lesions-toolkit/archive/refs/tags/v0.1.0-beta.tar.gz',   
   keywords = ['Segmentation', 'Fundus', 
               'CNN', 'Neural Networks',
               'PyTorch', 'Models', 
               'Semantic', 'Lesions'],  
   install_requires = ['torch', 'nntools', 'torchvision', 'opencv-python', 'numpy', 'matplotlib'],
   classifiers = [
     'Development Status :: 3 - Alpha',
```


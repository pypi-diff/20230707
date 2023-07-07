# Comparing `tmp/DupliPy-0.1.1.tar.gz` & `tmp/duplipy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DupliPy-0.1.1.tar", last modified: Fri Jul  7 10:49:36 2023, max compression
+gzip compressed data, was "duplipy-0.1.2.tar", last modified: Fri Jul  7 11:14:38 2023, max compression
```

## Comparing `DupliPy-0.1.1.tar` & `duplipy-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:49:36.492735 DupliPy-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-07 10:49:36.486736 DupliPy-0.1.1/DupliPy.egg-info/
--rw-rw-rw-   0        0        0      918 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      918 2023-07-07 10:49:36.490732 DupliPy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 10:49:36.492735 DupliPy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1264 2023-07-07 10:49:22.000000 DupliPy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:14:38.346128 duplipy-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-07 11:14:38.320133 duplipy-0.1.2/DupliPy.egg-info/
+-rw-rw-rw-   0        0        0      918 2023-07-07 11:14:38.000000 duplipy-0.1.2/DupliPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-07-07 11:14:38.000000 duplipy-0.1.2/DupliPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 11:14:38.000000 duplipy-0.1.2/DupliPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-07 11:14:38.000000 duplipy-0.1.2/DupliPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 11:14:38.000000 duplipy-0.1.2/DupliPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      918 2023-07-07 11:14:38.341128 duplipy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:14:38.347131 duplipy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-07-07 11:14:31.000000 duplipy-0.1.2/setup.py
```

### Comparing `DupliPy-0.1.1/DupliPy.egg-info/PKG-INFO` & `duplipy-0.1.2/DupliPy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: DupliPy
-Version: 0.1.1
+Name: duplipy
+Version: 0.1.2
 Summary: A package for formatting and text replication.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DupliPy-0.1.1/PKG-INFO` & `duplipy-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: DupliPy
-Version: 0.1.1
+Name: duplipy
+Version: 0.1.2
 Summary: A package for formatting and text replication.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DupliPy-0.1.1/setup.py` & `duplipy-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='DupliPy',
-    version='0.1.1',
+    name='duplipy',
+    version='0.1.2',
     author='Infinitode Pty Ltd',
     author_email='infinitode.ltd@gmail.com',
     description='A package for formatting and text replication.',
     long_description='DupliPy is a quick and easy-to-use package that can handle text formatting and data augmentation tasks for NLP in Python.',
     long_description_content_type='text/markdown',
     url='https://github.com/infinitode/duplipy',
     packages=find_packages(),
```


# Comparing `tmp/duplipy-0.1.3.tar.gz` & `tmp/duplipy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplipy-0.1.3.tar", last modified: Fri Jul  7 11:46:00 2023, max compression
+gzip compressed data, was "duplipy-0.1.4.tar", last modified: Fri Jul  7 12:47:56 2023, max compression
```

## Comparing `duplipy-0.1.3.tar` & `duplipy-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 11:46:00.799633 duplipy-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-07-07 11:46:00.777630 duplipy-0.1.3/DupliPy.egg-info/
--rw-rw-rw-   0        0        0      918 2023-07-07 11:46:00.000000 duplipy-0.1.3/DupliPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-07-07 11:46:00.000000 duplipy-0.1.3/DupliPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:46:00.000000 duplipy-0.1.3/DupliPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-07 11:46:00.000000 duplipy-0.1.3/DupliPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:46:00.000000 duplipy-0.1.3/DupliPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      918 2023-07-07 11:46:00.793633 duplipy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 11:46:00.801677 duplipy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1264 2023-07-07 11:44:25.000000 duplipy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:47:56.338250 duplipy-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-07-07 12:47:56.311253 duplipy-0.1.4/DupliPy.egg-info/
+-rw-rw-rw-   0        0        0      918 2023-07-07 12:47:55.000000 duplipy-0.1.4/DupliPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-07-07 12:47:56.000000 duplipy-0.1.4/DupliPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:47:55.000000 duplipy-0.1.4/DupliPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-07 12:47:55.000000 duplipy-0.1.4/DupliPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:47:55.000000 duplipy-0.1.4/DupliPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      918 2023-07-07 12:47:56.332253 duplipy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:47:56.339262 duplipy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-07-07 12:12:02.000000 duplipy-0.1.4/setup.py
```

### Comparing `duplipy-0.1.3/DupliPy.egg-info/PKG-INFO` & `duplipy-0.1.4/DupliPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplipy
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for formatting and text replication.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplipy-0.1.3/PKG-INFO` & `duplipy-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplipy
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for formatting and text replication.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplipy-0.1.3/setup.py` & `duplipy-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='duplipy',
-    version='0.1.3',
+    version='0.1.4',
     author='Infinitode Pty Ltd',
     author_email='infinitode.ltd@gmail.com',
     description='A package for formatting and text replication.',
     long_description='DupliPy is a quick and easy-to-use package that can handle text formatting and data augmentation tasks for NLP in Python.',
     long_description_content_type='text/markdown',
     url='https://github.com/infinitode/duplipy',
     packages=find_packages(),
```


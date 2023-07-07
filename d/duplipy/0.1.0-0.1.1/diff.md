# Comparing `tmp/DupliPy-0.1.0.tar.gz` & `tmp/DupliPy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DupliPy-0.1.0.tar", last modified: Fri Jul  7 09:46:18 2023, max compression
+gzip compressed data, was "DupliPy-0.1.1.tar", last modified: Fri Jul  7 10:49:36 2023, max compression
```

## Comparing `DupliPy-0.1.0.tar` & `DupliPy-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 09:46:18.041153 DupliPy-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-07 09:46:18.035147 DupliPy-0.1.0/DupliPy.egg-info/
--rw-rw-rw-   0        0        0      914 2023-07-07 09:46:17.000000 DupliPy-0.1.0/DupliPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-07 09:46:17.000000 DupliPy-0.1.0/DupliPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 09:46:17.000000 DupliPy-0.1.0/DupliPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-07 09:46:17.000000 DupliPy-0.1.0/DupliPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 09:46:17.000000 DupliPy-0.1.0/DupliPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      914 2023-07-07 09:46:18.040154 DupliPy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 09:46:18.042152 DupliPy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-07-07 09:42:50.000000 DupliPy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:36.492735 DupliPy-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:36.486736 DupliPy-0.1.1/DupliPy.egg-info/
+-rw-rw-rw-   0        0        0      918 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:49:36.000000 DupliPy-0.1.1/DupliPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      918 2023-07-07 10:49:36.490732 DupliPy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:49:36.492735 DupliPy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-07-07 10:49:22.000000 DupliPy-0.1.1/setup.py
```

### Comparing `DupliPy-0.1.0/DupliPy.egg-info/PKG-INFO` & `DupliPy-0.1.1/DupliPy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DupliPy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for formatting and text replication.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,8 +14,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-DupliPy is a quick and easy-to-use package that handle text formatting and data augmentation tasks for NLP in Python.
+DupliPy is a quick and easy-to-use package that can handle text formatting and data augmentation tasks for NLP in Python.
```

### Comparing `DupliPy-0.1.0/PKG-INFO` & `DupliPy-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DupliPy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for formatting and text replication.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,8 +14,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-DupliPy is a quick and easy-to-use package that handle text formatting and data augmentation tasks for NLP in Python.
+DupliPy is a quick and easy-to-use package that can handle text formatting and data augmentation tasks for NLP in Python.
```

### Comparing `DupliPy-0.1.0/setup.py` & `DupliPy-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DupliPy',
-    version='0.1.0',
+    version='0.1.1',
     author='Infinitode Pty Ltd',
     author_email='infinitode.ltd@gmail.com',
     description='A package for formatting and text replication.',
-    long_description='DupliPy is a quick and easy-to-use package that handle text formatting and data augmentation tasks for NLP in Python.',
+    long_description='DupliPy is a quick and easy-to-use package that can handle text formatting and data augmentation tasks for NLP in Python.',
     long_description_content_type='text/markdown',
     url='https://github.com/infinitode/duplipy',
     packages=find_packages(),
     install_requires=[
         'nltk',
         'numpy',
         'spacy',
```


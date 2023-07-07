# Comparing `tmp/process-twarc-0.1.tar.gz` & `tmp/process-twarc-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-twarc-0.1.tar", last modified: Fri Jul  7 13:23:54 2023, max compression
+gzip compressed data, was "process-twarc-0.11.tar", last modified: Fri Jul  7 13:34:53 2023, max compression
```

## Comparing `process-twarc-0.1.tar` & `process-twarc-0.11.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:23:54.742792 process-twarc-0.1/
--rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      690 2023-07-07 13:23:54.742792 process-twarc-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 13:23:54.736782 process-twarc-0.1/process-twarc/
--rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.1/process-twarc/__init__.py
--rw-rw-rw-   0        0        0     8476 2023-07-06 15:47:42.000000 process-twarc-0.1/process-twarc/util.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:23:54.742792 process-twarc-0.1/process_twarc.egg-info/
--rw-rw-rw-   0        0        0      690 2023-07-07 13:23:54.000000 process-twarc-0.1/process_twarc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-07 13:23:54.000000 process-twarc-0.1/process_twarc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:23:54.000000 process-twarc-0.1/process_twarc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-07 13:23:54.000000 process-twarc-0.1/process_twarc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 13:23:54.000000 process-twarc-0.1/process_twarc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-07 13:23:54.743797 process-twarc-0.1/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-07-07 13:23:05.000000 process-twarc-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:34:53.889692 process-twarc-0.11/
+-rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.11/LICENSE.txt
+-rw-rw-rw-   0        0        0      691 2023-07-07 13:34:53.889692 process-twarc-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 13:34:53.871582 process-twarc-0.11/process_twarc/
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.11/process_twarc/__init__.py
+-rw-rw-rw-   0        0        0     8476 2023-07-06 15:47:42.000000 process-twarc-0.11/process_twarc/util.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:34:53.887848 process-twarc-0.11/process_twarc.egg-info/
+-rw-rw-rw-   0        0        0      691 2023-07-07 13:34:53.000000 process-twarc-0.11/process_twarc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-07 13:34:53.000000 process-twarc-0.11/process_twarc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:34:53.000000 process-twarc-0.11/process_twarc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-07 13:34:53.000000 process-twarc-0.11/process_twarc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 13:34:53.000000 process-twarc-0.11/process_twarc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-07 13:34:53.893698 process-twarc-0.11/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-07-07 13:34:42.000000 process-twarc-0.11/setup.py
```

### Comparing `process-twarc-0.1/LICENSE.txt` & `process-twarc-0.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `process-twarc-0.1/PKG-INFO` & `process-twarc-0.11/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.1
+Version: 0.11
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.1/process-twarc/util.py` & `process-twarc-0.11/process_twarc/util.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.1/process_twarc.egg-info/PKG-INFO` & `process-twarc-0.11/process_twarc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.1
+Version: 0.11
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.1/setup.py` & `process-twarc-0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'process-twarc',         
-  packages = ['process-twarc'],   
-  version = '0.1',
+  packages = ['process_twarc'],   
+  version = '0.11',
   license='MIT',
   description = 'Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.',   # Give a short description about your library
   author = 'Jordan Wolfgang Klein',
   author_email = 'jordan.klein.21@um.edu.mt',
   url = 'https://github.com/user/Lone-Wolfgang',
   keywords = ['Twitter', 'Deduplication', "Tokenization", "Language Modeling"],
   install_requires=[
```


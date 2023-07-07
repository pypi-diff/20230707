# Comparing `tmp/cryptographyComplements-0.3.0.tar.gz` & `tmp/cryptographyComplements-0.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.3.0.tar", last modified: Fri Jul  7 00:56:12 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.3.0.1.tar", last modified: Fri Jul  7 01:01:09 2023, max compression
```

## Comparing `cryptographyComplements-0.3.0.tar` & `cryptographyComplements-0.3.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 00:56:12.693138 cryptographyComplements-0.3.0/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-07-07 00:56:12.691128 cryptographyComplements-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 00:56:12.684551 cryptographyComplements-0.3.0/cryptographyComplements/
--rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.0/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     4630 2023-07-07 00:09:52.000000 cryptographyComplements-0.3.0/cryptographyComplements/cryptosystems.py
--rw-rw-rw-   0        0        0    16189 2023-07-07 00:40:25.000000 cryptographyComplements-0.3.0/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2182 2023-07-06 23:56:59.000000 cryptographyComplements-0.3.0/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     2451 2023-07-07 00:05:14.000000 cryptographyComplements-0.3.0/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-07 00:56:12.688474 cryptographyComplements-0.3.0/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      285 2023-07-07 00:56:12.000000 cryptographyComplements-0.3.0/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 00:56:12.694135 cryptographyComplements-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      809 2023-06-23 18:35:31.000000 cryptographyComplements-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:01:09.301591 cryptographyComplements-0.3.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.3.0.1/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.3.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      581 2023-07-07 01:01:09.298635 cryptographyComplements-0.3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.3.0.1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:01:09.292191 cryptographyComplements-0.3.0.1/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     4630 2023-07-07 00:09:52.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    16189 2023-07-07 00:40:25.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2182 2023-07-06 23:56:59.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     2451 2023-07-07 00:05:14.000000 cryptographyComplements-0.3.0.1/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:01:09.296220 cryptographyComplements-0.3.0.1/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-07-07 01:01:09.000000 cryptographyComplements-0.3.0.1/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 01:01:09.302591 cryptographyComplements-0.3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-07-07 01:01:03.000000 cryptographyComplements-0.3.0.1/setup.py
```

### Comparing `cryptographyComplements-0.3.0/LICENSE` & `cryptographyComplements-0.3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.0/PKG-INFO` & `cryptographyComplements-0.3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.3.0
+Version: 0.3.0.1
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.3.0/cryptographyComplements/cryptosystems.py` & `cryptographyComplements-0.3.0.1/cryptographyComplements/cryptosystems.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.0/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.3.0.1/cryptographyComplements/mathFunctions.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.0/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.3.0.1/cryptographyComplements/primalityTests.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.0/cryptographyComplements/tools.py` & `cryptographyComplements-0.3.0.1/cryptographyComplements/tools.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.3.0/setup.py` & `cryptographyComplements-0.3.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from setuptools import setup, find_packages
 import decimal
 
 setup(
     name='cryptographyComplements',
-    version='0.3.0',
+    version='0.3.0.1',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
         'Source': 'https://github.com/Forzooo/cryptographyComplements',
         'Documentation': 'https://cryptographycomplements.readthedocs.io/'
     },
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
-    install_requires=[
-        'decimal',
-    ]
-
 )
```


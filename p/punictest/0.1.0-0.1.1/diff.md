# Comparing `tmp/punictest-0.1.0.tar.gz` & `tmp/punictest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punictest-0.1.0.tar", last modified: Thu Jul  6 22:05:43 2023, max compression
+gzip compressed data, was "punictest-0.1.1.tar", last modified: Thu Jul  6 22:23:47 2023, max compression
```

## Comparing `punictest-0.1.0.tar` & `punictest-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 22:05:43.763094 punictest-0.1.0/
--rw-rw-rw-   0        0        0     1085 2023-07-06 21:26:08.000000 punictest-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2191 2023-07-06 22:05:43.762013 punictest-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1546 2023-07-06 22:04:54.000000 punictest-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 22:05:43.726531 punictest-0.1.0/punic/
--rw-rw-rw-   0        0        0       24 2023-07-06 21:44:30.000000 punictest-0.1.0/punic/__init__.py
--rw-rw-rw-   0        0        0     1808 2023-07-06 21:49:36.000000 punictest-0.1.0/punic/punic.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:05:43.760012 punictest-0.1.0/punictest.egg-info/
--rw-rw-rw-   0        0        0     2191 2023-07-06 22:05:43.000000 punictest-0.1.0/punictest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-06 22:05:43.000000 punictest-0.1.0/punictest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 22:05:43.000000 punictest-0.1.0/punictest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 22:05:43.000000 punictest-0.1.0/punictest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 22:05:43.764609 punictest-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-07-06 22:05:09.000000 punictest-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:23:47.481964 punictest-0.1.1/
+-rw-rw-rw-   0        0        0     1085 2023-07-06 21:26:08.000000 punictest-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2187 2023-07-06 22:23:47.479934 punictest-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1542 2023-07-06 22:22:27.000000 punictest-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 22:23:47.354762 punictest-0.1.1/punic/
+-rw-rw-rw-   0        0        0       24 2023-07-06 21:44:30.000000 punictest-0.1.1/punic/__init__.py
+-rw-rw-rw-   0        0        0     1808 2023-07-06 21:49:36.000000 punictest-0.1.1/punic/punic.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:23:47.477562 punictest-0.1.1/punictest.egg-info/
+-rw-rw-rw-   0        0        0     2187 2023-07-06 22:23:47.000000 punictest-0.1.1/punictest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-07-06 22:23:47.000000 punictest-0.1.1/punictest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 22:23:47.000000 punictest-0.1.1/punictest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 22:23:47.000000 punictest-0.1.1/punictest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 22:23:47.481964 punictest-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-07-06 22:23:02.000000 punictest-0.1.1/setup.py
```

### Comparing `punictest-0.1.0/LICENSE` & `punictest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `punictest-0.1.0/PKG-INFO` & `punictest-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punictest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple unit testing for python
 Home-page: https://github.com/Somespi/Punic
 Author: Someone.
 Author-email: someonegithub@email.com
 Keywords: unit testing test automation quality assurance software development
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 ## Getting Started
 
 1. Install Punic: `pip install punictest`
 
 2. Write your tests using the `assert_` method:
 
 ```python
-from punictest import Punic
+from punic import Punic
 
 p = Punic()
 p.assert_(4, lambda: 2 + 2, "Addition")
 
 ``` 
 
 3. Run your test program.
```

### Comparing `punictest-0.1.0/README.md` & `punictest-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## Getting Started
 
 1. Install Punic: `pip install punictest`
 
 2. Write your tests using the `assert_` method:
 
 ```python
-from punictest import Punic
+from punic import Punic
 
 p = Punic()
 p.assert_(4, lambda: 2 + 2, "Addition")
 
 ``` 
 
 3. Run your test program.
```

### Comparing `punictest-0.1.0/punic/punic.py` & `punictest-0.1.1/punic/punic.py`

 * *Files identical despite different names*

### Comparing `punictest-0.1.0/punictest.egg-info/PKG-INFO` & `punictest-0.1.1/punictest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punictest
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple unit testing for python
 Home-page: https://github.com/Somespi/Punic
 Author: Someone.
 Author-email: someonegithub@email.com
 Keywords: unit testing test automation quality assurance software development
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,15 @@
 ## Getting Started
 
 1. Install Punic: `pip install punictest`
 
 2. Write your tests using the `assert_` method:
 
 ```python
-from punictest import Punic
+from punic import Punic
 
 p = Punic()
 p.assert_(4, lambda: 2 + 2, "Addition")
 
 ``` 
 
 3. Run your test program.
```

### Comparing `punictest-0.1.0/setup.py` & `punictest-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='punictest',
-    version='0.1.0',
+    version='0.1.1',
     description='Simple unit testing for python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Someone.',
     author_email='someonegithub@email.com',
     url='https://github.com/Somespi/Punic',
     packages=find_packages(),
```


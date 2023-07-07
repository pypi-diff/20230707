# Comparing `tmp/openi_test-0.1.6.tar.gz` & `tmp/openi_test-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi_test-0.1.6.tar", last modified: Fri Jul  7 06:56:07 2023, max compression
+gzip compressed data, was "dist\openi_test-0.1.7.tar", last modified: Fri Jul  7 07:11:36 2023, max compression
```

## Comparing `openi_test-0.1.6.tar` & `openi_test-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 06:56:07.604390 openi_test-0.1.6/
--rw-rw-rw-   0        0        0     4989 2023-07-07 06:56:07.602763 openi_test-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 06:56:07.604900 openi_test-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1228 2023-07-07 06:56:01.000000 openi_test-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 06:56:07.543683 openi_test-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 06:56:07.565650 openi_test-0.1.6/src/openi_test/
--rw-rw-rw-   0        0        0      120 2023-07-07 03:39:31.000000 openi_test-0.1.6/src/openi_test/__init__.py
--rw-rw-rw-   0        0        0      373 2023-07-05 09:26:46.000000 openi_test-0.1.6/src/openi_test/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-07 06:56:07.592783 openi_test-0.1.6/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     4989 2023-07-07 06:56:07.000000 openi_test-0.1.6/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-07-07 06:56:07.000000 openi_test-0.1.6/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 06:56:07.000000 openi_test-0.1.6/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 06:56:07.000000 openi_test-0.1.6/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-07 06:56:07.000000 openi_test-0.1.6/src/openi_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 06:56:07.598509 openi_test-0.1.6/test/
--rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.1.6/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:11:36.197740 openi_test-0.1.7/
+-rw-rw-rw-   0        0        0     4989 2023-07-07 07:11:36.195727 openi_test-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 07:11:36.197740 openi_test-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1228 2023-07-07 07:11:22.000000 openi_test-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:11:36.146742 openi_test-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 07:11:36.163726 openi_test-0.1.7/src/openi_test/
+-rw-rw-rw-   0        0        0      120 2023-07-07 07:11:14.000000 openi_test-0.1.7/src/openi_test/__init__.py
+-rw-rw-rw-   0        0        0      373 2023-07-05 09:26:46.000000 openi_test-0.1.7/src/openi_test/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:11:36.184728 openi_test-0.1.7/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     4989 2023-07-07 07:11:35.000000 openi_test-0.1.7/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-07-07 07:11:36.000000 openi_test-0.1.7/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 07:11:35.000000 openi_test-0.1.7/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 07:11:35.000000 openi_test-0.1.7/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-07 07:11:35.000000 openi_test-0.1.7/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 07:11:36.190729 openi_test-0.1.7/test/
+-rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.1.7/test/test_upload_multi.py
```

### Comparing `openi_test-0.1.6/PKG-INFO` & `openi_test-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi_test
-Version: 0.1.6
+Version: 0.1.7
 Summary: A test packages for openi_test pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.1.6/README.md` & `openi_test-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `openi_test-0.1.6/setup.py` & `openi_test-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi_test',
-    version='0.1.6',
+    version='0.1.7',
     description='A test packages for openi_test pypi',
     package_dir={'': 'src'},
     packages=['openi_test'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
```

### Comparing `openi_test-0.1.6/src/openi_test.egg-info/PKG-INFO` & `openi_test-0.1.7/src/openi_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.1.6
+Version: 0.1.7
 Summary: A test packages for openi_test pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.1.6/test/test_upload_multi.py` & `openi_test-0.1.7/test/test_upload_multi.py`

 * *Files identical despite different names*


# Comparing `tmp/openi_test-0.1.2.tar.gz` & `tmp/openi_test-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi_test-0.1.2.tar", last modified: Fri Jul  7 01:48:22 2023, max compression
+gzip compressed data, was "dist\openi_test-0.1.3.tar", last modified: Fri Jul  7 01:54:11 2023, max compression
```

## Comparing `openi_test-0.1.2.tar` & `openi_test-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 01:48:22.928913 openi_test-0.1.2/
--rw-rw-rw-   0        0        0     4984 2023-07-07 01:48:22.925953 openi_test-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 01:48:22.929523 openi_test-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1193 2023-07-07 01:48:15.000000 openi_test-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:48:22.861663 openi_test-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 01:48:22.874658 openi_test-0.1.2/src/openi/
--rw-rw-rw-   0        0        0      120 2023-07-07 01:47:40.000000 openi_test-0.1.2/src/openi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:48:22.884034 openi_test-0.1.2/src/openi/dataset/
--rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi_test-0.1.2/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0    12954 2023-07-05 09:26:46.000000 openi_test-0.1.2/src/openi/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:48:22.888462 openi_test-0.1.2/src/openi/utils/
--rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi_test-0.1.2/src/openi/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:48:22.916301 openi_test-0.1.2/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     4984 2023-07-07 01:48:22.000000 openi_test-0.1.2/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-07 01:48:22.000000 openi_test-0.1.2/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 01:48:22.000000 openi_test-0.1.2/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 01:48:22.000000 openi_test-0.1.2/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 01:48:22.000000 openi_test-0.1.2/src/openi_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 01:48:22.922150 openi_test-0.1.2/test/
--rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.1.2/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:54:11.514563 openi_test-0.1.3/
+-rw-rw-rw-   0        0        0     4984 2023-07-07 01:54:11.513564 openi_test-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 01:54:11.515563 openi_test-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-07-07 01:54:06.000000 openi_test-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:54:11.470564 openi_test-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 01:54:11.503563 openi_test-0.1.3/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     4984 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 01:54:11.508564 openi_test-0.1.3/test/
+-rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.1.3/test/test_upload_multi.py
```

### Comparing `openi_test-0.1.2/PKG-INFO` & `openi_test-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi_test
-Version: 0.1.2
+Version: 0.1.3
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.1.2/README.md` & `openi_test-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openi_test-0.1.2/setup.py` & `openi_test-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi_test',
-    version='0.1.2',
+    version='0.1.3',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi_test-0.1.2/src/openi_test.egg-info/PKG-INFO` & `openi_test-0.1.3/src/openi_test.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.1.2
+Version: 0.1.3
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.1.2/test/test_upload_multi.py` & `openi_test-0.1.3/test/test_upload_multi.py`

 * *Files identical despite different names*


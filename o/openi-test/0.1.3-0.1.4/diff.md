# Comparing `tmp/openi_test-0.1.3.tar.gz` & `tmp/openi_test-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi_test-0.1.3.tar", last modified: Fri Jul  7 01:54:11 2023, max compression
+gzip compressed data, was "dist\openi_test-0.1.4.tar", last modified: Fri Jul  7 02:21:45 2023, max compression
```

## Comparing `openi_test-0.1.3.tar` & `openi_test-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 01:54:11.514563 openi_test-0.1.3/
--rw-rw-rw-   0        0        0     4984 2023-07-07 01:54:11.513564 openi_test-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 01:54:11.515563 openi_test-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1193 2023-07-07 01:54:06.000000 openi_test-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:54:11.470564 openi_test-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 01:54:11.503563 openi_test-0.1.3/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     4984 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 01:54:11.000000 openi_test-0.1.3/src/openi_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 01:54:11.508564 openi_test-0.1.3/test/
--rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.1.3/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:21:45.812030 openi_test-0.1.4/
+-rw-rw-rw-   0        0        0     4984 2023-07-07 02:21:45.810027 openi_test-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:21:45.813030 openi_test-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-07-07 02:21:38.000000 openi_test-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:21:45.770029 openi_test-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 02:21:45.802028 openi_test-0.1.4/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     4984 2023-07-07 02:21:45.000000 openi_test-0.1.4/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-07-07 02:21:45.000000 openi_test-0.1.4/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:21:45.000000 openi_test-0.1.4/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 02:21:45.000000 openi_test-0.1.4/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:21:45.000000 openi_test-0.1.4/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 02:21:45.806030 openi_test-0.1.4/test/
+-rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.1.4/test/test_upload_multi.py
```

### Comparing `openi_test-0.1.3/PKG-INFO` & `openi_test-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi_test
-Version: 0.1.3
+Version: 0.1.4
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.1.3/README.md` & `openi_test-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openi_test-0.1.3/setup.py` & `openi_test-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi_test',
-    version='0.1.3',
+    version='0.1.4',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi_test-0.1.3/src/openi_test.egg-info/PKG-INFO` & `openi_test-0.1.4/src/openi_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.1.3
+Version: 0.1.4
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.1.3/test/test_upload_multi.py` & `openi_test-0.1.4/test/test_upload_multi.py`

 * *Files identical despite different names*


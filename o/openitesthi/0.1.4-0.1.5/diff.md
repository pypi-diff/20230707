# Comparing `tmp/openitesthi-0.1.4.tar.gz` & `tmp/openitesthi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openitesthi-0.1.4.tar", last modified: Fri Jul  7 02:42:23 2023, max compression
+gzip compressed data, was "dist\openitesthi-0.1.5.tar", last modified: Fri Jul  7 02:44:24 2023, max compression
```

## Comparing `openitesthi-0.1.4.tar` & `openitesthi-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:42:23.599594 openitesthi-0.1.4/
--rw-rw-rw-   0        0        0     4990 2023-07-07 02:42:23.597592 openitesthi-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openitesthi-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 02:42:23.600591 openitesthi-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1199 2023-07-07 02:41:58.000000 openitesthi-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:42:23.562591 openitesthi-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 02:42:23.590589 openitesthi-0.1.4/src/openitesthi.egg-info/
--rw-rw-rw-   0        0        0     4990 2023-07-07 02:42:23.000000 openitesthi-0.1.4/src/openitesthi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-07 02:42:23.000000 openitesthi-0.1.4/src/openitesthi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:42:23.000000 openitesthi-0.1.4/src/openitesthi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 02:42:23.000000 openitesthi-0.1.4/src/openitesthi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:42:23.000000 openitesthi-0.1.4/src/openitesthi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 02:42:23.594590 openitesthi-0.1.4/test/
--rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openitesthi-0.1.4/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:24.861399 openitesthi-0.1.5/
+-rw-rw-rw-   0        0        0     4990 2023-07-07 02:44:24.859394 openitesthi-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openitesthi-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:44:24.861399 openitesthi-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1199 2023-07-07 02:44:15.000000 openitesthi-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:24.821236 openitesthi-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:24.851400 openitesthi-0.1.5/src/openitesthi.egg-info/
+-rw-rw-rw-   0        0        0     4990 2023-07-07 02:44:24.000000 openitesthi-0.1.5/src/openitesthi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-07-07 02:44:24.000000 openitesthi-0.1.5/src/openitesthi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:44:24.000000 openitesthi-0.1.5/src/openitesthi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 02:44:24.000000 openitesthi-0.1.5/src/openitesthi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:44:24.000000 openitesthi-0.1.5/src/openitesthi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:24.856399 openitesthi-0.1.5/test/
+-rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openitesthi-0.1.5/test/test_upload_multi.py
```

### Comparing `openitesthi-0.1.4/PKG-INFO` & `openitesthi-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openitesthi
-Version: 0.1.4
+Version: 0.1.5
 Summary: A test packages for openi_test pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openitesthi-0.1.4/README.md` & `openitesthi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openitesthi-0.1.4/setup.py` & `openitesthi-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openitesthi',
-    version='0.1.4',
+    version='0.1.5',
     description='A test packages for openi_test pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openitesthi-0.1.4/src/openitesthi.egg-info/PKG-INFO` & `openitesthi-0.1.5/src/openitesthi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openitesthi
-Version: 0.1.4
+Version: 0.1.5
 Summary: A test packages for openi_test pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openitesthi-0.1.4/test/test_upload_multi.py` & `openitesthi-0.1.5/test/test_upload_multi.py`

 * *Files identical despite different names*


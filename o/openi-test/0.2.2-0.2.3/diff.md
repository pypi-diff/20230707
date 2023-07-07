# Comparing `tmp/openi_test-0.2.2.tar.gz` & `tmp/openi_test-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi_test-0.2.2.tar", last modified: Fri Jul  7 07:43:09 2023, max compression
+gzip compressed data, was "dist\openi_test-0.2.3.tar", last modified: Fri Jul  7 07:50:33 2023, max compression
```

## Comparing `openi_test-0.2.2.tar` & `openi_test-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.438964 openi_test-0.2.2/
--rw-rw-rw-   0        0        0     4989 2023-07-07 07:43:09.436967 openi_test-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 07:43:09.439968 openi_test-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1310 2023-07-07 07:43:01.000000 openi_test-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.337976 openi_test-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.361974 openi_test-0.2.2/src/openi_test/
--rw-rw-rw-   0        0        0      120 2023-07-07 07:11:14.000000 openi_test-0.2.2/src/openi_test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.406964 openi_test-0.2.2/src/openi_test/cloudbrain/
--rw-rw-rw-   0        0        0      105 2023-07-05 10:23:26.000000 openi_test-0.2.2/src/openi_test/cloudbrain/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-07-05 09:23:35.000000 openi_test-0.2.2/src/openi_test/cloudbrain/env_check.py
--rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi_test-0.2.2/src/openi_test/cloudbrain/helper.py
--rw-rw-rw-   0        0        0     1440 2023-06-09 01:59:04.000000 openi_test-0.2.2/src/openi_test/cloudbrain/minio_operate.py
--rw-rw-rw-   0        0        0     2708 2023-07-05 09:58:13.000000 openi_test-0.2.2/src/openi_test/cloudbrain/obs_operate.py
--rw-rw-rw-   0        0        0      373 2023-07-05 09:26:46.000000 openi_test-0.2.2/src/openi_test/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.415963 openi_test-0.2.2/src/openi_test/dataset/
--rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi_test-0.2.2/src/openi_test/dataset/__init__.py
--rw-rw-rw-   0        0        0    12954 2023-07-05 09:26:46.000000 openi_test-0.2.2/src/openi_test/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.424963 openi_test-0.2.2/src/openi_test/path/
--rw-rw-rw-   0        0        0       19 2023-07-05 10:08:36.000000 openi_test-0.2.2/src/openi_test/path/__init__.py
--rw-rw-rw-   0        0        0     2218 2023-07-07 07:42:21.000000 openi_test-0.2.2/src/openi_test/path/path.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.428963 openi_test-0.2.2/src/openi_test/utils/
--rw-rw-rw-   0        0        0      428 2023-07-05 09:26:46.000000 openi_test-0.2.2/src/openi_test/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.383968 openi_test-0.2.2/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     4989 2023-07-07 07:43:09.000000 openi_test-0.2.2/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-07-07 07:43:09.000000 openi_test-0.2.2/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:43:09.000000 openi_test-0.2.2/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 07:43:09.000000 openi_test-0.2.2/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-07 07:43:09.000000 openi_test-0.2.2/src/openi_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 07:43:09.431961 openi_test-0.2.2/test/
--rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.2.2/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.225671 openi_test-0.2.3/
+-rw-rw-rw-   0        0        0     4989 2023-07-07 07:50:33.223669 openi_test-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 07:50:33.225671 openi_test-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1310 2023-07-07 07:50:25.000000 openi_test-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.117670 openi_test-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.153667 openi_test-0.2.3/src/openi_test/
+-rw-rw-rw-   0        0        0      120 2023-07-07 07:11:14.000000 openi_test-0.2.3/src/openi_test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.194690 openi_test-0.2.3/src/openi_test/cloudbrain/
+-rw-rw-rw-   0        0        0       82 2023-07-07 07:50:00.000000 openi_test-0.2.3/src/openi_test/cloudbrain/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-07-05 09:23:35.000000 openi_test-0.2.3/src/openi_test/cloudbrain/env_check.py
+-rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi_test-0.2.3/src/openi_test/cloudbrain/helper.py
+-rw-rw-rw-   0        0        0     1440 2023-06-09 01:59:04.000000 openi_test-0.2.3/src/openi_test/cloudbrain/minio_operate.py
+-rw-rw-rw-   0        0        0     2708 2023-07-05 09:58:13.000000 openi_test-0.2.3/src/openi_test/cloudbrain/obs_operate.py
+-rw-rw-rw-   0        0        0      373 2023-07-05 09:26:46.000000 openi_test-0.2.3/src/openi_test/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.202687 openi_test-0.2.3/src/openi_test/dataset/
+-rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi_test-0.2.3/src/openi_test/dataset/__init__.py
+-rw-rw-rw-   0        0        0    12954 2023-07-05 09:26:46.000000 openi_test-0.2.3/src/openi_test/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.210669 openi_test-0.2.3/src/openi_test/path/
+-rw-rw-rw-   0        0        0       19 2023-07-05 10:08:36.000000 openi_test-0.2.3/src/openi_test/path/__init__.py
+-rw-rw-rw-   0        0        0     2218 2023-07-07 07:42:21.000000 openi_test-0.2.3/src/openi_test/path/path.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.215679 openi_test-0.2.3/src/openi_test/utils/
+-rw-rw-rw-   0        0        0      428 2023-07-05 09:26:46.000000 openi_test-0.2.3/src/openi_test/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.172668 openi_test-0.2.3/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     4989 2023-07-07 07:50:32.000000 openi_test-0.2.3/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-07-07 07:50:33.000000 openi_test-0.2.3/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 07:50:32.000000 openi_test-0.2.3/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 07:50:32.000000 openi_test-0.2.3/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-07 07:50:32.000000 openi_test-0.2.3/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 07:50:33.219667 openi_test-0.2.3/test/
+-rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.2.3/test/test_upload_multi.py
```

### Comparing `openi_test-0.2.2/PKG-INFO` & `openi_test-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi_test
-Version: 0.2.2
+Version: 0.2.3
 Summary: A test packages for openi_test pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.2.2/README.md` & `openi_test-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.2/setup.py` & `openi_test-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi_test',
-    version='0.2.2',
+    version='0.2.3',
     description='A test packages for openi_test pypi',
     package_dir={'': 'src'},
     packages=['openi_test','openi_test.dataset','openi_test.path','openi_test.cloudbrain','openi_test.utils'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
```

### Comparing `openi_test-0.2.2/src/openi_test/cloudbrain/env_check.py` & `openi_test-0.2.3/src/openi_test/cloudbrain/env_check.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.2/src/openi_test/cloudbrain/helper.py` & `openi_test-0.2.3/src/openi_test/cloudbrain/helper.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.2/src/openi_test/cloudbrain/minio_operate.py` & `openi_test-0.2.3/src/openi_test/cloudbrain/minio_operate.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.2/src/openi_test/cloudbrain/obs_operate.py` & `openi_test-0.2.3/src/openi_test/cloudbrain/obs_operate.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.2/src/openi_test/dataset/dataset.py` & `openi_test-0.2.3/src/openi_test/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.2/src/openi_test/path/path.py` & `openi_test-0.2.3/src/openi_test/path/path.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.2/src/openi_test.egg-info/PKG-INFO` & `openi_test-0.2.3/src/openi_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.2.2
+Version: 0.2.3
 Summary: A test packages for openi_test pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.2.2/src/openi_test.egg-info/SOURCES.txt` & `openi_test-0.2.3/src/openi_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.2/test/test_upload_multi.py` & `openi_test-0.2.3/test/test_upload_multi.py`

 * *Files identical despite different names*


# Comparing `tmp/openi_test-0.2.4.tar.gz` & `tmp/openi_test-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi_test-0.2.4.tar", last modified: Fri Jul  7 07:58:41 2023, max compression
+gzip compressed data, was "dist\openi_test-0.2.5.tar", last modified: Fri Jul  7 08:01:32 2023, max compression
```

## Comparing `openi_test-0.2.4.tar` & `openi_test-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.995844 openi_test-0.2.4/
--rw-rw-rw-   0        0        0     4989 2023-07-07 07:58:40.993841 openi_test-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 07:58:40.995844 openi_test-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1310 2023-07-07 07:58:36.000000 openi_test-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.738778 openi_test-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.852849 openi_test-0.2.4/src/openi_test/
--rw-rw-rw-   0        0        0      120 2023-07-07 07:11:14.000000 openi_test-0.2.4/src/openi_test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.954831 openi_test-0.2.4/src/openi_test/cloudbrain/
--rw-rw-rw-   0        0        0       82 2023-07-07 07:50:00.000000 openi_test-0.2.4/src/openi_test/cloudbrain/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-07-05 09:23:35.000000 openi_test-0.2.4/src/openi_test/cloudbrain/env_check.py
--rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi_test-0.2.4/src/openi_test/cloudbrain/helper.py
--rw-rw-rw-   0        0        0     1440 2023-06-09 01:59:04.000000 openi_test-0.2.4/src/openi_test/cloudbrain/minio_operate.py
--rw-rw-rw-   0        0        0     2708 2023-07-05 09:58:13.000000 openi_test-0.2.4/src/openi_test/cloudbrain/obs_operate.py
--rw-rw-rw-   0        0        0      373 2023-07-05 09:26:46.000000 openi_test-0.2.4/src/openi_test/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.972845 openi_test-0.2.4/src/openi_test/dataset/
--rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi_test-0.2.4/src/openi_test/dataset/__init__.py
--rw-rw-rw-   0        0        0    12954 2023-07-05 09:26:46.000000 openi_test-0.2.4/src/openi_test/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.981855 openi_test-0.2.4/src/openi_test/path/
--rw-rw-rw-   0        0        0       19 2023-07-05 10:08:36.000000 openi_test-0.2.4/src/openi_test/path/__init__.py
--rw-rw-rw-   0        0        0     2188 2023-07-07 07:58:16.000000 openi_test-0.2.4/src/openi_test/path/path.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.987846 openi_test-0.2.4/src/openi_test/utils/
--rw-rw-rw-   0        0        0      428 2023-07-05 09:26:46.000000 openi_test-0.2.4/src/openi_test/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.879845 openi_test-0.2.4/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     4989 2023-07-07 07:58:40.000000 openi_test-0.2.4/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-07-07 07:58:40.000000 openi_test-0.2.4/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:58:40.000000 openi_test-0.2.4/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 07:58:40.000000 openi_test-0.2.4/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-07 07:58:40.000000 openi_test-0.2.4/src/openi_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 07:58:40.990844 openi_test-0.2.4/test/
--rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.2.4/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.962249 openi_test-0.2.5/
+-rw-rw-rw-   0        0        0     4989 2023-07-07 08:01:32.961250 openi_test-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 08:01:32.962249 openi_test-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1310 2023-07-07 08:01:22.000000 openi_test-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.855255 openi_test-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.882255 openi_test-0.2.5/src/openi_test/
+-rw-rw-rw-   0        0        0      120 2023-07-07 07:11:14.000000 openi_test-0.2.5/src/openi_test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.930251 openi_test-0.2.5/src/openi_test/cloudbrain/
+-rw-rw-rw-   0        0        0       82 2023-07-07 07:50:00.000000 openi_test-0.2.5/src/openi_test/cloudbrain/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-07-05 09:23:35.000000 openi_test-0.2.5/src/openi_test/cloudbrain/env_check.py
+-rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi_test-0.2.5/src/openi_test/cloudbrain/helper.py
+-rw-rw-rw-   0        0        0     1440 2023-06-09 01:59:04.000000 openi_test-0.2.5/src/openi_test/cloudbrain/minio_operate.py
+-rw-rw-rw-   0        0        0     2708 2023-07-05 09:58:13.000000 openi_test-0.2.5/src/openi_test/cloudbrain/obs_operate.py
+-rw-rw-rw-   0        0        0      373 2023-07-05 09:26:46.000000 openi_test-0.2.5/src/openi_test/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.940258 openi_test-0.2.5/src/openi_test/dataset/
+-rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi_test-0.2.5/src/openi_test/dataset/__init__.py
+-rw-rw-rw-   0        0        0    12954 2023-07-05 09:26:46.000000 openi_test-0.2.5/src/openi_test/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.947251 openi_test-0.2.5/src/openi_test/path/
+-rw-rw-rw-   0        0        0       19 2023-07-05 10:08:36.000000 openi_test-0.2.5/src/openi_test/path/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-07-07 07:58:16.000000 openi_test-0.2.5/src/openi_test/path/path.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.953251 openi_test-0.2.5/src/openi_test/utils/
+-rw-rw-rw-   0        0        0      428 2023-07-05 09:26:46.000000 openi_test-0.2.5/src/openi_test/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.908251 openi_test-0.2.5/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     4989 2023-07-07 08:01:32.000000 openi_test-0.2.5/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-07-07 08:01:32.000000 openi_test-0.2.5/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 08:01:32.000000 openi_test-0.2.5/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 08:01:32.000000 openi_test-0.2.5/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-07 08:01:32.000000 openi_test-0.2.5/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 08:01:32.957267 openi_test-0.2.5/test/
+-rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.2.5/test/test_upload_multi.py
```

### Comparing `openi_test-0.2.4/PKG-INFO` & `openi_test-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi_test
-Version: 0.2.4
+Version: 0.2.5
 Summary: A test packages for openi_test pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.2.4/README.md` & `openi_test-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.4/setup.py` & `openi_test-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi_test',
-    version='0.2.4',
+    version='0.2.5',
     description='A test packages for openi_test pypi',
     package_dir={'': 'src'},
     packages=['openi_test','openi_test.dataset','openi_test.path','openi_test.cloudbrain','openi_test.utils'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
```

### Comparing `openi_test-0.2.4/src/openi_test/cloudbrain/env_check.py` & `openi_test-0.2.5/src/openi_test/cloudbrain/env_check.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.4/src/openi_test/cloudbrain/helper.py` & `openi_test-0.2.5/src/openi_test/cloudbrain/helper.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.4/src/openi_test/cloudbrain/minio_operate.py` & `openi_test-0.2.5/src/openi_test/cloudbrain/minio_operate.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.4/src/openi_test/cloudbrain/obs_operate.py` & `openi_test-0.2.5/src/openi_test/cloudbrain/obs_operate.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.4/src/openi_test/dataset/dataset.py` & `openi_test-0.2.5/src/openi_test/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.4/src/openi_test/path/path.py` & `openi_test-0.2.5/src/openi_test/path/path.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.4/src/openi_test.egg-info/PKG-INFO` & `openi_test-0.2.5/src/openi_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.2.4
+Version: 0.2.5
 Summary: A test packages for openi_test pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
```

### Comparing `openi_test-0.2.4/src/openi_test.egg-info/SOURCES.txt` & `openi_test-0.2.5/src/openi_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.4/test/test_upload_multi.py` & `openi_test-0.2.5/test/test_upload_multi.py`

 * *Files identical despite different names*


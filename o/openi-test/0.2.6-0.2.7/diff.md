# Comparing `tmp/openi_test-0.2.6.tar.gz` & `tmp/openi_test-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi_test-0.2.6.tar", last modified: Fri Jul  7 08:06:28 2023, max compression
+gzip compressed data, was "dist\openi_test-0.2.7.tar", last modified: Fri Jul  7 08:45:50 2023, max compression
```

## Comparing `openi_test-0.2.6.tar` & `openi_test-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:28.000780 openi_test-0.2.6/
--rw-rw-rw-   0        0        0     4989 2023-07-07 08:06:27.998777 openi_test-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3482 2023-07-06 08:09:07.000000 openi_test-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 08:06:28.001780 openi_test-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1310 2023-07-07 08:06:23.000000 openi_test-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:27.903784 openi_test-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:27.929778 openi_test-0.2.6/src/openi_test/
--rw-rw-rw-   0        0        0      120 2023-07-07 07:11:14.000000 openi_test-0.2.6/src/openi_test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:27.968800 openi_test-0.2.6/src/openi_test/cloudbrain/
--rw-rw-rw-   0        0        0       82 2023-07-07 07:50:00.000000 openi_test-0.2.6/src/openi_test/cloudbrain/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-07-05 09:23:35.000000 openi_test-0.2.6/src/openi_test/cloudbrain/env_check.py
--rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi_test-0.2.6/src/openi_test/cloudbrain/helper.py
--rw-rw-rw-   0        0        0     1440 2023-06-09 01:59:04.000000 openi_test-0.2.6/src/openi_test/cloudbrain/minio_operate.py
--rw-rw-rw-   0        0        0     2708 2023-07-05 09:58:13.000000 openi_test-0.2.6/src/openi_test/cloudbrain/obs_operate.py
--rw-rw-rw-   0        0        0      373 2023-07-05 09:26:46.000000 openi_test-0.2.6/src/openi_test/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:27.979778 openi_test-0.2.6/src/openi_test/dataset/
--rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi_test-0.2.6/src/openi_test/dataset/__init__.py
--rw-rw-rw-   0        0        0    12950 2023-07-07 08:06:15.000000 openi_test-0.2.6/src/openi_test/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:27.988788 openi_test-0.2.6/src/openi_test/path/
--rw-rw-rw-   0        0        0       19 2023-07-05 10:08:36.000000 openi_test-0.2.6/src/openi_test/path/__init__.py
--rw-rw-rw-   0        0        0     2188 2023-07-07 07:58:16.000000 openi_test-0.2.6/src/openi_test/path/path.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:27.992779 openi_test-0.2.6/src/openi_test/utils/
--rw-rw-rw-   0        0        0      428 2023-07-05 09:26:46.000000 openi_test-0.2.6/src/openi_test/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:27.948777 openi_test-0.2.6/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     4989 2023-07-07 08:06:27.000000 openi_test-0.2.6/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-07-07 08:06:27.000000 openi_test-0.2.6/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 08:06:27.000000 openi_test-0.2.6/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-07 08:06:27.000000 openi_test-0.2.6/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-07 08:06:27.000000 openi_test-0.2.6/src/openi_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 08:06:27.995777 openi_test-0.2.6/test/
--rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.2.6/test/test_upload_multi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.923395 openi_test-0.2.7/
+-rw-rw-rw-   0        0        0     4979 2023-07-07 08:45:50.922404 openi_test-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3477 2023-07-07 08:44:31.000000 openi_test-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 08:45:50.924400 openi_test-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-07-07 08:44:47.000000 openi_test-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.789769 openi_test-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.841769 openi_test-0.2.7/src/openi/
+-rw-rw-rw-   0        0        0      120 2023-07-07 07:11:14.000000 openi_test-0.2.7/src/openi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.871402 openi_test-0.2.7/src/openi/cloudbrain/
+-rw-rw-rw-   0        0        0       82 2023-07-07 07:50:00.000000 openi_test-0.2.7/src/openi/cloudbrain/__init__.py
+-rw-rw-rw-   0        0        0     1541 2023-07-05 09:23:35.000000 openi_test-0.2.7/src/openi/cloudbrain/env_check.py
+-rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi_test-0.2.7/src/openi/cloudbrain/helper.py
+-rw-rw-rw-   0        0        0     1440 2023-06-09 01:59:04.000000 openi_test-0.2.7/src/openi/cloudbrain/minio_operate.py
+-rw-rw-rw-   0        0        0     2708 2023-07-05 09:58:13.000000 openi_test-0.2.7/src/openi/cloudbrain/obs_operate.py
+-rw-rw-rw-   0        0        0      373 2023-07-05 09:26:46.000000 openi_test-0.2.7/src/openi/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.879401 openi_test-0.2.7/src/openi/dataset/
+-rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi_test-0.2.7/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0    12950 2023-07-07 08:06:15.000000 openi_test-0.2.7/src/openi/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.890400 openi_test-0.2.7/src/openi/path/
+-rw-rw-rw-   0        0        0       19 2023-07-05 10:08:36.000000 openi_test-0.2.7/src/openi/path/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-07-07 07:58:16.000000 openi_test-0.2.7/src/openi/path/path.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.894399 openi_test-0.2.7/src/openi/utils/
+-rw-rw-rw-   0        0        0      428 2023-07-05 09:26:46.000000 openi_test-0.2.7/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.914395 openi_test-0.2.7/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     4979 2023-07-07 08:45:50.000000 openi_test-0.2.7/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-07-07 08:45:50.000000 openi_test-0.2.7/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 08:45:50.000000 openi_test-0.2.7/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-07 08:45:50.000000 openi_test-0.2.7/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 08:45:50.000000 openi_test-0.2.7/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 08:45:50.917394 openi_test-0.2.7/test/
+-rw-rw-rw-   0        0        0      650 2023-07-05 09:26:46.000000 openi_test-0.2.7/test/test_upload_multi.py
```

### Comparing `openi_test-0.2.6/PKG-INFO` & `openi_test-0.2.7/src/openi_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: openi_test
-Version: 0.2.6
-Summary: A test packages for openi_test pypi
+Name: openi-test
+Version: 0.2.7
+Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
         
         > PYPI package for 启智AI协作平台。
@@ -20,15 +20,15 @@
           - 当前版本为了解决用户上传数据集的需求，建议在本地使用。后续版本将适配代码仓配置、隐藏token及云脑任务。
         
         ## 安装
         
         *适配python3.6及以上版本*
         
         ```bash
-        pip install -U openi-test
+        pip install -U openi
         ```
         
         ## 本地上传数据集示例
         
         **dataset.upload_file(file, username, repository, token, cluster = "NPU")**
         
         *上传本地单个文件到启智平台数据集，支持断点续传*
```

### Comparing `openi_test-0.2.6/README.md` & `openi_test-0.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   - 当前版本为了解决用户上传数据集的需求，建议在本地使用。后续版本将适配代码仓配置、隐藏token及云脑任务。
 
 ## 安装
 
 *适配python3.6及以上版本*
 
 ```bash
-pip install -U openi-test
+pip install -U openi
 ```
 
 ## 本地上传数据集示例
 
 **dataset.upload_file(file, username, repository, token, cluster = "NPU")**
 
 *上传本地单个文件到启智平台数据集，支持断点续传*
```

### Comparing `openi_test-0.2.6/setup.py` & `openi_test-0.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi_test',
-    version='0.2.6',
-    description='A test packages for openi_test pypi',
+    version='0.2.7',
+    description='A test packages for openi pypi',
     package_dir={'': 'src'},
-    packages=['openi_test','openi_test.dataset','openi_test.path','openi_test.cloudbrain','openi_test.utils'],
+    packages=['openi','openi.dataset','openi.path','openi.cloudbrain','openi.utils'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
     author_email='chenzh.ds@outlook.com',
     license='MIT',
     classifiers=[
```

### Comparing `openi_test-0.2.6/src/openi_test/cloudbrain/env_check.py` & `openi_test-0.2.7/src/openi/cloudbrain/env_check.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.6/src/openi_test/cloudbrain/helper.py` & `openi_test-0.2.7/src/openi/cloudbrain/helper.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.6/src/openi_test/cloudbrain/minio_operate.py` & `openi_test-0.2.7/src/openi/cloudbrain/minio_operate.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.6/src/openi_test/cloudbrain/obs_operate.py` & `openi_test-0.2.7/src/openi/cloudbrain/obs_operate.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.6/src/openi_test/dataset/dataset.py` & `openi_test-0.2.7/src/openi/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.6/src/openi_test/path/path.py` & `openi_test-0.2.7/src/openi/path/path.py`

 * *Files identical despite different names*

### Comparing `openi_test-0.2.6/src/openi_test.egg-info/PKG-INFO` & `openi_test-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: openi-test
-Version: 0.2.6
-Summary: A test packages for openi_test pypi
+Name: openi_test
+Version: 0.2.7
+Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # OpenI PyPi
         
         > PYPI package for 启智AI协作平台。
@@ -20,15 +20,15 @@
           - 当前版本为了解决用户上传数据集的需求，建议在本地使用。后续版本将适配代码仓配置、隐藏token及云脑任务。
         
         ## 安装
         
         *适配python3.6及以上版本*
         
         ```bash
-        pip install -U openi-test
+        pip install -U openi
         ```
         
         ## 本地上传数据集示例
         
         **dataset.upload_file(file, username, repository, token, cluster = "NPU")**
         
         *上传本地单个文件到启智平台数据集，支持断点续传*
```

### Comparing `openi_test-0.2.6/test/test_upload_multi.py` & `openi_test-0.2.7/test/test_upload_multi.py`

 * *Files identical despite different names*


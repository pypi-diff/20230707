# Comparing `tmp/alibabacloud_rds20140815-2.2.5.tar.gz` & `tmp/alibabacloud_rds20140815-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815-2.2.5.tar", last modified: Wed Jul  5 15:10:53 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815-2.2.6.tar", last modified: Thu Jul  6 15:10:45 2023, max compression
```

## Comparing `alibabacloud_rds20140815-2.2.5.tar` & `alibabacloud_rds20140815-2.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/
--rw-r--r--   0 root         (0) root         (0)     1783 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1662691 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2540490 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 15:10:53.000000 alibabacloud_rds20140815-2.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2023-07-05 15:10:52.000000 alibabacloud_rds20140815-2.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1662691 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2540490 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-07-06 15:10:45.000000 alibabacloud_rds20140815-2.2.6/setup.py
```

### Comparing `alibabacloud_rds20140815-2.2.5/ChangeLog.md` & `alibabacloud_rds20140815-2.2.6/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-05 Version: 2.2.5
+- Add AutoUseCoupon field.
+- Api Offline.
+
 2023-07-04 Version: 2.2.4
 - Fix bugs for  DescribeDedicatedHosts.
 - Fixed bugs add ERRORCODE.
 - Added serverless config to support serverless price query.
 
 2023-07-04 Version: 2.2.3
 - ModifyBackupPolicy API support parameter BackupPriority.
```

### Comparing `alibabacloud_rds20140815-2.2.5/LICENSE` & `alibabacloud_rds20140815-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.5/PKG-INFO` & `alibabacloud_rds20140815-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815
-Version: 2.2.5
+Version: 2.2.6
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815-2.2.5/README-CN.md` & `alibabacloud_rds20140815-2.2.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.5/README.md` & `alibabacloud_rds20140815-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.5/alibabacloud_rds20140815.egg-info/PKG-INFO` & `alibabacloud_rds20140815-2.2.6/alibabacloud_rds20140815.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815
-Version: 2.2.5
+Version: 2.2.6
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815-2.2.5/setup.py` & `alibabacloud_rds20140815-2.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds20140815.
 
-Created on 05/07/2023
+Created on 06/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds20140815"
 NAME = "alibabacloud_rds20140815" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds (20140815) SDK Library for Python"
```


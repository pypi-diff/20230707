# Comparing `tmp/moveFile-0.3.3.tar.gz` & `tmp/moveFile-0.3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveFile-0.3.3.tar", last modified: Tue May 16 06:02:11 2023, max compression
+gzip compressed data, was "moveFile-0.3.3.1.tar", last modified: Fri Jul  7 09:21:55 2023, max compression
```

## Comparing `moveFile-0.3.3.tar` & `moveFile-0.3.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 06:02:11.428736 moveFile-0.3.3/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 moveFile-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 moveFile-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      409 2023-05-16 06:02:11.429735 moveFile-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 moveFile-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 06:02:11.416737 moveFile-0.3.3/moveFile/
-drwxrwxrwx   0        0        0        0 2023-05-16 06:02:11.427736 moveFile-0.3.3/moveFile/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 moveFile-0.3.3/moveFile/Ui/__init__.py
--rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 moveFile-0.3.3/moveFile/Ui/moveFileUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 moveFile-0.3.3/moveFile/__init__.py
--rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 moveFile-0.3.3/moveFile/find_file_return_path_m1.pyd
--rw-rw-rw-   0        0        0   228352 2023-05-16 06:01:17.000000 moveFile-0.3.3/moveFile/moveFile.pyd
--rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 moveFile-0.3.3/moveFile/moveFileUi.pyd
--rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 moveFile-0.3.3/moveFile/optionDb.pyd
-drwxrwxrwx   0        0        0        0 2023-05-16 06:02:11.423736 moveFile-0.3.3/moveFile.egg-info/
--rw-rw-rw-   0        0        0      409 2023-05-16 06:02:11.000000 moveFile-0.3.3/moveFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-05-16 06:02:11.000000 moveFile-0.3.3/moveFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 06:02:11.000000 moveFile-0.3.3/moveFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 06:02:11.000000 moveFile-0.3.3/moveFile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2023-05-16 06:02:11.430737 moveFile-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      977 2023-05-16 06:00:19.000000 moveFile-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:21:55.025119 moveFile-0.3.3.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 moveFile-0.3.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 moveFile-0.3.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      411 2023-07-07 09:21:55.025119 moveFile-0.3.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 moveFile-0.3.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 09:21:55.002659 moveFile-0.3.3.1/moveFile/
+drwxrwxrwx   0        0        0        0 2023-07-07 09:21:55.022117 moveFile-0.3.3.1/moveFile/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-22 02:56:19.000000 moveFile-0.3.3.1/moveFile/Ui/__init__.py
+-rw-rw-rw-   0        0        0    71168 2023-04-28 06:15:40.000000 moveFile-0.3.3.1/moveFile/Ui/moveFileUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-22 08:31:58.000000 moveFile-0.3.3.1/moveFile/__init__.py
+-rw-rw-rw-   0        0        0    35840 2023-04-28 06:14:13.000000 moveFile-0.3.3.1/moveFile/find_file_return_path_m1.pyd
+-rw-rw-rw-   0        0        0   228352 2023-07-07 09:20:17.000000 moveFile-0.3.3.1/moveFile/moveFile.pyd
+-rw-rw-rw-   0        0        0    68608 2023-04-28 06:14:21.000000 moveFile-0.3.3.1/moveFile/moveFileUi.pyd
+-rw-rw-rw-   0        0        0    69632 2023-04-28 06:14:45.000000 moveFile-0.3.3.1/moveFile/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-07-07 09:21:55.016104 moveFile-0.3.3.1/moveFile.egg-info/
+-rw-rw-rw-   0        0        0      411 2023-07-07 09:21:54.000000 moveFile-0.3.3.1/moveFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-07-07 09:21:54.000000 moveFile-0.3.3.1/moveFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 09:21:54.000000 moveFile-0.3.3.1/moveFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 09:21:54.000000 moveFile-0.3.3.1/moveFile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2023-07-07 09:21:55.027120 moveFile-0.3.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-07-07 09:21:26.000000 moveFile-0.3.3.1/setup.py
```

### Comparing `moveFile-0.3.3/LICENSE.txt` & `moveFile-0.3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moveFile-0.3.3/setup.py` & `moveFile-0.3.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
 PATCH = 3
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "moveFile",
 	version = VERSION,
```


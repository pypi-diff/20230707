# Comparing `tmp/WordsToPdfs-0.3.2.tar.gz` & `tmp/WordsToPdfs-0.3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WordsToPdfs-0.3.2.tar", last modified: Fri May 12 07:24:36 2023, max compression
+gzip compressed data, was "WordsToPdfs-0.3.2.1.tar", last modified: Fri Jul  7 09:16:35 2023, max compression
```

## Comparing `WordsToPdfs-0.3.2.tar` & `WordsToPdfs-0.3.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 07:24:36.327478 WordsToPdfs-0.3.2/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 WordsToPdfs-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 WordsToPdfs-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      404 2023-05-12 07:24:36.327478 WordsToPdfs-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 WordsToPdfs-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 07:24:36.287480 WordsToPdfs-0.3.2/WordsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-05-12 07:24:36.312482 WordsToPdfs-0.3.2/WordsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.2/WordsToPdfs/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:24:36.322480 WordsToPdfs-0.3.2/WordsToPdfs/Ui/
--rw-rw-rw-   0        0        0    58880 2023-04-28 06:31:28.000000 WordsToPdfs-0.3.2/WordsToPdfs/Ui/WordToPdfUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.2/WordsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0   171008 2023-05-12 07:01:37.000000 WordsToPdfs-0.3.2/WordsToPdfs/WordsToPdfs.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.2/WordsToPdfs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:24:36.308483 WordsToPdfs-0.3.2/WordsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      404 2023-05-12 07:24:36.000000 WordsToPdfs-0.3.2/WordsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-05-12 07:24:36.000000 WordsToPdfs-0.3.2/WordsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 07:24:36.000000 WordsToPdfs-0.3.2/WordsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-12 07:24:36.000000 WordsToPdfs-0.3.2/WordsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-05-12 07:24:36.329485 WordsToPdfs-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      972 2023-05-12 07:24:32.000000 WordsToPdfs-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:16:35.432046 WordsToPdfs-0.3.2.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 WordsToPdfs-0.3.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 WordsToPdfs-0.3.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      406 2023-07-07 09:16:35.432046 WordsToPdfs-0.3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 WordsToPdfs-0.3.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 09:16:35.413043 WordsToPdfs-0.3.2.1/WordsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-07-07 09:16:35.425045 WordsToPdfs-0.3.2.1/WordsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.2.1/WordsToPdfs/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:16:35.430045 WordsToPdfs-0.3.2.1/WordsToPdfs/Ui/
+-rw-rw-rw-   0        0        0    58880 2023-04-28 06:31:28.000000 WordsToPdfs-0.3.2.1/WordsToPdfs/Ui/WordToPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.2.1/WordsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0   171008 2023-07-07 09:14:33.000000 WordsToPdfs-0.3.2.1/WordsToPdfs/WordsToPdfs.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.2.1/WordsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 09:16:35.423043 WordsToPdfs-0.3.2.1/WordsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      406 2023-07-07 09:16:35.000000 WordsToPdfs-0.3.2.1/WordsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-07-07 09:16:35.000000 WordsToPdfs-0.3.2.1/WordsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 09:16:35.000000 WordsToPdfs-0.3.2.1/WordsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 09:16:35.000000 WordsToPdfs-0.3.2.1/WordsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-07 09:16:35.434054 WordsToPdfs-0.3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-07-07 09:13:49.000000 WordsToPdfs-0.3.2.1/setup.py
```

### Comparing `WordsToPdfs-0.3.2/LICENSE.txt` & `WordsToPdfs-0.3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WordsToPdfs-0.3.2/setup.py` & `WordsToPdfs-0.3.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
 PATCH = 2
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "WordsToPdfs",
 	version = VERSION,
```


# Comparing `tmp/s3cps3-6.6.1.tar.gz` & `tmp/s3cps3-6.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/s3cps3-6.6.1.tar", last modified: Thu Jul  6 06:55:33 2023, max compression
+gzip compressed data, was "dist/s3cps3-6.6.2.tar", last modified: Thu Jul  6 11:57:14 2023, max compression
```

## Comparing `s3cps3-6.6.1.tar` & `s3cps3-6.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 06:55:33.000000 s3cps3-6.6.1/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1069 2023-07-03 09:25:58.000000 s3cps3-6.6.1/LICENSE
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       80 2023-07-05 10:09:29.000000 s3cps3-6.6.1/MANIFEST.in
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       72 2023-07-06 06:55:33.000000 s3cps3-6.6.1/PKG-INFO
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-05-29 11:05:45.000000 s3cps3-6.6.1/s3cps3/__init__.py
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1210 2023-06-26 09:37:27.000000 s3cps3-6.6.1/s3cps3/commons.py
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2212 2023-07-06 02:46:29.000000 s3cps3-6.6.1/s3cps3/listbucket.py
--rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)    10400 2023-07-06 02:25:10.000000 s3cps3-6.6.1/s3cps3/main.xsh
--rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       45 2023-07-05 10:52:13.000000 s3cps3-6.6.1/s3cps3/s32s3
--rwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      437 2023-05-29 13:19:00.000000 s3cps3-6.6.1/s3cps3/s3bigcp.sh
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     4119 2023-07-06 02:43:40.000000 s3cps3-6.6.1/s3cps3/s3cps3.py
-drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       72 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      299 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        1 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      165 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/requires.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        7 2023-07-06 06:55:33.000000 s3cps3-6.6.1/s3cps3.egg-info/top_level.txt
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       38 2023-07-06 06:55:33.000000 s3cps3-6.6.1/setup.cfg
--rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      646 2023-07-06 06:26:53.000000 s3cps3-6.6.1/setup.py
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 11:57:14.000000 s3cps3-6.6.2/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1069 2023-07-03 09:25:58.000000 s3cps3-6.6.2/LICENSE
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       80 2023-07-05 10:09:29.000000 s3cps3-6.6.2/MANIFEST.in
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      410 2023-07-06 11:57:14.000000 s3cps3-6.6.2/PKG-INFO
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 11:57:14.000000 s3cps3-6.6.2/s3cps3/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-05-29 11:05:45.000000 s3cps3-6.6.2/s3cps3/__init__.py
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     1210 2023-06-26 09:37:27.000000 s3cps3-6.6.2/s3cps3/commons.py
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     2212 2023-07-06 02:46:29.000000 s3cps3-6.6.2/s3cps3/listbucket.py
+-rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)    10400 2023-07-06 02:25:10.000000 s3cps3-6.6.2/s3cps3/main.xsh
+-rwxrwxrwx   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       38 2023-07-06 11:54:47.000000 s3cps3-6.6.2/s3cps3/s32s3
+-rwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      437 2023-05-29 13:19:00.000000 s3cps3-6.6.2/s3cps3/s3bigcp.sh
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)     4119 2023-07-06 02:43:40.000000 s3cps3-6.6.2/s3cps3/s3cps3.py
+drwxr-xr-x   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        0 2023-07-06 11:57:14.000000 s3cps3-6.6.2/s3cps3.egg-info/
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      410 2023-07-06 11:57:14.000000 s3cps3-6.6.2/s3cps3.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      299 2023-07-06 11:57:14.000000 s3cps3-6.6.2/s3cps3.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        1 2023-07-06 11:57:14.000000 s3cps3-6.6.2/s3cps3.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      165 2023-07-06 11:57:14.000000 s3cps3-6.6.2/s3cps3.egg-info/requires.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)        7 2023-07-06 11:57:14.000000 s3cps3-6.6.2/s3cps3.egg-info/top_level.txt
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)       38 2023-07-06 11:57:14.000000 s3cps3-6.6.2/setup.cfg
+-rw-r--r--   0 PJLAB\qinwenkai (409476540) PJLAB\domain^users (409469441)      777 2023-07-06 11:57:08.000000 s3cps3-6.6.2/setup.py
```

### Comparing `s3cps3-6.6.1/LICENSE` & `s3cps3-6.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.1/s3cps3/commons.py` & `s3cps3-6.6.2/s3cps3/commons.py`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.1/s3cps3/listbucket.py` & `s3cps3-6.6.2/s3cps3/listbucket.py`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.1/s3cps3/main.xsh` & `s3cps3-6.6.2/s3cps3/main.xsh`

 * *Files identical despite different names*

### Comparing `s3cps3-6.6.1/s3cps3/s3cps3.py` & `s3cps3-6.6.2/s3cps3/s3cps3.py`

 * *Files identical despite different names*


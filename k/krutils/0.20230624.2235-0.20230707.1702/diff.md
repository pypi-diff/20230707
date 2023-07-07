# Comparing `tmp/krutils-0.20230624.2235.tar.gz` & `tmp/krutils-0.20230707.1702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230624.2235.tar", last modified: Sat Jun 24 13:35:17 2023, max compression
+gzip compressed data, was "krutils-0.20230707.1702.tar", last modified: Fri Jul  7 08:02:12 2023, max compression
```

## Comparing `krutils-0.20230624.2235.tar` & `krutils-0.20230707.1702.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:35:17.065291 krutils-0.20230624.2235/
--rw-rw-rw-   0        0        0      526 2023-06-24 13:35:17.056208 krutils-0.20230624.2235/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230624.2235/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 13:35:16.996248 krutils-0.20230624.2235/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230624.2235/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230624.2235/krutils/CONST.py
--rw-rw-rw-   0        0        0      115 2023-06-07 14:26:39.000000 krutils-0.20230624.2235/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230624.2235/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     2956 2023-06-20 05:26:47.000000 krutils-0.20230624.2235/krutils/futils.py
--rw-rw-rw-   0        0        0    13843 2023-06-24 13:35:11.000000 krutils-0.20230624.2235/krutils/logger.py
--rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230624.2235/krutils/logger2.py
--rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230624.2235/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:35:17.029193 krutils-0.20230624.2235/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-06-24 13:35:16.000000 krutils-0.20230624.2235/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-24 13:35:16.000000 krutils-0.20230624.2235/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:35:16.000000 krutils-0.20230624.2235/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-24 13:35:16.000000 krutils-0.20230624.2235/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-24 13:35:16.000000 krutils-0.20230624.2235/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 13:35:17.070207 krutils-0.20230624.2235/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-06-24 13:35:16.000000 krutils-0.20230624.2235/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:35:17.036563 krutils-0.20230624.2235/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230624.2235/test/test_futils.py
--rw-rw-rw-   0        0        0      321 2023-06-24 13:23:59.000000 krutils-0.20230624.2235/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:02:12.254062 krutils-0.20230707.1702/
+-rw-rw-rw-   0        0        0      526 2023-07-07 08:02:12.251490 krutils-0.20230707.1702/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230707.1702/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 08:02:11.580729 krutils-0.20230707.1702/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230707.1702/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230707.1702/krutils/CONST.py
+-rw-rw-rw-   0        0        0      115 2023-06-07 14:26:39.000000 krutils-0.20230707.1702/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230707.1702/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2956 2023-06-20 05:26:47.000000 krutils-0.20230707.1702/krutils/futils.py
+-rw-rw-rw-   0        0        0    13860 2023-07-07 08:01:30.000000 krutils-0.20230707.1702/krutils/logger.py
+-rw-rw-rw-   0        0        0      669 2023-06-06 17:38:05.000000 krutils-0.20230707.1702/krutils/logger2.py
+-rw-rw-rw-   0        0        0    18188 2023-06-07 14:23:27.000000 krutils-0.20230707.1702/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:02:11.921426 krutils-0.20230707.1702/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-07-07 08:02:10.000000 krutils-0.20230707.1702/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-07 08:02:11.000000 krutils-0.20230707.1702/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 08:02:10.000000 krutils-0.20230707.1702/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-07 08:02:10.000000 krutils-0.20230707.1702/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-07 08:02:10.000000 krutils-0.20230707.1702/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 08:02:12.255258 krutils-0.20230707.1702/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-07-07 08:02:09.000000 krutils-0.20230707.1702/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 08:02:12.245315 krutils-0.20230707.1702/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230707.1702/test/test_futils.py
+-rw-rw-rw-   0        0        0      321 2023-06-24 13:23:59.000000 krutils-0.20230707.1702/test/test_logger.py
```

### Comparing `krutils-0.20230624.2235/krutils/CONST.py` & `krutils-0.20230707.1702/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230624.2235/krutils/_dbmgr.py` & `krutils-0.20230707.1702/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230624.2235/krutils/futils.py` & `krutils-0.20230707.1702/krutils/futils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230624.2235/krutils/logger.py` & `krutils-0.20230707.1702/krutils/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         # 파일이 존재하는가
         import os.path
         if (os.path.isfile(config_file_path) != True):
             return None
 
         # 파싱하자
         import json
-        with open(config_file_path) as _cfp:
+        with open(config_file_path, encoding='utf8') as _cfp:
             config_json = json.load(_cfp)
 
         if config_json == None:
             return None
 
         # config 객체 매핑하자
         parsed_config = _logger_config()
```

### Comparing `krutils-0.20230624.2235/krutils/logger2.py` & `krutils-0.20230707.1702/krutils/logger2.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230624.2235/krutils/utils.py` & `krutils-0.20230707.1702/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230624.2235/setup.py` & `krutils-0.20230707.1702/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230624.2235",
+    version="0.20230707.1702",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```


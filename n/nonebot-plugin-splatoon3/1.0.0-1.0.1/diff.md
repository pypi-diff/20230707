# Comparing `tmp/nonebot_plugin_splatoon3-1.0.0.tar.gz` & `tmp/nonebot_plugin_splatoon3-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nonebot_plugin_splatoon3-1.0.0.tar", last modified: Fri Jul  7 11:30:18 2023, max compression
+gzip compressed data, was "dist\nonebot_plugin_splatoon3-1.0.1.tar", last modified: Fri Jul  7 13:00:30 2023, max compression
```

## Comparing `nonebot_plugin_splatoon3-1.0.0.tar` & `nonebot_plugin_splatoon3-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 11:30:18.662140 nonebot_plugin_splatoon3-1.0.0/
--rw-rw-rw-   0        0        0     2078 2023-07-07 11:30:18.661143 nonebot_plugin_splatoon3-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1169 2023-07-07 10:34:04.000000 nonebot_plugin_splatoon3-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 11:30:18.647137 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/
--rw-rw-rw-   0        0        0    10325 2023-07-07 10:38:01.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/__init__.py
--rw-rw-rw-   0        0        0     1453 2023-07-02 05:32:58.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/_class.py
--rw-rw-rw-   0        0        0     1649 2023-07-07 05:55:36.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/admin_matcher.py
--rw-rw-rw-   0        0        0    11344 2023-07-07 05:59:37.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/data_source.py
--rw-rw-rw-   0        0        0     6509 2023-07-07 07:54:51.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/image.py
--rw-rw-rw-   0        0        0    11537 2023-07-05 03:39:05.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/image_db.py
--rw-rw-rw-   0        0        0    31239 2023-07-07 10:44:53.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/image_processer.py
--rw-rw-rw-   0        0        0    23190 2023-07-07 10:10:44.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/image_processer_tools.py
--rw-rw-rw-   0        0        0     5008 2023-07-07 05:21:51.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/static_data_getter.py
--rw-rw-rw-   0        0        0    14605 2023-07-06 05:17:15.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/translation.py
--rw-rw-rw-   0        0        0     1876 2023-07-07 09:22:20.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:30:18.658140 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3.egg-info/
--rw-rw-rw-   0        0        0     2078 2023-07-07 11:30:18.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-07-07 11:30:18.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:30:18.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-07 11:30:18.000000 nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 11:30:18.664140 nonebot_plugin_splatoon3-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3834 2023-07-07 11:17:59.000000 nonebot_plugin_splatoon3-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:00:30.659227 nonebot_plugin_splatoon3-1.0.1/
+-rw-rw-rw-   0        0        0     2078 2023-07-07 13:00:30.659227 nonebot_plugin_splatoon3-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2023-07-07 10:34:04.000000 nonebot_plugin_splatoon3-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 13:00:30.644019 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/
+-rw-rw-rw-   0        0        0    10325 2023-07-07 10:38:01.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/__init__.py
+-rw-rw-rw-   0        0        0     1453 2023-07-02 05:32:58.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/_class.py
+-rw-rw-rw-   0        0        0     1649 2023-07-07 05:55:36.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/admin_matcher.py
+-rw-rw-rw-   0        0        0    11344 2023-07-07 05:59:37.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/data_source.py
+-rw-rw-rw-   0        0        0     6509 2023-07-07 07:54:51.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/image.py
+-rw-rw-rw-   0        0        0    11537 2023-07-05 03:39:05.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/image_db.py
+-rw-rw-rw-   0        0        0    31239 2023-07-07 10:44:53.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/image_processer.py
+-rw-rw-rw-   0        0        0    23190 2023-07-07 10:10:44.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/image_processer_tools.py
+-rw-rw-rw-   0        0        0     5008 2023-07-07 05:21:51.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/static_data_getter.py
+-rw-rw-rw-   0        0        0    14605 2023-07-06 05:17:15.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/translation.py
+-rw-rw-rw-   0        0        0     1876 2023-07-07 09:22:20.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:00:30.656218 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3.egg-info/
+-rw-rw-rw-   0        0        0     2078 2023-07-07 13:00:30.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-07-07 13:00:30.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:00:30.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-07 13:00:30.000000 nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      598 2023-07-07 12:48:04.000000 nonebot_plugin_splatoon3-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:00:30.661239 nonebot_plugin_splatoon3-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3834 2023-07-07 12:59:16.000000 nonebot_plugin_splatoon3-1.0.1/setup.py
```

### Comparing `nonebot_plugin_splatoon3-1.0.0/PKG-INFO` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot_plugin_splatoon3
-Version: 1.0.0
+Name: nonebot-plugin-splatoon3
+Version: 1.0.1
 Summary: 一个基于nonebot2框架的splatoon3游戏日程查询插件
 Home-page: https://github.com/Skyminers/Bot-Splatoon3
 Author: Cypas_Nya
 Author-email: ayano05@outlook.com
 License: MIT
 Description: 
         # Splatoon 3 地图查询插件
```

### Comparing `nonebot_plugin_splatoon3-1.0.0/README.md` & `nonebot_plugin_splatoon3-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/__init__.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/_class.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/_class.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/admin_matcher.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/admin_matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/data_source.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/image.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/image_db.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/image_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/image_processer.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/image_processer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/image_processer_tools.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/image_processer_tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/static_data_getter.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/static_data_getter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/translation.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3/utils.py` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3.egg-info/PKG-INFO` & `nonebot_plugin_splatoon3-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-splatoon3
-Version: 1.0.0
+Name: nonebot_plugin_splatoon3
+Version: 1.0.1
 Summary: 一个基于nonebot2框架的splatoon3游戏日程查询插件
 Home-page: https://github.com/Skyminers/Bot-Splatoon3
 Author: Cypas_Nya
 Author-email: ayano05@outlook.com
 License: MIT
 Description: 
         # Splatoon 3 地图查询插件
```

### Comparing `nonebot_plugin_splatoon3-1.0.0/nonebot_plugin_splatoon3.egg-info/SOURCES.txt` & `nonebot_plugin_splatoon3-1.0.1/nonebot_plugin_splatoon3.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+pyproject.toml
 setup.py
 nonebot_plugin_splatoon3/__init__.py
 nonebot_plugin_splatoon3/_class.py
 nonebot_plugin_splatoon3/admin_matcher.py
 nonebot_plugin_splatoon3/data_source.py
 nonebot_plugin_splatoon3/image.py
 nonebot_plugin_splatoon3/image_db.py
```

### Comparing `nonebot_plugin_splatoon3-1.0.0/setup.py` & `nonebot_plugin_splatoon3-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "nonebot_plugin_splatoon3"
 DESCRIPTION = "一个基于nonebot2框架的splatoon3游戏日程查询插件"
 URL = "https://github.com/Skyminers/Bot-Splatoon3"
 EMAIL = "ayano05@outlook.com"
 AUTHOR = "Cypas_Nya"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```


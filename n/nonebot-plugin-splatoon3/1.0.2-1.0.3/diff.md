# Comparing `tmp/nonebot_plugin_splatoon3-1.0.2.tar.gz` & `tmp/nonebot_plugin_splatoon3-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nonebot_plugin_splatoon3-1.0.2.tar", last modified: Fri Jul  7 13:19:17 2023, max compression
+gzip compressed data, was "dist\nonebot_plugin_splatoon3-1.0.3.tar", last modified: Fri Jul  7 13:46:29 2023, max compression
```

## Comparing `nonebot_plugin_splatoon3-1.0.2.tar` & `nonebot_plugin_splatoon3-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:19:17.561616 nonebot_plugin_splatoon3-1.0.2/
--rw-rw-rw-   0        0        0     2078 2023-07-07 13:19:17.558694 nonebot_plugin_splatoon3-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1169 2023-07-07 10:34:04.000000 nonebot_plugin_splatoon3-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 13:19:17.547680 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/
--rw-rw-rw-   0        0        0    10325 2023-07-07 10:38:01.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/__init__.py
--rw-rw-rw-   0        0        0     1453 2023-07-02 05:32:58.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/_class.py
--rw-rw-rw-   0        0        0     1649 2023-07-07 05:55:36.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/admin_matcher.py
--rw-rw-rw-   0        0        0    11344 2023-07-07 05:59:37.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/data_source.py
--rw-rw-rw-   0        0        0     6509 2023-07-07 07:54:51.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/image.py
--rw-rw-rw-   0        0        0    11537 2023-07-05 03:39:05.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/image_db.py
--rw-rw-rw-   0        0        0    31239 2023-07-07 10:44:53.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/image_processer.py
--rw-rw-rw-   0        0        0    23190 2023-07-07 10:10:44.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/image_processer_tools.py
--rw-rw-rw-   0        0        0     5008 2023-07-07 05:21:51.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/static_data_getter.py
--rw-rw-rw-   0        0        0    14605 2023-07-06 05:17:15.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/translation.py
--rw-rw-rw-   0        0        0     1876 2023-07-07 09:22:20.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 13:19:17.555687 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3.egg-info/
--rw-rw-rw-   0        0        0     2078 2023-07-07 13:19:17.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-07-07 13:19:17.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:19:17.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-07 13:19:17.000000 nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      561 2023-07-07 13:19:11.000000 nonebot_plugin_splatoon3-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 13:19:17.563609 nonebot_plugin_splatoon3-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3834 2023-07-07 13:19:11.000000 nonebot_plugin_splatoon3-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:46:29.154327 nonebot_plugin_splatoon3-1.0.3/
+-rw-rw-rw-   0        0        0     2078 2023-07-07 13:46:29.150005 nonebot_plugin_splatoon3-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2023-07-07 10:34:04.000000 nonebot_plugin_splatoon3-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 13:46:29.139997 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/
+-rw-rw-rw-   0        0        0    10325 2023-07-07 10:38:01.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/__init__.py
+-rw-rw-rw-   0        0        0     1453 2023-07-02 05:32:58.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/_class.py
+-rw-rw-rw-   0        0        0     1649 2023-07-07 05:55:36.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/admin_matcher.py
+-rw-rw-rw-   0        0        0    11344 2023-07-07 05:59:37.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/data_source.py
+-rw-rw-rw-   0        0        0     6509 2023-07-07 07:54:51.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/image.py
+-rw-rw-rw-   0        0        0    11537 2023-07-05 03:39:05.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/image_db.py
+-rw-rw-rw-   0        0        0    31239 2023-07-07 10:44:53.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/image_processer.py
+-rw-rw-rw-   0        0        0    23190 2023-07-07 10:10:44.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/image_processer_tools.py
+-rw-rw-rw-   0        0        0     5008 2023-07-07 05:21:51.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/static_data_getter.py
+-rw-rw-rw-   0        0        0    14605 2023-07-06 05:17:15.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/translation.py
+-rw-rw-rw-   0        0        0     1876 2023-07-07 09:22:20.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:46:29.147010 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3.egg-info/
+-rw-rw-rw-   0        0        0     2078 2023-07-07 13:46:28.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-07-07 13:46:29.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:46:28.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-07 13:46:28.000000 nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      596 2023-07-07 13:46:24.000000 nonebot_plugin_splatoon3-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 13:46:29.156330 nonebot_plugin_splatoon3-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3834 2023-07-07 13:46:24.000000 nonebot_plugin_splatoon3-1.0.3/setup.py
```

### Comparing `nonebot_plugin_splatoon3-1.0.2/PKG-INFO` & `nonebot_plugin_splatoon3-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_splatoon3
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一个基于nonebot2框架的splatoon3游戏日程查询插件
 Home-page: https://github.com/Skyminers/Bot-Splatoon3
 Author: Cypas_Nya
 Author-email: ayano05@outlook.com
 License: MIT
 Description: 
         # Splatoon 3 地图查询插件
```

### Comparing `nonebot_plugin_splatoon3-1.0.2/README.md` & `nonebot_plugin_splatoon3-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/__init__.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/_class.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/_class.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/admin_matcher.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/admin_matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/data_source.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/image.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/image_db.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/image_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/image_processer.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/image_processer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/image_processer_tools.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/image_processer_tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/static_data_getter.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/static_data_getter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/translation.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3/utils.py` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3.egg-info/PKG-INFO` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-splatoon3
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一个基于nonebot2框架的splatoon3游戏日程查询插件
 Home-page: https://github.com/Skyminers/Bot-Splatoon3
 Author: Cypas_Nya
 Author-email: ayano05@outlook.com
 License: MIT
 Description: 
         # Splatoon 3 地图查询插件
```

### Comparing `nonebot_plugin_splatoon3-1.0.2/nonebot_plugin_splatoon3.egg-info/SOURCES.txt` & `nonebot_plugin_splatoon3-1.0.3/nonebot_plugin_splatoon3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_splatoon3-1.0.2/pyproject.toml` & `nonebot_plugin_splatoon3-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-splatoon3"
-version = "1.0.2"
+version = "1.0.3"
 description = "一个基于nonebot2框架的splatoon3游戏日程查询插件"
 authors = ["cypas <ayano05@outlook.com>"]
 readme = "README.md"
 packages = [{include = "nonebot_plugin_splatoon3"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -12,11 +12,12 @@
 cfscrape="^2.1.1"
 httpx="^0.24.1"
 nonebot2="^2.0.0"
 Pillow="9.5.0"
 playwright="^1.35.0"
 urllib3="1.26.16"
 requests="^2.28.2"
+nonebot-adapter-onebot = "^2.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_splatoon3-1.0.2/setup.py` & `nonebot_plugin_splatoon3-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "nonebot_plugin_splatoon3"
 DESCRIPTION = "一个基于nonebot2框架的splatoon3游戏日程查询插件"
 URL = "https://github.com/Skyminers/Bot-Splatoon3"
 EMAIL = "ayano05@outlook.com"
 AUTHOR = "Cypas_Nya"
 REQUIRES_PYTHON = ">=3.8.0"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```


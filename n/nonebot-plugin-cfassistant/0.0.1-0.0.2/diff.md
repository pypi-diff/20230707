# Comparing `tmp/nonebot-plugin-cfassistant-0.0.1.tar.gz` & `tmp/nonebot-plugin-cfassistant-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cfassistant-0.0.1.tar", last modified: Fri Jul  7 13:51:08 2023, max compression
+gzip compressed data, was "nonebot-plugin-cfassistant-0.0.2.tar", last modified: Fri Jul  7 14:00:09 2023, max compression
```

## Comparing `nonebot-plugin-cfassistant-0.0.1.tar` & `nonebot-plugin-cfassistant-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 13:51:08.876385 nonebot-plugin-cfassistant-0.0.1/
--rw-rw-rw-   0        0        0      266 2023-07-07 13:51:08.874385 nonebot-plugin-cfassistant-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 13:51:08.870267 nonebot-plugin-cfassistant-0.0.1/nonebot_plugin_cfassistant.egg-info/
--rw-rw-rw-   0        0        0      266 2023-07-07 13:51:08.000000 nonebot-plugin-cfassistant-0.0.1/nonebot_plugin_cfassistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-07 13:51:08.000000 nonebot-plugin-cfassistant-0.0.1/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:51:08.000000 nonebot-plugin-cfassistant-0.0.1/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-07 13:51:01.000000 nonebot-plugin-cfassistant-0.0.1/nonebot_plugin_cfassistant.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       67 2023-07-07 13:51:08.000000 nonebot-plugin-cfassistant-0.0.1/nonebot_plugin_cfassistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 13:51:08.000000 nonebot-plugin-cfassistant-0.0.1/nonebot_plugin_cfassistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 13:51:08.876385 nonebot-plugin-cfassistant-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-07-07 13:49:39.000000 nonebot-plugin-cfassistant-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:00:09.316328 nonebot-plugin-cfassistant-0.0.2/
+-rw-rw-rw-   0        0        0      266 2023-07-07 14:00:09.315322 nonebot-plugin-cfassistant-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3868 2023-07-07 13:47:44.000000 nonebot-plugin-cfassistant-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 14:00:09.297326 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant/
+-rw-rw-rw-   0        0        0     6509 2023-07-07 13:49:12.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant/__init__.py
+-rw-rw-rw-   0        0        0     2408 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant/changeRemind.py
+-rw-rw-rw-   0        0        0     8738 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant/updateContest.py
+-rw-rw-rw-   0        0        0     5176 2023-07-07 12:22:00.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant/updateUser.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:00:09.312806 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-07-07 14:00:09.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-07-07 14:00:09.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:00:09.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-07 14:00:08.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       67 2023-07-07 14:00:09.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-07 14:00:09.000000 nonebot-plugin-cfassistant-0.0.2/nonebot_plugin_cfassistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:00:09.317334 nonebot-plugin-cfassistant-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      563 2023-07-07 13:59:34.000000 nonebot-plugin-cfassistant-0.0.2/setup.py
```

### Comparing `nonebot-plugin-cfassistant-0.0.1/setup.py` & `nonebot-plugin-cfassistant-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 setup(
     name='nonebot-plugin-cfassistant', 
     version=VERSION,  
     description='一个支持CF(codeforces)平台查询比赛/比赛提醒/监测分数变化的nonebot机器人插件', 
     packages=find_packages(),
     zip_safe=False,
```


# Comparing `tmp/nonebot-plugin-cp-broadcast-0.0.2.tar.gz` & `tmp/nonebot-plugin-cp-broadcast-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cp-broadcast-0.0.2.tar", last modified: Fri Jul  7 05:14:58 2023, max compression
+gzip compressed data, was "nonebot-plugin-cp-broadcast-0.0.3.tar", last modified: Fri Jul  7 05:57:09 2023, max compression
```

## Comparing `nonebot-plugin-cp-broadcast-0.0.2.tar` & `nonebot-plugin-cp-broadcast-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 05:14:58.564758 nonebot-plugin-cp-broadcast-0.0.2/
--rw-rw-rw-   0        0        0     1094 2023-07-07 03:12:10.000000 nonebot-plugin-cp-broadcast-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      682 2023-07-07 05:14:58.564758 nonebot-plugin-cp-broadcast-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-07-07 04:37:17.000000 nonebot-plugin-cp-broadcast-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 05:14:58.557017 nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast/
--rw-rw-rw-   0        0        0    14178 2023-07-07 04:07:24.000000 nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast/__init__.py
--rw-rw-rw-   0        0        0      339 2023-07-07 04:07:32.000000 nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast/config.py
-drwxrwxrwx   0        0        0        0 2023-07-07 05:14:58.563254 nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast.egg-info/
--rw-rw-rw-   0        0        0      682 2023-07-07 05:14:58.000000 nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-07 05:14:58.000000 nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 05:14:58.000000 nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-07 05:14:58.000000 nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 05:14:58.564758 nonebot-plugin-cp-broadcast-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-07-07 05:14:54.000000 nonebot-plugin-cp-broadcast-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:57:09.165636 nonebot-plugin-cp-broadcast-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-07-07 03:12:10.000000 nonebot-plugin-cp-broadcast-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      682 2023-07-07 05:57:09.164637 nonebot-plugin-cp-broadcast-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-07-07 04:37:17.000000 nonebot-plugin-cp-broadcast-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 05:57:09.156257 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast/
+-rw-rw-rw-   0        0        0    14201 2023-07-07 05:32:51.000000 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-07-07 04:07:32.000000 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast/config.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:57:09.163637 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast.egg-info/
+-rw-rw-rw-   0        0        0      682 2023-07-07 05:57:09.000000 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-07-07 05:57:09.000000 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 05:57:09.000000 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-07 05:57:09.000000 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-07 05:57:09.000000 nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 05:57:09.165636 nonebot-plugin-cp-broadcast-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-07-07 05:57:03.000000 nonebot-plugin-cp-broadcast-0.0.3/setup.py
```

### Comparing `nonebot-plugin-cp-broadcast-0.0.2/LICENSE.txt` & `nonebot-plugin-cp-broadcast-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cp-broadcast-0.0.2/PKG-INFO` & `nonebot-plugin-cp-broadcast-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.0.2
+Version: 0.0.3
 Summary: A nonebot plugin package
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 Author: HuParry
 Author-email: huparry@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,17 @@
     usage="cf->查询cf比赛\n"\
         "nc/牛客->查询牛客比赛\n"\
         "atc->查询atcoder比赛\n"\
         "today->查询今天的比赛\n"\
         "next->查询明天之后的部分比赛\n"
         "update->更新比赛数据\n"\
         "about->{botname}的一些信息\n",
+    config=Config,
     extra={
-        "unique_name": "next_game",
+        "unique_name": "cp-broadcast",
         "example": "today",
         "author": "HuParry <huparry@outlook.com>",
         "version": "0.1.5",
     }
 )
```

#### html2text {}

```diff
@@ -12,16 +12,16 @@
 (get_driver().config.dict()).cp_broadcast_updatetime from nonebot.plugin import
 PluginMetadata __plugin_meta__ = PluginMetadata
 ( name="ç®æ³ç«èµæ¯èµæ¥è¯¢",
 description="å¯ä»¥æ¥è¯¢çå®¢ãatcoderãcodeforceså¹³å°çä»å¤©åè¿å å¤©çæ¯èµä¿¡æ¯",
 usage="cf->æ¥è¯¢cfæ¯èµ\n"\ "nc/çå®¢->æ¥è¯¢çå®¢æ¯èµ\n"\ "atc-
 >æ¥è¯¢atcoderæ¯èµ\n"\ "today->æ¥è¯¢ä»å¤©çæ¯èµ\n"\ "next-
 >æ¥è¯¢æå¤©ä¹åçé¨åæ¯èµ\n" "update->æ´æ°æ¯èµæ°æ®\n"\ "about->
-{botname}çä¸äºä¿¡æ¯\n", extra={ "unique_name": "next_game", "example":
-"today", "author": "HuParry
+{botname}çä¸äºä¿¡æ¯\n", config=Config, extra={ "unique_name": "cp-
+broadcast", "example": "today", "author": "HuParry
 outlook.com>", "version": "0.1.5", } ) try: scheduler = require
 ("nonebot_plugin_apscheduler").scheduler except BaseException: scheduler = None
 headers = { 'user-agent': FakeUserAgent().random }
 ###åè¡¨ä¸æ 0ä¸ºæ¯èµåç§°ãä¸æ 1ä¸ºæ¯èµæ¶é´ãä¸æ 2ä¸ºæ¯èµé¾æ¥
 cf = [] atc = [] nc = [] async def get_data_cf() -> bool: global cf url =
 'https://codeforces.com/api/contest.list?gym=false' num = 0
 #å°è¯è·åçæ¬¡æ°ï¼æå¤å°è¯ä¸æ¬¡ while num < 3 : try: if(len(cf) >
```

### Comparing `nonebot-plugin-cp-broadcast-0.0.2/nonebot_plugin_cp_broadcast.egg-info/PKG-INFO` & `nonebot-plugin-cp-broadcast-0.0.3/nonebot_plugin_cp_broadcast.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.0.2
+Version: 0.0.3
 Summary: A nonebot plugin package
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 Author: HuParry
 Author-email: huparry@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-cp-broadcast-0.0.2/setup.py` & `nonebot-plugin-cp-broadcast-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import setuptools #导入setuptools打包工具
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="nonebot-plugin-cp-broadcast", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.2",    #包版本号，便于维护版本
+    version="0.0.3",    #包版本号，便于维护版本
     author="HuParry",    #作者，可以写自己的姓名
     author_email="huparry@outlook.com",    #作者联系方式，可写自己的邮箱地址
     description="A nonebot plugin package",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/HuParry/nonebot-plugin-cp-broadcast",    #自己项目地址，比如github的项目地址
+    install_requires=[
+        'httpx',
+        'nonebot',
+        'fake_useragent',
+        'bs4',
+        'asyncio',
+        'datetime',
+        're'
+    ],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',    #对python的最低版本要求
```


# Comparing `tmp/nonebot_plugin_cp_broadcast-0.1.4.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-0.1.4.tar` & `nonebot_plugin_cp_broadcast-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-07-07 08:19:16.911194 nonebot_plugin_cp_broadcast-0.1.4/LICENSE
--rw-r--r--   0        0        0     3852 2023-07-07 08:19:16.915195 nonebot_plugin_cp_broadcast-0.1.4/README.md
--rw-r--r--   0        0        0    13953 2023-07-07 08:19:16.915195 nonebot_plugin_cp_broadcast-0.1.4/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0      332 2023-07-07 08:19:16.915195 nonebot_plugin_cp_broadcast-0.1.4/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0      625 2023-07-07 08:19:16.915195 nonebot_plugin_cp_broadcast-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3852 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/README.md
+-rw-r--r--   0        0        0    13953 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0      332 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0      590 2023-07-07 08:54:45.194905 nonebot_plugin_cp_broadcast-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-0.1.4/LICENSE` & `nonebot_plugin_cp_broadcast-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.1.4/README.md` & `nonebot_plugin_cp_broadcast-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.1.4/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-0.1.5/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.1.4/PKG-INFO` & `nonebot_plugin_cp_broadcast-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.1.4
-Summary: A nonebot plugin
+Version: 0.1.5
+Summary: A nonebot plugin package
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.1.4 Summary:
-A nonebot plugin License: MIT Author: HuParry Author-email: huparry@outlook.com
-Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio (>=3.4.3,<4.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: fake-useragent (>=1.1.3,<2.0.0) Requires-Dist: httpx
-(>=0.20.0,<1.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.1.5 Summary:
+A nonebot plugin package License: MIT Author: HuParry Author-email:
+huparry@outlook.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: asyncio (>=3.4.3,<4.0.0) Requires-
+Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
+Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-cp-broadcast _â¨ ä¸ä¸ª Codeforcesãçå®¢ç«èµãAtCoder
 å¹³å°çç¼ç¨ç«èµæ¥è¯¢æä»¶ï¼ACMerå¿å¤ â¨_ [license] [pypi] [python]
 ## ð ä»ç» å¯¹äºæ¯ä¸ä¸ª ACMer
```


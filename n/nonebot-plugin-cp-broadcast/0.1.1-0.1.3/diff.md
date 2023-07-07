# Comparing `tmp/nonebot_plugin_cp_broadcast-0.1.1.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-0.1.1.tar` & `nonebot_plugin_cp_broadcast-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-07-07 07:43:53.664999 nonebot_plugin_cp_broadcast-0.1.1/LICENSE
--rw-r--r--   0        0        0     3852 2023-07-07 07:43:53.664999 nonebot_plugin_cp_broadcast-0.1.1/README.md
--rw-r--r--   0        0        0    13953 2023-07-07 07:43:53.668999 nonebot_plugin_cp_broadcast-0.1.1/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0      332 2023-07-07 07:43:53.668999 nonebot_plugin_cp_broadcast-0.1.1/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0      485 2023-07-07 07:43:53.668999 nonebot_plugin_cp_broadcast-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-07 08:04:00.159662 nonebot_plugin_cp_broadcast-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3852 2023-07-07 08:04:00.159662 nonebot_plugin_cp_broadcast-0.1.3/README.md
+-rw-r--r--   0        0        0    13953 2023-07-07 08:04:00.163662 nonebot_plugin_cp_broadcast-0.1.3/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0      332 2023-07-07 08:04:00.163662 nonebot_plugin_cp_broadcast-0.1.3/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0      549 2023-07-07 08:04:00.163662 nonebot_plugin_cp_broadcast-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-0.1.1/LICENSE` & `nonebot_plugin_cp_broadcast-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.1.1/README.md` & `nonebot_plugin_cp_broadcast-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.1.1/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-0.1.3/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.1.1/PKG-INFO` & `nonebot_plugin_cp_broadcast-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.1.1
+Version: 0.1.3
 Summary: A nonebot plugin
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: DateTime (>=5.1,<6.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: httpx (>=0.20.0,<1.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.1.3 Summary:
 A nonebot plugin License: MIT Author: HuParry Author-email: huparry@outlook.com
 Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: DateTime (>=5.1,<6.0) Requires-Dist: asyncio (>=3.4.3,<4.0.0)
-Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist: fake-useragent
-(>=1.1.3,<2.0.0) Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist:
-nonebot2 (>=2.0.0,<3.0.0) Description-Content-Type: text/markdown
+Requires-Dist: asyncio (>=3.4.3,<4.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: fake-useragent (>=1.1.3,<2.0.0) Requires-Dist: httpx
+(>=0.20.0,<1.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Description-Content-Type:
+text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-cp-broadcast _â¨ ä¸ä¸ª Codeforcesãçå®¢ç«èµãAtCoder
 å¹³å°çç¼ç¨ç«èµæ¥è¯¢æä»¶ï¼ACMerå¿å¤ â¨_ [license] [pypi] [python]
 ## ð ä»ç» å¯¹äºæ¯ä¸ä¸ª ACMer
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
```


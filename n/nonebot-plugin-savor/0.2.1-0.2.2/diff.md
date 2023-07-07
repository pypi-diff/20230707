# Comparing `tmp/nonebot-plugin-savor-0.2.1.tar.gz` & `tmp/nonebot-plugin-savor-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-savor-0.2.1.tar", last modified: Tue Nov  1 07:04:30 2022, max compression
+gzip compressed data, was "nonebot-plugin-savor-0.2.2.tar", last modified: Fri Jul  7 18:19:12 2023, max compression
```

## Comparing `nonebot-plugin-savor-0.2.1.tar` & `nonebot-plugin-savor-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-11-01 07:04:22.713541 nonebot-plugin-savor-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-01 07:04:22.713541 nonebot-plugin-savor-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-11-01 07:04:22.713541 nonebot-plugin-savor-0.2.1/nonebot_plugin_savor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-11-01 07:04:22.713541 nonebot-plugin-savor-0.2.1/nonebot_plugin_savor/savor.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-11-01 07:04:22.713541 nonebot-plugin-savor-0.2.1/pyproject.toml
--rw-------   0 runner    (1001) docker     (121)     2421 2022-11-01 07:04:30.085563 nonebot-plugin-savor-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-07 18:19:02.945081 nonebot-plugin-savor-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2054 2023-07-07 18:19:02.945081 nonebot-plugin-savor-0.2.2/README.md
+-rw-r--r--   0        0        0     1415 2023-07-07 18:19:02.945081 nonebot-plugin-savor-0.2.2/nonebot_plugin_savor/__init__.py
+-rw-r--r--   0        0        0     1773 2023-07-07 18:19:02.949081 nonebot-plugin-savor-0.2.2/nonebot_plugin_savor/savor.py
+-rw-r--r--   0        0        0      650 2023-07-07 18:19:02.949081 nonebot-plugin-savor-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 nonebot-plugin-savor-0.2.2/PKG-INFO
```

### Comparing `nonebot-plugin-savor-0.2.1/LICENSE` & `nonebot-plugin-savor-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-savor-0.2.1/README.md` & `nonebot-plugin-savor-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,12 +69,12 @@
 
 </details>
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| 鉴赏/分析 + 图片 | 否 | 群聊/私聊 | 分析发送的图片, 支持回复图片 |
+| 鉴赏图片/分析图片 + 图片 | 否 | 群聊/私聊 | 分析发送的图片, 支持回复图片 |
 
 **注意**
 
 默认情况下, 您应该在指令前加上命令前缀, 通常是 /
```

#### html2text {}

```diff
@@ -8,11 +8,11 @@
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-savor
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-savor   pdm pdm add nonebot-plugin-savor
 poetry poetry add nonebot-plugin-savor   conda conda install nonebot-plugin-
 savor  æå¼ nonebot2 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥
 nonebot.load_plugin('nonebot_plugin_savor')  ## ð ä½¿ç¨ ### æä»¤è¡¨ |
-æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| | é´èµ/
-åæ + å¾ç | å¦ | ç¾¤è/ç§è | åæåéçå¾ç,
-æ¯æåå¤å¾ç | **æ³¨æ** é»è®¤æåµä¸,
+æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+é´èµå¾ç/åæå¾ç + å¾ç | å¦ | ç¾¤è/ç§è |
+åæåéçå¾ç, æ¯æåå¤å¾ç | **æ³¨æ** é»è®¤æåµä¸,
 æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ /
```

### Comparing `nonebot-plugin-savor-0.2.1/nonebot_plugin_savor/__init__.py` & `nonebot-plugin-savor-0.2.2/nonebot_plugin_savor/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import Arg
 from nonebot.typing import T_State
 
 from .savor import savor_image
 
-analysis = on_command("鉴赏", aliases={"分析", "解析"})
+analysis = on_command("鉴赏图片", aliases={"分析图片", "解析图片"}, block=True)
 
 
 @analysis.handle()
 async def image_analysis(event: MessageEvent, matcher: Matcher):
     message = reply.message if (reply := event.reply) else event.message
     if imgs := message["image"]:
         matcher.set_arg("imgs", imgs)
 
 
 @analysis.got("imgs", prompt="请发送需要分析的图片")
 async def get_image(state: T_State, imgs: Message = Arg()):
     urls = extract_image_urls(imgs)
     if not urls:
-        await analysis.reject("没有找到图片, 请重新发送")
+        await analysis.finish("没有找到图片, 分析结束")
     state["urls"] = urls
 
 
 @analysis.handle()
 async def analysis_handle(state: T_State):
     await analysis.send("正在分析图像, 请稍等……")
     try:
         result = await savor_image(state["urls"][0])
     except Exception as e:
         logger.opt(exception=e).error("分析图像失败")
         await analysis.finish("分析失败, 请稍后重试", reply_message=True)
     msg = ", ".join(i["label"] for i in result if not i["label"].startswith("rating:"))
-    await analysis.finish(f"分析结果如下:\n{msg}", reply_message=True)
+    await analysis.finish(msg, reply_message=True)
```

### Comparing `nonebot-plugin-savor-0.2.1/pyproject.toml` & `nonebot-plugin-savor-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "nonebot-plugin-savor"
-version = "0.2.1"
+version = "0.2.2"
 description = "NoneBot2 plugin for image analysis"
 authors = [
     { name = "Akirami", email = "Akiramiaya@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc1",
     "nonebot-adapter-onebot>=2.1.3",
     "httpx>=0.23.0",
     "Pillow<10.0.0,>=9.2.0",
+    "websockets>=10.4",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot-plugin-savor-0.2.1/PKG-INFO` & `nonebot-plugin-savor-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-savor
-Version: 0.2.1
+Version: 0.2.2
 Summary: NoneBot2 plugin for image analysis
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/A-kirami/nonebot-plugin-savor
 Project-URL: Repository, https://github.com/A-kirami/nonebot-plugin-savor
 Description-Content-Type: text/markdown
@@ -80,12 +80,12 @@
 
 </details>
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| 鉴赏/分析 + 图片 | 否 | 群聊/私聊 | 分析发送的图片, 支持回复图片 |
+| 鉴赏图片/分析图片 + 图片 | 否 | 群聊/私聊 | 分析发送的图片, 支持回复图片 |
 
 **注意**
 
 默认情况下, 您应该在指令前加上命令前缀, 通常是 /
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-savor Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-savor Version: 0.2.2 Summary:
 NoneBot2 plugin for image analysis License: MIT Author-email: Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 A-kirami/nonebot-plugin-savor Project-URL: Repository, https://github.com/A-
 kirami/nonebot-plugin-savor Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # nonebot-plugin-savor _â¨ äºæ¬¡åå¾ååæ â¨_ [license] [pypi]
@@ -13,11 +13,11 @@
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-savor
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-savor   pdm pdm add nonebot-plugin-savor
 poetry poetry add nonebot-plugin-savor   conda conda install nonebot-plugin-
 savor  æå¼ nonebot2 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥
 nonebot.load_plugin('nonebot_plugin_savor')  ## ð ä½¿ç¨ ### æä»¤è¡¨ |
-æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| | é´èµ/
-åæ + å¾ç | å¦ | ç¾¤è/ç§è | åæåéçå¾ç,
-æ¯æåå¤å¾ç | **æ³¨æ** é»è®¤æåµä¸,
+æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+é´èµå¾ç/åæå¾ç + å¾ç | å¦ | ç¾¤è/ç§è |
+åæåéçå¾ç, æ¯æåå¤å¾ç | **æ³¨æ** é»è®¤æåµä¸,
 æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ /
```


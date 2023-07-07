# Comparing `tmp/ailingbot-0.0.7.tar.gz` & `tmp/ailingbot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailingbot-0.0.7.tar", max compression
+gzip compressed data, was "ailingbot-0.0.8.tar", max compression
```

## Comparing `ailingbot-0.0.7.tar` & `ailingbot-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.7/LICENSE
--rw-r--r--   0        0        0    30572 2023-07-05 05:45:21.083788 ailingbot-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.7/ailingbot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.7/ailingbot/channels/__init__.py
--rw-r--r--   0        0        0     3343 2023-06-30 08:53:14.045465 ailingbot-0.0.7/ailingbot/channels/channel.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.7/ailingbot/channels/dingtalk/__init__.py
--rw-r--r--   0        0        0     6335 2023-06-29 07:16:47.029744 ailingbot-0.0.7/ailingbot/channels/dingtalk/agent.py
--rw-r--r--   0        0        0      758 2023-07-03 06:42:19.271831 ailingbot-0.0.7/ailingbot/channels/dingtalk/render.py
--rw-r--r--   0        0        0     4273 2023-06-29 07:16:46.998937 ailingbot-0.0.7/ailingbot/channels/dingtalk/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.7/ailingbot/channels/feishu/__init__.py
--rw-r--r--   0        0        0     5760 2023-06-29 04:10:57.580967 ailingbot-0.0.7/ailingbot/channels/feishu/agent.py
--rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.7/ailingbot/channels/feishu/render.py
--rw-r--r--   0        0        0     7052 2023-06-29 04:26:54.855074 ailingbot-0.0.7/ailingbot/channels/feishu/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.7/ailingbot/channels/slack/__init__.py
--rw-r--r--   0        0        0     2447 2023-06-30 09:13:29.198690 ailingbot-0.0.7/ailingbot/channels/slack/agent.py
--rw-r--r--   0        0        0     4291 2023-07-03 06:42:26.641074 ailingbot-0.0.7/ailingbot/channels/slack/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.7/ailingbot/channels/wechatwork/__init__.py
--rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.7/ailingbot/channels/wechatwork/agent.py
--rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.7/ailingbot/channels/wechatwork/encrypt.py
--rw-r--r--   0        0        0     1251 2023-07-03 06:41:46.703144 ailingbot-0.0.7/ailingbot/channels/wechatwork/render.py
--rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.7/ailingbot/channels/wechatwork/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.7/ailingbot/chat/__init__.py
--rw-r--r--   0        0        0     2067 2023-06-29 05:19:20.215510 ailingbot-0.0.7/ailingbot/chat/chatbot.py
--rw-r--r--   0        0        0     2318 2023-07-03 06:37:54.116046 ailingbot-0.0.7/ailingbot/chat/messages.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.7/ailingbot/chat/policies/__init__.py
--rw-r--r--   0        0        0     2147 2023-07-05 04:01:50.888063 ailingbot-0.0.7/ailingbot/chat/policies/conversation.py
--rw-r--r--   0        0        0     3502 2023-07-05 04:01:50.889513 ailingbot-0.0.7/ailingbot/chat/policies/document_qa.py
--rw-r--r--   0        0        0     1669 2023-07-05 04:01:50.890389 ailingbot-0.0.7/ailingbot/chat/policy.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.7/ailingbot/cli/__init__.py
--rw-r--r--   0        0        0     8827 2023-07-05 04:01:50.891165 ailingbot-0.0.7/ailingbot/cli/cli.py
--rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.7/ailingbot/cli/options.py
--rw-r--r--   0        0        0     4051 2023-07-03 06:42:26.636556 ailingbot-0.0.7/ailingbot/cli/render.py
--rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.7/ailingbot/config.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.7/ailingbot/endpoint/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.7/ailingbot/shared/__init__.py
--rw-r--r--   0        0        0     3953 2023-06-27 05:30:31.536603 ailingbot-0.0.7/ailingbot/shared/abc.py
--rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.7/ailingbot/shared/errors.py
--rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.7/ailingbot/shared/misc.py
--rw-r--r--   0        0        0     1115 2023-07-05 05:59:13.000686 ailingbot-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    32140 1970-01-01 00:00:00.000000 ailingbot-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.8/LICENSE
+-rw-r--r--   0        0        0    34967 2023-07-07 08:36:42.584754 ailingbot-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.8/ailingbot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.8/ailingbot/channels/__init__.py
+-rw-r--r--   0        0        0     3343 2023-06-30 08:53:14.045465 ailingbot-0.0.8/ailingbot/channels/channel.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.8/ailingbot/channels/dingtalk/__init__.py
+-rw-r--r--   0        0        0     6335 2023-06-29 07:16:47.029744 ailingbot-0.0.8/ailingbot/channels/dingtalk/agent.py
+-rw-r--r--   0        0        0      758 2023-07-03 06:42:19.271831 ailingbot-0.0.8/ailingbot/channels/dingtalk/render.py
+-rw-r--r--   0        0        0     4273 2023-06-29 07:16:46.998937 ailingbot-0.0.8/ailingbot/channels/dingtalk/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.8/ailingbot/channels/feishu/__init__.py
+-rw-r--r--   0        0        0     5760 2023-06-29 04:10:57.580967 ailingbot-0.0.8/ailingbot/channels/feishu/agent.py
+-rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.8/ailingbot/channels/feishu/render.py
+-rw-r--r--   0        0        0     7052 2023-06-29 04:26:54.855074 ailingbot-0.0.8/ailingbot/channels/feishu/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.8/ailingbot/channels/slack/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-30 09:13:29.198690 ailingbot-0.0.8/ailingbot/channels/slack/agent.py
+-rw-r--r--   0        0        0     4291 2023-07-03 06:42:26.641074 ailingbot-0.0.8/ailingbot/channels/slack/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.8/ailingbot/channels/wechatwork/__init__.py
+-rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.8/ailingbot/channels/wechatwork/agent.py
+-rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.8/ailingbot/channels/wechatwork/encrypt.py
+-rw-r--r--   0        0        0     1251 2023-07-03 06:41:46.703144 ailingbot-0.0.8/ailingbot/channels/wechatwork/render.py
+-rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.8/ailingbot/channels/wechatwork/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.8/ailingbot/chat/__init__.py
+-rw-r--r--   0        0        0     2067 2023-07-07 06:28:24.691934 ailingbot-0.0.8/ailingbot/chat/chatbot.py
+-rw-r--r--   0        0        0     2318 2023-07-03 06:37:54.116046 ailingbot-0.0.8/ailingbot/chat/messages.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.8/ailingbot/chat/policies/__init__.py
+-rw-r--r--   0        0        0     2147 2023-07-05 04:01:50.888063 ailingbot-0.0.8/ailingbot/chat/policies/conversation.py
+-rw-r--r--   0        0        0     3502 2023-07-05 04:01:50.889513 ailingbot-0.0.8/ailingbot/chat/policies/document_qa.py
+-rw-r--r--   0        0        0     1669 2023-07-05 04:01:50.890389 ailingbot-0.0.8/ailingbot/chat/policy.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.8/ailingbot/cli/__init__.py
+-rw-r--r--   0        0        0     9259 2023-07-07 08:11:26.508013 ailingbot-0.0.8/ailingbot/cli/cli.py
+-rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.8/ailingbot/cli/options.py
+-rw-r--r--   0        0        0     4051 2023-07-03 06:42:26.636556 ailingbot-0.0.8/ailingbot/cli/render.py
+-rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.8/ailingbot/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.8/ailingbot/endpoint/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-07 07:41:03.634382 ailingbot-0.0.8/ailingbot/endpoint/model.py
+-rw-r--r--   0        0        0     4522 2023-07-07 08:10:47.681227 ailingbot-0.0.8/ailingbot/endpoint/server.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.8/ailingbot/shared/__init__.py
+-rw-r--r--   0        0        0     3953 2023-07-07 04:02:04.496159 ailingbot-0.0.8/ailingbot/shared/abc.py
+-rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.8/ailingbot/shared/errors.py
+-rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.8/ailingbot/shared/misc.py
+-rw-r--r--   0        0        0     1115 2023-07-07 08:36:53.301342 ailingbot-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    36535 1970-01-01 00:00:00.000000 ailingbot-0.0.8/PKG-INFO
```

### Comparing `ailingbot-0.0.7/LICENSE` & `ailingbot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/channel.py` & `ailingbot-0.0.8/ailingbot/channels/channel.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/dingtalk/agent.py` & `ailingbot-0.0.8/ailingbot/channels/dingtalk/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/dingtalk/render.py` & `ailingbot-0.0.8/ailingbot/channels/dingtalk/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/dingtalk/webhook.py` & `ailingbot-0.0.8/ailingbot/channels/dingtalk/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/feishu/agent.py` & `ailingbot-0.0.8/ailingbot/channels/feishu/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/feishu/render.py` & `ailingbot-0.0.8/ailingbot/channels/feishu/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/feishu/webhook.py` & `ailingbot-0.0.8/ailingbot/channels/feishu/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/slack/agent.py` & `ailingbot-0.0.8/ailingbot/channels/slack/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/slack/webhook.py` & `ailingbot-0.0.8/ailingbot/channels/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/wechatwork/agent.py` & `ailingbot-0.0.8/ailingbot/channels/wechatwork/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/wechatwork/encrypt.py` & `ailingbot-0.0.8/ailingbot/channels/wechatwork/encrypt.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/wechatwork/render.py` & `ailingbot-0.0.8/ailingbot/channels/wechatwork/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/channels/wechatwork/webhook.py` & `ailingbot-0.0.8/ailingbot/channels/wechatwork/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/chat/chatbot.py` & `ailingbot-0.0.8/ailingbot/chat/chatbot.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/chat/messages.py` & `ailingbot-0.0.8/ailingbot/chat/messages.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/chat/policies/conversation.py` & `ailingbot-0.0.8/ailingbot/chat/policies/conversation.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/chat/policies/document_qa.py` & `ailingbot-0.0.8/ailingbot/chat/policies/document_qa.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/chat/policy.py` & `ailingbot-0.0.8/ailingbot/chat/policy.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/cli/cli.py` & `ailingbot-0.0.8/ailingbot/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import uvicorn
 from loguru import logger
 from prompt_toolkit import PromptSession
 from prompt_toolkit.formatted_text import FormattedText
 from rich.console import Console
 
 import ailingbot.shared.errors
+from ailingbot import endpoint
 from ailingbot.channels.channel import ChannelWebhookFactory
 from ailingbot.chat.chatbot import ChatBot
 from ailingbot.chat.messages import (
     TextRequestMessage,
     FallbackResponseMessage,
     MessageScope,
 )
@@ -318,9 +319,26 @@
         click.style(
             text=f'Configuration file {file_path} has been created.',
             fg='green',
         )
     )
 
 
+@command_line_tools.command(name='api', help='Run endpoint server.')
+@options.log_level_option
+@options.log_file_option
+@_coro_cmd
+async def serve(
+    log_level: str,
+    log_file: str,
+):
+    _set_logger(sink=log_file, level=log_level)
+
+    config = uvicorn.Config(
+        app='ailingbot.endpoint.server:app', **settings.uvicorn
+    )
+    server = uvicorn.Server(config)
+    await server.serve()
+
+
 if __name__ == '__main__':
     command_line_tools(prog_name='ailingbot')
```

### Comparing `ailingbot-0.0.7/ailingbot/cli/options.py` & `ailingbot-0.0.8/ailingbot/cli/options.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/cli/render.py` & `ailingbot-0.0.8/ailingbot/cli/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/config.py` & `ailingbot-0.0.8/ailingbot/config.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/shared/abc.py` & `ailingbot-0.0.8/ailingbot/shared/abc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/shared/errors.py` & `ailingbot-0.0.8/ailingbot/shared/errors.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/ailingbot/shared/misc.py` & `ailingbot-0.0.8/ailingbot/shared/misc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.7/pyproject.toml` & `ailingbot-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ailingbot"
-version = "0.0.7"
+version = "0.0.8"
 description = "An all-in-one solution to empower your IM bot with AI."
 authors = ["ericzhang-cn <ericzhang.buaa@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `ailingbot-0.0.7/PKG-INFO` & `ailingbot-0.0.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailingbot
-Version: 0.0.7
+Version: 0.0.8
 Summary: An all-in-one solution to empower your IM bot with AI.
 License: MIT
 Author: ericzhang-cn
 Author-email: ericzhang.buaa@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,786 +34,819 @@
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Requires-Dist: uvicorn (>=0.19.0,<0.20.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
-🇨🇳[简体中文](https://github.com/ericzhang-cn/ailingbot/blob/main/README.md)
-🇬🇧[English](https://github.com/ericzhang-cn/ailingbot/blob/main/README_en.md)
+🇬🇧[English](https://github.com/ericzhang-cn/ailingbot/blob/main/README.md)
+🇨🇳[简体中文](https://github.com/ericzhang-cn/ailingbot/blob/main/README_zh_CN.md)
 
 ---
 
 ![Python package workflow](https://github.com/ericzhang-cn/ailingbot/actions/workflows/python-package.yml/badge.svg)
 ![Pylint workflow](https://github.com/ericzhang-cn/ailingbot/actions/workflows/pylint.yml/badge.svg)
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/logo.png" alt="AilingBot" width="300">
 </p>
 
-<p align="center"><b>AilingBot - 一站式解决方案，为你的IM机器人接入AI强大能力。</b></p>
+<p align="center"><b>AilingBot - One-stop solution to empower your IM bot with AI.</b></p>
 
-# 目录
+# Table of Contents
 
-* [AilingBot是什么](#ailingbot是什么)
-* [特点](#特点)
-* [<g-emoji class="g-emoji" alias="rocket" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f680.png">🚀</g-emoji>快速开始](#快速开始)
-    * [5分钟启动一个AI聊天机器人](#5分钟启动一个ai聊天机器人)
-        * [通过Docker](#通过docker)
-        * [通过PIP](#通过pip)
-            * [安装](#安装)
-            * [生成配置文件](#生成配置文件)
-            * [启动机器人](#启动机器人)
-    * [接入企业微信](#接入企业微信)
-        * [通过Docker](#通过docker-1)
-        * [通过PIP](#通过pip-1)
-            * [安装](#安装-1)
-            * [生成配置文件](#生成配置文件-1)
-            * [修改配置文件](#修改配置文件)
-            * [启动服务](#启动服务)
-    * [接入飞书](#接入飞书)
-        * [通过Docker](#通过docker-2)
-        * [通过PIP](#通过pip-2)
-            * [安装](#安装-2)
-            * [生成配置文件](#生成配置文件-2)
-            * [修改配置文件](#修改配置文件-1)
-            * [启动服务](#启动服务-1)
-    * [接入钉钉](#接入钉钉)
-        * [通过Docker](#通过docker-3)
-        * [通过PIP](#通过pip-3)
-            * [安装](#安装-3)
-            * [生成配置文件](#生成配置文件-3)
-            * [修改配置文件](#修改配置文件-2)
-            * [启动服务](#启动服务-2)
-    * [接入Slack](#接入slack)
-        * [通过Docker](#通过docker-4)
-        * [通过PIP](#通过pip-4)
-            * [安装](#安装-4)
-            * [生成配置文件](#生成配置文件-4)
-            * [修改配置文件](#修改配置文件-3)
-            * [启动服务](#启动服务-3)
-* [<g-emoji class="g-emoji" alias="book" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4d6.png">📖</g-emoji>使用指南](#使用指南)
-    * [主要流程](#主要流程)
-    * [主要概念](#主要概念)
-    * [配置](#配置)
-        * [配置方式](#配置方式)
-        * [配置映射关系](#配置映射关系)
-        * [配置项](#配置项)
-            * [通用](#通用)
-            * [内置会话策略配置](#内置会话策略配置)
+* [What is AilingBot](#what-is-ailingbot)
+* [Features](#features)
+* [Quick Start](#-quick-start)
+    * [Start an AI chatbot in 5 minutes](#start-an-ai-chatbot-in-5-minutes)
+        * [Using Docker](#using-docker)
+        * [Using PIP](#using-pip)
+            * [Installation](#installation)
+            * [Generate Configuration File](#generate-configuration-file)
+            * [Start the Chatbot](#start-the-chatbot)
+    * [Start API Service](#start-api-service)
+        * [Using Docker](#using-docker-1)
+        * [Using PIP](#using-pip-1)
+            * [Installation](#installation-1)
+            * [Generate Configuration File](#generate-configuration-file-1)
+            * [Start the Service](#start-the-service)
+    * [Integrating with WeChat Work](#integrating-with-wechat-work)
+        * [Using Docker](#using-docker-2)
+        * [Using PIP](#using-pip-2)
+            * [Installation](#installation-2)
+            * [Generate Configuration File](#generate-configuration-file-2)
+            * [Modify Configuration File](#modify-configuration-file)
+            * [Start the Service](#start-the-service-1)
+    * [Integrating with Feishu](#integrating-with-feishu)
+        * [Using Docker](#using-docker-3)
+        * [Using PIP](#using-pip-3)
+            * [Installation](#installation-3)
+            * [Generate Configuration File](#generate-configuration-file-3)
+            * [Modify Configuration File](#modify-configuration-file-1)
+            * [Start the Service](#start-the-service-2)
+    * [Integrating with DingTalk](#integrating-with-dingtalk)
+        * [Using Docker](#using-docker-4)
+        * [Using PIP](#using-pip-4)
+            * [Installation](#installation-4)
+            * [Generate Configuration File](#generate-configuration-file-4)
+            * [Modify Configuration File](#modify-configuration-file-2)
+            * [Start the Service](#start-the-service-3)
+    * [Integrating with Slack](#integrating-with-slack)
+        * [Using Docker](#using-docker-5)
+        * [Using PIP](#using-pip-5)
+            * [Installation](#installation-5)
+            * [Generate Configuration File](#generate-configuration-file-5)
+            * [Modify Configuration File](#modify-configuration-file-3)
+            * [Start the Service](#start-the-service-4)
+* [<g-emoji class="g-emoji" alias="book" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4d6.png">📖</g-emoji>User Guide](#user-guide)
+    * [Main Process](#main-process)
+    * [Main Concepts](#main-concepts)
+    * [Configuration](#configuration)
+        * [Configuration Methods](#configuration-methods)
+        * [Configuration Mapping](#configuration-mapping)
+        * [Configuration Items](#configuration-items)
+            * [General](#general)
+            * [Built-in Policy Configuration](#built-in-policy-configuration)
                 * [conversation](#conversation)
                 * [document_qa](#document_qa)
-            * [模型配置](#模型配置)
+            * [Model Configuration](#model-configuration)
                 * [OpenAI](#openai)
-            * [内置Channel配置](#内置channel配置)
-                * [企业微信](#企业微信)
-                * [飞书](#飞书)
-                * [钉钉](#钉钉)
-                * [Slack](#slack)
-    * [命令行工具](#命令行工具)
-        * [初始化配置文件（init）](#初始化配置文件init)
-            * [使用方法](#使用方法)
+    * [Command Line Tools](#command-line-tools)
+        * [Initialize Configuration File (init)](#initialize-configuration-file-init)
+            * [Usage](#usage)
             * [Options](#options)
-        * [查看当前配置（config）](#查看当前配置config)
-            * [使用方法](#使用方法-1)
+        * [View Current Configuration (config)](#view-current-configuration-config)
+            * [Usage](#usage-1)
             * [Options](#options-1)
-        * [启动命令行机器人（chat）](#启动命令行机器人chat)
-            * [使用方法](#使用方法-2)
+        * [Start Command Line Bot (chat)](#start-command-line-bot-chat)
+            * [Usage](#usage-2)
             * [Options](#options-2)
-        * [启动Webhook服务（serve）](#启动webhook服务serve)
-            * [使用方法](#使用方法-3)
+        * [Start Webhook Service (serve)](#start-webhook-service-serve)
+            * [Usage](#usage-3)
             * [Options](#options-3)
-* [💻开发指南](#开发指南)
-    * [开发总则](#开发总则)
-    * [开发对话策略](#开发对话策略)
-    * [开发Channel](#开发channel)
-* [<g-emoji class="g-emoji" alias="thinking" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f914.png">🤔</g-emoji>常见问题](#常见问题)
-* [🎯发展计划](#发展计划)
+        * [Start API Service (api)](#start-api-service-api)
+            * [Usage](#usage-4)
+            * [Options](#options-4)
+    * [<g-emoji class="g-emoji" alias="electric_plug" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f50c.png">🔌</g-emoji>API](#api)
+* [<g-emoji class="g-emoji" alias="computer" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f4bb.png">💻</g-emoji>Development Guide](#development-guide)
+    * [Development Guidelines](#development-guidelines)
+    * [Developing Chat Policy](#developing-chat-policy)
+    * [Developing Channel](#developing-channel)
+* [<g-emoji class="g-emoji" alias="thinking" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f914.png">🤔</g-emoji>Frequently Asked Questions](#frequently-asked-questions)
+* [<g-emoji class="g-emoji" alias="dart" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f3af.png">🎯</g-emoji>Roadmap](#roadmap)
+
+# What is AilingBot
+
+AilingBot is an open-source engineering development framework and an all-in-one solution for integrating AI models into
+IM chatbots. With AilingBot, you can:
+
+- ☕ **Code-free usage**: Quickly integrate existing AI large-scale models into mainstream IM chatbots (such as WeChat
+  Work, Feishu, DingTalk, Slack etc.) to interact with AI models through IM chatbots and complete business
+  requirements. Currently, AilingBot has built-in capabilities for multi-turn dialogue and document knowledge Q&A, and
+  more capabilities will be added in the future.
+- 🛠️**Secondary development**: AilingBot provides a clear engineering architecture, interface definition, and necessary
+  basic components. You do not need to develop the engineering framework for large-scale model services from scratch.
+  You only need to implement your Chat Policy and complete end-to-end AI model empowerment to IM chatbots through simple
+  configurations. It also supports expanding to your own end (such as your own IM, web application, or mobile
+  application) by developing your own channel.
+
+# Features
+
+- 💯 **Open source & Free**: Completely open source and free.
+- 📦 **Ready to use**: No need for development, with pre-installed capabilities to integrate with existing mainstream IM
+  and AI models.
+- 🔗 **LangChain Friendly**: Easy to integrate with LangChain.
+- 🧩 **Modular**: The project is organized in a modular way, with modules dependent on each other through abstract
+  protocols. Modules of the same type can be implemented by implementing the protocol, allowing for plug-and-play.
+- 💻 **Extensible**: AilingBot can be extended to new usage scenarios and capabilities. For example, integrating with new
+  IMs, new AI models, or customizing your own chat policy.
+- 🔥 **High performance**: AilingBot uses a coroutine-based asynchronous mode to improve system concurrency performance.
+  At the same time, system concurrency processing capabilities can be further improved through multi-processes.
+- 🔌 **API Integration**: AilingBot provides a set of clear API interfaces for easy integration and collaboration with
+  other systems and processes.
 
-# AilingBot是什么
+# 🚀 Quick Start
 
-AilingBot是一个开源的工程开发框架，同时也是IM机器人接入AI模型的一站式解决方案。通过AilingBot你可以：
+## Start an AI chatbot in 5 minutes
 
-- ☕**零代码使用**：快速将现有AI大模型能力接入主流IM机器人（如企业微信、飞书、钉钉、Slack等），实现通过IM机器人与AI大模型交互以完成业务需求。目前内置了多轮对话和文档知识问答两种能力，未来将内置更多能力
-- 🛠️**二次开发**：AilingBot提供了一套清晰的工程架构、接口定义和必需基础组件，无需从头开始重复开发大模型服务的工程框架，只需实现自己Chat
-  Policy，并通过一些简单的配置，就能完成端到端的AI模型对IM机器人的赋能。同时也支持通过开发自己的Channel扩展到你自己的端（如自己的IM、Web应用或移动端应用）
-
-# 特点
-
-- 💯**开源&免费**：完全开源且免费
-- 📦**开箱即用**：无需开发，预置接入现有主流IM及AI模型的能力
-- 🔗**LangChain友好**：方便集成LangChain
-- 🧩**模块化**：项目采用模块化组织，模块之间通过抽象协议依赖，同类模块实现协议即可即插即用
-- 💻**可扩展**：可以扩展AilingBot的使用场景和能力。例如接入到新的IM，新的AI模型，或者定制自己的对话策略
-- 🔥**高性能**：AilingBot采用基于协程的异步模式，提高系统的高并发性能。同时可以通过多进程进一步提升系统的高并发处理能力
-- 🔌**通过API集成**：AilingBot提供一组清晰的API接口，方便与其他系统及流程集成协同
-
-# 🚀快速开始
-
-## 5分钟启动一个AI聊天机器人
-
-下面将看到如何通过AilingBot快速启动一个基于命令行界面的AI机器人，效果如图：
+Below is a guide on how to quickly start an AI chatbot based on the command-line interface using AilingBot. The effect
+is shown in the following figure:
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/command-line-screenshot.png" alt="命令行机器人"/>
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/command-line-screenshot.png" alt="Command-line chatbot"/>
 </p>
 
+> 💡 First, you need to have an OpenAI API key. If you don't have one, refer to relevant materials on the Internet to
+> obtain it.
 
-> 💡首先你需要有一个OpenAI API key。如果没有参考互联网上相关资料获取
-
-### 通过Docker
+### Using Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -it --rm \
-  -e  AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
+  -e  AILINGBOT_POLICY__LLM__OPENAI_API_KEY={your OpenAI API key} \
   ailingbot poetry run ailingbot chat
 ```
 
-### 通过PIP
+### Using PIP
 
-#### 安装
+#### Installation
 
 ```shell
 pip install ailingbot
 ```
 
-#### 生成配置文件
+#### Generate Configuration File
 
 ```shell
 ailingbot init --silence --overwrite
 ```
 
-此时在当前目录会创建一个叫settings.toml的文件，这个文件就是AilingBot的配置文件。
-接下来修改必要配置，启动机器人只需一项配置，找到settings.toml中以下部分：
+This will create a file called `settings.toml` in the current directory, which is the configuration file for AilingBot.
+Next, modify the necessary configurations. To start the bot, only one configuration is needed. Find the following
+section in `settings.toml`:
 
 ```toml
 [policy.llm]
 _type = "openai"
 model_name = "gpt-3.5-turbo"
 openai_api_key = ""
 temperature = 0
 ```
 
-将其中`openai_api_key`的值改为你的真实OpenAI API key。
+Change the value of `openai_api_key` to your actual OpenAI API key.
 
-#### 启动机器人
+#### Start the Chatbot
 
-通过如下命令启动机器人：
+Start the chatbot with the following command:
 
 ```shell
 ailingbot chat
 ```
 
-## 接入企业微信
+## Start API Service
+
+### Using Docker
+
+```shell
+git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
+cd ailingbot
+docker build -t ailingbot .
+docker run -it --rm \
+  -e  AILINGBOT_POLICY__LLM__OPENAI_API_KEY={your OpenAI API key} \
+  ailingbot poetry run ailingbot api
+```
+
+### Using PIP
+
+#### Installation
+
+```shell
+pip install ailingbot
+```
+
+#### Generate Configuration File
+
+Same as starting the command line bot.
+
+#### Start the Service
+
+Start the bot using the following command:
+
+```shell
+ailingbot api
+```
+
+Now, enter `http://localhost:8080/docs` in your browser to see the API documentation. (If it is not a local start,
+please enter `http://{your public IP}:8080/docs`)
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/swagger.png" alt="Swagger API Documentation"/>
+</p>
+
+Here is an example request:
+
+```shell
+curl -X 'POST' \
+  'http://localhost:8080/chat/' \
+  -H 'accept: application/json' \
+  -H 'Content-Type: application/json' \
+  -d '{
+  "text": "你好"
+}'
+```
+
+And the response:
 
-下面演示如何快速将上面的机器人接入企业微信。
+```json
+{
+  "type": "text",
+  "conversation_id": "default_conversation",
+  "uuid": "afb35218-2978-404a-ab39-72a9db6f303b",
+  "ack_uuid": "3f09933c-e577-49a5-8f56-fa328daa136f",
+  "receiver_id": "anonymous",
+  "scope": "user",
+  "meta": {},
+  "echo": {},
+  "text": "你好！很高兴和你聊天。有什么我可以帮助你的吗？",
+  "reason": null,
+  "suggestion": null
+}
+```
 
-### 通过Docker
+## Integrating with WeChat Work
+
+Here's a guide on how to quickly integrate the chatbot with WeChat Work.
+
+### Using Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
-  -e AILINGBOT_POLICY__NAME=conversation \
-  -e AILINGBOT_POLICY__HISTORY_SIZE=5 \
-  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
-  -e AILINGBOT_CHANNEL__NAME=wechatwork \
-  -e AILINGBOT_CHANNEL__CORPID={你的企业微信机器人corpid} \
-  -e AILINGBOT_CHANNEL__CORPSECRET={你的企业微信机器人corpsecret} \
-  -e AILINGBOT_CHANNEL__AGENTID={你的企业微信机器人agentid} \
-  -e AILINGBOT_CHANNEL__TOKEN={你的企业微信机器人webhook token} \
-  -e AILINGBOT_CHANNEL__AES_KEY={你的企业微信机器人webhook aes_key} \
-  -p 8080:8080
-  ailingbot poetry run ailingbot serve
+-e AILINGBOT_POLICY__NAME=conversation \
+-e AILINGBOT_POLICY__HISTORY_SIZE=5 \
+-e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={your OpenAI API key
+} \
+-e AILINGBOT_CHANNEL__NAME=wechatwork \
+-e AILINGBOT_CHANNEL__CORPID={your WeChat Work robot's corpid} \
+-e AILINGBOT_CHANNEL__CORPSECRET={
+your WeChat Work robot's corpsecret} \
+-e AILINGBOT_CHANNEL__AGENTID={your WeChat Work robot's agentid} \
+-e AILINGBOT_CHANNEL__TOKEN={
+your WeChat Work robot's webhook token} \
+-e AILINGBOT_CHANNEL__AES_KEY={your WeChat Work robot's webhook aes_key} \
+-p 8080: 8080
+ailingbot poetry run ailingbot serve
 ```
 
-### 通过PIP
+### Using PIP
 
-#### 安装
+#### Installation
 
 ```shell
 pip install ailingbot
 ```
 
-#### 生成配置文件
+#### Generate Configuration File
 
 ```shell
 ailingbot init --silence --overwrite
 ```
 
-#### 修改配置文件
+#### Modify Configuration File
 
-打开`settings.toml`，将其中的下面部分填入你的企业微信应用真实信息：
+Open `settings.toml`, and fill in the following section with your WeChat Work robot's real information:
 
 ```toml
 [channel]
 name = "wechatwork"
-corpid = "" # 填写真实信息
-corpsecret = "" # 填写真实信息
-agentid = 0 # 填写真实信息
-token = "" # 填写真实信息
-aes_key = "" # 填写真实信息
+corpid = "" # Fill in with real information
+corpsecret = "" # Fill in with real information
+agentid = 0 # Fill in with real information
+token = "" # Fill in with real information
+aes_key = "" # Fill in with real information
 ```
 
-在llm中填入你的OpenAI API Key：
+In the `llm` section, fill in your OpenAI API Key:
 
 ```toml
 [policy.llm]
 _type = "openai"
 model_name = "gpt-3.5-turbo"
-openai_api_key = "" # 这里填入真实OpenAI API Key
+openai_api_key = "" # Fill in with your real OpenAI API Key here
 temperature = 0
 ```
 
-#### 启动服务
+#### Start the Service
 
 ```shell
 ailingbot serve
 ```
 
-最后我们需要去企业微信的管理后台，将webhook地址配置好，以便企业微信知道将接收到的用户消息转发到我们的webhook。
-Webhook的URL为：`http(s)://你的公网IP:8080/webhook/wechatwork/event/`
+Finally, we need to go to the WeChat Work admin console to configure the webhook address so that WeChat Work knows to
+forward the received user messages to our webhook.
+The webhook URL is: `http(s)://your_public_IP:8080/webhook/wechatwork/event/`
 
-完成以上配置后，就可以在企业微信中找到机器人，进行对话了：
+After completing the above configuration, you can find the chatbot in WeChat Work and start chatting:
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/wechatwork-screenshot.png" alt="企业微信机器人" width="300"/>
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/wechatwork-screenshot.png" alt="WeChat Work chatbot" width="300"/>
 </p>
 
-## 接入飞书
+## Integrating with Feishu
 
-下面演示如何快速将上面的机器人接入飞书，并启用一个新的对话策略：上传文档并针对文档进行知识问答。
+Here's a guide on how to quickly integrate the chatbot with Feishu and enable a new conversation policy: uploading
+documents and performing knowledge-based question answering on them.
 
-### 通过Docker
+### Using Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
   -e AILINGBOT_POLICY__NAME=document_qa \
   -e AILINGBOT_POLICY__CHUNK_SIZE=1000 \
   -e AILINGBOT_POLICY__CHUNK_OVERLAP=0 \
-  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
+  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={your OpenAI API key} \
   -e AILINGBOT_POLICY__LLM__MODEL_NAME=gpt-3.5-turbo-16k \
   -e AILINGBOT_CHANNEL__NAME=feishu \
-  -e AILINGBOT_CHANNEL__APP_ID={你的飞书机器人app id} \
-  -e AILINGBOT_CHANNEL__APP_SECRET={你的飞书机器人app secret} \
-  -e AILINGBOT_CHANNEL__VERIFICATION_TOKEN={你的飞书机器人webhook verification token} \
+  -e AILINGBOT_CHANNEL__APP_ID={your Feishu robot's app id} \
+  -e AILINGBOT_CHANNEL__APP_SECRET={your Feishu robot's app secret} \
+  -e AILINGBOT_CHANNEL__VERIFICATION_TOKEN={your Feishu robot's webhook verification token} \
   -p 8080:8080
   ailingbot poetry run ailingbot serve
 ```
 
-### 通过PIP
+### Using PIP
 
-#### 安装
+#### Installation
 
 ```shell
 pip install ailingbot
 ```
 
-#### 生成配置文件
+#### Generate Configuration File
 
 ```shell
 ailingbot init --silence --overwrite
 ```
 
-#### 修改配置文件
+#### Modify Configuration File
 
-打开`settings.toml`，将其中的channel部分改为如下，并填入你的飞书真实信息：
+Open `settings.toml`, and change the `channel` section to the following, filling in your Feishu robot's real
+information:
 
 ```toml
 [channel]
 name = "feishu"
-app_id = "" # 填写真实信息
-app_secret = "" # 填写真实信息
-verification_token = "" # 填写真实信息
+app_id = "" # Fill in with real information
+app_secret = "" # Fill in with real information
+verification_token = "" # Fill in with real information
 ```
 
-将policy部分替换为文档问答策略：
+Replace the `policy` section with the following document QA policy:
 
 ```toml
 [policy]
 name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 5
 ```
 
-最后建议在使用文档问答策略时，使用16k模型，因此将`policy.llm.model_name`修改为如下配置：
+Finally, it is recommended to use the 16k model when using the document QA policy. Therefore,
+change `policy.llm.model_name` to the following configuration:
 
 ```toml
 [policy.llm]
 _type = "openai"
-model_name = "gpt-3.5-turbo-16k" # 这里改为gpt-3.5-turbo-16k
-openai_api_key = "" # 填写真实信息
+model_name = "gpt-3.5-turbo-16k" # Change to gpt-3.5-turbo-16k
+openai_api_key = "" # Fill in with real information
 temperature = 0
 ```
 
-#### 启动服务
+#### Start the Service
 
 ```shell
 ailingbot serve
 ```
 
-最后我们需要去飞书的管理后台，将webhook地址配置好。
-飞书Webhook的URL为：`http(s)://你的公网IP:8080/webhook/feishu/event/`
+Finally, we need to go to the Feishu admin console to configure the webhook address.
+The webhook URL for Feishu is: `http(s)://your_public_IP:8080/webhook/feishu/event/`
 
-完成以上配置后，就可以在飞书中找到机器人，进行对话了：
+After completing the above configuration, you can find the chatbot in Feishu and start chatting:
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/feishu-screenshot.png" alt="飞书机器人" width="1000"/>
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/feishu-screenshot.png" alt="Feishu chatbot" width="1000"/>
 </p>
 
-## 接入钉钉
+## Integrating with DingTalk
 
-下面演示如何快速将上面的机器人接入钉钉。
+Here's a guide on how to quickly integrate the chatbot with DingTalk.
 
-### 通过Docker
+### Using Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
   -e AILINGBOT_POLICY__NAME=conversation \
   -e AILINGBOT_POLICY__HISTORY_SIZE=5 \
-  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
+  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={your OpenAI API key} \
   -e AILINGBOT_CHANNEL__NAME=dingtalk \
-  -e AILINGBOT_CHANNEL__APP_KEY={你的钉钉机器人app key} \
-  -e AILINGBOT_CHANNEL__APP_SECRET={你的钉钉机器人app secret} \
-  -e AILINGBOT_CHANNEL__ROBOT_CODE={你的钉钉机器人robot code} \
+  -e AILINGBOT_CHANNEL__APP_KEY={your DingTalk robot's app key} \
+  -e AILINGBOT_CHANNEL__APP_SECRET={your DingTalk robot's app secret} \
+  -e AILINGBOT_CHANNEL__ROBOT_CODE={your DingTalk robot's robot code} \
   -p 8080:8080
   ailingbot poetry run ailingbot serve
 ```
 
-### 通过PIP
+### Using PIP
 
-#### 安装
+#### Installation
 
 ```shell
 pip install ailingbot
 ```
 
-#### 生成配置文件
+#### Generate Configuration File
 
 ```shell
 ailingbot init --silence --overwrite
 ```
 
-#### 修改配置文件
+#### Modify Configuration File
 
-打开`settings.toml`，将其中的channel部分改为如下，并填入你的飞书真实信息：
+Open `settings.toml`, and change the `channel` section to the following, filling in your DingTalk robot's real
+information:
 
 ```toml
 [channel]
 name = "dingtalk"
-app_key = "" # 填写真实信息
-app_secret = "" # 填写真实信息
-robot_code = "" # 填写真实信息
+app_key = "" # Fill in with real information
+app_secret = "" # Fill in with real information
+robot_code = "" # Fill in with real information
 ```
 
-#### 启动服务
+#### Start the Service
 
 ```shell
 ailingbot serve
 ```
 
-最后我们需要去钉钉的管理后台，将webhook地址配置好。
-钉钉Webhook的URL为：`http(s)://你的公网IP:8080/webhook/dingtalk/event/`
+Finally, we need to go to the DingTalk admin console to configure the webhook address.
+The webhook URL for DingTalk is: `http(s)://your_public_IP:8080/webhook/dingtalk/event/`
 
-完成以上配置后，就可以在钉钉中找到机器人，进行对话了：
+After completing the above configuration, you can find the chatbot in DingTalk and start chatting:
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/dingtalk-screenshot.png" alt="钉钉机器人" />
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/dingtalk-screenshot.png" alt="DingTalk chatbot" />
 </p>
 
-## 接入Slack
+## Integrating with Slack
 
-下面演示如何快速将上面的机器人接入Slack，并启用文档知识问答策略。
+Here's a guide on how to quickly integrate the chatbot with Slack and enable a new conversation policy: uploading
+documents and performing knowledge-based question answering on them.
 
-### 通过Docker
+### Using Docker
 
 ```shell
 git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
 cd ailingbot
 docker build -t ailingbot .
 docker run -d \
   -e AILINGBOT_POLICY__NAME=document_qa \
   -e AILINGBOT_POLICY__CHUNK_SIZE=1000 \
   -e AILINGBOT_POLICY__CHUNK_OVERLAP=0 \
-  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
+  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={your OpenAI API key} \
   -e AILINGBOT_POLICY__LLM__MODEL_NAME=gpt-3.5-turbo-16k \
   -e AILINGBOT_CHANNEL__NAME=slack \
-  -e AILINGBOT_CHANNEL__VERIFICATION_TOKEN={你的Slack App webhook verification token} \
-  -e AILINGBOT_CHANNEL__OAUTH_TOKEN={你的Slack App oauth token} \
+  -e AILINGBOT_CHANNEL__VERIFICATION_TOKEN={your Slack App webhook verification token} \
+  -e AILINGBOT_CHANNEL__OAUTH_TOKEN={your Slack App oauth token} \
   -p 8080:8080
   ailingbot poetry run ailingbot serve
 ```
 
-### 通过PIP
+### Using PIP
 
-#### 安装
+#### Installation
 
 ```shell
 pip install ailingbot
 ```
 
-#### 生成配置文件
+#### Generate Configuration File
 
 ```shell
 ailingbot init --silence --overwrite
 ```
 
-#### 修改配置文件
+#### Modify Configuration File
 
-打开`settings.toml`，将其中的channel部分改为如下，并填入你的飞书真实信息：
+Open `settings.toml`, and change the `channel` section to the following, filling in your Slack robot's real information:
 
 ```toml
 [channel]
 name = "slack"
-verification_token = "" # 填写真实信息
-oauth_token = "" # 填写真实信息
+verification_token = "" # Fill in with real information
+oauth_token = "" # Fill in with real information
 ```
 
-将policy部分替换为文档问答策略：
+Replace the `policy` section with the following document QA policy:
 
 ```toml
 [policy]
 name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 5
 ```
 
-最后建议在使用文档问答策略时，使用16k模型，因此将`policy.llm.model_name`修改为如下配置：
+Finally, it is recommended to use the 16k model when using the document QA policy. Therefore,
+change `policy.llm.model_name` to the following configuration:
 
 ```toml
 [policy.llm]
 _type = "openai"
-model_name = "gpt-3.5-turbo-16k" # 这里改为gpt-3.5-turbo-16k
-openai_api_key = "" # 填写真实信息
+model_name = "gpt-3.5-turbo-16k" # Change to gpt-3.5-turbo-16k
+openai_api_key = "" # Fill in with real information
 temperature = 0
 ```
 
-#### 启动服务
+#### Start the Service
 
 ```shell
 ailingbot serve
 ```
 
-最后我们需要去Slack的管理后台，将webhook地址配置好。
-飞书Webhook的URL为：`http(s)://你的公网IP:8080/webhook/slack/event/`
+Finally, we need to go to the Slack admin console to configure the webhook address.
+The webhook URL for Slack is: `http(s)://your_public_IP:8080/webhook/slack/event/`
 
-完成以上配置后，就可以在Slack中找到机器人，进行对话了：
+After completing the above configuration, you can find the chatbot in Slack and start chatting:
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/slack-screenshot.png" alt="Slack机器人" width="1000"/>
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/slack-screenshot.png" alt="Slack chatbot" width="1000"/>
 </p>
 
-# 📖使用指南
+# 📖User Guide
 
-## 主要流程
+## Main Process
 
-AilingBot的主要处理流程如下图：
+The main processing flow of AilingBot is as follows:
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/flow.png" alt="主要流程" width="500"/>
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/flow.png" alt="Main Process" width="500"/>
 </p>
 
-1. 首先用户将消息发送给IM的机器人
-2. 如果配置了webhook，即时通讯工具会将发送给机器人的请求转发到webhook服务地址
-3. Webhook服务将IM原始消息经过处理，转为AilingBot内部的消息格式，发送给ChatBot
-4. ChatBot会根据所配置的会话策略（Chat Policy），处理请求并形成响应消息。这个过程中，ChatBot
-   可能会进行请求大语言模型、访问向量数据库、调用外部API等操作以完成请求处理
-5. ChatBot将响应信息发送给IM Agent，IM Agent负责将AilingBot内部响应信息格式转换成
-   特定IM的格式，并调用IM开放能力API发送响应消息
-6. IM机器人将消息显示给用户，完成整个处理过程
-
-## 主要概念
-
-- **IM机器人**：多数即时通讯工具内置的能力，允许管理员创建一个机器人，并通过程序处理用户的消息
-- **Channel**：Channel表示不同终端，可以是一个IM，也可能是一个自定义终端（如Web）
-- **Webhook**：一个http(s)服务，用于接收IM机器人转发的用户消息，不同Channel对于webhook有自己的规范，因此需要有自己的webhook实现
-- **IM Agent**：用于调用IM开放能力API，不同的IM开放能力API不同，因此每个Channel需要有对应Agent实现
-- **ChatBot**：用于接收和响应用户消息的核心组件
-- **会话策略**：具体定义如何响应用户，被ChatBot调用。一个会话策略具体定义了机器人的能力，如闲聊、进行知识问答等
-- **LLM**：大语言模型，如何OpenAI的ChatGPT，开放的ChatGLM等均属于不同的大语言模型，大语言模型是实现AI能力的关键组件
-
-## 配置
-
-### 配置方式
-
-AilingBot的配置可以通过两种方式：
-
-- **通过配置文件**：AilingBot读取当前目录的`settings.toml`作为配置文件，其文件格式为[TOML](https://toml.io/en/)
-  具体配置项见下文
-- **通过环境变量**：AilingBot也会读取环境变量中配置项，具体环境变量列表见下文
-
-> 💡配置文件和环境变量可以混合使用，当一个配置项同时存在于两者时，优先使用环境变量
-
-### 配置映射关系
-
-所有配置，TOML配置键和环境变量有如下映射关系：
-
-- 所有环境变量以`AILINGBOT_`开头
-- 层级之间用两个下划线`__`隔开
-- 配置键内部的下划线在环境变量中保留
-- 不区分大小写
-
-例如：
-
-- `some_conf`的对应环境变量为`AILINGBOT_SOME_CONF`
-- `some_conf.conf_1`的对应环境变量为`AILINGBOT_SOME_CONF__CONF_1`
-- `some_conf.conf_1.subconf`的对应环境变量为`AILINGBOT_SOME_CONF__CONF_1__SUBCONF`
-
-### 配置项
-
-#### 通用
-
-| 配置项       | 说明                                                                                     | TOML                 | 环境变量                            |
-|-----------|----------------------------------------------------------------------------------------|----------------------|---------------------------------|
-| 语言        | 语言码（参考：http://www.lingoes.net/en/translator/langcode.htm）                              | lang                 | AILINGBOT_LANG                  |
-| 时区        | 时区码（参考：https://en.wikipedia.org/wiki/List_of_tz_database_time_zones                    | tz                   | AILINGBOT_TZ                    |
-| 会话策略名称    | 预置会话策略名称或完整会话策略class路径                                                                 | policy.name          | AILINGBOT_POLICY__NAME          |
-| Channel名称 | 预置Channel名称                                                                            | channel.name         | AILINGBOT_CHANNEL__NAME         |
-| Webhook路径 | 非预置Channel webhook的完整class路径                                                           | channel.webhook_name | AILINGBOT_CHANNEL__WEBHOOK_NAME |
-| Agent路径   | 非预置Channel agent的完整class路径                                                             | channel.agent_name   | AILINGBOT_CHANNEL__AGENT_NAME   |
-| Uvicorn配置 | 所有uvicorn配置（参考：[uvicorn settings](https://www.uvicorn.org/settings/)），这部分配置会透传给uvicorn | uvicorn.*            | AILINGBOT_UVICORN__*            |
+1. First, the user sends a message to the IM bot.
+2. If a webhook is configured, the instant messaging tool will forward the request sent to the bot to the webhook
+   service address.
+3. The webhook service processes the original IM message and converts it into AilingBot's internal message format, which
+   is then sent to ChatBot.
+4. ChatBot processes the request and forms a response message based on the configured chat policy. During this process,
+   ChatBot may perform operations such as requesting a large language model, accessing a vector database, or calling an
+   external API to complete the request processing.
+5. ChatBot sends the response message to the IM Agent. The IM Agent is responsible for converting the AilingBot internal
+   response message format into a specific IM format and calling the IM open capability API to send the response
+   message.
+6. The IM bot displays the message to the user, completing the entire processing process.
+
+## Main Concepts
+
+- **IM bot**: A capability built into most instant messaging tools that allows administrators to create a bot and
+  process user messages through a program.
+- **Channel**: A channel represents different terminals, which can be an IM or a custom terminal (such as the web).
+- **Webhook**: An HTTP(S) service used to receive user messages forwarded by IM bots. Different channels have their own
+  specifications for webhooks, so each channel requires its own webhook implementation.
+- **IM Agent**: Used to call IM open capability APIs. Different IM open capability APIs are different, so each channel
+  requires a corresponding agent implementation.
+- **ChatBot**: The core component used to receive and respond to user messages.
+- **Chat Policy**: Defines how to respond to users and is called by ChatBot. A chat policy specifically defines the
+  robot's abilities, such as chitchat or knowledge Q&A.
+- **LLM**: Large language model, such as OpenAI's ChatGPT and open ChatGLM, are all different large language models. The
+  large language model is a key component for implementing AI capabilities.
+
+## Configuration
+
+### Configuration Methods
+
+AilingBot can be configured in two ways:
+
+- **Using configuration files**: AilingBot reads `settings.toml` in the current directory as the configuration file
+  in [TOML](https://toml.io/en/) format. Please refer to the following section for specific configuration items.
+- **Using environment variables**: AilingBot also reads configuration items in environment variables. Please refer to
+  the following section for a list of environment variables.
+
+> 💡 Both configuration files and environment variables can be used together. If a configuration item exists in both, the
+> environment variable takes precedence.
+
+### Configuration Mapping
+
+All configurations have the following mappings between TOML keys and environment variables:
+
+- All environment variables start with `AILINGBOT_`.
+- Double underscores `__` are used as separators between levels.
+- Underscores in configuration keys are preserved in environment variables.
+- Case-insensitive.
+
+For example:
+
+- The corresponding environment variable of `some_conf` is `AILINGBOT_SOME_CONF`.
+- The corresponding environment variable of `some_conf.conf_1` is `AILINGBOT_SOME_CONF__CONF_1`.
+- The corresponding environment variable of `some_conf.conf_1.subconf` is `AILINGBOT_SOME_CONF__CONF_1__SUBCONF`.
+
+### Configuration Items
+
+#### General
+
+| Configuration Item | Description                                                                                                                                   | TOML                 | Environment Variable            |
+|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------|---------------------------------|
+| Language           | Language code (Reference: http://www.lingoes.net/en/translator/langcode.htm)                                                                  | lang                 | AILINGBOT_LANG                  |
+| Timezone           | Timezone code (Reference: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)                                                       | tz                   | AILINGBOT_TZ                    |
+| Policy Name        | Predefined policy name or complete policy class path                                                                                          | policy.name          | AILINGBOT_POLICY__NAME          |
+| Channel Name       | Predefined channel name                                                                                                                       | channel.name         | AILINGBOT_CHANNEL__NAME         |
+| Webhook Path       | Complete class path of non-predefined channel webhook                                                                                         | channel.webhook_name | AILINGBOT_CHANNEL__WEBHOOK_NAME |
+| Agent Path         | Complete class path of non-predefined channel agent                                                                                           | channel.agent_name   | AILINGBOT_CHANNEL__AGENT_NAME   |
+| Uvicorn Config     | All uvicorn configurations (Reference: [uvicorn settings](https://www.uvicorn.org/settings/)). These configurations will be passed to uvicorn | uvicorn.*            | AILINGBOT_UVICORN__*            |
 
-配置示例：
+Configuration example:
 
 ```toml
 lang = "zh_CN"
 tz = "Asia/Shanghai"
 
 [policy]
 name = "conversation"
-# 更多policy配置
-
-[policy.llm]
-# 模型配置
+# More policy configurations
 
 [channel]
 name = "wechatwork"
-# 更多channel配置
+# More channel configurations
 
 [uvicorn]
 host = "0.0.0.0"
 port = 8080
 ```
 
-#### 内置会话策略配置
+#### Built-in Policy Configuration
 
 ##### conversation
 
-conversation使用LangChain的Conversation作为会话策略，其效果为直接和LLM对话，且带有对话历史上下文，因此可以进行多轮会话。
+Conversation uses LangChain's Conversation as the policy, which enables direct interaction with LLM and has a
+conversation history context, enabling multi-turn conversations.
 
-| 配置项    | 说明          | TOML                | 环境变量                           |
-|--------|-------------|---------------------|--------------------------------|
-| 会话历史长度 | 表示保留多少轮历史会话 | policy.history_size | AILINGBOT_POLICY__HISTORY_SIZE |
+| Configuration Item | Description                                                   | TOML                | Environment Variable           |
+|--------------------|---------------------------------------------------------------|---------------------|--------------------------------|
+| History Size       | Indicates how many rounds of historical conversations to keep | policy.history_size | AILINGBOT_POLICY__HISTORY_SIZE |
 
-配置示例：
+Configuration example:
 
 ```toml
-# 使用conversation策略，保留5轮历史会话
+# Use the conversation policy and keep 5 rounds of historical conversations
 [policy]
 name = "conversation"
 history_size = 5
 ```
 
 ##### document_qa
 
-document_qa使用LangChain的[Stuff](https://python.langchain.com/docs/modules/chains/document/stuff)作为对话策略。
-用户可上传一个文档，然后针对文档内容进行提问。
+Document_qa uses LangChain's [Stuff](https://python.langchain.com/docs/modules/chains/document/stuff) as the policy.
+Users can upload a document and then ask questions based on the document content.
 
-| 配置项     | 说明                                 | TOML                 | 环境变量                            |
-|---------|------------------------------------|----------------------|---------------------------------|
-| 文档切分块大小 | 对应LangChain Splitter的chunk_size    | policy.chunk_size    | AILINGBOT_POLICY__CHUNK_SIZE    |
-| 文档切重叠   | 对应LangChain Splitter的chunk_overlap | policy.chunk_overlap | AILINGBOT_POLICY__CHUNK_OVERLAP |
+| Configuration Item | Description                                       | TOML                 | Environment Variable            |
+|--------------------|---------------------------------------------------|----------------------|---------------------------------|
+| Chunk Size         | Corresponds to LangChain Splitter's chunk_size    | policy.chunk_size    | AILINGBOT_POLICY__CHUNK_SIZE    |
+| Chunk Overlap      | Corresponds to LangChain Splitter's chunk_overlap | policy.chunk_overlap | AILINGBOT_POLICY__CHUNK_OVERLAP |
 
-配置示例：
+Configuration example:
 
 ```toml
-# 使用document_qa策略，chunk_size和chunk_overlap分别配置为1000和0
+# Use the document_qa policy, with chunk_size and chunk_overlap set to 1000 and 0, respectively
 [policy]
 name = "document_qa"
 chunk_size = 1000
 chunk_overlap = 0
 ```
 
-#### 模型配置
+#### Model Configuration
 
-模型配置与LangChain保持一致，下面给出示例。
+The model configuration is consistent with LangChain. The following is an example.
 
 ##### OpenAI
 
 ```toml
 [policy.llm]
-_type = "openai" # 对应环境变量AILINGBOT_POLICY__LLM___TYPE
-model_name = "gpt-3.5-turbo" # 对应环境变量AILINGBOT_POLICY__LLM__MODEL_NAME
-openai_api_key = "sk-pd8******************************HQQS241dNrHH1kv" # 对应环境变量AILINGBOT_POLICY__LLM__OPENAI_API_KEY
-temperature = 0 # 对应环境变量AILINGBOT_POLICY__LLM__TEMPERATURE
+_type = "openai" # Corresponding environment variable: AILINGBOT_POLICY__LLM___TYPE
+model_name = "gpt-3.5-turbo" # Corresponding environment variable: AILINGBOT_POLICY__LLM__MODEL_NAME
+openai_api_key = "sk-pd8I'm sorry, it seems like your message got cut off. Can you please provide me with more information or clarify your request?
 ```
 
-#### 内置Channel配置
-
-##### 企业微信
-
-| 配置项         | 说明                        | TOML               | 环境变量                          |
-|-------------|---------------------------|--------------------|-------------------------------|
-| Corp ID     | 企业微信自建app的corpid          | channel.corpid     | AILINGBOT_CHANNEL__CORPID     |
-| Corp Secret | 企业微信自建app的corpsecret      | channel.corpsecret | AILINGBOT_CHANNEL__CORPSECRET |
-| Agent ID    | 企业微信自建app的agentid         | channel.agentid    | AILINGBOT_CHANNEL__AGENTID    |
-| TOKEN       | 企业微信自建app的webhook token   | channel.token      | AILINGBOT_CHANNEL__TOKEN      |
-| AES KEY     | 企业微信自建app的webhook aes key | channel.aes_key    | AILINGBOT_CHANNEL__AES_KEY    |
-
-配置示例：
-
-```toml
-[channel]
-name = "wechatwork"
-corpid = "wwb**********ddb40"
-corpsecret = "TG3t******************************hZslJNe5Q"
-agentid = 1000001
-token = "j9SK**********zLeJdFSYh"
-aes_key = "7gCwzwH******************************p1p0O8"
-```
-
-##### 飞书
-
-| 配置项                | 说明                                | TOML                       | 环境变量                                  |
-|--------------------|-----------------------------------|----------------------------|---------------------------------------|
-| App ID             | 飞书自建应用的app id                     | channel.app_id             | AILINGBOT_CHANNEL__APP_ID             |
-| App Secret         | 飞书自建应用的app secret                 | channel.app_secret         | AILINGBOT_CHANNEL__APP_SECRET         |
-| Verification Token | 飞书自建应用的webhook verification token | channel.verification_token | AILINGBOT_CHANNEL__VERIFICATION_TOKEN |
-
-配置示例：
-
-```toml
-[channel]
-name = "feishu"
-app_id = "cli_a**********9d00e"
-app_secret = "y********************cyk8AxmYVDD"
-verification_token = "yIJ********************7bfNHUcYH"
-```
+## Command Line Tools
 
-##### 钉钉
+### Initialize Configuration File (init)
 
-| 配置项        | 说明                | TOML               | 环境变量                          |
-|------------|-------------------|--------------------|-------------------------------|
-| App Key    | 钉钉自建应用的app key    | channel.app_key    | AILINGBOT_CHANNEL__APP_KEY    |
-| App Secret | 钉钉自建应用的app secret | channel.app_secret | AILINGBOT_CHANNEL__APP_SECRET |
-| Robot Code | 钉钉自建应用的robot code | channel.robot_code | AILINGBOT_CHANNEL__ROBOT_CODE |
-
-配置示例：
-
-```toml
-[channel]
-name = "dingtalk"
-app_key = "dingi**********wymdr"
-app_secret = "ombrcUp****************************************GL2AwObLjILUY1MzD"
-robot_code = "ding**********owymdr"
-```
-
-##### Slack
-
-| 配置项                | 说明                         | TOML                       | 环境变量                                  |
-|--------------------|----------------------------|----------------------------|---------------------------------------|
-| Verification Token | Slack应用的verification token | channel.verification_token | AILINGBOT_CHANNEL__VERIFICATION_TOKEN |
-| OAuth token        | Slack应用的oauth token        | channel.oauth_token        | AILINGBOT_CHANNEL__OAUTH_TOKEN        |
-
-配置示例：
-
-```toml
-[channel]
-name = "slack"
-verification_token = "HzBGs1**********39gZG2P0"
-oauth_token = "xoxb-2**********27-5**********23-if**********H1QEGUItx2Yz"
-```
+#### Usage
 
-## 命令行工具
-
-### 初始化配置文件（init）
-
-#### 使用方法
-
-`init`命令将在当前目录生成配置文件settings.toml。默认情况下，将以交互方式询问用户，
-可以使用`--silence`让生成过程不询问用户，直接使用默认配置。
+The `init` command generates a configuration file `settings.toml` in the current directory. By default, the user will be
+prompted interactively. You can use the `--silence` option to generate the configuration file directly using default
+settings.
 
 ```text
 Usage: ailingbot init [OPTIONS]
 
-  Initialize the AilingBot environment.
+Initialize the AilingBot environment.
 
 Options:
-  --silence    Without asking the user.
-  --overwrite  Overwrite existing file if a file with the same name already
-               exists.
-  --help       Show this message and exit.
+--silence    Without asking the user.
+--overwrite  Overwrite existing file if a file with the same name already
+exists.
+--help       Show this message and exit.
 ```
 
 #### Options
 
-| Option      | 说明                     | 类型   | 备注 |
-|-------------|------------------------|------|----|
-| --silence   | 不询问用户，直接生成默认配置         | Flag |    |
-| --overwrite | 允许覆盖当前目录的settings.toml | Flag |    |
+| Option      | Description                                                          | Type | Remarks |
+|-------------|----------------------------------------------------------------------|------|---------|
+| --silence   | Generate the default configuration directly without asking the user. | Flag |         |
+| --overwrite | Allow overwriting the `settings.toml` file in the current directory. | Flag |         |
 
-### 查看当前配置（config）
+### View Current Configuration (config)
 
-`config`命令将读取当前环境的配置（包括配置文件及环境变量配置，并进行合并）。
+The `config` command reads the current environment configuration (including the configuration file and environment
+variables) and merges them.
 
-#### 使用方法
+#### Usage
 
 ```text
 Usage: ailingbot config [OPTIONS]
 
   Show current configuration information.
 
 Options:
   -k, --config-key TEXT  Configuration key.
   --help                 Show this message and exit.
 ```
 
 #### Options
 
-| Option           | 说明  | 类型     | 备注             |
-|------------------|-----|--------|----------------|
-| -k, --config-key | 配置键 | String | 不传入的话，显示完整配置信息 |
+| Option           | Description       | Type   | Remarks                                                                  |
+|------------------|-------------------|--------|--------------------------------------------------------------------------|
+| -k, --config-key | Configuration key | String | If not passed, the complete configuration information will be displayed. |
 
-### 启动命令行机器人（chat）
+### Start Command Line Bot (chat)
 
-`chat`命令启动一个交互式命令行机器人，用于测试当前chat policy。
+The `chat` command starts an interactive command-line bot for testing the current chat policy.
 
-#### 使用方法
+#### Usage
 
 ```text
 Usage: ailingbot chat [OPTIONS]
 
   Start an interactive bot conversation environment.
 
 Options:
   --debug  Enable debug mode.
   --help   Show this message and exit.
 ```
 
 #### Options
 
-| Option  | 说明        | 类型   | 备注                     |
-|---------|-----------|------|------------------------|
-| --debug | 开启debug模式 | Flag | Debug模式将输出更多内容，如prompt |
+| Option  | Description       | Type | Remarks                                                          |
+|---------|-------------------|------|------------------------------------------------------------------|
+| --debug | Enable debug mode | Flag | The debug mode will output more information, such as the prompt. |
 
-### 启动Webhook服务（serve）
+### Start Webhook Service (serve)
 
-`serve`命令启动Webhook HTTP server，用于真正实现和具体IM进行交互。
+The `serve` command starts a Webhook HTTP server for interacting with specific IM.
 
-#### 使用方法
+#### Usage
 
 ```text
 Usage: ailingbot serve [OPTIONS]
 
   Run webhook server to receive events.
 
 Options:
@@ -826,71 +859,109 @@
                                   environment variable AILINGBOT_LOG_FILE if
                                   is not passed into).  [default: STDERR]
   --help                          Show this message and exit.
 ```
 
 #### Options
 
-| Option      | 说明                  | 类型     | 备注                    |
-|-------------|---------------------|--------|-----------------------|
-| --log-level | 显示日志级别，将显示此级别及以上的日志 | String | 默认显示所有级别（TRACE）       |
-| --log-file  | 日志输出位置              | String | 默认情况日志打印到标准错误（STDERR） |
+| Option      | Description                                                              | Type   | Remarks                                                     |
+|-------------|--------------------------------------------------------------------------|--------|-------------------------------------------------------------|
+| --log-level | The minimum severity level from which logged messages should be sent to. | String | By default, all log levels will be displayed (TRACE).       |
+| --log-file  | The location where logs are output.                                      | String | By default, logs will be output to standard error (STDERR). |
+
+### Start API Service (api)
+
+The `api` command starts the API HTTP server.
+
+#### Usage
+
+```text
+Usage: ailingbot api [OPTIONS]
+
+Run endpoint server.
+
+Options:
+  --log-level [TRACE|DEBUG|INFO|SUCCESS|WARNING|ERROR|CRITICAL]
+                                  The minimum severity level from which logged
+                                  messages should be sent to(read from
+                                  environment variable AILINGBOT_LOG_LEVEL if
+                                  is not passed into).  [default: TRACE]
+  --log-file TEXT                 STDOUT, STDERR, or file path(read from
+                                  environment variable AILINGBOT_LOG_FILE if
+                                  is not passed into).  [default: STDERR]
+  --help                          Show this message and exit.
+```
+
+#### Options
+
+| Option      | Description                                                        | Type   | Remarks                                                 |
+|-------------|--------------------------------------------------------------------|--------|---------------------------------------------------------|
+| --log-level | Display log level, which will display logs at this level and above | String | By default, all levels are displayed (TRACE)            |
+| --log-file  | Log output location                                                | String | By default, logs are printed to standard error (STDERR) |
 
-# 💻开发指南
+## 🔌API
 
-## 开发总则
+TBD
+
+# 💻Development Guide
+
+## Development Guidelines
 
 TBD
 
-## 开发对话策略
+## Developing Chat Policy
 
 TBD
 
-## 开发Channel
+## Developing Channel
 
 TBD
 
-# 🤔常见问题
+# 🤔Frequently Asked Questions
 
-- 由于企业微信不支持上传文件事件的回调，因此企业微信暂时不能使用内置的document_qa策略
-- 各个IM的webhook需要公网IP，如果你暂时没有，可以考虑通过"内网穿透"方案在本地测试，具体方法请参考网上资料
-- 我们预期chat policy应该是无状态的，状态应该保存在外部，但是具体实现时policy仍然有可能存在本地状态（如在本地变量中存储了对话历史）。因此当uvicorn有多个worker进程时，由于没一个进程都有单独的chat
-  policy实例，所以这些本地状态无法共享，而同一个用户的请求可能会被不同worker响应，因此导致预期之外的行为。要避免这种行为，请保证一下两个条件至少有一个被满足：
-    - Chat policy不使用本地状态
-    - 只启动一个uvicorn worker
-
-# 🎯发展计划
-
-- [ ] 提供完善的使用文档和开发者文档
-- [ ] 支持更多的Channel
-    - [x] 企业微信
-    - [x] 飞书
-    - [x] 钉钉
+- Due to the fact that WeChat Work does not support uploading file event callbacks, the built-in `document_qa`
+  policy cannot be used for WeChat Work.
+- The webhook of each IM requires a public IP. If you do not have one, you can consider testing locally through the "
+  intranet penetration" solution. Please refer to online resources for specific methods.
+- We expect the chat policy to be stateless, and the state should be stored externally. However, in specific
+  implementations, the policy may still have local states (such as storing conversation history in local variables).
+  Therefore, when uvicorn has multiple worker processes, these local states cannot be shared because each process has a
+  separate chat policy instance, and a request from the same user may be responded to by different workers, leading to
+  unexpected behavior. To avoid this, please ensure that at least one of the following two conditions is met:
+    - Chat policy does not use local states.
+    - Only one uvicorn worker is started.
+
+# 🎯Roadmap
+
+- [ ] Provide complete usage and developer documentation.
+- [ ] Support more channels.
+    - [x] WeChat Work
+    - [x] Feishu
+    - [x] DingTalk
     - [x] Slack
-- [ ] 更多请求消息类型的支持
-    - [x] 文本请求
-    - [ ] 图片请求
-    - [x] 文件请求
-- [ ] 更多响应消息类型的支持
-    - [x] 文本响应
-    - [ ] 图片响应
-    - [ ] 文件响应
-    - [ ] Markdown响应
-    - [ ] 表格响应
-- [ ] 开发更多的开箱即用的对话策略
-    - [x] 多轮会话策略
-    - [x] 文档问答策略
-    - [ ] 数据库问答策略
-    - [ ] 在线搜索问答策略
-- [ ] 支持通过HTTP调用独立的对话策略服务
-- [ ] 基础组件抽象
-    - [ ] 大语言模型
-    - [ ] 知识库
+- [ ] Support more request message types.
+    - [x] Text request
+    - [ ] Image request
+    - [x] File request
+- [ ] Support more response message types.
+    - [x] Text response
+    - [ ] Image response
+    - [ ] File response
+    - [ ] Markdown response
+    - [ ] Table response
+- [ ] Develop more out-of-the-box chat policies.
+    - [x] Multi-round conversation policy
+    - [x] Document question and answer policy
+    - [ ] Database question and answer policy
+    - [ ] Online search question and answer policy
+- [ ] Support calling standalone chat policy services through HTTP.
+- [ ] Abstract basic components
+    - [ ] Large language model
+    - [ ] Knowledge base
     - [ ] Tools
-- [ ] 支持本地模型部署
+- [ ] Support local model deployment.
     - [ ] ChatGLM-6B
-- [ ] 支持通过API调用
-- [ ] Web管理后台及可视化配置管理
-- [x] 提供基于Docker容器的部署能力
-- [ ] 增强系统的可观测性和可治理性
-- [ ] 完善的测试用例
-
+- [x] Support API.
+- [ ] Web management background and visual configuration management.
+- [x] Provide deployment capability based on Docker containers.
+- [ ] Enhance the observability and controllability of the system.
+- [ ] Complete test cases.
```


# Comparing `tmp/xxx-chat-0.0.2.tar.gz` & `tmp/xxx-chat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxx-chat-0.0.2.tar", last modified: Thu Jul  6 03:06:43 2023, max compression
+gzip compressed data, was "xxx-chat-0.0.3.tar", last modified: Thu Jul  6 03:13:10 2023, max compression
```

## Comparing `xxx-chat-0.0.2.tar` & `xxx-chat-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.760973 xxx-chat-0.0.2/
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1062 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/LICENSE
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1064 2023-07-06 03:06:43.760724 xxx-chat-0.0.2/PKG-INFO
--rw-r--r--   0 taofoxtel   (503) staff       (20)      665 2023-07-05 09:36:04.000000 xxx-chat-0.0.2/README.md
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.756036 xxx-chat-0.0.2/command/
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/command/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1107 2023-07-06 03:00:54.000000 xxx-chat-0.0.2/command/__main__.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.756589 xxx-chat-0.0.2/commons/
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/commons/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)     2506 2023-07-06 03:03:46.000000 xxx-chat-0.0.2/commons/config.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.757143 xxx-chat-0.0.2/configuration/
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/configuration/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1213 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/configuration/profile_config.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)       38 2023-07-06 03:06:43.761055 xxx-chat-0.0.2/setup.cfg
--rw-r--r--   0 taofoxtel   (503) staff       (20)      811 2023-07-06 03:04:22.000000 xxx-chat-0.0.2/setup.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.757998 xxx-chat-0.0.2/utils/
--rw-r--r--   0 taofoxtel   (503) staff       (20)      772 2023-07-06 01:29:12.000000 xxx-chat-0.0.2/utils/CommonUtil.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/utils/__init__.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1506 2023-07-06 03:00:54.000000 xxx-chat-0.0.2/utils/logger.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.758595 xxx-chat-0.0.2/xxx/
--rw-r--r--   0 taofoxtel   (503) staff       (20)     2527 2023-07-06 03:00:54.000000 xxx-chat-0.0.2/xxx/CommandChat.py
--rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.2/xxx/__init__.py
-drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:06:43.760347 xxx-chat-0.0.2/xxx_chat.egg-info/
--rw-r--r--   0 taofoxtel   (503) staff       (20)     1064 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/PKG-INFO
--rw-r--r--   0 taofoxtel   (503) staff       (20)      445 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/SOURCES.txt
--rw-r--r--   0 taofoxtel   (503) staff       (20)        1 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/dependency_links.txt
--rw-r--r--   0 taofoxtel   (503) staff       (20)       46 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/entry_points.txt
--rw-r--r--   0 taofoxtel   (503) staff       (20)        6 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/requires.txt
--rw-r--r--   0 taofoxtel   (503) staff       (20)       40 2023-07-06 03:06:43.000000 xxx-chat-0.0.2/xxx_chat.egg-info/top_level.txt
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:13:10.354507 xxx-chat-0.0.3/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1062 2023-04-12 09:19:49.000000 xxx-chat-0.0.3/LICENSE
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1064 2023-07-06 03:13:10.354245 xxx-chat-0.0.3/PKG-INFO
+-rw-r--r--   0 taofoxtel   (503) staff       (20)      665 2023-07-05 09:36:04.000000 xxx-chat-0.0.3/README.md
+-rw-r--r--   0 taofoxtel   (503) staff       (20)       38 2023-07-06 03:13:10.354593 xxx-chat-0.0.3/setup.cfg
+-rw-r--r--   0 taofoxtel   (503) staff       (20)      819 2023-07-06 03:13:02.000000 xxx-chat-0.0.3/setup.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:13:10.347647 xxx-chat-0.0.3/xxx_chat.egg-info/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1064 2023-07-06 03:13:10.000000 xxx-chat-0.0.3/xxx_chat.egg-info/PKG-INFO
+-rw-r--r--   0 taofoxtel   (503) staff       (20)      553 2023-07-06 03:13:10.000000 xxx-chat-0.0.3/xxx_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        1 2023-07-06 03:13:10.000000 xxx-chat-0.0.3/xxx_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 taofoxtel   (503) staff       (20)       54 2023-07-06 03:13:10.000000 xxx-chat-0.0.3/xxx_chat.egg-info/entry_points.txt
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        6 2023-07-06 03:13:10.000000 xxx-chat-0.0.3/xxx_chat.egg-info/requires.txt
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        8 2023-07-06 03:13:10.000000 xxx-chat-0.0.3/xxx_chat.egg-info/top_level.txt
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:13:10.347990 xxx-chat-0.0.3/xxxchat/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:10:34.000000 xxx-chat-0.0.3/xxxchat/__init__.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:13:10.348497 xxx-chat-0.0.3/xxxchat/command/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.3/xxxchat/command/__init__.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1139 2023-07-06 03:11:32.000000 xxx-chat-0.0.3/xxxchat/command/__main__.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:13:10.349701 xxx-chat-0.0.3/xxxchat/commons/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.3/xxxchat/commons/__init__.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     2514 2023-07-06 03:11:32.000000 xxx-chat-0.0.3/xxxchat/commons/config.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:13:10.350531 xxx-chat-0.0.3/xxxchat/configuration/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.3/xxxchat/configuration/__init__.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1229 2023-07-06 03:11:32.000000 xxx-chat-0.0.3/xxxchat/configuration/profile_config.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:13:10.352303 xxx-chat-0.0.3/xxxchat/utils/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)      772 2023-07-06 01:29:12.000000 xxx-chat-0.0.3/xxxchat/utils/CommonUtil.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.3/xxxchat/utils/__init__.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     1506 2023-07-06 03:00:54.000000 xxx-chat-0.0.3/xxxchat/utils/logger.py
+drwxr-xr-x   0 taofoxtel   (503) staff       (20)        0 2023-07-06 03:13:10.353917 xxx-chat-0.0.3/xxxchat/xxx/
+-rw-r--r--   0 taofoxtel   (503) staff       (20)     2551 2023-07-06 03:11:32.000000 xxx-chat-0.0.3/xxxchat/xxx/CommandChat.py
+-rw-r--r--   0 taofoxtel   (503) staff       (20)        0 2023-04-12 09:19:49.000000 xxx-chat-0.0.3/xxxchat/xxx/__init__.py
```

### Comparing `xxx-chat-0.0.2/LICENSE` & `xxx-chat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xxx-chat-0.0.2/PKG-INFO` & `xxx-chat-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xxx-chat
-Version: 0.0.2
+Version: 0.0.3
 Summary: use command to chat with openai models, for :bear:
 Home-page: https://github.com/
 Author: xoto
 Author-email: xxx.tao.c@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xxx-chat-0.0.2/README.md` & `xxx-chat-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xxx-chat-0.0.2/command/__main__.py` & `xxx-chat-0.0.3/xxxchat/command/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import absolute_import
 
 import click
 import pkg_resources
 
-import utils.logger as logger
-from configuration.profile_config import add_profile, add_default_profile
-from utils.CommonUtil import waiting_stop
-from xxx.CommandChat import CommandChat
+import xxxchat.utils.logger as logger
+from xxxchat.configuration.profile_config import add_profile, add_default_profile
+from xxxchat.utils.CommonUtil import waiting_stop
+from xxxchat.xxx.CommandChat import CommandChat
 
 VERSION = pkg_resources.require("xxx-chat")[0].version
 
 
 @click.group()
 @click.version_option(version=VERSION, prog_name='xxx-chat')
 def commandchat_operator():
```

### Comparing `xxx-chat-0.0.2/commons/config.py` & `xxx-chat-0.0.3/xxxchat/commons/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import configparser
 import logging
 import os
 
 import pkg_resources
 
-import utils.logger as logger
+import xxxchat.utils.logger as logger
 
 config = configparser.SafeConfigParser()
 
 def get_home_path():
     homedir = os.environ.get('HOME', None)
     if os.name == 'nt':
         homedir = os.path.expanduser('~')
```

### Comparing `xxx-chat-0.0.2/configuration/profile_config.py` & `xxx-chat-0.0.3/xxxchat/configuration/profile_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import click
 
-import commons.config as config
-import utils.logger as logger
+from xxxchat import commons as config
+import xxxchat.utils.logger as logger
 
 
 def add_default_profile():
     api_key = click.prompt(logger.style('\n[default] Your default api_key '),
-                             default=config.get_default_env("api_key"), type=str)
+                           default=config.get_default_env("api_key"), type=str)
     config.set_env('default', 'api_key', api_key)
     limit_history = click.prompt(logger.style('\n[default] Your default limit_history '),
-                             default=config.get_default_env("limit_history"), type=str)
+                                 default=config.get_default_env("limit_history"), type=str)
     config.set_env('default', 'limit_history', limit_history)
 
 
 def input_config_vars(profile_name, key_name, is_default_exist):
     if is_default_exist:
         default_value = config.get_env('default', key_name)
         user_input = click.prompt(logger.style('\ndefault value  ' + key_name), default=default_value, type=str)
```

### Comparing `xxx-chat-0.0.2/setup.py` & `xxx-chat-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='xxx-chat',
-    version='0.0.2',
+    version='0.0.3',
     entry_points={
         'console_scripts': [
-            'xxx = command.__main__:main'
+            'xxx = xxxchat.command.__main__:main'
         ]
     },
     author="xoto",
     author_email="xxx.tao.c@gmail.com",
     description="use command to chat with openai models, for :bear:",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `xxx-chat-0.0.2/utils/CommonUtil.py` & `xxx-chat-0.0.3/xxxchat/utils/CommonUtil.py`

 * *Files identical despite different names*

### Comparing `xxx-chat-0.0.2/utils/logger.py` & `xxx-chat-0.0.3/xxxchat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `xxx-chat-0.0.2/xxx/CommandChat.py` & `xxx-chat-0.0.3/xxxchat/xxx/CommandChat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import http.client
 import json
 import os
 
-import utils.logger as logger
-from commons.config import get_env
-from utils.CommonUtil import waiting_start, waiting_stop
+import xxxchat.utils.logger as logger
+from xxxchat.commons.config import get_env
+from xxxchat.utils.CommonUtil import waiting_start, waiting_stop
 
 
 def get_home_path():
     homedir = os.environ.get('HOME', None)
     if os.name == 'nt':
         homedir = os.path.expanduser('~')
     return homedir
```

### Comparing `xxx-chat-0.0.2/xxx_chat.egg-info/PKG-INFO` & `xxx-chat-0.0.3/xxx_chat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xxx-chat
-Version: 0.0.2
+Version: 0.0.3
 Summary: use command to chat with openai models, for :bear:
 Home-page: https://github.com/
 Author: xoto
 Author-email: xxx.tao.c@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


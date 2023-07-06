# Comparing `tmp/chai-guanaco-1.0.2.tar.gz` & `tmp/chai-guanaco-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.0.2.tar", last modified: Thu Jul  6 19:39:29 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.0.3.tar", last modified: Thu Jul  6 23:11:29 2023, max compression
```

## Comparing `chai-guanaco-1.0.2.tar` & `chai-guanaco-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/
--rw-rw-r--   0 tom       (1002) tom       (1002)    10663 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     8969 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/README.md
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/
--rw-rw-r--   0 tom       (1002) tom       (1002)    10663 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     1221 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/chai_guanaco.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/requirements.txt
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/resources/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/resources/bot_config/
--rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/blade.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/captain_wyatt.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/coffee_shop_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/filbert.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/leo.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/levi.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/mr_wilson.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/nerd_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/scaramouche.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/story_teller.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/vampire_queen.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/resources/bot_config/wednesday_addams.json
--rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/setup.cfg
--rw-rw-r--   0 tom       (1002) tom       (1002)      925 2023-07-06 19:39:17.000000 chai-guanaco-1.0.2/setup.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/src/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/src/chai_guanaco/
--rw-rw-r--   0 tom       (1002) tom       (1002)      224 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/src/chai_guanaco/__init__.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     4853 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/src/chai_guanaco/chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3220 2023-07-04 17:14:25.000000 chai-guanaco-1.0.2/src/chai_guanaco/feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/src/chai_guanaco/formatters.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-06 19:37:53.000000 chai-guanaco-1.0.2/src/chai_guanaco/login_cli.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     6659 2023-07-06 19:37:53.000000 chai-guanaco-1.0.2/src/chai_guanaco/submit.py
--rw-rw-r--   0 tom       (1002) tom       (1002)      496 2023-07-04 17:14:25.000000 chai-guanaco-1.0.2/src/chai_guanaco/utils.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 19:39:29.000000 chai-guanaco-1.0.2/tests/
--rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-06 19:37:56.000000 chai-guanaco-1.0.2/tests/test_chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.2/tests/test_feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-04 17:14:25.000000 chai-guanaco-1.0.2/tests/test_login.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     6235 2023-07-04 17:14:25.000000 chai-guanaco-1.0.2/tests/test_submit.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/
+-rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-07-06 21:45:32.000000 chai-guanaco-1.0.3/MANIFEST.in
+-rw-rw-r--   0 tom       (1002) tom       (1002)    10663 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     8969 2023-07-06 23:07:27.000000 chai-guanaco-1.0.3/README.md
+-rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 21:12:53.000000 chai-guanaco-1.0.3/requirements.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/setup.cfg
+-rw-rw-r--   0 tom       (1002) tom       (1002)      988 2023-07-06 23:11:25.000000 chai-guanaco-1.0.3/setup.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco/
+-rw-rw-r--   0 tom       (1002) tom       (1002)      224 2023-07-06 21:12:53.000000 chai-guanaco-1.0.3/src/chai_guanaco/__init__.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3220 2023-07-04 17:14:25.000000 chai-guanaco-1.0.3/src/chai_guanaco/feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-06 19:37:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/formatters.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-06 21:12:53.000000 chai-guanaco-1.0.3/src/chai_guanaco/login_cli.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/blade.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/captain_wyatt.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/filbert.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/leo.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/levi.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/mr_wilson.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/nerd_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/scaramouche.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/story_teller.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/vampire_queen.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/wednesday_addams.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6659 2023-07-06 21:12:53.000000 chai-guanaco-1.0.3/src/chai_guanaco/submit.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)      496 2023-07-04 17:14:25.000000 chai-guanaco-1.0.3/src/chai_guanaco/utils.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/
+-rw-rw-r--   0 tom       (1002) tom       (1002)    10663 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1254 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/not-zip-safe
+-rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/tests/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-06 21:05:17.000000 chai-guanaco-1.0.3/tests/test_chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.3/tests/test_feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-04 17:14:25.000000 chai-guanaco-1.0.3/tests/test_login.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6235 2023-07-04 17:14:25.000000 chai-guanaco-1.0.3/tests/test_submit.py
```

### Comparing `chai-guanaco-1.0.2/PKG-INFO` & `chai-guanaco-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.2
+Version: 1.0.3
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -171,15 +171,15 @@
         ## Resources
         |                                                                        |                                                                                                 |
         | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
         | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
         | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
         | 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
         |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
-        |💬 [Example Conversations](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Here you can find 1000 example conversations from the Chai Platform     |
+        |💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
         | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
         
         
         ## 🦙 Hosted & Sponsored By
         
         <a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
```

### Comparing `chai-guanaco-1.0.2/README.md` & `chai-guanaco-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 ## Resources
 |                                                                        |                                                                                                 |
 | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
 | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
 | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
 | 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
 |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
-|💬 [Example Conversations](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Here you can find 1000 example conversations from the Chai Platform     |
+|💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
 | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
 
 
 ## 🦙 Hosted & Sponsored By
 
 <a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
```

### Comparing `chai-guanaco-1.0.2/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.0.3/src/chai_guanaco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.2
+Version: 1.0.3
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -171,15 +171,15 @@
         ## Resources
         |                                                                        |                                                                                                 |
         | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
         | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
         | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
         | 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
         |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
-        |💬 [Example Conversations](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Here you can find 1000 example conversations from the Chai Platform     |
+        |💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
         | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
         
         
         ## 🦙 Hosted & Sponsored By
         
         <a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
```

### Comparing `chai-guanaco-1.0.2/chai_guanaco.egg-info/SOURCES.txt` & `chai-guanaco-1.0.3/src/chai_guanaco.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,34 @@
+MANIFEST.in
 README.md
 requirements.txt
 setup.py
-./src/chai_guanaco/__init__.py
-./src/chai_guanaco/chat.py
-./src/chai_guanaco/feedback.py
-./src/chai_guanaco/formatters.py
-./src/chai_guanaco/login_cli.py
-./src/chai_guanaco/submit.py
-./src/chai_guanaco/utils.py
-chai_guanaco.egg-info/PKG-INFO
-chai_guanaco.egg-info/SOURCES.txt
-chai_guanaco.egg-info/dependency_links.txt
-chai_guanaco.egg-info/entry_points.txt
-chai_guanaco.egg-info/not-zip-safe
-chai_guanaco.egg-info/requires.txt
-chai_guanaco.egg-info/top_level.txt
-resources/bot_config/blade.json
-resources/bot_config/captain_wyatt.json
-resources/bot_config/coffee_shop_girl.json
-resources/bot_config/filbert.json
-resources/bot_config/leo.json
-resources/bot_config/levi.json
-resources/bot_config/mr_wilson.json
-resources/bot_config/nerd_girl.json
-resources/bot_config/scaramouche.json
-resources/bot_config/story_teller.json
-resources/bot_config/vampire_queen.json
-resources/bot_config/wednesday_addams.json
 src/chai_guanaco/__init__.py
 src/chai_guanaco/chat.py
 src/chai_guanaco/feedback.py
 src/chai_guanaco/formatters.py
 src/chai_guanaco/login_cli.py
 src/chai_guanaco/submit.py
 src/chai_guanaco/utils.py
+src/chai_guanaco.egg-info/PKG-INFO
+src/chai_guanaco.egg-info/SOURCES.txt
+src/chai_guanaco.egg-info/dependency_links.txt
+src/chai_guanaco.egg-info/entry_points.txt
+src/chai_guanaco.egg-info/not-zip-safe
+src/chai_guanaco.egg-info/requires.txt
+src/chai_guanaco.egg-info/top_level.txt
+src/chai_guanaco/resources/bot_config/blade.json
+src/chai_guanaco/resources/bot_config/captain_wyatt.json
+src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
+src/chai_guanaco/resources/bot_config/filbert.json
+src/chai_guanaco/resources/bot_config/leo.json
+src/chai_guanaco/resources/bot_config/levi.json
+src/chai_guanaco/resources/bot_config/mr_wilson.json
+src/chai_guanaco/resources/bot_config/nerd_girl.json
+src/chai_guanaco/resources/bot_config/scaramouche.json
+src/chai_guanaco/resources/bot_config/story_teller.json
+src/chai_guanaco/resources/bot_config/vampire_queen.json
+src/chai_guanaco/resources/bot_config/wednesday_addams.json
 tests/test_chat.py
 tests/test_feedback.py
 tests/test_login.py
 tests/test_submit.py
```

### Comparing `chai-guanaco-1.0.2/resources/bot_config/blade.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/blade.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/captain_wyatt.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/captain_wyatt.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/coffee_shop_girl.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/filbert.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/filbert.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/leo.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/leo.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/levi.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/levi.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/mr_wilson.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/mr_wilson.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/nerd_girl.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/nerd_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/scaramouche.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/scaramouche.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/story_teller.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/story_teller.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/vampire_queen.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/vampire_queen.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/resources/bot_config/wednesday_addams.json` & `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/wednesday_addams.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/setup.py` & `chai-guanaco-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
 else:
-    version = "1.0.2"
+    version = "1.0.3"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
     author='Chai Research Corp.',
     author_email='hello@chai-research.com',
     license='MIT',
-    packages=["chai_guanaco"],
-    package_dir={"chai_guanaco": "./src/chai_guanaco/"},
+    packages=find_packages(where='src'),
+    package_dir={"": "src"},
+    package_data={"chai_guanaco": ["resources/*"]},
     url='https://www.chai-research.com',
     zip_safe=False,
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=requirements,
+    include_package_data=True,
     entry_points={
-        'console_scripts': ['chai-guanaco = chai_guanaco.login_cli:cli'],
+        'console_scripts': ['chai-guanaco=chai_guanaco.login_cli:cli'],
     },
 )
```

### Comparing `chai-guanaco-1.0.2/src/chai_guanaco/chat.py` & `chai-guanaco-1.0.3/src/chai_guanaco/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from chai_guanaco.login_cli import auto_authenticate
 from chai_guanaco.utils import print_color
 
 
 BASE_URL = "https://guanaco-submitter.chai-research.com"
 
 REPO_PATH = os.path.dirname(os.path.abspath(__file__))
-RESOURCE_DIR = os.path.join(REPO_PATH, '..', '..', 'resources', 'bot_config')
+RESOURCE_DIR = os.path.join(REPO_PATH, 'resources', 'bot_config')
 
 
 class SubmissionChatbot():
     """
     Chat with a model that has been submitted and deployed to Chai Guanaco
 
     Attributes
```

### Comparing `chai-guanaco-1.0.2/src/chai_guanaco/feedback.py` & `chai-guanaco-1.0.3/src/chai_guanaco/feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/src/chai_guanaco/formatters.py` & `chai-guanaco-1.0.3/src/chai_guanaco/formatters.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/src/chai_guanaco/login_cli.py` & `chai-guanaco-1.0.3/src/chai_guanaco/login_cli.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/src/chai_guanaco/submit.py` & `chai-guanaco-1.0.3/src/chai_guanaco/submit.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/tests/test_chat.py` & `chai-guanaco-1.0.3/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/tests/test_feedback.py` & `chai-guanaco-1.0.3/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/tests/test_login.py` & `chai-guanaco-1.0.3/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.2/tests/test_submit.py` & `chai-guanaco-1.0.3/tests/test_submit.py`

 * *Files identical despite different names*


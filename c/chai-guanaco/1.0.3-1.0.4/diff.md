# Comparing `tmp/chai-guanaco-1.0.3.tar.gz` & `tmp/chai-guanaco-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.0.3.tar", last modified: Thu Jul  6 23:11:29 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.0.4.tar", last modified: Thu Jul  6 23:24:57 2023, max compression
```

## Comparing `chai-guanaco-1.0.3.tar` & `chai-guanaco-1.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/
--rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-07-06 21:45:32.000000 chai-guanaco-1.0.3/MANIFEST.in
--rw-rw-r--   0 tom       (1002) tom       (1002)    10663 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     8969 2023-07-06 23:07:27.000000 chai-guanaco-1.0.3/README.md
--rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 21:12:53.000000 chai-guanaco-1.0.3/requirements.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/setup.cfg
--rw-rw-r--   0 tom       (1002) tom       (1002)      988 2023-07-06 23:11:25.000000 chai-guanaco-1.0.3/setup.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco/
--rw-rw-r--   0 tom       (1002) tom       (1002)      224 2023-07-06 21:12:53.000000 chai-guanaco-1.0.3/src/chai_guanaco/__init__.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3220 2023-07-04 17:14:25.000000 chai-guanaco-1.0.3/src/chai_guanaco/feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-06 19:37:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/formatters.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-06 21:12:53.000000 chai-guanaco-1.0.3/src/chai_guanaco/login_cli.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/
--rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/blade.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/captain_wyatt.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/filbert.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/leo.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/levi.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/mr_wilson.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/nerd_girl.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/scaramouche.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/story_teller.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/vampire_queen.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-06 21:12:56.000000 chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/wednesday_addams.json
--rw-rw-r--   0 tom       (1002) tom       (1002)     6659 2023-07-06 21:12:53.000000 chai-guanaco-1.0.3/src/chai_guanaco/submit.py
--rw-rw-r--   0 tom       (1002) tom       (1002)      496 2023-07-04 17:14:25.000000 chai-guanaco-1.0.3/src/chai_guanaco/utils.py
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/
--rw-rw-r--   0 tom       (1002) tom       (1002)    10663 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1002) tom       (1002)     1254 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/src/chai_guanaco.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:11:29.000000 chai-guanaco-1.0.3/tests/
--rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-06 21:05:17.000000 chai-guanaco-1.0.3/tests/test_chat.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.3/tests/test_feedback.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-04 17:14:25.000000 chai-guanaco-1.0.3/tests/test_login.py
--rw-rw-r--   0 tom       (1002) tom       (1002)     6235 2023-07-04 17:14:25.000000 chai-guanaco-1.0.3/tests/test_submit.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/
+-rw-rw-r--   0 tom       (1002) tom       (1002)       47 2023-07-06 21:45:32.000000 chai-guanaco-1.0.4/MANIFEST.in
+-rw-rw-r--   0 tom       (1002) tom       (1002)    10662 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     8968 2023-07-06 23:24:38.000000 chai-guanaco-1.0.4/README.md
+-rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 21:12:53.000000 chai-guanaco-1.0.4/requirements.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       38 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/setup.cfg
+-rw-rw-r--   0 tom       (1002) tom       (1002)      988 2023-07-06 23:24:48.000000 chai-guanaco-1.0.4/setup.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/chai_guanaco/
+-rw-rw-r--   0 tom       (1002) tom       (1002)      224 2023-07-06 21:12:53.000000 chai-guanaco-1.0.4/src/chai_guanaco/__init__.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     4841 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3220 2023-07-04 17:14:25.000000 chai-guanaco-1.0.4/src/chai_guanaco/feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1756 2023-07-06 19:37:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/formatters.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1966 2023-07-06 21:12:53.000000 chai-guanaco-1.0.4/src/chai_guanaco/login_cli.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1332 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/blade.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1529 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/captain_wyatt.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2031 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1305 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/filbert.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1050 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/leo.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1053 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/levi.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1821 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/mr_wilson.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1094 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/nerd_girl.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2205 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/scaramouche.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1386 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/story_teller.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2510 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/vampire_queen.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2246 2023-07-06 21:12:56.000000 chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/wednesday_addams.json
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6659 2023-07-06 21:12:53.000000 chai-guanaco-1.0.4/src/chai_guanaco/submit.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)      496 2023-07-04 17:14:25.000000 chai-guanaco-1.0.4/src/chai_guanaco/utils.py
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/
+-rw-rw-r--   0 tom       (1002) tom       (1002)    10662 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1002) tom       (1002)     1254 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       61 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)        1 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/not-zip-safe
+-rw-rw-r--   0 tom       (1002) tom       (1002)       40 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1002) tom       (1002)       13 2023-07-06 23:24:56.000000 chai-guanaco-1.0.4/src/chai_guanaco.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1002) tom       (1002)        0 2023-07-06 23:24:57.000000 chai-guanaco-1.0.4/tests/
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3537 2023-07-06 21:05:17.000000 chai-guanaco-1.0.4/tests/test_chat.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     3454 2023-06-27 20:36:12.000000 chai-guanaco-1.0.4/tests/test_feedback.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     2842 2023-07-04 17:14:25.000000 chai-guanaco-1.0.4/tests/test_login.py
+-rw-rw-r--   0 tom       (1002) tom       (1002)     6235 2023-07-04 17:14:25.000000 chai-guanaco-1.0.4/tests/test_submit.py
```

### Comparing `chai-guanaco-1.0.3/PKG-INFO` & `chai-guanaco-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.3
+Version: 1.0.4
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -89,15 +89,15 @@
         
         
         **Chat With Your Model Submission**
         
         Once your model is deployed, you can verify its behaviour and raw input by running:
         
         ```python
-        chatbot = chai.ChatWithSubmission(submission_id)
+        chatbot = chai.SubmissionChatbot(submission_id)
         chatbot.chat('nerd_girl', show_model_input=False)
         ```
         
         Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
         
         You can get a list of avaliable bots by running:
```

### Comparing `chai-guanaco-1.0.3/README.md` & `chai-guanaco-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 
 **Chat With Your Model Submission**
 
 Once your model is deployed, you can verify its behaviour and raw input by running:
 
 ```python
-chatbot = chai.ChatWithSubmission(submission_id)
+chatbot = chai.SubmissionChatbot(submission_id)
 chatbot.chat('nerd_girl', show_model_input=False)
 ```
 
 Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
 
 You can get a list of avaliable bots by running:
```

### Comparing `chai-guanaco-1.0.3/setup.py` & `chai-guanaco-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
 else:
-    version = "1.0.3"
+    version = "1.0.4"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
     author='Chai Research Corp.',
     author_email='hello@chai-research.com',
```

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/chat.py` & `chai-guanaco-1.0.4/src/chai_guanaco/chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/feedback.py` & `chai-guanaco-1.0.4/src/chai_guanaco/feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/formatters.py` & `chai-guanaco-1.0.4/src/chai_guanaco/formatters.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/login_cli.py` & `chai-guanaco-1.0.4/src/chai_guanaco/login_cli.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/blade.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/blade.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/captain_wyatt.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/captain_wyatt.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/filbert.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/filbert.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/leo.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/leo.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/levi.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/levi.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/mr_wilson.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/mr_wilson.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/nerd_girl.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/nerd_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/scaramouche.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/scaramouche.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/story_teller.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/story_teller.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/vampire_queen.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/vampire_queen.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/resources/bot_config/wednesday_addams.json` & `chai-guanaco-1.0.4/src/chai_guanaco/resources/bot_config/wednesday_addams.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco/submit.py` & `chai-guanaco-1.0.4/src/chai_guanaco/submit.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.0.4/src/chai_guanaco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.0.3
+Version: 1.0.4
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
 Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
         
@@ -89,15 +89,15 @@
         
         
         **Chat With Your Model Submission**
         
         Once your model is deployed, you can verify its behaviour and raw input by running:
         
         ```python
-        chatbot = chai.ChatWithSubmission(submission_id)
+        chatbot = chai.SubmissionChatbot(submission_id)
         chatbot.chat('nerd_girl', show_model_input=False)
         ```
         
         Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
         
         You can get a list of avaliable bots by running:
```

### Comparing `chai-guanaco-1.0.3/src/chai_guanaco.egg-info/SOURCES.txt` & `chai-guanaco-1.0.4/src/chai_guanaco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/tests/test_chat.py` & `chai-guanaco-1.0.4/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/tests/test_feedback.py` & `chai-guanaco-1.0.4/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/tests/test_login.py` & `chai-guanaco-1.0.4/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.0.3/tests/test_submit.py` & `chai-guanaco-1.0.4/tests/test_submit.py`

 * *Files identical despite different names*


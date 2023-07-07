# Comparing `tmp/myass-0.1.0.tar.gz` & `tmp/myass-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myass-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "myass-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `myass-0.1.0.tar` & `myass-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1080 2023-07-06 18:58:54.600427 myass-0.1.0/LICENSE
--rw-r--r--   0        0        0       56 2023-07-06 22:09:52.816683 myass-0.1.0/README.md
--rw-r--r--   0        0        0      350 2023-07-06 22:07:47.717738 myass-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       35 2023-07-06 22:23:48.032975 myass-0.1.0/src/myass/__init__.py
--rw-r--r--   0        0        0      703 2023-07-06 22:16:05.939889 myass-0.1.0/src/myass/assistant.py
--rw-r--r--   0        0        0      306 2023-07-06 17:55:43.657716 myass-0.1.0/src/myass/config.py
--rw-r--r--   0        0        0      285 1970-01-01 00:00:00.000000 myass-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-06 18:58:54.600427 myass-0.1.1/LICENSE
+-rw-r--r--   0        0        0       56 2023-07-06 22:09:52.816683 myass-0.1.1/README.md
+-rw-r--r--   0        0        0      403 2023-07-07 14:41:42.624549 myass-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-07-07 14:39:12.385995 myass-0.1.1/src/myass/__init__.py
+-rw-r--r--   0        0        0      730 2023-07-07 14:37:11.663825 myass-0.1.1/src/myass/assistant.py
+-rw-r--r--   0        0        0      375 2023-07-07 14:43:46.730022 myass-0.1.1/src/myass/cli.py
+-rw-r--r--   0        0        0      306 2023-07-07 14:37:18.963754 myass-0.1.1/src/myass/config.py
+-rw-r--r--   0        0        0       25 2023-07-07 14:32:54.096308 myass-0.1.1/src/myass/config_default.yaml
+-rw-r--r--   0        0        0      306 1970-01-01 00:00:00.000000 myass-0.1.1/PKG-INFO
```

### Comparing `myass-0.1.0/LICENSE` & `myass-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myass-0.1.0/src/myass/assistant.py` & `myass-0.1.1/src/myass/assistant.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import copy
+
 import oaix
 
 import myass.config
 
 
 class Assistant:
     def __init__(self, name):
-        self.config = myass.config.Configuration(name)
+        self.config = myass.config.Config(name)
         self.api = oaix.Api()
+        self.messages = []
 
     def __call__(self, content=None, messages=None):
-        params = self.config.flatten()
-        try:
-            params['model']
-        except KeyError:
-            params['model'] = 'gpt-3.5-turbo'
+        params = copy.deepcopy(self.config.flatten())
         if messages is not None:
-            params['messages'].extend(messages)
+            self.messages.extend(messages)
         if content is not None:
-            params['messages'].append({'role': 'user', 'content': content})
+            self.messages.append({'role': 'user', 'content': content})
+        params['messages'].extend(self.messages)
         r = self.api.post('chat/completions', json=params)
         for choice in r['choices']:
             yield choice['message']['content']
+            self.messages.append(choice['message'])
```


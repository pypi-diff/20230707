# Comparing `tmp/llm-to-corpus-0.0.2.tar.gz` & `tmp/llm-to-corpus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-to-corpus-0.0.2.tar", last modified: Mon Jul  3 20:49:16 2023, max compression
+gzip compressed data, was "llm-to-corpus-0.0.3.tar", last modified: Fri Jul  7 11:22:08 2023, max compression
```

## Comparing `llm-to-corpus-0.0.2.tar` & `llm-to-corpus-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:49:16.900550 llm-to-corpus-0.0.2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-06-10 18:10:04.000000 llm-to-corpus-0.0.2/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2258 2023-07-03 20:49:16.900550 llm-to-corpus-0.0.2/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1657 2023-07-03 20:42:55.000000 llm-to-corpus-0.0.2/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:49:16.896550 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2258 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      398 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       61 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       37 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       18 2023-07-03 20:49:16.000000 llm-to-corpus-0.0.2/llm_to_corpus.egg-info/top_level.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-07-03 20:49:16.900550 llm-to-corpus-0.0.2/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1214 2023-07-03 20:45:37.000000 llm-to-corpus-0.0.2/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:49:16.896550 llm-to-corpus-0.0.2/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-03 20:49:16.900550 llm-to-corpus-0.0.2/src/llm_to_corpus/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1405 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/bloom.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1215 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/chatgpt.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3341 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/cli.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      931 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-07-03 20:46:18.000000 llm-to-corpus-0.0.2/src/llm_to_corpus/version.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-07 11:22:08.376189 llm-to-corpus-0.0.3/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-06-10 18:10:04.000000 llm-to-corpus-0.0.3/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2258 2023-07-07 11:22:08.376189 llm-to-corpus-0.0.3/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1657 2023-07-03 20:42:55.000000 llm-to-corpus-0.0.3/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-07 11:22:08.376189 llm-to-corpus-0.0.3/llm_to_corpus.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2258 2023-07-07 11:22:08.000000 llm-to-corpus-0.0.3/llm_to_corpus.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      398 2023-07-07 11:22:08.000000 llm-to-corpus-0.0.3/llm_to_corpus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-07-07 11:22:08.000000 llm-to-corpus-0.0.3/llm_to_corpus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       61 2023-07-07 11:22:08.000000 llm-to-corpus-0.0.3/llm_to_corpus.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       37 2023-07-07 11:22:08.000000 llm-to-corpus-0.0.3/llm_to_corpus.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       18 2023-07-07 11:22:08.000000 llm-to-corpus-0.0.3/llm_to_corpus.egg-info/top_level.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-07-07 11:22:08.376189 llm-to-corpus-0.0.3/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1214 2023-07-03 20:45:37.000000 llm-to-corpus-0.0.3/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-07 11:22:08.375189 llm-to-corpus-0.0.3/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-07-07 11:22:08.376189 llm-to-corpus-0.0.3/src/llm_to_corpus/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1405 2023-07-03 20:27:37.000000 llm-to-corpus-0.0.3/src/llm_to_corpus/bloom.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1264 2023-07-07 11:20:16.000000 llm-to-corpus-0.0.3/src/llm_to_corpus/chatgpt.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3341 2023-07-07 11:18:43.000000 llm-to-corpus-0.0.3/src/llm_to_corpus/cli.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      983 2023-07-07 11:20:16.000000 llm-to-corpus-0.0.3/src/llm_to_corpus/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-07-07 11:19:22.000000 llm-to-corpus-0.0.3/src/llm_to_corpus/version.py
```

### Comparing `llm-to-corpus-0.0.2/LICENSE` & `llm-to-corpus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.2/PKG-INFO` & `llm-to-corpus-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-to-corpus
-Version: 0.0.2
+Version: 0.0.3
 Summary: Large language model to corpus
 Home-page: https://github.com/jordimas/llm-to-corpus/
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `llm-to-corpus-0.0.2/README.md` & `llm-to-corpus-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.2/llm_to_corpus.egg-info/PKG-INFO` & `llm-to-corpus-0.0.3/llm_to_corpus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-to-corpus
-Version: 0.0.2
+Version: 0.0.3
 Summary: Large language model to corpus
 Home-page: https://github.com/jordimas/llm-to-corpus/
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `llm-to-corpus-0.0.2/setup.py` & `llm-to-corpus-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.2/src/llm_to_corpus/bloom.py` & `llm-to-corpus-0.0.3/src/llm_to_corpus/bloom.py`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.2/src/llm_to_corpus/chatgpt.py` & `llm-to-corpus-0.0.3/src/llm_to_corpus/chatgpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import openai
 import time
 
 
 class ChatGPT:
-    def __init__(self, prompt):
+    def __init__(self, prompt, model_name):
         self.prompt = prompt
+        self.model_name = model_name
 
     def query_thread(self, text, translations, index):
         #    print(f"translate_thread. Entry: {text}")
         while True:
             try:
                 completion = openai.ChatCompletion.create(
-                    model="gpt-3.5-turbo",
+                    model=self.model_name,
                     temperature=0,
                     max_tokens=2000,
                     messages=[
                         {
                             "role": "system",
                             "content": "You are a helpful assistant.",
                         },
```

### Comparing `llm-to-corpus-0.0.2/src/llm_to_corpus/cli.py` & `llm-to-corpus-0.0.3/src/llm_to_corpus/cli.py`

 * *Files identical despite different names*

### Comparing `llm-to-corpus-0.0.2/src/llm_to_corpus/models.py` & `llm-to-corpus-0.0.3/src/llm_to_corpus/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 from .chatgpt import ChatGPT
 from .bloom import Bloom
 
 
 class Models:
     MODELS_DESCRIPTION = {
         "gpt-3.5-turbo": "OpenAI most capable GPT-3.5 model",
+        "gpt-4": "OpenAI GPT 4.0 model",
         "mt0-xxl-mt": "Bloom's 13B parameter model finetuned on xP3",
     }
 
     def get_choices(self):
         return self.MODELS_DESCRIPTION.keys()
 
     def get_descriptions(self):
         return self.MODELS_DESCRIPTION
 
     def get_model(self, model_name, prompt):
-        if model_name == "gpt-3.5-turbo":
+        if model_name.startswith("gpt"):
             key = os.environ.get("OPENAI_API_KEY")
             if key is None or len(key) == 0:
                 raise RuntimeError(
                     "You should set OPENAI_API_KEY environment variable with you OpenAI key"
                 )
-            model = ChatGPT(prompt)
+            model = ChatGPT(prompt, model_name)
         elif model_name == "mt0-xxl-mt":
             model = Bloom(prompt)
         else:
             raise RuntimeError(f"Unknown model {model_name}")
 
         return model
```


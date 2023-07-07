# Comparing `tmp/BlitzChain-0.3.0.tar.gz` & `tmp/BlitzChain-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.3.0.tar", last modified: Mon Jul  3 10:53:48 2023, max compression
+gzip compressed data, was "BlitzChain-0.4.0.tar", last modified: Fri Jul  7 08:07:33 2023, max compression
```

## Comparing `BlitzChain-0.3.0.tar` & `BlitzChain-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 10:53:48.814935 BlitzChain-0.3.0/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 10:53:48.811730 BlitzChain-0.3.0/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-03 10:53:48.000000 BlitzChain-0.3.0/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-03 10:53:48.000000 BlitzChain-0.3.0/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-03 10:53:48.000000 BlitzChain-0.3.0/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-03 10:53:48.000000 BlitzChain-0.3.0/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-03 10:53:48.000000 BlitzChain-0.3.0/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.3.0/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-03 10:53:48.814731 BlitzChain-0.3.0/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.3.0/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 10:53:48.812790 BlitzChain-0.3.0/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-03 10:53:43.000000 BlitzChain-0.3.0/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     5898 2023-07-03 10:53:15.000000 BlitzChain-0.3.0/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 10:04:06.000000 BlitzChain-0.3.0/blitzchain/splitter.py
--rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.3.0/blitzchain/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 10:53:48.813257 BlitzChain-0.3.0/cli/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.3.0/cli/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.3.0/cli/main.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-03 10:53:48.814987 BlitzChain-0.3.0/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.3.0/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-03 10:53:48.814327 BlitzChain-0.3.0/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.3.0/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.3.0/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.3.0/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.092063 BlitzChain-0.4.0/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.088495 BlitzChain-0.4.0/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-07 08:07:33.000000 BlitzChain-0.4.0/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.4.0/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-07 08:07:33.091754 BlitzChain-0.4.0/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-07-07 08:06:07.000000 BlitzChain-0.4.0/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.089844 BlitzChain-0.4.0/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-07 08:06:26.000000 BlitzChain-0.4.0/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     5898 2023-07-07 08:06:27.000000 BlitzChain-0.4.0/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-07-03 10:04:06.000000 BlitzChain-0.4.0/blitzchain/splitter.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.4.0/blitzchain/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.090437 BlitzChain-0.4.0/cli/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.4.0/cli/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.4.0/cli/main.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-07 08:07:33.092154 BlitzChain-0.4.0/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.4.0/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-07 08:07:33.091343 BlitzChain-0.4.0/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.4.0/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.4.0/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.4.0/tests/test_qa.py
```

### Comparing `BlitzChain-0.3.0/LICENSE` & `BlitzChain-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.3.0/README.md` & `BlitzChain-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 ```
 
 ## Retrieving RAG Results
 
 ```python
 collection.generative_qa(
     user_input="Why?",
-    answer_fields=["content"],
+    prompt_fields=["content"],
 )
 ```
 
 # Documentation
 
 If you would like to read more about how to use this - 
 we recommend visiting [https://docs.twilix.io](https://docs.twilix.io)
```

### Comparing `BlitzChain-0.3.0/blitzchain/api.py` & `BlitzChain-0.4.0/blitzchain/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,27 +75,27 @@
             json={
                 "collection": self.collection_name,
                 "url": url
             }
         )
         return get_json_response(response)
     
-    def generative_qa(self, user_input: str, answer_fields: list,
+    def generative_qa(self, user_input: str, prompt_fields: list,
         conversation_id: str=None, limit: int=5, fields: list=None,
         include_rerank: bool=False, minimum_rerank_score: float=0.7,
         include_moderation: bool=False
     ):
         """Get an answer based on a question that you ask.
         """
         url =  self.base_url + "collection/generative-qa"
         print(url)
         data={
             "collection": self.collection_name,
             "userInput": user_input,
-            "answerFields": answer_fields,
+            "promptFields": prompt_fields,
             "limit": limit,
             "fields": fields,
             "includeRerank": include_rerank,
             "minimumRerankScore": minimum_rerank_score,
             "include_moderation": include_moderation
         }
         if conversation_id:
@@ -107,27 +107,27 @@
                 "Content-Type": "application/json",
                 "Authorization": "Bearer " + self.api_key
             },
             json=data
         )
         return get_json_response(response)
 
-    def copilot(self, user_input: str, answer_fields: list,
+    def copilot(self, user_input: str, prompt_fields: list,
         conversation_id: str=None, limit: int=5, fields: list=None,
         include_rerank: bool=False, minimum_rerank_score: float=0.7,
         include_moderation: bool=False
     ):
         """Get an answer based on a question that you ask.
         """
         url =  self.base_url + "collection/generative-code-qa"
         print(url)
         data={
             "collection": self.collection_name,
             "userInput": user_input,
-            "answerFields": answer_fields,
+            "promptFields": prompt_fields,
             "limit": limit,
             "fields": fields,
             "includeRerank": include_rerank,
             "minimumRerankScore": minimum_rerank_score,
             "includeModeration": include_moderation
         }
         if conversation_id:
```

### Comparing `BlitzChain-0.3.0/blitzchain/splitter.py` & `BlitzChain-0.4.0/blitzchain/splitter.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.3.0/blitzchain/utils.py` & `BlitzChain-0.4.0/blitzchain/utils.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.3.0/tests/test_pdf.py` & `BlitzChain-0.4.0/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.3.0/tests/test_qa.py` & `BlitzChain-0.4.0/tests/test_qa.py`

 * *Files identical despite different names*


# Comparing `tmp/langdash-1.7.0b0.tar.gz` & `tmp/langdash-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.7.0b0.tar", last modified: Wed Jun 28 08:04:36 2023, max compression
+gzip compressed data, was "langdash-1.7.1.tar", last modified: Fri Jul  7 17:44:09 2023, max compression
```

## Comparing `langdash-1.7.0b0.tar` & `langdash-1.7.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.072261 langdash-1.7.0b0/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.0b0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.0b0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3726 2023-06-28 08:04:36.068261 langdash-1.7.0b0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-23 20:18:20.000000 langdash-1.7.0b0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.064261 langdash-1.7.0b0/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-28 08:01:09.000000 langdash-1.7.0b0/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.068261 langdash-1.7.0b0/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.0b0/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14903 2023-06-28 07:18:05.000000 langdash-1.7.0b0/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.0b0/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.0b0/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.064261 langdash-1.7.0b0/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.0b0/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.0b0/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6738 2023-06-28 07:20:44.000000 langdash-1.7.0b0/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1341 2023-06-28 07:36:19.000000 langdash-1.7.0b0/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.0b0/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.0b0/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.068261 langdash-1.7.0b0/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.0b0/langdash/models/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.068261 langdash-1.7.0b0/langdash/models/_mixins/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.0b0/langdash/models/_mixins/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.0b0/langdash/models/_mixins/tensor_based_infer_mixin.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.068261 langdash-1.7.0b0/langdash/models/_tokenizer/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.0b0/langdash/models/_tokenizer/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.0b0/langdash/models/_tokenizer/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.7.0b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.0b0/langdash/models/_tokenizer/hf_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.0b0/langdash/models/_tokenizer/rwkv_tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.0b0/langdash/models/_tokenizer/tokenizer.py
--rw-rw-r--   0 user      (1000) user      (1000)     5280 2023-06-27 18:43:45.000000 langdash-1.7.0b0/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     4932 2023-06-27 18:24:11.000000 langdash-1.7.0b0/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.0b0/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     8993 2023-06-27 20:26:11.000000 langdash-1.7.0b0/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.0b0/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.0b0/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.0b0/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.0b0/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.064261 langdash-1.7.0b0/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.0b0/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.0b0/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.0b0/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.0b0/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-28 08:04:36.064261 langdash-1.7.0b0/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3726 2023-06-28 08:04:36.000000 langdash-1.7.0b0/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1654 2023-06-28 08:04:36.000000 langdash-1.7.0b0/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-28 08:04:36.000000 langdash-1.7.0b0/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      199 2023-06-28 08:04:36.000000 langdash-1.7.0b0/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-28 08:04:36.000000 langdash-1.7.0b0/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-28 08:04:36.072261 langdash-1.7.0b0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.0b0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.181198 langdash-1.7.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.7.1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.7.1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3724 2023-07-07 17:44:09.181198 langdash-1.7.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-23 20:18:20.000000 langdash-1.7.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.177197 langdash-1.7.1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       76 2023-07-07 17:41:14.000000 langdash-1.7.1/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.177197 langdash-1.7.1/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      177 2023-06-27 17:54:15.000000 langdash-1.7.1/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14903 2023-06-28 07:18:05.000000 langdash-1.7.1/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9394 2023-06-28 07:12:18.000000 langdash-1.7.1/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.7.1/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.173197 langdash-1.7.1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.7.1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.7.1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6738 2023-06-28 07:20:44.000000 langdash-1.7.1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1341 2023-06-28 07:36:19.000000 langdash-1.7.1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1661 2023-06-28 07:07:44.000000 langdash-1.7.1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9137 2023-06-28 07:27:22.000000 langdash-1.7.1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.181198 langdash-1.7.1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.7.1/langdash/models/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.181198 langdash-1.7.1/langdash/models/_mixins/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.1/langdash/models/_mixins/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3412 2023-06-21 10:26:00.000000 langdash-1.7.1/langdash/models/_mixins/tensor_based_infer_mixin.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.181198 langdash-1.7.1/langdash/models/_tokenizer/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-13 06:53:56.000000 langdash-1.7.1/langdash/models/_tokenizer/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-12 18:40:51.000000 langdash-1.7.1/langdash/models/_tokenizer/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1532 2023-06-13 05:07:37.000000 langdash-1.7.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2269 2023-06-21 10:26:00.000000 langdash-1.7.1/langdash/models/_tokenizer/hf_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1546 2023-06-22 00:31:04.000000 langdash-1.7.1/langdash/models/_tokenizer/rwkv_tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)      664 2023-06-13 05:07:37.000000 langdash-1.7.1/langdash/models/_tokenizer/tokenizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5280 2023-06-27 18:43:45.000000 langdash-1.7.1/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4932 2023-06-27 18:24:11.000000 langdash-1.7.1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.7.1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9063 2023-07-06 10:32:23.000000 langdash-1.7.1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.7.1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5632 2023-06-27 18:22:06.000000 langdash-1.7.1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.7.1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3450 2023-06-14 22:44:24.000000 langdash-1.7.1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.177197 langdash-1.7.1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.7.1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.7.1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.7.1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2861 2023-06-19 07:37:15.000000 langdash-1.7.1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-07 17:44:09.177197 langdash-1.7.1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3724 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1654 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      199 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-07-07 17:44:09.000000 langdash-1.7.1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-07 17:44:09.181198 langdash-1.7.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2023-06-23 20:18:20.000000 langdash-1.7.1/setup.py
```

### Comparing `langdash-1.7.0b0/LICENSE.txt` & `langdash-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/PKG-INFO` & `langdash-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.0b0
+Version: 1.7.1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.7.0b0/README.md` & `langdash-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/chains/chains.py` & `langdash-1.7.1/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/chains/nodes.py` & `langdash-1.7.1/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/classify/token_qa.py` & `langdash-1.7.1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/core.py` & `langdash-1.7.1/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/infer.py` & `langdash-1.7.1/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/llm.py` & `langdash-1.7.1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/llm_session.py` & `langdash-1.7.1/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/_mixins/tensor_based_infer_mixin.py` & `langdash-1.7.1/langdash/models/_mixins/tensor_based_infer_mixin.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/_tokenizer/_bpe.py` & `langdash-1.7.1/langdash/models/_tokenizer/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/_tokenizer/bytes_dict_tokenizer.py` & `langdash-1.7.1/langdash/models/_tokenizer/bytes_dict_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/_tokenizer/hf_tokenizer.py` & `langdash-1.7.1/langdash/models/_tokenizer/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/_tokenizer/rwkv_tokenizer.py` & `langdash-1.7.1/langdash/models/_tokenizer/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/_tokenizer/tokenizer.py` & `langdash-1.7.1/langdash/models/_tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/ctransformers.py` & `langdash-1.7.1/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/llama_cpp.py` & `langdash-1.7.1/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/mock.py` & `langdash-1.7.1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/rwkv_cpp.py` & `langdash-1.7.1/langdash/models/rwkv_cpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import langdash.sampling as sampling
 from ._tokenizer.rwkv_tokenizer import RwkvTokenizer
 from ._mixins.tensor_based_infer_mixin import TensorBasedInferMixin
 
 _rwkv_lib: Optional[str] = None
 _rwkv_cpp_folder: Optional[str] = None
 
-RWKV_CPP_COMMIT_DEFAULT = "6b26e0db28b26f0fb2c73c5aa6ff490818fb1456"
+RWKV_CPP_COMMIT_DEFAULT = "84634c047a9831b16cdf1cc3f2626e0ef0b2373b"
 RWKV_CPP_COMMIT = os.environ.get(
   "LANGDASH_RWKV_CPP_COMMIT", RWKV_CPP_COMMIT_DEFAULT
 )
 RWKV_CPP_FORCE_RECOMPILE = os.environ.get(
   "LANGDASH_RWKV_CPP_FORCE_RECOMPILE", ""
 ) == "1"
 RWKV_CPP_ENABLE_EVAL_SEQUENCE = os.environ.get(
@@ -160,16 +160,17 @@
       batch_size = self.batch_size
       for i in range(0, len(tokens), batch_size):
         logits_out, state = self.model.eval_sequence(
           tokens[i:i + batch_size], state, state, logits_out
         )
       return logits_out, state
     else:
-      for tokid in tokens:
-        logits_out, state = self.model.eval(tokid, state, state, logits_out)
+      for tokid in tokens[:-1]:
+        _, state = self.model.eval(tokid, state, state, None)
+      logits_out, state = self.model.eval(tokens[-1], state, state, logits_out)
       return logits_out, state
 
 
 class RwkvCppSession(
   TensorBasedInferMixin,
   LLMGenerationSessionForRawText["RwkvCppModel", RwkvCppState, torch.Tensor]
 ):
```

### Comparing `langdash-1.7.0b0/langdash/models/sentence_transformers.py` & `langdash-1.7.1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/models/transformers.py` & `langdash-1.7.1/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/response.py` & `langdash-1.7.1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/sampling.py` & `langdash-1.7.1/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/search/embedding_search.py` & `langdash-1.7.1/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/search/engine.py` & `langdash-1.7.1/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash/search/multichoice_search.py` & `langdash-1.7.1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/langdash.egg-info/PKG-INFO` & `langdash-1.7.1/langdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.7.0b0
+Version: 1.7.1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `langdash-1.7.0b0/langdash.egg-info/SOURCES.txt` & `langdash-1.7.1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.7.0b0/setup.py` & `langdash-1.7.1/setup.py`

 * *Files identical despite different names*


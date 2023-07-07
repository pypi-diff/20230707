# Comparing `tmp/doctran-0.0.4.tar.gz` & `tmp/doctran-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran-0.0.4.tar", max compression
+gzip compressed data, was "doctran-0.0.5.tar", max compression
```

## Comparing `doctran-0.0.4.tar` & `doctran-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.4/LICENSE
--rw-r--r--   0        0        0     8124 2023-07-07 20:26:59.304557 doctran-0.0.4/README.md
--rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.4/doctran/__init__.py
--rw-r--r--   0        0        0     7658 2023-07-07 20:36:08.795957 doctran-0.0.4/doctran/doctran.py
--rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.4/doctran/transformers/__init__.py
--rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.4/doctran/transformers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.4/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
--rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.4/doctran/transformers/__pycache__/prompts.cpython-310.pyc
--rw-r--r--   0        0        0    10879 2023-07-02 01:44:18.224865 doctran-0.0.4/doctran/transformers/__pycache__/transformers.cpython-310.pyc
--rw-r--r--   0        0        0    12106 2023-07-07 20:34:46.888870 doctran-0.0.4/doctran/transformers/transformers.py
--rw-r--r--   0        0        0      587 2023-07-07 21:33:59.256312 doctran-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8877 1970-01-01 00:00:00.000000 doctran-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.5/LICENSE
+-rw-r--r--   0        0        0     8124 2023-07-07 20:26:59.304557 doctran-0.0.5/README.md
+-rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.5/doctran/__init__.py
+-rw-r--r--   0        0        0     7658 2023-07-07 20:36:08.795957 doctran-0.0.5/doctran/doctran.py
+-rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.5/doctran/transformers/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.5/doctran/transformers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.5/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
+-rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.5/doctran/transformers/__pycache__/prompts.cpython-310.pyc
+-rw-r--r--   0        0        0    10879 2023-07-02 01:44:18.224865 doctran-0.0.5/doctran/transformers/__pycache__/transformers.cpython-310.pyc
+-rw-r--r--   0        0        0    12106 2023-07-07 20:34:46.888870 doctran-0.0.5/doctran/transformers/transformers.py
+-rw-r--r--   0        0        0      587 2023-07-07 21:41:14.704305 doctran-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8877 1970-01-01 00:00:00.000000 doctran-0.0.5/PKG-INFO
```

### Comparing `doctran-0.0.4/LICENSE` & `doctran-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran-0.0.4/README.md` & `doctran-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `doctran-0.0.4/doctran/doctran.py` & `doctran-0.0.5/doctran/doctran.py`

 * *Files identical despite different names*

### Comparing `doctran-0.0.4/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc` & `doctran-0.0.5/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.4/doctran/transformers/__pycache__/transformers.cpython-310.pyc` & `doctran-0.0.5/doctran/transformers/__pycache__/transformers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `doctran-0.0.4/doctran/transformers/transformers.py` & `doctran-0.0.5/doctran/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `doctran-0.0.4/pyproject.toml` & `doctran-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "doctran"
-version = "0.0.4"
+version = "0.0.5"
 description = "Document transformation framework for vector based retrieval"
 authors = ["Jason Fan <jason.wc.fan@gmail.com>", "Ayan Bandyopadhyay <ayanb9440@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pydantic = "^1.10.9"
 lxml = "^4.9.2"
 openai = "^0.27.8"
 presidio-analyzer = "^2.2.33"
 presidio-anonymizer = "^2.2.33"
 spacy = "^3.5.4"
-tiktoken = "^0.4.0"
+tiktoken = "^0.3.3"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `doctran-0.0.4/PKG-INFO` & `doctran-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: doctran
-Version: 0.0.4
+Version: 0.0.5
 Summary: Document transformation framework for vector based retrieval
 Author: Jason Fan
 Author-email: jason.wc.fan@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: presidio-analyzer (>=2.2.33,<3.0.0)
 Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: spacy (>=3.5.4,<4.0.0)
-Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Description-Content-Type: text/markdown
 
 <h2 align="center">
 🐛 Doctran
 </h2>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: doctran Version: 0.0.4 Summary: Document
+Metadata-Version: 2.1 Name: doctran Version: 0.0.5 Summary: Document
 transformation framework for vector based retrieval Author: Jason Fan Author-
 email: jason.wc.fan@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-Dist: presidio-analyzer
 (>=2.2.33,<3.0.0) Requires-Dist: presidio-anonymizer (>=2.2.33,<3.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0) Requires-Dist: spacy (>=3.5.4,<4.0.0)
-Requires-Dist: tiktoken (>=0.4.0,<0.5.0) Description-Content-Type: text/
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0) Description-Content-Type: text/
 markdown
                            ***** ð Doctran *****
       Document transformation framework to improve vector search results
                                     [Slack]
  [License] [Issues] [Twitter]
 Vector databases are useful for retrieving context for LLMs, however they
 struggle to find relevant information if the source documents are indexed
```


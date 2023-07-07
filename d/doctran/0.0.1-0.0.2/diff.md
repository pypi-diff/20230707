# Comparing `tmp/doctran-0.0.1.tar.gz` & `tmp/doctran-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran-0.0.1.tar", max compression
+gzip compressed data, was "doctran-0.0.2.tar", max compression
```

## Comparing `doctran-0.0.1.tar` & `doctran-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.1/LICENSE
--rw-r--r--   0        0        0     4562 2023-07-02 14:08:09.069031 doctran-0.0.1/README.md
--rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.1/doctran/__init__.py
--rw-r--r--   0        0        0     7533 2023-07-02 02:13:13.276556 doctran-0.0.1/doctran/doctran.py
--rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.1/doctran/transformers/__init__.py
--rw-r--r--   0        0        0    12122 2023-07-02 01:43:59.344967 doctran-0.0.1/doctran/transformers/transformers.py
--rw-r--r--   0        0        0      684 2023-07-02 15:08:24.397662 doctran-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 doctran-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.2/LICENSE
+-rw-r--r--   0        0        0     8028 2023-07-02 17:43:40.049930 doctran-0.0.2/README.md
+-rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.2/doctran/__init__.py
+-rw-r--r--   0        0        0     7684 2023-07-07 17:58:31.686595 doctran-0.0.2/doctran/doctran.py
+-rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.2/doctran/transformers/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-01 18:31:07.391598 doctran-0.0.2/doctran/transformers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8900 2023-06-30 02:26:08.286700 doctran-0.0.2/doctran/transformers/__pycache__/document_transformers.cpython-310.pyc
+-rw-r--r--   0        0        0      462 2023-06-29 15:35:41.652339 doctran-0.0.2/doctran/transformers/__pycache__/prompts.cpython-310.pyc
+-rw-r--r--   0        0        0    10879 2023-07-02 01:44:18.224865 doctran-0.0.2/doctran/transformers/__pycache__/transformers.cpython-310.pyc
+-rw-r--r--   0        0        0    12122 2023-07-02 01:43:59.344967 doctran-0.0.2/doctran/transformers/transformers.py
+-rw-r--r--   0        0        0      684 2023-07-07 18:00:27.310514 doctran-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8930 1970-01-01 00:00:00.000000 doctran-0.0.2/PKG-INFO
```

### Comparing `doctran-0.0.1/LICENSE` & `doctran-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `doctran-0.0.1/doctran/doctran.py` & `doctran-0.0.2/doctran/doctran.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import importlib
+import yaml
 import openai
 import uuid
 from enum import Enum
 import spacy
 from presidio_analyzer import AnalyzerEngine
 from presidio_analyzer.nlp_engine import NlpEngineProvider
 from presidio_anonymizer import AnonymizerEngine
@@ -79,14 +80,18 @@
     content_type: ContentType
     raw_content: str
     transformed_content: str
     config: DoctranConfig
     extracted_properties: Optional[Dict[str, Any]] = {}
     metadata: Optional[Dict[str, Any]] = None
 
+    def properties_as_yaml(self) -> str:
+        yaml_out = yaml.dump(self.extracted_properties, sort_keys=False)
+        return yaml_out
+
     def extract(self, *, properties: List[ExtractProperty]) -> 'DocumentTransformationBuilder':
         transformation_builder = DocumentTransformationBuilder(self)
         transformation_builder.extract(properties=properties)
         return transformation_builder
     
     def summarize(self, token_limit: int) -> 'DocumentTransformationBuilder':
         transformation_builder = DocumentTransformationBuilder(self)
```

### Comparing `doctran-0.0.1/doctran/transformers/transformers.py` & `doctran-0.0.2/doctran/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `doctran-0.0.1/pyproject.toml` & `doctran-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doctran"
-version = "0.0.1"
+version = "0.0.2"
 description = "Document transformation framework for vector based retrieval"
 authors = ["Jason Fan <jason.wc.fan@gmail.com>", "Ayan Bandyopadhyay <ayanb9440@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.9"
```


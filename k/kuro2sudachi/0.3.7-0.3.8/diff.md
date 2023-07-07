# Comparing `tmp/kuro2sudachi-0.3.7.tar.gz` & `tmp/kuro2sudachi-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuro2sudachi-0.3.7.tar", max compression
+gzip compressed data, was "kuro2sudachi-0.3.8.tar", max compression
```

## Comparing `kuro2sudachi-0.3.7.tar` & `kuro2sudachi-0.3.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2904 2023-06-26 15:47:20.263852 kuro2sudachi-0.3.7/README.md
--rw-r--r--   0        0        0      659 2023-07-07 12:03:17.498785 kuro2sudachi-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.3.7/src/kuro2sudachi/__init__.py
--rw-r--r--   0        0        0     6492 2023-07-07 11:56:16.740436 kuro2sudachi-0.3.7/src/kuro2sudachi/core.py
--rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.3.7/src/kuro2sudachi/normalizer.py
--rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.3.7/src/kuro2sudachi/rewrite.def
--rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 kuro2sudachi-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     2904 2023-06-26 15:47:20.263852 kuro2sudachi-0.3.8/README.md
+-rw-r--r--   0        0        0      676 2023-07-07 17:33:33.868630 kuro2sudachi-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 15:47:20.267195 kuro2sudachi-0.3.8/src/kuro2sudachi/__init__.py
+-rw-r--r--   0        0        0     6438 2023-07-07 17:40:23.845774 kuro2sudachi-0.3.8/src/kuro2sudachi/core.py
+-rw-r--r--   0        0        0     2736 2023-06-26 15:47:20.267634 kuro2sudachi-0.3.8/src/kuro2sudachi/normalizer.py
+-rw-r--r--   0        0        0     5426 2023-06-26 15:47:20.267809 kuro2sudachi-0.3.8/src/kuro2sudachi/rewrite.def
+-rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 kuro2sudachi-0.3.8/PKG-INFO
```

### Comparing `kuro2sudachi-0.3.7/README.md` & `kuro2sudachi-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.3.7/pyproject.toml` & `kuro2sudachi-0.3.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuro2sudachi"
-version = "0.3.7"
+version = "0.3.8"
 description = ""
 authors = ["po3rin"]
 repository = "http://github.com/po3rin/kuro2sudachi"
 homepage = "http://github.com/po3rin/kuro2sudachi"
 readme = "README.md"
 license = "Apache-2.0"
 include = ["rewrite.def"]
@@ -12,18 +12,19 @@
 [tool.poetry.scripts]
 kuro2sudachi = "kuro2sudachi.core:cli"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 jaconv = "^0.2.4"
 importlib-metadata = "^6.7.0"
-sudachipy = "^0.5.2"
+sudachipy = "^0.6.7"
 sudachidict-core = "^20230110"
 sudachidict-full = "^20230110"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^6.2.1"
+twine = "^4.0.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `kuro2sudachi-0.3.7/src/kuro2sudachi/core.py` & `kuro2sudachi-0.3.8/src/kuro2sudachi/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from sudachipy import dictionary
-from sudachipy import tokenizer
-from sudachipy.plugin import oov
+from sudachipy import dictionary, tokenizer
 from kuro2sudachi.normalizer import SudachiCharNormalizer
 import jaconv
 import fileinput
 import argparse
 import json
 import os
 import re
```

### Comparing `kuro2sudachi-0.3.7/src/kuro2sudachi/normalizer.py` & `kuro2sudachi-0.3.8/src/kuro2sudachi/normalizer.py`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.3.7/src/kuro2sudachi/rewrite.def` & `kuro2sudachi-0.3.8/src/kuro2sudachi/rewrite.def`

 * *Files identical despite different names*

### Comparing `kuro2sudachi-0.3.7/PKG-INFO` & `kuro2sudachi-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuro2sudachi
-Version: 0.3.7
+Version: 0.3.8
 Summary: 
 Home-page: http://github.com/po3rin/kuro2sudachi
 License: Apache-2.0
 Author: po3rin
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: importlib-metadata (>=6.7.0,<7.0.0)
 Requires-Dist: jaconv (>=0.2.4,<0.3.0)
 Requires-Dist: sudachidict-core (>=20230110,<20230111)
 Requires-Dist: sudachidict-full (>=20230110,<20230111)
-Requires-Dist: sudachipy (>=0.5.2,<0.6.0)
+Requires-Dist: sudachipy (>=0.6.7,<0.7.0)
 Project-URL: Repository, http://github.com/po3rin/kuro2sudachi
 Description-Content-Type: text/markdown
 
 # kuro2sudachi
 
 [![PyPi version](https://img.shields.io/pypi/v/kuro2sudachi.svg)](https://pypi.python.org/pypi/kuro2sudachi/)
 ![PyTest](https://github.com/po3rin/kuro2sudachi/workflows/PyTest/badge.svg)
```


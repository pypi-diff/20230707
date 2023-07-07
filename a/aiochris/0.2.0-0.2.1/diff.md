# Comparing `tmp/aiochris-0.2.0.tar.gz` & `tmp/aiochris-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiochris-0.2.0.tar", max compression
+gzip compressed data, was "aiochris-0.2.1.tar", max compression
```

## Comparing `aiochris-0.2.0.tar` & `aiochris-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-04-25 22:52:21.857534 aiochris-0.2.0/LICENSE
--rw-r--r--   0        0        0     1738 2023-04-25 22:52:21.857534 aiochris-0.2.0/README.md
--rw-r--r--   0        0        0      574 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/__init__.py
--rw-r--r--   0        0        0     6243 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/admin.py
--rw-r--r--   0        0        0     1335 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/anon.py
--rw-r--r--   0        0        0     9627 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/authed.py
--rw-r--r--   0        0        0     3495 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/base.py
--rw-r--r--   0        0        0     1707 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/normal.py
--rw-r--r--   0        0        0     2284 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/examples.md
--rw-r--r--   0        0        0     4811 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/home.md
--rw-r--r--   0        0        0       97 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/__init__.py
--rw-r--r--   0        0        0     1143 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/collection_client.py
--rw-r--r--   0        0        0     4969 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/http.py
--rw-r--r--   0        0        0     4664 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/linked.py
--rw-r--r--   0        0        0     1450 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/metaprog.py
--rw-r--r--   0        0        0        0 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/__init__.py
--rw-r--r--   0        0        0     1638 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/collection_links.py
--rw-r--r--   0        0        0     2912 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/data.py
--rw-r--r--   0        0        0      644 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/enums.py
--rw-r--r--   0        0        0     5061 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/logged_in.py
--rw-r--r--   0        0        0      833 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/public.py
--rw-r--r--   0        0        0     3118 2023-04-25 22:52:21.861534 aiochris-0.2.0/aiochris/models/types.py
--rw-r--r--   0        0        0       31 2023-04-25 22:52:21.861534 aiochris-0.2.0/aiochris/util/__init__.py
--rw-r--r--   0        0        0      698 2023-04-25 22:52:21.861534 aiochris-0.2.0/aiochris/util/errors.py
--rw-r--r--   0        0        0     6920 2023-04-25 22:52:21.861534 aiochris-0.2.0/aiochris/util/search.py
--rw-r--r--   0        0        0      768 2023-04-25 22:52:21.861534 aiochris-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 aiochris-0.2.0/setup.py
--rw-r--r--   0        0        0     2368 1970-01-01 00:00:00.000000 aiochris-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-07 17:16:46.450027 aiochris-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1738 2023-07-07 17:16:46.450027 aiochris-0.2.1/README.md
+-rw-r--r--   0        0        0      574 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/__init__.py
+-rw-r--r--   0        0        0     6243 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/admin.py
+-rw-r--r--   0        0        0     1335 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/anon.py
+-rw-r--r--   0        0        0     9627 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/authed.py
+-rw-r--r--   0        0        0     3495 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/base.py
+-rw-r--r--   0        0        0     1707 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/client/normal.py
+-rw-r--r--   0        0        0     2284 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/examples.md
+-rw-r--r--   0        0        0     4811 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/home.md
+-rw-r--r--   0        0        0       97 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/collection_client.py
+-rw-r--r--   0        0        0     4969 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/http.py
+-rw-r--r--   0        0        0     4664 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/linked.py
+-rw-r--r--   0        0        0     1450 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/link/metaprog.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/__init__.py
+-rw-r--r--   0        0        0     1638 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/collection_links.py
+-rw-r--r--   0        0        0     2912 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/data.py
+-rw-r--r--   0        0        0      644 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/enums.py
+-rw-r--r--   0        0        0     5061 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/logged_in.py
+-rw-r--r--   0        0        0      833 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/public.py
+-rw-r--r--   0        0        0     3118 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/models/types.py
+-rw-r--r--   0        0        0       31 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/util/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/util/errors.py
+-rw-r--r--   0        0        0     6920 2023-07-07 17:16:46.450027 aiochris-0.2.1/aiochris/util/search.py
+-rw-r--r--   0        0        0      782 2023-07-07 17:16:46.450027 aiochris-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 aiochris-0.2.1/PKG-INFO
```

### Comparing `aiochris-0.2.0/LICENSE` & `aiochris-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/README.md` & `aiochris-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/__init__.py` & `aiochris-0.2.1/aiochris/__init__.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/client/admin.py` & `aiochris-0.2.1/aiochris/client/admin.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/client/anon.py` & `aiochris-0.2.1/aiochris/client/anon.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/client/authed.py` & `aiochris-0.2.1/aiochris/client/authed.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/client/base.py` & `aiochris-0.2.1/aiochris/client/base.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/client/normal.py` & `aiochris-0.2.1/aiochris/client/normal.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/examples.md` & `aiochris-0.2.1/aiochris/examples.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/home.md` & `aiochris-0.2.1/aiochris/home.md`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/link/collection_client.py` & `aiochris-0.2.1/aiochris/link/collection_client.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/link/http.py` & `aiochris-0.2.1/aiochris/link/http.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/link/linked.py` & `aiochris-0.2.1/aiochris/link/linked.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/link/metaprog.py` & `aiochris-0.2.1/aiochris/link/metaprog.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/models/collection_links.py` & `aiochris-0.2.1/aiochris/models/collection_links.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/models/data.py` & `aiochris-0.2.1/aiochris/models/data.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/models/enums.py` & `aiochris-0.2.1/aiochris/models/enums.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/models/logged_in.py` & `aiochris-0.2.1/aiochris/models/logged_in.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/models/public.py` & `aiochris-0.2.1/aiochris/models/public.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/models/types.py` & `aiochris-0.2.1/aiochris/models/types.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/util/errors.py` & `aiochris-0.2.1/aiochris/util/errors.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/aiochris/util/search.py` & `aiochris-0.2.1/aiochris/util/search.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.2.0/pyproject.toml` & `aiochris-0.2.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "aiochris"
-version = "0.2.0"
+version = "0.2.1"
 description = "ChRIS client built on aiohttp"
 authors = ["FNNDSC <dev@babyMRI.org>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.3"
 
-# https://github.com/yukinarit/pyserde/issues/292
-pyserde = "^0.10.0"
+pyserde = "^0.11.1"
 async-property = "^0.2.1"
-yarl = "^1.8.2"
+# bug in yarl v1.9
+# https://github.com/aio-libs/yarl/issues/862
+yarl = "1.8.2"
 aiofiles = "^23.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 pre-commit = "^3.2.2"
 pytest-mock = "^3.10.0"
```

### Comparing `aiochris-0.2.0/PKG-INFO` & `aiochris-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aiochris
-Version: 0.2.0
+Version: 0.2.1
 Summary: ChRIS client built on aiohttp
 License: MIT
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: async-property (>=0.2.1,<0.3.0)
-Requires-Dist: pyserde (>=0.10.0,<0.11.0)
-Requires-Dist: yarl (>=1.8.2,<2.0.0)
+Requires-Dist: pyserde (>=0.11.1,<0.12.0)
+Requires-Dist: yarl (==1.8.2)
 Description-Content-Type: text/markdown
 
 # aiochris
 
 [![Tests](https://github.com/FNNDSC/aiochris/actions/workflows/test.yml/badge.svg)](https://github.com/FNNDSC/aiochris/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/FNNDSC/aiochris/branch/master/graph/badge.svg?token=48EEYZ3PUU)](https://codecov.io/gh/FNNDSC/aiochris)
 [![PyPI](https://img.shields.io/pypi/v/aiochris)](https://pypi.org/project/aiochris/)
```


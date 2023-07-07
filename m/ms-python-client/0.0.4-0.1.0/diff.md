# Comparing `tmp/ms_python_client-0.0.4.tar.gz` & `tmp/ms_python_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_python_client-0.0.4.tar", max compression
+gzip compressed data, was "ms_python_client-0.1.0.tar", max compression
```

## Comparing `ms_python_client-0.0.4.tar` & `ms_python_client-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     1100 2023-07-07 12:31:27.736644 ms_python_client-0.0.4/LICENSE
--rw-r--r--   0        0        0     5433 2023-07-07 12:31:27.736644 ms_python_client-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-07-07 12:31:27.736644 ms_python_client-0.0.4/ms_python_client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 12:31:27.736644 ms_python_client-0.0.4/ms_python_client/components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 12:31:27.736644 ms_python_client-0.0.4/ms_python_client/components/events/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 12:31:27.736644 ms_python_client-0.0.4/ms_python_client/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-07-07 12:31:27.736644 ms_python_client-0.0.4/ms_python_client/utils/logger.py
--rw-r--r--   0        0        0     1033 2023-07-07 12:31:27.736644 ms_python_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6187 1970-01-01 00:00:00.000000 ms_python_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5433 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/__init__.py
+-rw-r--r--   0        0        0     5332 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/api_client.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/components/events/__init__.py
+-rw-r--r--   0        0        0     5111 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/ms_api_client.py
+-rw-r--r--   0        0        0     1023 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/ms_client_interface.py
+-rw-r--r--   0        0        0        0 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/utils/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/utils/file_system.py
+-rw-r--r--   0        0        0     1276 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/utils/init_from_env.py
+-rw-r--r--   0        0        0      729 2023-07-07 15:32:03.054291 ms_python_client-0.1.0/ms_python_client/utils/logger.py
+-rw-r--r--   0        0        0     1034 2023-07-07 15:32:03.058291 ms_python_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 ms_python_client-0.1.0/PKG-INFO
```

### Comparing `ms_python_client-0.0.4/LICENSE` & `ms_python_client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.0.4/README.md` & `ms_python_client-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.0.4/ms_python_client/utils/logger.py` & `ms_python_client-0.1.0/ms_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.0.4/pyproject.toml` & `ms_python_client-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ms-python-client"
-version = "0.0.4"
+version = "0.1.0"
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
-description = "This package is used to interact with the microsoft grap API"
+description = "This package is used to interact with the microsoft graph API"
 authors = ["Samuel Guillemet <samuel.guillemet@telecom-sudparis.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ms_python_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ms_python_client-0.0.4/PKG-INFO` & `ms_python_client-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ms-python-client
-Version: 0.0.4
-Summary: This package is used to interact with the microsoft grap API
+Version: 0.1.0
+Summary: This package is used to interact with the microsoft graph API
 License: MIT
 Author: Samuel Guillemet
 Author-email: samuel.guillemet@telecom-sudparis.eu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


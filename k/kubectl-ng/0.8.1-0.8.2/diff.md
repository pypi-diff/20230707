# Comparing `tmp/kubectl_ng-0.8.1.tar.gz` & `tmp/kubectl_ng-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubectl_ng-0.8.1.tar", max compression
+gzip compressed data, was "kubectl_ng-0.8.2.tar", max compression
```

## Comparing `kubectl_ng-0.8.1.tar` & `kubectl_ng-0.8.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       80 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/README.md
--rw-r--r--   0        0        0      185 2023-07-06 14:11:29.525393 kubectl_ng-0.8.1/kubectl_ng/__init__.py
--rw-r--r--   0        0        0     4592 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/kubectl_ng/_api_resources.py
--rw-r--r--   0        0        0      769 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/kubectl_ng/_formatters.py
--rw-r--r--   0        0        0     4285 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/kubectl_ng/_get.py
--rw-r--r--   0        0        0     1981 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/kubectl_ng/_version.py
--rw-r--r--   0        0        0     5464 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/kubectl_ng/_wait.py
--rw-r--r--   0        0        0      758 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/kubectl_ng/cli.py
--rw-r--r--   0        0        0     1029 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/kubectl_ng/tests/test_formatters.py
--rw-r--r--   0        0        0      818 2023-07-06 14:11:10.949115 kubectl_ng-0.8.1/kubectl_ng/tests/test_version.py
--rw-r--r--   0        0        0      623 2023-07-06 14:11:29.525393 kubectl_ng-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 kubectl_ng-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/README.md
+-rw-r--r--   0        0        0      185 2023-07-07 11:06:51.582885 kubectl_ng-0.8.2/kubectl_ng/__init__.py
+-rw-r--r--   0        0        0     4592 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/kubectl_ng/_api_resources.py
+-rw-r--r--   0        0        0      769 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/kubectl_ng/_formatters.py
+-rw-r--r--   0        0        0     4285 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/kubectl_ng/_get.py
+-rw-r--r--   0        0        0     1981 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/kubectl_ng/_version.py
+-rw-r--r--   0        0        0     5464 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/kubectl_ng/_wait.py
+-rw-r--r--   0        0        0      758 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/kubectl_ng/cli.py
+-rw-r--r--   0        0        0     1029 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/kubectl_ng/tests/test_formatters.py
+-rw-r--r--   0        0        0      818 2023-07-07 11:06:34.846398 kubectl_ng-0.8.2/kubectl_ng/tests/test_version.py
+-rw-r--r--   0        0        0      623 2023-07-07 11:06:51.582885 kubectl_ng-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 kubectl_ng-0.8.2/PKG-INFO
```

### Comparing `kubectl_ng-0.8.1/kubectl_ng/_api_resources.py` & `kubectl_ng-0.8.2/kubectl_ng/_api_resources.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.8.1/kubectl_ng/_formatters.py` & `kubectl_ng-0.8.2/kubectl_ng/_formatters.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.8.1/kubectl_ng/_get.py` & `kubectl_ng-0.8.2/kubectl_ng/_get.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.8.1/kubectl_ng/_version.py` & `kubectl_ng-0.8.2/kubectl_ng/_version.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.8.1/kubectl_ng/_wait.py` & `kubectl_ng-0.8.2/kubectl_ng/_wait.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.8.1/kubectl_ng/cli.py` & `kubectl_ng-0.8.2/kubectl_ng/cli.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.8.1/kubectl_ng/tests/test_formatters.py` & `kubectl_ng-0.8.2/kubectl_ng/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.8.1/kubectl_ng/tests/test_version.py` & `kubectl_ng-0.8.2/kubectl_ng/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.8.1/pyproject.toml` & `kubectl_ng-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kubectl-ng"
-version = "0.8.1"
+version = "0.8.2"
 description = ""
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 readme = "README.md"
 packages = [{include = "kubectl_ng"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `kubectl_ng-0.8.1/PKG-INFO` & `kubectl_ng-0.8.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubectl-ng
-Version: 0.8.1
+Version: 0.8.2
 Summary: 
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


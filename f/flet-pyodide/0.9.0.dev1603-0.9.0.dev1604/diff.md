# Comparing `tmp/flet_pyodide-0.9.0.dev1603.tar.gz` & `tmp/flet_pyodide-0.9.0.dev1604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.9.0.dev1603.tar", max compression
+gzip compressed data, was "flet_pyodide-0.9.0.dev1604.tar", max compression
```

## Comparing `flet_pyodide-0.9.0.dev1603.tar` & `flet_pyodide-0.9.0.dev1604.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2264 2023-07-06 01:33:30.014795 flet_pyodide-0.9.0.dev1603/README.md
--rw-r--r--   0        0        0      644 2023-07-06 01:34:10.341675 flet_pyodide-0.9.0.dev1603/pyproject.toml
--rw-r--r--   0        0        0       61 2023-07-06 01:33:30.014795 flet_pyodide-0.9.0.dev1603/src/flet/__init__.py
--rw-r--r--   0        0        0       31 2023-07-06 01:33:30.014795 flet_pyodide-0.9.0.dev1603/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-06 01:33:30.014795 flet_pyodide-0.9.0.dev1603/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-07-06 01:33:30.014795 flet_pyodide-0.9.0.dev1603/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-07-06 01:33:30.014795 flet_pyodide-0.9.0.dev1603/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3851 2023-07-06 01:33:30.014795 flet_pyodide-0.9.0.dev1603/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2023-07-06 01:33:30.014795 flet_pyodide-0.9.0.dev1603/src/flet/version.py
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.9.0.dev1603/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-07-06 16:33:37.320957 flet_pyodide-0.9.0.dev1604/README.md
+-rw-r--r--   0        0        0      644 2023-07-06 16:34:13.236828 flet_pyodide-0.9.0.dev1604/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-07-06 16:33:37.320957 flet_pyodide-0.9.0.dev1604/src/flet/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-06 16:33:37.320957 flet_pyodide-0.9.0.dev1604/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-06 16:33:37.320957 flet_pyodide-0.9.0.dev1604/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-07-06 16:33:37.320957 flet_pyodide-0.9.0.dev1604/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-07-06 16:33:37.320957 flet_pyodide-0.9.0.dev1604/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3851 2023-07-06 16:33:37.320957 flet_pyodide-0.9.0.dev1604/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-07-06 16:33:37.320957 flet_pyodide-0.9.0.dev1604/src/flet/version.py
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.9.0.dev1604/PKG-INFO
```

### Comparing `flet_pyodide-0.9.0.dev1603/README.md` & `flet_pyodide-0.9.0.dev1604/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1603/pyproject.toml` & `flet_pyodide-0.9.0.dev1604/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.9.0.dev1603"
+version = "0.9.0.dev1604"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.9.0.dev1603"
+flet-core = "0.9.0.dev1604"
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `flet_pyodide-0.9.0.dev1603/src/flet/flet.py` & `flet_pyodide-0.9.0.dev1604/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1603/src/flet/pyodide_connection.py` & `flet_pyodide-0.9.0.dev1604/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.9.0.dev1603/PKG-INFO` & `flet_pyodide-0.9.0.dev1604/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.9.0.dev1603
+Version: 0.9.0.dev1604
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.9.0.dev1603)
+Requires-Dist: flet-core (==0.9.0.dev1604)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```


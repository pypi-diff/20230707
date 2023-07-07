# Comparing `tmp/flet_embed-0.9.0.dev1603.tar.gz` & `tmp/flet_embed-0.9.0.dev1604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_embed-0.9.0.dev1603.tar", max compression
+gzip compressed data, was "flet_embed-0.9.0.dev1604.tar", max compression
```

## Comparing `flet_embed-0.9.0.dev1603.tar` & `flet_embed-0.9.0.dev1604.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/README.md
--rw-r--r--   0        0        0      758 2023-07-06 01:34:09.689679 flet_embed-0.9.0.dev1603/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/src/flet/__init__.py
--rw-r--r--   0        0        0       32 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/src/flet/auth/__init__.py
--rw-r--r--   0        0        0       42 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/src/flet/auth/providers/__init__.py
--rw-r--r--   0        0        0       31 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0       55 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/src/flet/plotly_chart.py
--rw-r--r--   0        0        0       44 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/src/flet/utils/__init__.py
--rw-r--r--   0        0        0      103 2023-07-06 01:33:30.014795 flet_embed-0.9.0.dev1603/src/flet/version.py
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 flet_embed-0.9.0.dev1603/PKG-INFO
+-rw-r--r--   0        0        0      212 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/README.md
+-rw-r--r--   0        0        0      758 2023-07-06 16:34:12.688829 flet_embed-0.9.0.dev1604/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/src/flet/__init__.py
+-rw-r--r--   0        0        0       32 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/src/flet/auth/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/src/flet/auth/providers/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0       55 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0       44 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/src/flet/utils/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-06 16:33:37.320957 flet_embed-0.9.0.dev1604/src/flet/version.py
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 flet_embed-0.9.0.dev1604/PKG-INFO
```

### Comparing `flet_embed-0.9.0.dev1603/pyproject.toml` & `flet_embed-0.9.0.dev1604/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-embed"
-version = "0.9.0.dev1603"
+version = "0.9.0.dev1604"
 description = "Flet Embed - embed Python into Flutter apps"
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
-flet-runtime = "0.9.0.dev1603"
+flet-runtime = "0.9.0.dev1604"
 python = "^3.7"
 typing-extensions = { version = "^4.6.2", python = "<3.8" }
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.6"
 pytest = "^7.2.0"
```

### Comparing `flet_embed-0.9.0.dev1603/PKG-INFO` & `flet_embed-0.9.0.dev1604/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-embed
-Version: 0.9.0.dev1603
+Version: 0.9.0.dev1604
 Summary: Flet Embed - embed Python into Flutter apps
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-runtime (==0.9.0.dev1603)
+Requires-Dist: flet-runtime (==0.9.0.dev1604)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet embedded library
```

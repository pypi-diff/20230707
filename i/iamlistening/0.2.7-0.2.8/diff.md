# Comparing `tmp/iamlistening-0.2.7.tar.gz` & `tmp/iamlistening-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.2.7.tar", max compression
+gzip compressed data, was "iamlistening-0.2.8.tar", max compression
```

## Comparing `iamlistening-0.2.7.tar` & `iamlistening-0.2.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-06 13:18:14.182083 iamlistening-0.2.7/LICENSE
--rw-r--r--   0        0        0     3065 2023-07-06 13:18:14.182083 iamlistening-0.2.7/README.md
--rw-r--r--   0        0        0       99 2023-07-06 13:18:14.862084 iamlistening-0.2.7/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-06 13:18:14.186083 iamlistening-0.2.7/iamlistening/config.py
--rw-r--r--   0        0        0      805 2023-07-06 13:18:14.186083 iamlistening-0.2.7/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     3961 2023-07-06 13:18:14.186083 iamlistening-0.2.7/iamlistening/main.py
--rw-r--r--   0        0        0     2163 2023-07-06 13:18:14.858085 iamlistening-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 iamlistening-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-07 20:16:40.297994 iamlistening-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3065 2023-07-07 20:16:40.297994 iamlistening-0.2.8/README.md
+-rw-r--r--   0        0        0       99 2023-07-07 20:16:41.126000 iamlistening-0.2.8/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-07 20:16:40.297994 iamlistening-0.2.8/iamlistening/config.py
+-rw-r--r--   0        0        0      805 2023-07-07 20:16:40.297994 iamlistening-0.2.8/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3961 2023-07-07 20:16:40.297994 iamlistening-0.2.8/iamlistening/main.py
+-rw-r--r--   0        0        0     2341 2023-07-07 20:16:41.126000 iamlistening-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 iamlistening-0.2.8/PKG-INFO
```

### Comparing `iamlistening-0.2.7/LICENSE` & `iamlistening-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.7/README.md` & `iamlistening-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.7/iamlistening/config.py` & `iamlistening-0.2.8/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.7/iamlistening/default_settings.toml` & `iamlistening-0.2.8/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.7/iamlistening/main.py` & `iamlistening-0.2.8/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.7/pyproject.toml` & `iamlistening-0.2.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+
 [tool.poetry]
 name = "iamlistening"
-version = "0.2.7"
+version = "0.2.8"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
@@ -19,21 +24,38 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 telethon= "^1.28.5"
 py-cord= "^2.4.1"
 simplematrixbotlib= "^2.9.0"
 
+
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^7.34.3"
+
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^6.0.0"
+sphinx_bootstrap_theme = "^0.8.1"
+sphinx-autoapi = "^2.1.1"
+sphinx-copybutton= "^0.5.2"
+myst-parser = "^2.0.0"
+sphinx-notfound-page = "*"
+
+
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 
@@ -41,23 +63,14 @@
 omit = [
     "tests/*",
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
-[tool.poetry.group.docs.dependencies]
-sphinx = "^7.0.1"
-sphinx-autoapi = "^2.1.0"
-furo = "^2023.5.20"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","iamlistening/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
```

### Comparing `iamlistening-0.2.7/PKG-INFO` & `iamlistening-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


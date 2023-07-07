# Comparing `tmp/findmyorder-1.5.4.tar.gz` & `tmp/findmyorder-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.5.4.tar", max compression
+gzip compressed data, was "findmyorder-1.5.5.tar", max compression
```

## Comparing `findmyorder-1.5.4.tar` & `findmyorder-1.5.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-06 13:19:58.174734 findmyorder-1.5.4/LICENSE
--rw-r--r--   0        0        0     3046 2023-07-06 13:19:58.174734 findmyorder-1.5.4/README.md
--rw-r--r--   0        0        0      113 2023-07-06 13:19:58.998758 findmyorder-1.5.4/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-07-06 13:19:58.174734 findmyorder-1.5.4/findmyorder/config.py
--rw-r--r--   0        0        0     2848 2023-07-06 13:19:58.174734 findmyorder-1.5.4/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5780 2023-07-06 13:19:58.174734 findmyorder-1.5.4/findmyorder/main.py
--rw-r--r--   0        0        0     2132 2023-07-06 13:19:58.998758 findmyorder-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 findmyorder-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-07 20:11:59.409327 findmyorder-1.5.5/LICENSE
+-rw-r--r--   0        0        0     3046 2023-07-07 20:11:59.409327 findmyorder-1.5.5/README.md
+-rw-r--r--   0        0        0      113 2023-07-07 20:12:00.157332 findmyorder-1.5.5/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-07 20:11:59.409327 findmyorder-1.5.5/findmyorder/config.py
+-rw-r--r--   0        0        0     2495 2023-07-07 20:11:59.409327 findmyorder-1.5.5/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5779 2023-07-07 20:11:59.409327 findmyorder-1.5.5/findmyorder/main.py
+-rw-r--r--   0        0        0     2307 2023-07-07 20:12:00.157332 findmyorder-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 findmyorder-1.5.5/PKG-INFO
```

### Comparing `findmyorder-1.5.4/LICENSE` & `findmyorder-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.4/README.md` & `findmyorder-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.4/findmyorder/config.py` & `findmyorder-1.5.5/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.5.4/findmyorder/default_settings.toml` & `findmyorder-1.5.5/findmyorder/default_settings.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,14 @@
 # export TT_PORT=8081
 
 
 [default]
 VALUE = "Production - Default"
 findmyorder_enabled = true
 action_identifier = "BUY SELL LONG SHORT"
-# action_in_identifier = "BUY LONG"
-# action_out_identifier = "SELL SHORT"
-# actions = [
-#     { identifier = "BUY", type = "IN" },
-#     { identifier = "SELL", type = "OUT" },
-#     { identifier = "LONG", type = "IN" },
-#     { identifier = "SHORT", type = "OUT" }
-# ]
 stop_loss_identifier = "sl="
 take_profit_identifier = 'tp='
 quantity_identifier = 'q='
 order_type_identifier = "spot future margin"
 leverage_type_identifier = "cross isolated"
 comment_identifier = "comment="
 stop_loss = 1000
@@ -44,22 +36,20 @@
 
 
 
 [testing]
 VALUE = "On Testing"
 findmyorder_enabled = true
 action_identifier = "BUY SELL LONG SHORT"
-# action_in_identifier = "BUY LONG"
-# action_out_identifier = "SELL SHORT"
-# actions = [
-#     { identifier = "BUY", type = "IN" },
-#     { identifier = "SELL", type = "OUT" },
-#     { identifier = "LONG", type = "IN" },
-#     { identifier = "SHORT", type = "OUT" }
-# ]
+actions = [
+    { identifier = "BUY", type = "BUY" },
+    { identifier = "SELL", type = "SELL" },
+    { identifier = "LONG", type = "BUY" },
+    { identifier = "SHORT", type = "SELL" }
+]
 stop_loss_identifier = "sl="
 take_profit_identifier = 'tp='
 quantity_identifier = 'q='
 order_type_identifier = "spot future margin"
 leverage_type_identifier = "cross isolated"
 comment_identifier = "comment="
 stop_loss = 1000
```

### Comparing `findmyorder-1.5.4/findmyorder/main.py` & `findmyorder-1.5.5/findmyorder/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
             return e
 
     async def get_order(
         self,
         msg: str,
     ):
         """get an order."""
-
         if await self.search(msg):
             order = await self.identify_order(msg)
             if isinstance(order, dict):
                 order["timestamp"] = datetime.utcnow().strftime(
                     "%Y-%m-%dT%H:%M:%SZ")
             print(settings.instrument_mapping)
             if settings.instrument_mapping:
```

### Comparing `findmyorder-1.5.4/pyproject.toml` & `findmyorder-1.5.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+
 [tool.poetry]
 name = "findmyorder"
-version = "1.5.4"
+version = "1.5.5"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -12,27 +17,41 @@
 
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/findmyorder/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/findmyorder/discussions"
 "Issues" =  "https://github.com/mraniki/findmyorder/issues"
 
+
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 pyparsing = "^3.0.9"
 emoji = "^2.5.1"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^7.34.3"
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.0.0"
+sphinx_bootstrap_theme = "^0.8.1"
+sphinx-autoapi = "^2.1.1"
+sphinx-copybutton= "^0.5.2"
+myst-parser = "^2.0.0"
+sphinx-notfound-page = "*"
+
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 
@@ -40,23 +59,14 @@
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
 version_variable = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
```

### Comparing `findmyorder-1.5.4/PKG-INFO` & `findmyorder-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.5.4
+Version: 1.5.5
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.5.4 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.5.5 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist:
```


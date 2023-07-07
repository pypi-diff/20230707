# Comparing `tmp/parse2docs-0.1.2.tar.gz` & `tmp/parse2docs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse2docs-0.1.2.tar", max compression
+gzip compressed data, was "parse2docs-0.1.3.tar", max compression
```

## Comparing `parse2docs-0.1.2.tar` & `parse2docs-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-07-05 15:11:05.572033 parse2docs-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-07-05 08:28:22.956230 parse2docs-0.1.2/parse2docs/__init__.py
--rw-r--r--   0        0        0     1547 2023-07-05 16:59:52.093819 parse2docs-0.1.2/parse2docs/app.py
--rw-r--r--   0        0        0     1832 2023-07-05 13:10:09.703606 parse2docs-0.1.2/parse2docs/argfinder.py
--rw-r--r--   0        0        0     3414 2023-07-05 16:47:41.952690 parse2docs-0.1.2/parse2docs/markdown_renderer.py
--rw-r--r--   0        0        0      687 2023-07-05 16:58:17.189525 parse2docs-0.1.2/parse2docs/module_loader.py
--rw-r--r--   0        0        0      661 2023-07-05 17:00:46.053445 parse2docs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2219 2023-07-05 16:54:12.878792 parse2docs-0.1.2/README.md
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 parse2docs-0.1.2/setup.py
--rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 parse2docs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-07 19:08:04.727356 parse2docs-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2440 2023-07-07 19:08:04.727356 parse2docs-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 19:08:04.727356 parse2docs-0.1.3/parse2docs/__init__.py
+-rw-r--r--   0        0        0     1547 2023-07-07 19:08:04.727356 parse2docs-0.1.3/parse2docs/app.py
+-rw-r--r--   0        0        0     1779 2023-07-07 19:08:04.727356 parse2docs-0.1.3/parse2docs/argfinder.py
+-rw-r--r--   0        0        0     3411 2023-07-07 19:08:04.727356 parse2docs-0.1.3/parse2docs/markdown_renderer.py
+-rw-r--r--   0        0        0      687 2023-07-07 19:08:04.727356 parse2docs-0.1.3/parse2docs/module_loader.py
+-rw-r--r--   0        0        0      661 2023-07-07 19:08:04.727356 parse2docs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 parse2docs-0.1.3/PKG-INFO
```

### Comparing `parse2docs-0.1.2/LICENSE` & `parse2docs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parse2docs-0.1.2/parse2docs/app.py` & `parse2docs-0.1.3/parse2docs/app.py`

 * *Files identical despite different names*

### Comparing `parse2docs-0.1.2/parse2docs/argfinder.py` & `parse2docs-0.1.3/parse2docs/argfinder.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-"""Module for finding ArgumentParser objects in Python scripts."""
-
-import inspect
-from argparse import ArgumentParser
-from types import ModuleType
-
-
-def get_argparser_from_module(module: ModuleType) -> ArgumentParser:
-    """Find ArgumentParser in a given module.
-
-    This function first looks for argparse.ArgumentParser instances in the
-    module scope. If it doesn't find any, it then looks for functions that take
-    no parameters, executes them, and checks if they return an
-    argparse.ArgumentParser instance.
-
-    Returns:
-        ArgumentParser: ArgumentParser object from the Python script file.
-
-    Raises:
-        ValueError: If no ArgumentParser object is found in the provided file.
-    """
-
-    search_functions = [_find_parser_in_scope, _find_parser_in_functions]
-    parser = next((func(module) for func in search_functions if func(module)), None)
-
-    if parser is None:
-        raise ValueError("No ArgumentParser object found in the provided file.")
-
-    return parser
-
-
-def _find_parser_in_scope(module: ModuleType) -> ArgumentParser | None:
-    for _, obj in inspect.getmembers(module):
-        if isinstance(obj, ArgumentParser):
-            return obj
-
-
-def _find_parser_in_functions(module: ModuleType) -> ArgumentParser | None:
-    for _, obj in inspect.getmembers(module):
-        # We only care about functions
-        if not inspect.isfunction(obj):
-            continue
-
-        try:
-            # We only care about functions that take no parameters
-            if len(inspect.signature(obj).parameters) > 0:
-                continue
-            result = obj()
-            if isinstance(result, ArgumentParser):
-                return result
-        # If we can't inspect the function, just skip it
-        except TypeError:
-            pass
+"""Module for finding ArgumentParser objects in Python scripts."""
+
+import inspect
+from argparse import ArgumentParser
+from types import ModuleType
+
+
+def get_argparser_from_module(module: ModuleType) -> ArgumentParser:
+    """Find ArgumentParser in a given module.
+
+    This function first looks for argparse.ArgumentParser instances in the
+    module scope. If it doesn't find any, it then looks for functions that take
+    no parameters, executes them, and checks if they return an
+    argparse.ArgumentParser instance.
+
+    Returns:
+        ArgumentParser: ArgumentParser object from the Python script file.
+
+    Raises:
+        ValueError: If no ArgumentParser object is found in the provided file.
+    """
+
+    search_functions = [_find_parser_in_scope, _find_parser_in_functions]
+    parser = next((func(module) for func in search_functions if func(module)), None)
+
+    if parser is None:
+        raise ValueError("No ArgumentParser object found in the provided file.")
+
+    return parser
+
+
+def _find_parser_in_scope(module: ModuleType) -> ArgumentParser | None:
+    for _, obj in inspect.getmembers(module):
+        if isinstance(obj, ArgumentParser):
+            return obj
+
+
+def _find_parser_in_functions(module: ModuleType) -> ArgumentParser | None:
+    for _, obj in inspect.getmembers(module):
+        # We only care about functions
+        if not inspect.isfunction(obj):
+            continue
+
+        try:
+            # We only care about functions that take no parameters
+            if len(inspect.signature(obj).parameters) > 0:
+                continue
+            result = obj()
+            if isinstance(result, ArgumentParser):
+                return result
+        # If we can't inspect the function, just skip it
+        except TypeError:
+            pass
```

### Comparing `parse2docs-0.1.2/parse2docs/markdown_renderer.py` & `parse2docs-0.1.3/parse2docs/markdown_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return f"## Overall Usage Example\n\n`{script_name}`\n\n"
 
     return f"## Overall Usage Example\n\n`{script_name} {cmd_example}`\n\n"
 
 
 def _get_script_name() -> str:
     # Running from the command line, so the script name is the last argument
-    if sys.argv[0] == "parse2docs":
+    if "parse2docs" in sys.argv:
         return Path(sys.argv[-1]).name
 
     # When running from a module, the script name is the module name
     return Path(__file__).name
 
 
 def _get_example_value_from_action(action: Action) -> str:
```

### Comparing `parse2docs-0.1.2/parse2docs/module_loader.py` & `parse2docs-0.1.3/parse2docs/module_loader.py`

 * *Files identical despite different names*

### Comparing `parse2docs-0.1.2/pyproject.toml` & `parse2docs-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parse2docs"
-version = "0.1.2"
+version = "0.1.3"
 description = "Generate usage documentation from Python scripts using the `argparse` module"
 authors = ["Fernando Cordeiro"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `parse2docs-0.1.2/README.md` & `parse2docs-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # Parse 2 Docs
 
+![PyPI](https://img.shields.io/pypi/v/parse2docs)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Tests](https://github.com/MrCordeiro/parse2docs/actions/workflows/tests.yml/badge.svg)](https://github.com/MrCordeiro/parse2docs/actions/workflows/tests.yml)
+[![Linters](https://github.com/MrCordeiro/parse2docs/actions/workflows/linters.yml/badge.svg)](https://github.com/MrCordeiro/parse2docs/actions/workflows/linters.yml)
+
 `parse2docs` is a Python library that allows you to automatically generate usage documentation in Markdown format from Python scripts using the `argparse` module.
 
 ## Features
 
 * Scans the Python script for instances of `argparse.ArgumentParser`.
 * Generates a Markdown file with usage documentation based on the `ArgumentParser` object.
 * The generated documentation includes a table of contents, descriptions of each command line argument, and examples if provided.
 * Works with `ArgumentParser` instances declared at the module level or returned by functions.
 
 ## Installation
 
-### Via `pip`
-
 `parse2docs` can be installed via `pip`:
 
 ```shell
 pip install parse2docs
 ```
 
-### Via `poetry`
-
-`parse2docs` can be installed via Poetry. To install the library, clone this repository to your local machine and use Poetry to install:
-
-```shell
-git clone https://github.com/yourusername/parse2docs.git
-cd parse2docs
-poetry install
-```
-
 ## Usage
 
 There are two ways to use parse2docs, either as a Python module in your script or directly from the command line using the provided command.
 
 ### As a Python module
 
 ```python
```

### Comparing `parse2docs-0.1.2/PKG-INFO` & `parse2docs-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 Metadata-Version: 2.1
 Name: parse2docs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate usage documentation from Python scripts using the `argparse` module
 License: MIT
 Author: Fernando Cordeiro
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Parse 2 Docs
 
+![PyPI](https://img.shields.io/pypi/v/parse2docs)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Tests](https://github.com/MrCordeiro/parse2docs/actions/workflows/tests.yml/badge.svg)](https://github.com/MrCordeiro/parse2docs/actions/workflows/tests.yml)
+[![Linters](https://github.com/MrCordeiro/parse2docs/actions/workflows/linters.yml/badge.svg)](https://github.com/MrCordeiro/parse2docs/actions/workflows/linters.yml)
+
 `parse2docs` is a Python library that allows you to automatically generate usage documentation in Markdown format from Python scripts using the `argparse` module.
 
 ## Features
 
 * Scans the Python script for instances of `argparse.ArgumentParser`.
 * Generates a Markdown file with usage documentation based on the `ArgumentParser` object.
 * The generated documentation includes a table of contents, descriptions of each command line argument, and examples if provided.
 * Works with `ArgumentParser` instances declared at the module level or returned by functions.
 
 ## Installation
 
-### Via `pip`
-
 `parse2docs` can be installed via `pip`:
 
 ```shell
 pip install parse2docs
 ```
 
-### Via `poetry`
-
-`parse2docs` can be installed via Poetry. To install the library, clone this repository to your local machine and use Poetry to install:
-
-```shell
-git clone https://github.com/yourusername/parse2docs.git
-cd parse2docs
-poetry install
-```
-
 ## Usage
 
 There are two ways to use parse2docs, either as a Python module in your script or directly from the command line using the provided command.
 
 ### As a Python module
 
 ```python
```


# Comparing `tmp/clementine-2023.6.12.tar.gz` & `tmp/clementine-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clementine-2023.6.12.tar", last modified: Mon Jun 12 19:16:18 2023, max compression
+gzip compressed data, was "clementine-2023.7.7.tar", last modified: Fri Jul  7 18:41:10 2023, max compression
```

## Comparing `clementine-2023.6.12.tar` & `clementine-2023.7.7.tar`

### file list

```diff
@@ -1,24 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.316277 clementine-2023.6.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 19:16:05.000000 clementine-2023.6.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-12 19:16:18.316277 clementine-2023.6.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-12 19:16:05.000000 clementine-2023.6.12/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-12 19:16:05.000000 clementine-2023.6.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:16:18.316277 clementine-2023.6.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:16:05.000000 clementine-2023.6.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.312276 clementine-2023.6.12/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.316277 clementine-2023.6.12/src/clementine/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/blossom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.316277 clementine-2023.6.12/src/clementine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.316277 clementine-2023.6.12/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-12 19:16:05.000000 clementine-2023.6.12/tests/test_blossom.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-12 19:16:05.000000 clementine-2023.6.12/tests/test_clementine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:41:10.196844 clementine-2023.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 18:40:56.000000 clementine-2023.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-07 18:41:10.196844 clementine-2023.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-07 18:40:56.000000 clementine-2023.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-07 18:40:56.000000 clementine-2023.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:41:10.196844 clementine-2023.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:40:56.000000 clementine-2023.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:41:10.192844 clementine-2023.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:41:10.196844 clementine-2023.7.7/src/clementine/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:41:10.196844 clementine-2023.7.7/src/clementine/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/about/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/about/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:41:10.196844 clementine-2023.7.7/src/clementine/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:41:10.196844 clementine-2023.7.7/src/clementine/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/cli/commands/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/cli/commands/_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-07 18:40:56.000000 clementine-2023.7.7/src/clementine/screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:41:10.196844 clementine-2023.7.7/src/clementine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-07 18:41:10.000000 clementine-2023.7.7/src/clementine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-07 18:41:10.000000 clementine-2023.7.7/src/clementine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:41:10.000000 clementine-2023.7.7/src/clementine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 18:41:10.000000 clementine-2023.7.7/src/clementine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 18:41:10.000000 clementine-2023.7.7/src/clementine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 18:41:10.000000 clementine-2023.7.7/src/clementine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:41:10.196844 clementine-2023.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 18:40:56.000000 clementine-2023.7.7/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-07 18:40:56.000000 clementine-2023.7.7/tests/test_importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-07 18:40:56.000000 clementine-2023.7.7/tests/test_screenshot.py
```

### Comparing `clementine-2023.6.12/LICENSE` & `clementine-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clementine-2023.6.12/PKG-INFO` & `clementine-2023.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clementine
-Version: 2023.6.12
+Version: 2023.7.7
 Summary: 🍊 A sweet little Python package
 Author-email: Suzen Fylke <codesue@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Suzen Fylke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: blossom
 Provides-Extra: fruit
 Provides-Extra: leaves
 Provides-Extra: rind
 Provides-Extra: seeds
 Provides-Extra: sprout
@@ -50,15 +50,16 @@
 
 [![License][license_badge]][license_link]
 [![PyPI][pypi_badge]][pypi_link]
 [![Repo Size][repo_size_badge]][repo_size_link]
 [![Docs][docs_badge]][docs_link]
 [![Release][release_badge]][release_link]
 
-Clementine is a sweet little Python package.
+Clementine is a sweet little Python package. It's just for fun and shouldn't
+be used for anything serious.
 
 ## Installation
 
 Installing with pip:
 
 ```sh
 pip install clementine
```

### Comparing `clementine-2023.6.12/README.md` & `clementine-2023.7.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 [![License][license_badge]][license_link]
 [![PyPI][pypi_badge]][pypi_link]
 [![Repo Size][repo_size_badge]][repo_size_link]
 [![Docs][docs_badge]][docs_link]
 [![Release][release_badge]][release_link]
 
-Clementine is a sweet little Python package.
+Clementine is a sweet little Python package. It's just for fun and shouldn't
+be used for anything serious.
 
 ## Installation
 
 Installing with pip:
 
 ```sh
 pip install clementine
```

### Comparing `clementine-2023.6.12/pyproject.toml` & `clementine-2023.7.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Dependencies are automatically generated from the script
+# scripts/update_pyproject_deps.py. Do not edit them manually.
+
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clementine"
 dynamic = ["version"]
@@ -14,35 +17,94 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
-dependencies = ["click"]
-requires-python = ">=3.8"
+dependencies = ["click", "pyperclip"]
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
-blossom = ["bokeh", "gradio", "playwright"]
-fruit = ["catppuccin-matplotlib", "numpy", "pandas", "scikit-learn", "torch"]
-leaves = ["mkdocs-walt", "mkdocstrings[python]"]
-rind = ["build", "twine"]
-seeds = ["isort", "pip-tools", "pre-commit", "pytest", "ruff", "yapf"]
-sprout = ["notebook", "rich"]
-tree = ["clementine[blossom,fruit,leaves,rind,seeds,sprout]"]
+blossom = [
+    "bokeh",
+    "gradio",
+    "playwright",
+]
+fruit = [
+    "catppuccin-matplotlib",
+    "numpy",
+    "pandas",
+    "scikit-learn",
+    "torch",
+]
+leaves = [
+    "mkdocs-walt",
+    "mkdocstrings[python]",
+]
+rind = [
+    "build",
+    "tomlkit",
+    "twine",
+]
+seeds = [
+    "bandit[toml]",
+    "black",
+    "isort",
+    "mypy",
+    "pip-tools",
+    "pre-commit",
+    "pytest",
+    "ruff",
+]
+sprout = [
+    "notebook",
+    "rich",
+]
+tree = [
+    "bokeh",
+    "gradio",
+    "playwright",
+    "catppuccin-matplotlib",
+    "numpy",
+    "pandas",
+    "scikit-learn",
+    "torch",
+    "mkdocs-walt",
+    "mkdocstrings[python]",
+    "build",
+    "tomlkit",
+    "twine",
+    "bandit[toml]",
+    "black",
+    "isort",
+    "mypy",
+    "pip-tools",
+    "pre-commit",
+    "pytest",
+    "ruff",
+    "notebook",
+    "rich",
+]
 
 [project.urls]
 "Documentation" = "https://codesue.github.io/clementine"
 "Source Code" = "https://github.com/codesue/clementine"
 "Bug Tracker" = "https://github.com/codesue/clementine/issues"
 
 [project.scripts]
 clementine = "clementine.cli:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "clementine.__version__"}
 
-[tool.yapf]
-based_on_style = "pep8"
-indent_width = 2
-split_before_first_argument = true
-dedent_closing_brackets = true
+[tool.setuptools.package-data]
+clementine = ["py.typed"]
+
+[tool.bandit]
+exclude_dirs = ["scripts"]
+
+[tool.bandit.assert_used]
+skips = ["tests/**"]
+
+[tool.mypy]
+mypy_path = "stubs"
```

### Comparing `clementine-2023.6.12/src/clementine/blossom.py` & `clementine-2023.7.7/src/clementine/screenshot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,127 +1,129 @@
-"""Visualization and demonstration utilities."""
+"""Screenshot utilities."""
 
 import asyncio
-import builtins
-import importlib
 import os
 from typing import Optional
 
+from clementine import env, importing
+
+__all__ = ["async_screenshot", "screenshot"]
+
+_PLAYWRIGHT_IMPORT_ERROR_MESSAGE = (
+    "The Playwright Python package is not installed. Install it with "
+    "`pip install playwright`."
+)
+
+pw_async_api = importing.maybe_import_module(
+    "playwright.async_api", _PLAYWRIGHT_IMPORT_ERROR_MESSAGE
+)
+pw_api_types = importing.maybe_import_module(
+    "playwright._impl._api_types", _PLAYWRIGHT_IMPORT_ERROR_MESSAGE
+)
+
 
 async def async_screenshot(
     url: str,
     *,
     output_dir: Optional[str] = None,
     filename: Optional[str] = None,
-    full_page: bool = False
+    full_page: bool = False,
 ) -> list[str]:
-  """Take screenshots of a webpage in light and dark mode.
+    """Take screenshots of a webpage in light and dark mode.
 
-  Use `blossom.async_screenshot()` in asynchronous contexts, such as in a Jupyter
-  notebook. Use `blossom.screenshot()` in synchronous contexts, such as in a
-  synchronous Python script.
-
-  **Prerequisites**:
-
-  1. Install the Playwright Python package: `pip install playwright`.
-  2. Install the Playwright browser dependencies: `playwright install webkit`.
-
-
-  **Example usage**:
-
-  In a Python script:
-
-  ```python
-  from clementine import blossom
-
-  paths = blossom.screenshot('https://example.com')
-  ```
-
-  In a Jupyter notebook or other asynchronous context:
-
-  ```python
-  from clementine import blossom
-  from IPython.display import display, Image
-
-  paths = await blossom.async_screenshot('https://example.com')
-  for path in paths:
-    display(Image(path, width=600))
-  ```
-
-  Args:
-    url: The URL to take screenshots of. The URL must include the scheme, e.g. 
-      https:// or file:///.
-    output_dir: The directory to save the screenshots to. Defaults to
-      'screenshots' in the current working directory.
-    filename: The base filename to use for the screenshots. Defaults to
-      'screenshot'. The screenshots will be saved as screenshot-light.png and
-      screenshot-dark.png, for example.
-    full_page: Whether to take a screenshot of the full page. Defaults to False.
-
-  Raises:
-    ImportError: If the Playwright Python package is not installed.
-    Error: If the browser cannot be launched or an invalid url is provided.
-
-  Returns:
-    A list of the paths to the screenshots.
-  """
-  try:
-    pw_async_api = importlib.import_module('playwright.async_api')
-    pw_api_types = importlib.import_module('playwright._impl._api_types')
-  except ImportError as e:
-    raise ImportError(
-        'The Playwright Python package is not installed. Install it with '
-        '`pip install playwright`.'
-    ) from e
-
-  async_playwright = pw_async_api.async_playwright
-  PlaywrightError = pw_api_types.Error
-
-  output_dir = output_dir or os.path.join(os.getcwd(), 'screenshots')
-  filename = filename or 'screenshot'
-  output_paths = []
-
-  async with async_playwright() as p:
-    try:
-      browser = await p.webkit.launch()
-    except PlaywrightError as e:
-      raise OSError(
-          'The browser could not be launched. Install the Playwright browser '
-          'dependencies with `playwright install webkit`.'
-      ) from e
-
-    page = await browser.new_page()
-    await page.goto(url)
-
-    os.makedirs(output_dir, exist_ok=True)
-    for color_scheme in ('light', 'dark'):
-      await page.emulate_media(color_scheme=color_scheme)
-      path = os.path.join(output_dir, f'{filename}-{color_scheme}.png')
-      await page.screenshot(path=path, full_page=full_page)
-      output_paths.append(path)
+    Use `screenshot.async_screenshot()` in asynchronous contexts, such as in a Jupyter
+    notebook. Use `screenshot.screenshot()` in synchronous contexts, such as in a
+    synchronous Python script.
+
+    **Prerequisites**:
+
+    1. Install the Playwright Python package: `pip install playwright`.
+    2. Install the Playwright browser dependencies: `playwright install webkit`.
+
+
+    **Example usage**:
+
+    In a Python script:
+
+    ```python
+    from clementine import screenshot
+
+    paths = screenshot.screenshot('https://example.com')
+    ```
+
+    In a Jupyter notebook or other asynchronous context:
+
+    ```python
+    from clementine import screenshot
+    from IPython.display import display, Image
+
+    paths = await screenshot.async_screenshot('https://example.com')
+    for path in paths:
+        display(Image(path, width=600))
+    ```
+
+    Args:
+      url: The URL to take screenshots of. The URL must include the scheme, e.g.
+        https:// or file:///.
+      output_dir: The directory to save the screenshots to. Defaults to
+        'screenshots' in the current working directory.
+      filename: The base filename to use for the screenshots. Defaults to
+        'screenshot'. The screenshots will be saved as screenshot-light.png and
+        screenshot-dark.png, for example.
+      full_page: Whether to take a screenshot of the full page. Defaults to False.
+
+    Raises:
+      ImportError: If the Playwright Python package is not installed.
+      Error: If the browser cannot be launched or an invalid url is provided.
+
+    Returns:
+      A list of the paths to the screenshots.
+    """
+    output_dir = output_dir or os.path.join(os.getcwd(), "screenshots")
+    filename = filename or "screenshot"
+    output_paths = []
+
+    async with pw_async_api.async_playwright() as p:
+        try:
+            browser = await p.webkit.launch()
+        except pw_api_types.Error as e:
+            raise OSError(
+                "The browser could not be launched. Install the Playwright "
+                "browser dependencies with `playwright install webkit`."
+            ) from e
+
+        page = await browser.new_page()
+        await page.goto(url)
+
+        os.makedirs(output_dir, exist_ok=True)
+        for color_scheme in ("light", "dark"):
+            await page.emulate_media(color_scheme=color_scheme)
+            path = os.path.join(output_dir, f"{filename}-{color_scheme}.png")
+            await page.screenshot(path=path, full_page=full_page)
+            output_paths.append(path)
 
-    await browser.close()
+        await browser.close()
 
-  return output_paths
+    return output_paths
 
 
 def screenshot(
     url: str,
     *,
     output_dir: Optional[str] = None,
     filename: Optional[str] = None,
-    full_page=False
+    full_page=False,
 ) -> list[str]:
-  """Runs the coroutine function `blossom.async_screenshot()` and returns its
-  results."""
-  screenshot.__doc__ = async_screenshot.__doc__
-  if getattr(builtins, '__IPYTHON__', False):
-    raise RuntimeError(
-        'The function `blossom.screenshot()` cannot be called in an asynchronous '
-        'context, such as in a Jupyter notebook. Use `blossom.async_screenshot()` '
-        'instead.'
+    """Runs the coroutine function `screenshot.async_screenshot()` and returns its
+    results."""
+    screenshot.__doc__ = async_screenshot.__doc__
+    if env.is_notebook():
+        raise RuntimeError(
+            "The function `screenshot.screenshot()` cannot be called in "
+            "an asynchronous context, such as in a Jupyter notebook. "
+            "Use `screenshot.async_screenshot()` instead."
+        )
+    return asyncio.run(
+        async_screenshot(
+            url, output_dir=output_dir, filename=filename, full_page=full_page
+        )
     )
-  return asyncio.run(
-      async_screenshot(
-          url, output_dir=output_dir, filename=filename, full_page=full_page
-      )
-  )
```

### Comparing `clementine-2023.6.12/src/clementine/cli.py` & `clementine-2023.7.7/src/clementine/cli/commands/_screenshot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,41 @@
-"""The clementine CLI."""
+"""The clementine CLI screenshot commands."""
 
 import click
 
-from clementine import about, blossom
+from clementine.screenshot import screenshot as _screenshot
 
-_CONTEXT_SETTINGS = {
-    'help_option_names': ['-h', '--help'],
-}
 
-
-@click.group(context_settings=_CONTEXT_SETTINGS, help=about.__description__)
-@click.version_option(
-    about.__version__, '-v', '--version', message=about.__pretty_version__
-)
-def main():
-  """The main entry point for the clementine CLI."""
-  pass
-
-
-@main.command()
-@click.argument('url')
+@click.command()
+@click.argument("url")
 @click.option(
-    '-o',
-    '--output-dir',
+    "-o",
+    "--output-dir",
     help=(
         'The directory to save the screenshots to. Defaults to "screenshots" '
-        'in the current working directory.'
-    )
+        "in the current working directory."
+    ),
 )
 @click.option(
-    '-f',
-    '--filename',
+    "-f",
+    "--filename",
     help=(
         'The base filename to use for the screenshots. Defaults to "screenshot". '
-        'The screenshots will be saved as screenshot-light.png and '
-        'screenshot-dark.png, for example.'
-    )
+        "The screenshots will be saved as screenshot-light.png and "
+        "screenshot-dark.png, for example."
+    ),
 )
 @click.option(
-    '--full-page/--no-full-page',
+    "--full-page/--no-full-page",
     default=False,
-    help='Whether to take a screenshot of the full page. Defaults to False.'
+    help="Whether to take a screenshot of the full page. Defaults to False.",
 )
 def screenshot(url, output_dir, filename, full_page):
-  """Take screenshots of a webpage in light and dark mode. The URL must include
-  the scheme, e.g. https:// or file:///.
-  """
-  paths = blossom.screenshot(
-      url, output_dir=output_dir, filename=filename, full_page=full_page
-  )
-  click.echo(f'The screenshots of {url} were saved at these paths: ')
-  for path in paths:
-    click.echo(f'- {path}')
-
-
-if __name__ == '__main__':
-  main()
+    """Take screenshots of a webpage in light and dark mode. The URL must include
+    the scheme, e.g. https:// or file:///.
+    """
+    paths = _screenshot(
+        url, output_dir=output_dir, filename=filename, full_page=full_page
+    )
+    click.echo(f"The screenshots of {url} were saved at these paths: ")
+    for path in paths:
+        click.echo(f"- {path}")
```

### Comparing `clementine-2023.6.12/src/clementine.egg-info/PKG-INFO` & `clementine-2023.7.7/src/clementine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clementine
-Version: 2023.6.12
+Version: 2023.7.7
 Summary: 🍊 A sweet little Python package
 Author-email: Suzen Fylke <codesue@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Suzen Fylke
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: blossom
 Provides-Extra: fruit
 Provides-Extra: leaves
 Provides-Extra: rind
 Provides-Extra: seeds
 Provides-Extra: sprout
@@ -50,15 +50,16 @@
 
 [![License][license_badge]][license_link]
 [![PyPI][pypi_badge]][pypi_link]
 [![Repo Size][repo_size_badge]][repo_size_link]
 [![Docs][docs_badge]][docs_link]
 [![Release][release_badge]][release_link]
 
-Clementine is a sweet little Python package.
+Clementine is a sweet little Python package. It's just for fun and shouldn't
+be used for anything serious.
 
 ## Installation
 
 Installing with pip:
 
 ```sh
 pip install clementine
```

### Comparing `clementine-2023.6.12/tests/test_blossom.py` & `clementine-2023.7.7/tests/test_screenshot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Tests for clementine.blossom."""
+"""Tests for clementine.screenshot."""
 
 import os
 from unittest import mock
 
 import pytest
 
-from clementine import blossom
+from clementine import screenshot
 
 
 def test_screenshot(tmp_path):
-  webpage = tmp_path / 'index.html'
-  webpage.write_text(
-      '''
+    webpage = tmp_path / "index.html"
+    webpage.write_text(
+        """
       <!DOCTYPE html>
       <html>
         <head>
           <style>
             body {
               background-color: #000;
               color: #fff;
@@ -28,26 +28,26 @@
             }
           </style>
         <head>
         <body>
           <h1>Hello, world!</h1>
         </body>
       </html>
-      '''
-  )
-  expected_paths = [
-      os.path.join(tmp_path, 'screenshot-light.png'),
-      os.path.join(tmp_path, 'screenshot-dark.png'),
-  ]
-
-  paths = blossom.screenshot(f'file://{str(webpage)}', output_dir=tmp_path)
-  assert sorted(paths) == sorted(expected_paths)
-  for path in paths:
-    assert os.path.exists(path)
-    assert os.stat(path).st_size > 0
+      """
+    )
+    expected_paths = [
+        os.path.join(tmp_path, "screenshot-light.png"),
+        os.path.join(tmp_path, "screenshot-dark.png"),
+    ]
+
+    paths = screenshot.screenshot(f"file://{str(webpage)}", output_dir=tmp_path)
+    assert sorted(paths) == sorted(expected_paths)
+    for path in paths:
+        assert os.path.exists(path)
+        assert os.stat(path).st_size > 0
 
 
-@mock.patch.dict('builtins.__dict__', {'__IPYTHON__': True})
+@mock.patch.dict("builtins.__dict__", {"__IPYTHON__": True})
 def test_screenshot_raises_error_in_notebooks():
-  with pytest.raises(RuntimeError) as execinfo:
-    blossom.screenshot('https://example.com')
-    assert 'Use `blossom.async_screenshot()` instead.' in str(execinfo.value)
+    with pytest.raises(RuntimeError) as execinfo:
+        screenshot.screenshot("https://example.com")
+        assert "Use `screenshot.async_screenshot()` instead." in str(execinfo.value)
```


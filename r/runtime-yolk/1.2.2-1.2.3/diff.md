# Comparing `tmp/runtime-yolk-1.2.2.tar.gz` & `tmp/runtime-yolk-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtime-yolk-1.2.2.tar", last modified: Tue Nov  1 04:06:57 2022, max compression
+gzip compressed data, was "runtime-yolk-1.2.3.tar", last modified: Fri Jul  7 01:52:29 2023, max compression
```

## Comparing `runtime-yolk-1.2.2.tar` & `runtime-yolk-1.2.3.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-11-01 04:06:57.830000 runtime-yolk-1.2.2/
--rw-r--r--   0 preocts   (1000) preocts   (1000)     1064 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/LICENSE
--rw-r--r--   0 preocts   (1000) preocts   (1000)     9863 2022-11-01 04:06:57.830000 runtime-yolk-1.2.2/PKG-INFO
--rw-r--r--   0 preocts   (1000) preocts   (1000)     7972 2022-11-01 04:00:40.000000 runtime-yolk-1.2.2/README.md
--rw-r--r--   0 preocts   (1000) preocts   (1000)     2587 2022-11-01 04:05:49.000000 runtime-yolk-1.2.2/pyproject.toml
--rw-r--r--   0 preocts   (1000) preocts   (1000)       38 2022-11-01 04:06:57.830000 runtime-yolk-1.2.2/setup.cfg
--rw-r--r--   0 preocts   (1000) preocts   (1000)       74 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/setup.py
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-11-01 04:06:57.830000 runtime-yolk-1.2.2/src/
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-11-01 04:06:57.830000 runtime-yolk-1.2.2/src/runtime_yolk/
--rw-r--r--   0 preocts   (1000) preocts   (1000)      233 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/src/runtime_yolk/__init__.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     3275 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/src/runtime_yolk/config_loader.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     3152 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/src/runtime_yolk/env_cli.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     2745 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/src/runtime_yolk/env_loader.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)       27 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/src/runtime_yolk/py.typed
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-11-01 04:06:57.830000 runtime-yolk-1.2.2/src/runtime_yolk/util/
--rw-r--r--   0 preocts   (1000) preocts   (1000)        0 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/src/runtime_yolk/util/__init__.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)      632 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/src/runtime_yolk/util/file_rule.py
--rw-r--r--   0 preocts   (1000) preocts   (1000)     3800 2022-11-01 03:57:11.000000 runtime-yolk-1.2.2/src/runtime_yolk/yolk.py
-drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2022-11-01 04:06:57.830000 runtime-yolk-1.2.2/src/runtime_yolk.egg-info/
--rw-r--r--   0 preocts   (1000) preocts   (1000)     9863 2022-11-01 04:06:57.000000 runtime-yolk-1.2.2/src/runtime_yolk.egg-info/PKG-INFO
--rw-r--r--   0 preocts   (1000) preocts   (1000)      525 2022-11-01 04:06:57.000000 runtime-yolk-1.2.2/src/runtime_yolk.egg-info/SOURCES.txt
--rw-r--r--   0 preocts   (1000) preocts   (1000)        1 2022-11-01 04:06:57.000000 runtime-yolk-1.2.2/src/runtime_yolk.egg-info/dependency_links.txt
--rw-r--r--   0 preocts   (1000) preocts   (1000)       55 2022-11-01 04:06:57.000000 runtime-yolk-1.2.2/src/runtime_yolk.egg-info/entry_points.txt
--rw-r--r--   0 preocts   (1000) preocts   (1000)       96 2022-11-01 04:06:57.000000 runtime-yolk-1.2.2/src/runtime_yolk.egg-info/requires.txt
--rw-r--r--   0 preocts   (1000) preocts   (1000)       13 2022-11-01 04:06:57.000000 runtime-yolk-1.2.2/src/runtime_yolk.egg-info/top_level.txt
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-07 01:52:29.615116 runtime-yolk-1.2.3/
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     1064 2023-07-07 01:07:20.000000 runtime-yolk-1.2.3/LICENSE
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     9625 2023-07-07 01:52:29.615116 runtime-yolk-1.2.3/PKG-INFO
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     7734 2023-07-07 01:07:20.000000 runtime-yolk-1.2.3/README.md
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     2269 2023-07-07 01:43:28.000000 runtime-yolk-1.2.3/pyproject.toml
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       38 2023-07-07 01:52:29.615116 runtime-yolk-1.2.3/setup.cfg
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-07 01:52:29.615116 runtime-yolk-1.2.3/src/
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-07 01:52:29.615116 runtime-yolk-1.2.3/src/runtime_yolk/
+-rw-r--r--   0 preocts   (1000) preocts   (1000)      233 2023-07-07 01:07:20.000000 runtime-yolk-1.2.3/src/runtime_yolk/__init__.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     3169 2023-07-07 01:37:41.000000 runtime-yolk-1.2.3/src/runtime_yolk/config_loader.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     3152 2023-07-07 01:07:20.000000 runtime-yolk-1.2.3/src/runtime_yolk/env_cli.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     2648 2023-07-07 01:07:20.000000 runtime-yolk-1.2.3/src/runtime_yolk/env_loader.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       27 2023-07-07 01:07:20.000000 runtime-yolk-1.2.3/src/runtime_yolk/py.typed
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-07 01:52:29.615116 runtime-yolk-1.2.3/src/runtime_yolk/util/
+-rw-r--r--   0 preocts   (1000) preocts   (1000)        0 2023-07-07 01:07:20.000000 runtime-yolk-1.2.3/src/runtime_yolk/util/__init__.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)      632 2023-07-07 01:07:20.000000 runtime-yolk-1.2.3/src/runtime_yolk/util/file_rule.py
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     3794 2023-07-07 01:18:11.000000 runtime-yolk-1.2.3/src/runtime_yolk/yolk.py
+drwxr-xr-x   0 preocts   (1000) preocts   (1000)        0 2023-07-07 01:52:29.615116 runtime-yolk-1.2.3/src/runtime_yolk.egg-info/
+-rw-r--r--   0 preocts   (1000) preocts   (1000)     9625 2023-07-07 01:52:29.000000 runtime-yolk-1.2.3/src/runtime_yolk.egg-info/PKG-INFO
+-rw-r--r--   0 preocts   (1000) preocts   (1000)      516 2023-07-07 01:52:29.000000 runtime-yolk-1.2.3/src/runtime_yolk.egg-info/SOURCES.txt
+-rw-r--r--   0 preocts   (1000) preocts   (1000)        1 2023-07-07 01:52:29.000000 runtime-yolk-1.2.3/src/runtime_yolk.egg-info/dependency_links.txt
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       55 2023-07-07 01:52:29.000000 runtime-yolk-1.2.3/src/runtime_yolk.egg-info/entry_points.txt
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       96 2023-07-07 01:52:29.000000 runtime-yolk-1.2.3/src/runtime_yolk.egg-info/requires.txt
+-rw-r--r--   0 preocts   (1000) preocts   (1000)       13 2023-07-07 01:52:29.000000 runtime-yolk-1.2.3/src/runtime_yolk.egg-info/top_level.txt
```

### Comparing `runtime-yolk-1.2.2/LICENSE` & `runtime-yolk-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runtime-yolk-1.2.2/PKG-INFO` & `runtime-yolk-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtime-yolk
-Version: 1.2.2
+Version: 1.2.3
 Summary: This project aims to create a single library for run-time initiation tasks that are often duplicated across many projects.
 Author-email: Preocts <preocts@preocts.com>
 License: MIT License
         
         Copyright (c) 2021 Preocts
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,32 +26,32 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/Preocts/runtime-yolk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
-[![Python 3.7 | 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
+[![Python 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Preocts/runtime-yolk/main.svg)](https://results.pre-commit.ci/latest/github/Preocts/runtime-yolk/main)
 [![Python tests](https://github.com/Preocts/runtime-yolk/actions/workflows/python-tests.yml/badge.svg?branch=main)](https://github.com/Preocts/runtime-yolk/actions/workflows/python-tests.yml)
 
 # runtime-yolk
 
 ## Requirements
 
-- [Python](https://python.org) >= 3.7
+- [Python](https://python.org) >= 3.8
 
 Load your local `.env` file to environ, load your application.ini which can be
 environment specific, and setup basic logging behavior all with a single call.
 Designed to be low effort, runtime-yolk works well in the initial entry point of
 a project and doesn't add additional requires to downstream libraries.
 
 - Environment variables are loaded from the `.env` file, or specified source,
@@ -106,15 +106,15 @@
 
 Sample:
 
 ```ini
 [DEFAULT]
 logging_level = DEBUG
 logging_format = %(asctime)s - %(levelname)s - %(name)s - %(message)s
-environment = {{ENVIRONMENT}}
+environment = {{YOLK_ENVIRONMENT}}
 ```
 
 ### `.env` file loading
 
 `.env` files are loaded with the expectation of key = value pairs. `#` comments are allowed as well as blank lines.
 
 Current format for the `.env` file supports strings only and is parsed in
@@ -265,16 +265,14 @@
 
 ## Makefile
 
 This repo has a Makefile with some quality of life scripts if the system
 supports `make`.  Please note there are no checks for an active `venv` in the
 Makefile.
 
-| PHONY         | Description                                                                |
-| ------------- | -------------------------------------------------------------------------- |
-| `init`        | Update pip to newest version                                               |
-| `install`     | install the project                                                        |
-| `install-dev` | install development/test requirements and project as editable install      |
-| `upgrade-dev` | update all dependencies, regenerate requirements.txt (disabled by default) |
-| `coverage`    | Runs `tox -p`. results to stdout, json, and html                           |
-| `build-dist`  | Build source distribution and wheel distribution                           |
-| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts       |
+| PHONY         | Description                                                           |
+| ------------- | --------------------------------------------------------------------- |
+| `install-dev` | install development/test requirements and project as editable install |
+| `coverage`    | Run coverage and output console report                                |
+| `docker-test` | Run coverage and tests in a docker container.                         |
+| `build-dist`  | Build source distribution and wheel distribution                      |
+| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts  |
```

### Comparing `runtime-yolk-1.2.2/README.md` & `runtime-yolk-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-[![Python 3.7 | 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
+[![Python 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Preocts/runtime-yolk/main.svg)](https://results.pre-commit.ci/latest/github/Preocts/runtime-yolk/main)
 [![Python tests](https://github.com/Preocts/runtime-yolk/actions/workflows/python-tests.yml/badge.svg?branch=main)](https://github.com/Preocts/runtime-yolk/actions/workflows/python-tests.yml)
 
 # runtime-yolk
 
 ## Requirements
 
-- [Python](https://python.org) >= 3.7
+- [Python](https://python.org) >= 3.8
 
 Load your local `.env` file to environ, load your application.ini which can be
 environment specific, and setup basic logging behavior all with a single call.
 Designed to be low effort, runtime-yolk works well in the initial entry point of
 a project and doesn't add additional requires to downstream libraries.
 
 - Environment variables are loaded from the `.env` file, or specified source,
@@ -68,15 +68,15 @@
 
 Sample:
 
 ```ini
 [DEFAULT]
 logging_level = DEBUG
 logging_format = %(asctime)s - %(levelname)s - %(name)s - %(message)s
-environment = {{ENVIRONMENT}}
+environment = {{YOLK_ENVIRONMENT}}
 ```
 
 ### `.env` file loading
 
 `.env` files are loaded with the expectation of key = value pairs. `#` comments are allowed as well as blank lines.
 
 Current format for the `.env` file supports strings only and is parsed in
@@ -227,16 +227,14 @@
 
 ## Makefile
 
 This repo has a Makefile with some quality of life scripts if the system
 supports `make`.  Please note there are no checks for an active `venv` in the
 Makefile.
 
-| PHONY         | Description                                                                |
-| ------------- | -------------------------------------------------------------------------- |
-| `init`        | Update pip to newest version                                               |
-| `install`     | install the project                                                        |
-| `install-dev` | install development/test requirements and project as editable install      |
-| `upgrade-dev` | update all dependencies, regenerate requirements.txt (disabled by default) |
-| `coverage`    | Runs `tox -p`. results to stdout, json, and html                           |
-| `build-dist`  | Build source distribution and wheel distribution                           |
-| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts       |
+| PHONY         | Description                                                           |
+| ------------- | --------------------------------------------------------------------- |
+| `install-dev` | install development/test requirements and project as editable install |
+| `coverage`    | Run coverage and output console report                                |
+| `docker-test` | Run coverage and tests in a docker container.                         |
+| `build-dist`  | Build source distribution and wheel distribution                      |
+| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts  |
```

### Comparing `runtime-yolk-1.2.2/pyproject.toml` & `runtime-yolk-1.2.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "runtime-yolk"
-version = "1.2.2"
-requires-python = ">=3.7"
+version = "1.2.3"
+requires-python = ">=3.8"
 description = "This project aims to create a single library for run-time initiation tasks that are often duplicated across many projects."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { email = "preocts@preocts.com", name = "Preocts" }
 ]
 maintainers = []
@@ -87,39 +87,28 @@
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
     "\\.\\.\\.",
 ]
 
-# This is ignored by flake8, here in case they decide to add it in the future
-[tool.flake8]
-ignore = "W503,E203"
-max-line-length = 88
-
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py37,py38,py39,py310,py311,coverage,pre-commit
+envlist = py38,py39,py310,py311,py312,mypy,coverage
 skip_missing_interpreters = true
-isolated_build = True
 
 [testenv]
 deps = .[test]
 commands =
     coverage run -p -m pytest tests/
 
 [testenv:coverage]
-depends = py37,py38,py39,py310,py311
-parallel_show_output = true
 commands =
     python -m coverage combine
     python -m coverage report -m --fail-under=50
     python -m coverage json
 
-[testenv:pre-commit]
-depends = coverage
-parallel_show_output = true
-skip_install = true
-deps = pre-commit
-commands = pre-commit run --all-files --show-diff-on-failure
+[testenv:mypy]
+deps = mypy
+commands = mypy -p runtime_yolk --no-incremental
 """
```

### Comparing `runtime-yolk-1.2.2/src/runtime_yolk/config_loader.py` & `runtime-yolk-1.2.3/src/runtime_yolk/config_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,26 @@
         """
         Create a new instance of Config.
 
         Args:
             working_directory: Set the working directory where file(s) will be loaded.
         """
         self._working_directory = working_directory or Path().cwd()
-        self._config = ConfigParser(interpolation=None)
+        self.config = ConfigParser(interpolation=None)
 
         self._build_default_config()
 
         # Store loaded config file names to prevent loading the same file twice.
         self._loaded_configs: set[Path] = set()
 
     def _build_default_config(self) -> None:
         """Build and populate the default config."""
-        self._config["DEFAULT"] = {
-            "environment": os.getenv("ENVIRONMENT", ""),
-            "logging_level": os.getenv("LOGGING_LEVEL", "ERROR"),
+        self.config["DEFAULT"] = {
+            "environment": os.getenv("YOLK_ENVIRONMENT", ""),
+            "logging_level": os.getenv("LOGGING_LEVEL", "WARNING"),
             "logging_format": "%(asctime)s - %(levelname)s - %(name)s - %(message)s",
         }
 
     def load(
         self,
         *,
         config_name: str = "application",
@@ -65,23 +65,19 @@
         _file = self._working_directory / get_file_name(config_file, yolk_environment)
 
         if _file.is_file() and _file not in self._loaded_configs:
             contents = self._interpolate_environment(_file.read_text())
 
             # Load the discovered content as a configuration string
             # ConfigParser handles invalid content
-            self._config.read_string(contents)
+            self.config.read_string(contents)
             self._loaded_configs.add(_file)
 
             # If the config file has an environment set, attempt to load the next file.
-            if self._config.get("DEFAULT", "environment", fallback=None):
-                self._load(config_file, self._config.get("DEFAULT", "environment"))
+            if self.config.get("DEFAULT", "environment", fallback=None):
+                self._load(config_file, self.config.get("DEFAULT", "environment"))
 
     def _interpolate_environment(self, contents: str) -> str:
         """Interpolate {{keywords}} to matching environment variable values."""
         for match in re.finditer(INTERPOLATE_PATTERN, contents):
             contents = re.sub(match.group(0), os.getenv(match.group(1), ""), contents)
         return contents
-
-    def get_config(self) -> ConfigParser:
-        """Get the config object."""
-        return self._config
```

### Comparing `runtime-yolk-1.2.2/src/runtime_yolk/env_cli.py` & `runtime-yolk-1.2.3/src/runtime_yolk/env_cli.py`

 * *Files identical despite different names*

### Comparing `runtime-yolk-1.2.2/src/runtime_yolk/env_loader.py` & `runtime-yolk-1.2.3/src/runtime_yolk/env_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 import re
 from pathlib import Path
 
 
 class EnvLoader:
     """Load local .env file into environment variables."""
 
-    LTQUOTES_RE = re.compile(r"([\"'])(.*)\1$|^(.*)$")
-    EXPORT_PREFIX_RE = re.compile(r"^\s*?export\s*", flags=re.IGNORECASE)
-
     def __init__(self, working_directory: Path | None = None) -> None:
         """
         Create .env loader.
 
         Args:
             working_directory: Set the working directory where file(s) will be loaded.
         """
@@ -72,13 +69,13 @@
 
             loaded_values[key] = value
 
         return loaded_values
 
     def _remove_lt_quotes(self, in_: str) -> str:
         """Remove matched leading and trailing single or double quotes."""
-        match = self.LTQUOTES_RE.match(in_)
+        match = re.match(r"([\"'])(.*)\1$|^(.*)$", in_)
         return match.group(2) if match and match.group(2) else in_
 
     def _strip_export(self, in_: str) -> str:
         """Remove leading 'export ' prefix, case agnostic."""
-        return self.EXPORT_PREFIX_RE.sub("", in_)
+        return re.sub(r"^\s*?export\s*", "", in_, flags=re.IGNORECASE)
```

### Comparing `runtime-yolk-1.2.2/src/runtime_yolk/util/file_rule.py` & `runtime-yolk-1.2.3/src/runtime_yolk/util/file_rule.py`

 * *Files identical despite different names*

### Comparing `runtime-yolk-1.2.2/src/runtime_yolk/yolk.py` & `runtime-yolk-1.2.3/src/runtime_yolk/yolk.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             self.load_env()
             self.load_config()
             self.set_logging()
 
     @property
     def config(self) -> ConfigParser:
         """Return loaded ConfigParser object."""
-        return self._config.get_config()
+        return self._config.config
 
     def load_config(self, config_name: str = "application") -> None:
         """
         Load configuration from a file, layers loads onto existing loaded data.
 
         Args:
             config_name: The name of the config file without the extension
```

### Comparing `runtime-yolk-1.2.2/src/runtime_yolk.egg-info/PKG-INFO` & `runtime-yolk-1.2.3/src/runtime_yolk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtime-yolk
-Version: 1.2.2
+Version: 1.2.3
 Summary: This project aims to create a single library for run-time initiation tasks that are often duplicated across many projects.
 Author-email: Preocts <preocts@preocts.com>
 License: MIT License
         
         Copyright (c) 2021 Preocts
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,32 +26,32 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/Preocts/runtime-yolk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
-[![Python 3.7 | 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
+[![Python 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Preocts/runtime-yolk/main.svg)](https://results.pre-commit.ci/latest/github/Preocts/runtime-yolk/main)
 [![Python tests](https://github.com/Preocts/runtime-yolk/actions/workflows/python-tests.yml/badge.svg?branch=main)](https://github.com/Preocts/runtime-yolk/actions/workflows/python-tests.yml)
 
 # runtime-yolk
 
 ## Requirements
 
-- [Python](https://python.org) >= 3.7
+- [Python](https://python.org) >= 3.8
 
 Load your local `.env` file to environ, load your application.ini which can be
 environment specific, and setup basic logging behavior all with a single call.
 Designed to be low effort, runtime-yolk works well in the initial entry point of
 a project and doesn't add additional requires to downstream libraries.
 
 - Environment variables are loaded from the `.env` file, or specified source,
@@ -106,15 +106,15 @@
 
 Sample:
 
 ```ini
 [DEFAULT]
 logging_level = DEBUG
 logging_format = %(asctime)s - %(levelname)s - %(name)s - %(message)s
-environment = {{ENVIRONMENT}}
+environment = {{YOLK_ENVIRONMENT}}
 ```
 
 ### `.env` file loading
 
 `.env` files are loaded with the expectation of key = value pairs. `#` comments are allowed as well as blank lines.
 
 Current format for the `.env` file supports strings only and is parsed in
@@ -265,16 +265,14 @@
 
 ## Makefile
 
 This repo has a Makefile with some quality of life scripts if the system
 supports `make`.  Please note there are no checks for an active `venv` in the
 Makefile.
 
-| PHONY         | Description                                                                |
-| ------------- | -------------------------------------------------------------------------- |
-| `init`        | Update pip to newest version                                               |
-| `install`     | install the project                                                        |
-| `install-dev` | install development/test requirements and project as editable install      |
-| `upgrade-dev` | update all dependencies, regenerate requirements.txt (disabled by default) |
-| `coverage`    | Runs `tox -p`. results to stdout, json, and html                           |
-| `build-dist`  | Build source distribution and wheel distribution                           |
-| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts       |
+| PHONY         | Description                                                           |
+| ------------- | --------------------------------------------------------------------- |
+| `install-dev` | install development/test requirements and project as editable install |
+| `coverage`    | Run coverage and output console report                                |
+| `docker-test` | Run coverage and tests in a docker container.                         |
+| `build-dist`  | Build source distribution and wheel distribution                      |
+| `clean`       | Deletes build, tox, coverage, pytest, mypy, cache, and pyc artifacts  |
```

### Comparing `runtime-yolk-1.2.2/src/runtime_yolk.egg-info/SOURCES.txt` & `runtime-yolk-1.2.3/src/runtime_yolk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 src/runtime_yolk/__init__.py
 src/runtime_yolk/config_loader.py
 src/runtime_yolk/env_cli.py
 src/runtime_yolk/env_loader.py
 src/runtime_yolk/py.typed
 src/runtime_yolk/yolk.py
 src/runtime_yolk.egg-info/PKG-INFO
```


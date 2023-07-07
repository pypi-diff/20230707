# Comparing `tmp/hickleable-0.1.1.tar.gz` & `tmp/hickleable-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hickleable-0.1.1.tar", last modified: Fri Sep 16 22:10:59 2022, max compression
+gzip compressed data, was "hickleable-0.2.1.tar", last modified: Fri Jul  7 19:09:24 2023, max compression
```

## Comparing `hickleable-0.1.1.tar` & `hickleable-0.2.1.tar`

### file list

```diff
@@ -1,50 +1,56 @@
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/
--rw-r--r--   0 steven    (1000) steven    (1000)      101 2022-09-15 19:35:02.000000 hickleable-0.1.1/.coveragerc
--rw-r--r--   0 steven    (1000) steven    (1000)      528 2022-09-15 22:45:18.000000 hickleable-0.1.1/.flake8
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.238106 hickleable-0.1.1/.github/
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.238106 hickleable-0.1.1/.github/workflows/
--rw-r--r--   0 steven    (1000) steven    (1000)     1884 2022-09-15 19:53:42.000000 hickleable-0.1.1/.github/workflows/deploy.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)      968 2022-09-16 13:24:54.000000 hickleable-0.1.1/.github/workflows/testsuite.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)     1808 2022-09-16 22:08:53.000000 hickleable-0.1.1/.gitignore
--rw-r--r--   0 steven    (1000) steven    (1000)      284 2022-09-15 19:34:48.000000 hickleable-0.1.1/.isort.cfg
--rw-r--r--   0 steven    (1000) steven    (1000)     1237 2022-09-15 19:34:35.000000 hickleable-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)      659 2022-09-16 20:01:58.000000 hickleable-0.1.1/.readthedocs.yml
--rw-r--r--   0 steven    (1000) steven    (1000)       65 2022-09-16 16:13:21.000000 hickleable-0.1.1/CHANGELOG.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     1070 2022-09-15 19:27:24.000000 hickleable-0.1.1/LICENSE
--rw-r--r--   0 steven    (1000) steven    (1000)     5715 2022-09-16 22:10:59.248106 hickleable-0.1.1/PKG-INFO
--rw-r--r--   0 steven    (1000) steven    (1000)     5260 2022-09-16 21:18:33.000000 hickleable-0.1.1/README.rst
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/docs/
--rw-r--r--   0 steven    (1000) steven    (1000)     5586 2022-09-15 19:37:32.000000 hickleable-0.1.1/docs/Makefile
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/docs/_static/
--rw-r--r--   0 steven    (1000) steven    (1000)       18 2022-09-15 19:37:33.000000 hickleable-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 steven    (1000) steven    (1000)       43 2022-09-15 19:37:33.000000 hickleable-0.1.1/docs/changelog.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     8295 2022-09-16 16:10:13.000000 hickleable-0.1.1/docs/conf.py
--rw-r--r--   0 steven    (1000) steven    (1000)        0 2022-09-16 16:10:51.000000 hickleable-0.1.1/docs/contents.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      159 2022-09-16 20:47:49.000000 hickleable-0.1.1/docs/environment.yaml
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/docs/faqs/
--rw-r--r--   0 steven    (1000) steven    (1000)      115 2022-09-15 19:44:32.000000 hickleable-0.1.1/docs/faqs/misc.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     1272 2022-09-16 16:11:54.000000 hickleable-0.1.1/docs/index.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      120 2022-09-16 16:13:20.000000 hickleable-0.1.1/docs/installation.rst
--rw-r--r--   0 steven    (1000) steven    (1000)       63 2022-09-15 19:43:51.000000 hickleable-0.1.1/docs/license.rst
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/docs/reference/
--rw-r--r--   0 steven    (1000) steven    (1000)      186 2022-09-15 20:01:33.000000 hickleable-0.1.1/docs/reference/index.rst
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/docs/templates/
--rw-r--r--   0 steven    (1000) steven    (1000)      564 2022-09-15 19:37:33.000000 hickleable-0.1.1/docs/templates/class.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      727 2022-09-15 19:37:33.000000 hickleable-0.1.1/docs/templates/module.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      426 2022-09-15 19:42:47.000000 hickleable-0.1.1/docs/tutorials.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      106 2022-09-16 16:13:21.000000 hickleable-0.1.1/docs/usage.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      315 2022-09-15 19:58:28.000000 hickleable-0.1.1/pyproject.toml
--rw-r--r--   0 steven    (1000) steven    (1000)     1160 2022-09-16 22:10:59.248106 hickleable-0.1.1/setup.cfg
--rw-r--r--   0 steven    (1000) steven    (1000)       60 2022-09-15 19:33:22.000000 hickleable-0.1.1/setup.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.238106 hickleable-0.1.1/src/
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/src/hickleable/
--rw-r--r--   0 steven    (1000) steven    (1000)     9042 2022-09-16 22:08:54.000000 hickleable-0.1.1/src/hickleable/__init__.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/src/hickleable.egg-info/
--rw-r--r--   0 steven    (1000) steven    (1000)     5715 2022-09-16 22:10:59.000000 hickleable-0.1.1/src/hickleable.egg-info/PKG-INFO
--rw-r--r--   0 steven    (1000) steven    (1000)      783 2022-09-16 22:10:59.000000 hickleable-0.1.1/src/hickleable.egg-info/SOURCES.txt
--rw-r--r--   0 steven    (1000) steven    (1000)        1 2022-09-16 22:10:59.000000 hickleable-0.1.1/src/hickleable.egg-info/dependency_links.txt
--rw-r--r--   0 steven    (1000) steven    (1000)        1 2022-09-15 21:37:18.000000 hickleable-0.1.1/src/hickleable.egg-info/not-zip-safe
--rw-r--r--   0 steven    (1000) steven    (1000)      141 2022-09-16 22:10:59.000000 hickleable-0.1.1/src/hickleable.egg-info/requires.txt
--rw-r--r--   0 steven    (1000) steven    (1000)       11 2022-09-16 22:10:59.000000 hickleable-0.1.1/src/hickleable.egg-info/top_level.txt
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2022-09-16 22:10:59.248106 hickleable-0.1.1/tests/
--rw-r--r--   0 steven    (1000) steven    (1000)     3678 2022-09-15 22:45:47.000000 hickleable-0.1.1/tests/test_hickleable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 19:09:10.000000 hickleable-0.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-07 19:09:10.000000 hickleable-0.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.526201 hickleable-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.526201 hickleable-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/release-draft.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 19:09:10.000000 hickleable-0.2.1/.github/workflows/testsuite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-07 19:09:10.000000 hickleable-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 19:09:10.000000 hickleable-0.2.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-07 19:09:10.000000 hickleable-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 19:09:10.000000 hickleable-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 19:09:10.000000 hickleable-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 19:09:24.530201 hickleable-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-07 19:09:10.000000 hickleable-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/faqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/faqs/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-07 19:09:10.000000 hickleable-0.2.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 19:09:10.000000 hickleable-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-07 19:09:24.534201 hickleable-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 19:09:10.000000 hickleable-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.522201 hickleable-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/src/hickleable/
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-07 19:09:10.000000 hickleable-0.2.1/src/hickleable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/src/hickleable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 19:09:24.000000 hickleable-0.2.1/src/hickleable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:09:24.530201 hickleable-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-07 19:09:10.000000 hickleable-0.2.1/tests/test_hickleable.py
```

### Comparing `hickleable-0.1.1/.github/workflows/testsuite.yaml` & `hickleable-0.2.1/.github/workflows/testsuite.yaml`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/.gitignore` & `hickleable-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/.pre-commit-config.yaml` & `hickleable-0.2.1/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 exclude: '^docs/conf.py'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.2.0
+  rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
   - id: check-xml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=no']
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 6.0.0
   hooks:
   - id: flake8
     additional_dependencies:
       - flake8-comprehensions
       - flake8-logging-format
       - flake8-builtins
       - flake8-eradicate
@@ -35,26 +35,26 @@
       - flake8-markdown
       - flake8-bugbear
       - flake8-comprehensions
       - flake8-print
 
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.3.0
   hooks:
   - id: black
 
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/pre-commit/pygrep-hooks
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
     - id: rst-backticks
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v2.32.0
+  rev: v3.8.0
   hooks:
   -   id: pyupgrade
       args: [--py38-plus]
```

### Comparing `hickleable-0.1.1/.readthedocs.yml` & `hickleable-0.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/LICENSE` & `hickleable-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/PKG-INFO` & `hickleable-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hickleable
-Version: 0.1.1
+Version: 0.2.1
 Summary: A simple decorator to make your classes hickle-able
 Home-page: https://github.com/steven-murray/hickleable
 Author: Steven Murray
 License: mit
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `hickleable-0.1.1/README.rst` & `hickleable-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/docs/Makefile` & `hickleable-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/docs/conf.py` & `hickleable-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/docs/index.rst` & `hickleable-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/docs/templates/class.rst` & `hickleable-0.2.1/docs/templates/class.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/docs/templates/module.rst` & `hickleable-0.2.1/docs/templates/module.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/setup.cfg` & `hickleable-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hickleable-0.1.1/src/hickleable/__init__.py` & `hickleable-0.2.1/src/hickleable/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 """A package defining convenience functions for hickle.
 
 The primary function defined is :func:`hickleable`, a decorator to put on top of classes
 that usually magically makes them hickle-able (without resorting to pickling).
 """
 from __future__ import annotations
 
+import hickle
 import inspect
 import warnings
 from functools import cached_property
 from h5py import AttributeManager, Group
 from hickle.lookup import LoaderManager, PyContainer
 from pathlib import Path
 from typing import Any, Callable, Iterable, List, Tuple
 
 DumpOutput = Tuple[Group, List[Tuple[str, Any, dict, dict]]]
 DumpFunctionType = Callable[[Any, Group, str], DumpOutput]
 
+try:
+    import yaml
+except ImportError:
+    yaml = None
+
 
 def hickleable(
     hkl_str: bytes | None = None,
     dump_function: None | DumpFunctionType = None,
     load_container: None | Callable[[Any], PyContainer] | PyContainer = None,
     metadata_keys: Iterable[str] | None = None,
     evaluate_cached_properties: bool = False,
@@ -110,15 +116,16 @@
                     state = py_obj.__dict__
 
                 for k in metadata_keys or []:
                     if k in state:
                         ds.attrs[k] = state.pop(k)
                     else:
                         warnings.warn(
-                            f"Ignoring metadata key {k} since it's not in the object."
+                            f"Ignoring metadata key {k} since it's not in the object.",
+                            stacklevel=2,
                         )
 
                 subitems = []
                 for k, v in state.items():
                     subitems.append((k, v, {}, kwargs))
 
                 return ds, subitems
@@ -214,7 +221,15 @@
 
 LoaderManager.register_class(
     Path,
     b"PosixPath",
     dump_function=_path_dump_function,
     load_function=_load_path,
 )
+
+if yaml is not None:
+    # Register a YAML loader for hickle-dumped files.
+    def _hickle_yaml_loader(path):
+        return hickle.load(path)
+
+    yaml.add_constructor("!hickle", _hickle_yaml_loader, Loader=yaml.FullLoader)
+    yaml.add_constructor("!hickle", _hickle_yaml_loader, Loader=yaml.Loader)
```

### Comparing `hickleable-0.1.1/src/hickleable.egg-info/PKG-INFO` & `hickleable-0.2.1/src/hickleable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hickleable
-Version: 0.1.1
+Version: 0.2.1
 Summary: A simple decorator to make your classes hickle-able
 Home-page: https://github.com/steven-murray/hickleable
 Author: Steven Murray
 License: mit
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `hickleable-0.1.1/src/hickleable.egg-info/SOURCES.txt` & `hickleable-0.2.1/src/hickleable.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 .coveragerc
 .flake8
 .gitignore
 .isort.cfg
 .pre-commit-config.yaml
 .readthedocs.yml
-CHANGELOG.rst
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+.github/dependabot.yml
+.github/labels.yml
+.github/release-drafter.yml
+.github/workflows/auto-merge-deps.yml
+.github/workflows/check-build.yml
 .github/workflows/deploy.yaml
+.github/workflows/labeler.yml
+.github/workflows/release-draft.yml
 .github/workflows/testsuite.yaml
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/contents.rst
 docs/environment.yaml
 docs/index.rst
```

### Comparing `hickleable-0.1.1/tests/test_hickleable.py` & `hickleable-0.2.1/tests/test_hickleable.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     @cached_property
     def big_old_computation(self):
         time.sleep(0.1)
         return time.time()
 
     def __attrs_post_init__(self):
         if self.a == "warnme":
-            warnings.warn("warning you!")
+            warnings.warn("warning you!", stacklevel=2)
 
 
 @hickleable(evaluate_cached_properties=True)
 @attr.s(frozen=True)
 class FrozenWithCachedPropertyEval:
     a = attr.ib("stuff")
```


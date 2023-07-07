# Comparing `tmp/unimport-0.9.6.tar.gz` & `tmp/unimport-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimport-0.9.6.tar", last modified: Wed May  4 12:33:50 2022, max compression
+gzip compressed data, was "unimport-1.0.0.tar", last modified: Fri Jul  7 11:07:58 2023, max compression
```

## Comparing `unimport-0.9.6.tar` & `unimport-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:50.089495 unimport-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-05-04 12:33:49.000000 unimport-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-05-04 12:33:50.089495 unimport-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-05-04 12:33:49.000000 unimport-0.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-04 12:33:50.089495 unimport-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-05-04 12:33:49.000000 unimport-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:50.085495 unimport-0.9.6/unimport/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16345 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/color.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:50.089495 unimport-0.9.6/unimport/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/permission.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     4397 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/refactor.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/relate.py
--rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     4935 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 12:33:50.089495 unimport-0.9.6/unimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3373 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-05-04 12:33:50.000000 unimport-0.9.6/unimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 12:33:49.000000 unimport-0.9.6/unimport.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:07:58.294135 unimport-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 11:07:44.000000 unimport-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-07 11:07:58.294135 unimport-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-07 11:07:44.000000 unimport-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 11:07:44.000000 unimport-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-07 11:07:58.294135 unimport-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:07:58.290135 unimport-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:07:58.290135 unimport-1.0.0/src/unimport/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:07:58.294135 unimport-1.0.0/src/unimport/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/analyzers/decarators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/analyzers/import_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/analyzers/importable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/analyzers/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/analyzers/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/analyzers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:07:58.294135 unimport-1.0.0/src/unimport/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/commands/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/commands/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/commands/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-07 11:07:44.000000 unimport-1.0.0/src/unimport/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:07:58.294135 unimport-1.0.0/src/unimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-07 11:07:58.000000 unimport-1.0.0/src/unimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-07 11:07:58.000000 unimport-1.0.0/src/unimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:07:58.000000 unimport-1.0.0/src/unimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 11:07:58.000000 unimport-1.0.0/src/unimport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 11:07:58.000000 unimport-1.0.0/src/unimport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 11:07:58.000000 unimport-1.0.0/src/unimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:07:58.000000 unimport-1.0.0/src/unimport.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:07:58.294135 unimport-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-07 11:07:44.000000 unimport-1.0.0/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 11:07:44.000000 unimport-1.0.0/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-07 11:07:44.000000 unimport-1.0.0/tests/test_linesep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-07 11:07:44.000000 unimport-1.0.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-07 11:07:44.000000 unimport-1.0.0/tests/test_utils.py
```

### Comparing `unimport-0.9.6/LICENSE` & `unimport-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unimport-0.9.6/PKG-INFO` & `unimport-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 Metadata-Version: 2.1
 Name: unimport
-Version: 0.9.6
-Summary: A linter, formatter for finding and removing unused import statements.
-Home-page: https://github.com/hakancelik96/unimport
+Version: 1.0.0
+Summary: The ultimate linter and formatter for removing unused import statements in your code.
+Home-page: https://unimport.hakancelik.dev/
 Author: Hakan Çelik
-Author-email: hakancelik96@outlook.com
+Author-email: hakancelikdev@gmail.com
 License: MIT
 Project-URL: Documentation, https://unimport.hakancelik.dev/
-Project-URL: Issues, https://github.com/hakancelik96/unimport/issues
-Project-URL: Changelog, https://unimport.hakancelik.dev/changelog/
-Description: ![unimport](docs/assets/logo/unimport.png)
-        
-        **A linter, formatter for finding and removing unused import statements.**
-        
-        [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hakancelik96/unimport/master.svg)](https://results.pre-commit.ci/latest/github/hakancelik96/unimport/master)
-        ![test](https://github.com/hakancelik96/unimport/workflows/Test/badge.svg)
-        
-        [![Pypi](https://img.shields.io/pypi/v/unimport)](https://pypi.org/project/unimport/)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unimport)
-        [![Downloads](https://static.pepy.tech/personalized-badge/unimport?period=total&units=none&left_color=grey&right_color=red&left_text=downloads)](https://pepy.tech/project/unimport)
-        [![License](https://img.shields.io/github/license/hakancelik96/unimport.svg)](https://github.com/hakancelik96/unimport/blob/master/LICENSE)
-        
-        [![Forks](https://img.shields.io/github/forks/hakancelik96/unimport)](https://github.com/hakancelik96/unimport/fork)
-        [![Issues](https://img.shields.io/github/issues/hakancelik96/unimport)](https://github.com/hakancelik96/unimport/issues)
-        [![Stars](https://img.shields.io/github/stars/hakancelik96/unimport)](https://github.com/hakancelik96/unimport/stargazers)
-        
-        [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ad6385b18b524cf2b100aa646358b89f)](https://www.codacy.com/gh/hakancelik96/unimport/dashboard?utm_source=github.com&utm_medium=referral&utm_content=hakancelik96/unimport&utm_campaign=Badge_Grade)
-        [![Codecov](https://codecov.io/gh/hakancelik96/unimport/branch/master/graph/badge.svg)](https://codecov.io/gh/hakancelik96/unimport)
-        [![Contributors](https://img.shields.io/github/contributors/hakancelik96/unimport)](https://github.com/hakancelik96/unimport/graphs/contributors)
-        [![Last Commit](https://img.shields.io/github/last-commit/hakancelik96/unimport.svg)](https://github.com/hakancelik96/unimport/commits/master)
-        
-        For more information see: https://unimport.hakancelik.dev/
-        
+Project-URL: Issues, https://github.com/hakancelikdev/unimport/issues/
+Project-URL: Changelog, https://unimport.hakancelik.dev/1.0.0/CHANGELOG/
 Keywords: unused,import
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Environment :: Console
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Environment :: Console
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
+![unimport](https://raw.githubusercontent.com/hakancelikdev/unimport/main/docs/assets/logo/unimport.png)
+
+**🚀 The ultimate linter and formatter for removing unused import statements in your
+code.**
+
+Looking for a way to eliminate those pesky unused import statements in your code? Look
+no further than Unimport! This powerful tool serves as both a linter and formatter,
+making it easy to detect and remove any imports that are no longer needed. Say goodbye
+to cluttered, inefficient code and hello to a cleaner, more streamlined development
+process with Unimport.
+
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hakancelikdev/unimport/main.svg)](https://results.pre-commit.ci/latest/github/hakancelikdev/unimport/main)
+![test](https://github.com/hakancelikdev/unimport/workflows/Test/badge.svg)
+
+[![Pypi](https://img.shields.io/pypi/v/unimport)](https://pypi.org/project/unimport/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unimport)
+[![Downloads](https://static.pepy.tech/personalized-badge/unimport?period=total&units=international_system&left_color=grey&right_color=red&left_text=downloads)](https://pepy.tech/project/unimport)
+[![License](https://img.shields.io/github/license/hakancelikdev/unimport.svg)](https://github.com/hakancelikdev/unimport/blob/main/LICENSE)
+
+[![Forks](https://img.shields.io/github/forks/hakancelikdev/unimport)](https://github.com/hakancelikdev/unimport/fork)
+[![Issues](https://img.shields.io/github/issues/hakancelikdev/unimport)](https://github.com/hakancelikdev/unimport/issues)
+[![Stars](https://img.shields.io/github/stars/hakancelikdev/unimport)](https://github.com/hakancelikdev/unimport/stargazers)
+
+[![Codecov](https://codecov.io/gh/hakancelikdev/unimport/branch/main/graph/badge.svg)](https://codecov.io/gh/hakancelikdev/unimport)
+[![Contributors](https://img.shields.io/github/contributors/hakancelikdev/unimport)](https://github.com/hakancelikdev/unimport/graphs/contributors)
+[![Last Commit](https://img.shields.io/github/last-commit/hakancelikdev/unimport.svg)](https://github.com/hakancelikdev/unimport/commits/main)
+
+For more information see: https://unimport.hakancelik.dev/
+
+Try it out now using the Unimport Playground,
+https://playground-unimport.hakancelik.dev/
```

### Comparing `unimport-0.9.6/unimport/color.py` & `unimport-1.0.0/src/unimport/color.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-import argparse
 import sys
 from typing import Tuple
 
+from unimport.enums import Color
+
 __all__ = (
-    "BLACK",
-    "BLUE",
-    "BOLD_WHITE",
-    "COLOR_CHOICES",
-    "CYAN",
-    "GREEN",
-    "MAGENTA",
-    "RED",
-    "RESET",
     "TERMINAL_SUPPORT_COLOR",
-    "WHITE",
-    "YELLOW",
-    "add_color_option",
     "difference",
     "paint",
-    "use_color",
 )
 
 if sys.platform == "win32":  # pragma: no cover (windows)
 
     def _enable() -> None:
         from ctypes import POINTER, WINFUNCTYPE, WinError, windll
         from ctypes.wintypes import BOOL, DWORD, HANDLE
@@ -70,59 +58,24 @@
     except OSError:
         TERMINAL_SUPPORT_COLOR = False
     else:
         TERMINAL_SUPPORT_COLOR = True
 else:  # pragma: win32 no cover
     TERMINAL_SUPPORT_COLOR = True
 
-RESET = "\033[0m"
-BLACK = "\033[30m"
-RED = "\033[31m"
-GREEN = "\033[32m"
-YELLOW = "\033[33m"
-BLUE = "\033[34m"
-MAGENTA = "\033[35m"
-CYAN = "\033[36m"
-WHITE = "\033[97m"
-BOLD_WHITE = "\033[1;37m"
-
-COLOR_CHOICES = ("auto", "always", "never")
-
-
-def paint(text: str, color: str, use_color_setting: bool = True) -> str:
-    if use_color_setting:
-        return color + text + RESET
-    else:
-        return text
-
-
-def use_color(setting: str) -> bool:
-    if setting not in COLOR_CHOICES:
-        raise ValueError(setting)
-
-    return setting == "always" or (
-        setting == "auto" and sys.stderr.isatty() and TERMINAL_SUPPORT_COLOR
-    )
-
 
-def add_color_option(parser: argparse.ArgumentParser) -> None:
-    parser.add_argument(
-        "--color",
-        default="auto",
-        type=use_color,
-        metavar="{" + ",".join(COLOR_CHOICES) + "}",
-        help="Select whether to use color in the output. Defaults to `%(default)s`.",
-    )
+def paint(text: str, color: Color, use_color: bool = True) -> str:
+    return color.value + text + Color.RESET.value if use_color else text
 
 
-def difference(text: Tuple[str, ...]) -> str:  # pragma: no cover
+def difference(text: Tuple[str, ...], use_color: bool = True) -> str:  # pragma: no cover
     lines = list(text)
     for i, line in enumerate(lines):
         if line.startswith("+++") or line.startswith("---"):
-            lines[i] = paint(line, BOLD_WHITE)
+            lines[i] = paint(line, Color.BOLD_WHITE, use_color)
         elif line.startswith("@@"):
-            lines[i] = paint(line, CYAN)
+            lines[i] = paint(line, Color.CYAN, use_color)
         elif line.startswith("+"):
-            lines[i] = paint(line, GREEN)
+            lines[i] = paint(line, Color.GREEN, use_color)
         elif line.startswith("-"):
-            lines[i] = paint(line, RED)
+            lines[i] = paint(line, Color.RED, use_color)
     return "\n".join(lines)
```

### Comparing `unimport-0.9.6/unimport/refactor.py` & `unimport-1.0.0/src/unimport/refactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import List, Optional, Sequence, Union, cast
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.metadata import CodeRange, PositionProvider
 
-from unimport import constants as C
+from unimport import typing as T
 from unimport.statement import Import, ImportFrom
 
 __all__ = ("refactor_string",)
 
 
 class _RemoveUnusedImportTransformer(cst.CSTTransformer):
     __slots__ = ("unused_imports",)
 
     METADATA_DEPENDENCIES = (PositionProvider,)
 
-    def __init__(
-        self, unused_imports: List[Union[Import, ImportFrom]]
-    ) -> None:
+    def __init__(self, unused_imports: List[Union[Import, ImportFrom]]) -> None:
+        super().__init__()
+
         self.unused_imports = unused_imports
 
     @staticmethod
     def get_import_name_from_attr(attr_node: cst.Attribute) -> str:
         name = [attr_node.attr.value]  # last value
         node = attr_node.value
         while m.matches(node, m.OneOf(m.Name(), m.Attribute())):
@@ -30,89 +30,71 @@
                 node = node.value
             else:
                 name.append(cst.ensure_type(node, cst.Name).value)
                 break
         name.reverse()
         return ".".join(name)
 
-    def is_import_used(
-        self, import_name: str, column: int, location: CodeRange
-    ) -> bool:
+    def is_import_used(self, import_name: str, column: int, location: CodeRange) -> bool:
         for imp in self.unused_imports:
             if all(
                 (
                     imp.name == import_name,
                     imp.lineno == location.start.line,
                     imp.column == column,
                 )
             ):
                 return False
         return True
 
-    def get_location(
-        self, node: Union[cst.Import, cst.ImportFrom]
-    ) -> CodeRange:
+    def get_location(self, node: Union[cst.Import, cst.ImportFrom]) -> CodeRange:
         return self.get_metadata(cst.metadata.PositionProvider, node)
 
     @staticmethod
-    def get_rpar(
-        rpar: Optional[cst.RightParen], location: CodeRange
-    ) -> Optional[cst.RightParen]:
+    def get_rpar(rpar: Optional[cst.RightParen], location: CodeRange) -> Optional[cst.RightParen]:
         if not rpar or location.start.line == location.end.line:
             return rpar
         else:
-            return cst.RightParen(
-                whitespace_before=cst.ParenthesizedWhitespace()
-            )
+            return cst.RightParen(whitespace_before=cst.ParenthesizedWhitespace())
 
     def leave_import_alike(
-        self, original_node: C.CSTImportT, updated_node: C.CSTImportT
-    ) -> Union[cst.RemovalSentinel, C.CSTImportT]:
+        self, original_node: T.CSTImportT, updated_node: T.CSTImportT
+    ) -> Union[cst.RemovalSentinel, T.CSTImportT]:
         names_to_keep = []
         names = cast(Sequence[cst.ImportAlias], updated_node.names)
         # already handled by leave_ImportFrom
         for column, import_alias in enumerate(names):
             if isinstance(import_alias.name, cst.Attribute):
-                import_name = self.get_import_name_from_attr(
-                    attr_node=import_alias.name
-                )
+                if import_alias.asname:
+                    import_name = import_alias.asname.name.value
+                else:
+                    import_name = self.get_import_name_from_attr(attr_node=import_alias.name)
             else:
                 raw_import = import_alias.asname or import_alias
                 raw_import_name = cst.ensure_type(raw_import.name, cst.Name)
                 import_name = raw_import_name.value
-            if self.is_import_used(
-                import_name, column + 1, self.get_location(original_node)
-            ):
+            if self.is_import_used(import_name, column + 1, self.get_location(original_node)):
                 names_to_keep.append(import_alias)
         if not names_to_keep:
             return cst.RemoveFromParent()
         elif len(names) == len(names_to_keep):
             return updated_node
         else:
-            names_to_keep[-1] = names_to_keep[-1].with_changes(
-                comma=cst.MaybeSentinel.DEFAULT
-            )
+            names_to_keep[-1] = names_to_keep[-1].with_changes(comma=cst.MaybeSentinel.DEFAULT)
             if isinstance(updated_node, cst.ImportFrom):
-                rpar = self.get_rpar(
-                    updated_node.rpar, self.get_location(original_node)
-                )
+                rpar = self.get_rpar(updated_node.rpar, self.get_location(original_node))
                 updated_node = updated_node.with_changes(rpar=rpar)
 
             updated_node = updated_node.with_changes(names=names_to_keep)
-            return cast(C.CSTImportT, updated_node)
+            return cast(T.CSTImportT, updated_node)
 
     @staticmethod
-    def leave_StarImport(
-        updated_node: cst.ImportFrom,
-        imp: ImportFrom,
-    ) -> Union[cst.ImportFrom, cst.RemovalSentinel]:
+    def leave_StarImport(updated_node: cst.ImportFrom, imp: ImportFrom) -> Union[cst.ImportFrom, cst.RemovalSentinel]:
         if imp.suggestions:
-            names_to_suggestions = [
-                cst.ImportAlias(cst.Name(module)) for module in imp.suggestions
-            ]
+            names_to_suggestions = [cst.ImportAlias(cst.Name(module)) for module in imp.suggestions]
             return updated_node.with_changes(names=names_to_suggestions)
         else:
             return cst.RemoveFromParent()
 
     def leave_Import(
         self, original_node: cst.Import, updated_node: cst.Import
     ) -> Union[cst.RemovalSentinel, cst.Import]:
@@ -121,42 +103,33 @@
     def leave_ImportFrom(
         self, original_node: cst.ImportFrom, updated_node: cst.ImportFrom
     ) -> Union[cst.RemovalSentinel, cst.ImportFrom]:
         if isinstance(updated_node.names, cst.ImportStar):
 
             def get_star_imp() -> Optional[ImportFrom]:
                 if isinstance(updated_node.module, cst.Attribute):
-                    import_name = self.get_import_name_from_attr(
-                        attr_node=updated_node.module
-                    )
+                    import_name = self.get_import_name_from_attr(attr_node=updated_node.module)
                 else:
                     import_name = updated_node.module.value
                 location = self.get_location(original_node)
                 for imp in self.unused_imports:
-                    if (
-                        isinstance(imp, ImportFrom)
-                        and imp.name == import_name
-                        and imp.lineno == location.start.line
-                    ):
+                    if isinstance(imp, ImportFrom) and imp.name == import_name and imp.lineno == location.start.line:
                         return imp
                 else:
                     return None
 
             imp = get_star_imp()
             if imp:
                 return self.leave_StarImport(updated_node, imp)
             else:
                 return original_node
+
         return self.leave_import_alike(original_node, updated_node)
 
 
-def refactor_string(
-    source: str,
-    unused_imports: List[Union[Import, ImportFrom]],
-) -> str:
+def refactor_string(source: str, unused_imports: List[Union[Import, ImportFrom]]) -> str:
     if unused_imports:
         wrapper = cst.MetadataWrapper(cst.parse_module(source))
-        fixed_module = wrapper.visit(
-            _RemoveUnusedImportTransformer(unused_imports)
-        )
+        fixed_module = wrapper.visit(_RemoveUnusedImportTransformer(unused_imports))
         return fixed_module.code
+
     return source
```

### Comparing `unimport-0.9.6/unimport/statement.py` & `unimport-1.0.0/src/unimport/statement.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,66 @@
 import ast
+import dataclasses
 import operator
-import sys
-from dataclasses import dataclass, field
-from typing import ClassVar, Iterator, List, Set, Union
+from typing import ClassVar, Iterator, List, Optional, Set, Union
 
-if sys.version_info >= (3, 8):
+from unimport import constants as C
+
+if C.PY38_PLUS:
     from typing import Literal  # unimport: skip
 else:
-    from typing_extensions import Literal
+    from typing_extensions import Literal  # type: ignore
 
 
 __all__ = ("Import", "ImportFrom", "Name", "Scope")
 
 
-@dataclass
+@dataclasses.dataclass
 class Import:
     imports: ClassVar[List[Union["Import", "ImportFrom"]]] = []
 
     lineno: int
     column: int
     name: str
     package: str
 
-    node: ast.AST = field(init=False, repr=False, compare=False)
+    node: Union[ast.Import, ast.ImportFrom] = dataclasses.field(init=False, repr=False, compare=False)
 
     def __len__(self) -> int:
         return operator.length_hint(self.name.split("."))
 
-    def is_match_sub_packages(self, name_name) -> bool:
+    def is_match_sub_packages(self, name_name: str) -> bool:
         return self.name.split(".")[0] == name_name
 
     @property
     def scope(self):
         return Scope.get_scope_by_current_node(self)
 
     def is_used(self) -> bool:
         for name in self.scope.names:
-            if name is None:
-                continue
-
             if name.match_import:
                 if name.match_import == self:
                     return True
             elif name.match(self):
                 return True
 
         return False
 
     def match_nearest_duplicate_import(self, name: "Name") -> bool:
         nearest_import = None
 
         scope = name.scope
         while scope:
-            imports = [
-                _import
-                for _import in scope.imports
-                if name.match_2(_import) and name.lineno > _import.lineno
-            ]
+            imports = [_import for _import in scope.imports if name.match_2(_import) and name.lineno > _import.lineno]
             scope = scope.parent
 
             if imports:
                 nearest_import = max(
                     filter(
-                        lambda _import: _import.lineno
-                        == max(
-                            imports, key=lambda _import: _import.lineno
-                        ).lineno,
+                        lambda _import: _import.lineno == max(imports, key=lambda _import: _import.lineno).lineno,
                         imports,
                     ),
                     key=lambda _import: _import.column,
                 )
 
             if nearest_import == self:
                 return True
@@ -77,97 +68,87 @@
         return False
 
     @property
     def is_duplicate(self) -> bool:
         return [_import.name for _import in self.imports].count(self.name) > 1
 
     @classmethod
-    def get_unused_imports(
-        cls, include_star_import: bool = False
-    ) -> Iterator[Union["Import", "ImportFrom"]]:
+    def get_unused_imports(cls, *, include_star_import: bool = False) -> Iterator[Union["Import", "ImportFrom"]]:
         for imp in reversed(Import.imports):
-            if (
-                include_star_import
-                and isinstance(imp, ImportFrom)
-                and imp.star
-            ):
+            if include_star_import and isinstance(imp, ImportFrom) and imp.star:
                 yield imp
             elif not imp.is_used():
                 yield imp
 
     @classmethod
-    def register(
-        cls, lineno: int, column: int, name: str, package: str, node: ast.AST
-    ) -> None:
+    def register(cls, *, lineno: int, column: int, name: str, package: str, node: ast.Import) -> None:
         _import = cls(lineno, column, name, package)
         _import.node = node
         cls.imports.append(_import)
 
         Scope.register(_import)
 
     @classmethod
     def clear(cls):
         cls.imports.clear()
 
 
-@dataclass
+@dataclasses.dataclass
 class ImportFrom(Import):
     star: bool
     suggestions: List[str]
 
-    def is_match_sub_packages(self, name_name):
+    def is_match_sub_packages(self, name_name: str) -> Literal[False]:
         return False
 
     @classmethod
     def register(  # type: ignore
         cls,
+        *,
         lineno: int,
         column: int,
         name: str,
         package: str,
-        node: ast.AST,
         star: bool,
         suggestions: List[str],
+        node: ast.ImportFrom,
     ) -> None:
         _import = cls(lineno, column, name, package, star, suggestions)
         _import.node = node
         cls.imports.append(_import)
 
         Scope.register(_import)
 
 
-@dataclass
+@dataclasses.dataclass
 class Name:
     names: ClassVar[List["Name"]] = []
 
     lineno: int
     name: str
     is_all: bool = False
 
-    node: ast.AST = field(init=False, repr=False, compare=False)
-    match_import: Union[Import, Literal[False]] = field(
+    node: Union[ast.Name, ast.Attribute, ast.Constant] = dataclasses.field(init=False, repr=False, compare=False)
+    match_import: Union[Import, ImportFrom, Literal[False]] = dataclasses.field(
         init=False, repr=False, compare=False, default=False
     )
 
     @property
     def is_attribute(self):
         return "." in self.name
 
     def match_2(self, imp: Union[Import, ImportFrom]) -> bool:
         if self.is_all:
             is_match = self.name == imp.name
         elif self.is_attribute:
             is_match = imp.lineno < self.lineno and (
-                ".".join(self.name.split(".")[: len(imp)]) == imp.name
-                or imp.is_match_sub_packages(self.name)
+                ".".join(self.name.split(".")[: len(imp)]) == imp.name or imp.is_match_sub_packages(self.name)
             )
         else:
-            is_match = (imp.lineno < self.lineno) and (
-                self.name == imp.name or imp.is_match_sub_packages(self.name)
-            )
+            is_match = (imp.lineno < self.lineno) and (self.name == imp.name or imp.is_match_sub_packages(self.name))
 
         return is_match
 
     def match(self, imp: Union[Import, ImportFrom]) -> bool:
         is_match = self.match_2(imp)
 
         if is_match and imp.is_duplicate:
@@ -180,47 +161,45 @@
 
     @property
     def scope(self):
         return Scope.get_scope_by_current_node(self)
 
     @classmethod
     def register(
-        cls, lineno: int, name: str, node: ast.AST, is_all: bool = False
+        cls, *, lineno: int, name: str, node: Union[ast.Name, ast.Attribute, ast.Constant], is_all: bool = False
     ) -> None:
         _name = cls(lineno, name, is_all)
         _name.node = node
         cls.names.append(_name)
 
         Scope.register(_name, is_global=is_all)
 
     @classmethod
     def clear(cls) -> None:
         cls.names.clear()
 
 
-@dataclass
+@dataclasses.dataclass
 class Scope:
     scopes: ClassVar[List["Scope"]] = []
     current_scope: ClassVar[List["Scope"]] = []
 
     node: ast.AST
 
-    current_nodes: List[Union[Import, ImportFrom, Name]] = field(
+    current_nodes: List[Union[Import, ImportFrom, Name]] = dataclasses.field(
         default_factory=list, init=False, repr=False, compare=False
     )
-    parent: "Scope" = field(default=None, repr=False)
-    child_scopes: Set["Scope"] = field(
-        default_factory=set, init=False, repr=False, compare=False
-    )
+    parent: "Scope" = dataclasses.field(default=None, repr=False)
+    child_scopes: Set["Scope"] = dataclasses.field(default_factory=set, init=False, repr=False, compare=False)
 
     def __hash__(self) -> int:
         return hash(self.node)
 
     @classmethod
-    def get_curent_scope(cls) -> "Scope":
+    def get_current_scope(cls) -> "Scope":
         return cls.current_scope[-1]
 
     @classmethod
     def get_global_scope(cls) -> "Scope":
         global_scope = cls.scopes[0]
         assert global_scope.parent is None
         return global_scope
@@ -230,29 +209,25 @@
         parent = None
         scope = Scope(tree, parent)
         cls.current_scope.append(scope)
         cls.scopes.append(scope)  # global scope added to cls.scopes
 
     @classmethod
     def add_current_scope(cls, node: ast.AST) -> None:
-        parent = cls.get_curent_scope()
+        parent = cls.get_current_scope()
         scope = Scope(node, parent)
         cls.current_scope.append(scope)
 
     @classmethod
     def remove_current_scope(cls):
         cls.current_scope.pop()
 
     @classmethod
-    def register(
-        cls, current_node: Union[Import, ImportFrom, Name], *, is_global=False
-    ) -> None:
-        scope = cls.get_previous_scope(
-            cls.get_global_scope() if is_global else cls.get_curent_scope()
-        )
+    def register(cls, current_node: Union[Import, ImportFrom, Name], *, is_global=False) -> None:
+        scope = cls.get_previous_scope(cls.get_global_scope() if is_global else cls.get_current_scope())
 
         # current nodes add to scope
         scope.current_nodes.append(current_node)
 
         # child scopes add to scope
         if scope.parent is None:
             return
@@ -265,36 +240,31 @@
 
             child_scope = parent
             if parent.parent is None:
                 break
             parent = cls.get_previous_scope(parent.parent)
 
     @classmethod
-    def get_scope_by_current_node(
-        cls, current_node: Union[Import, ImportFrom, Name]
-    ) -> "Scope":
+    def get_scope_by_current_node(cls, current_node: Union[Import, ImportFrom, Name]) -> Optional["Scope"]:
         for scope in cls.scopes:
             if current_node in scope.current_nodes:
                 return scope
+
         return None
 
     @property
     def names(self) -> Iterator[Name]:
-        yield from filter(  # type: ignore
-            lambda node: isinstance(node, Name), self.current_nodes
-        )
+        yield from filter(lambda node: isinstance(node, Name), self.current_nodes)  # type: ignore
 
         for child_scope in self.child_scopes:
             yield from child_scope.names
 
     @property
     def imports(self) -> Iterator[Import]:
-        yield from filter(  # type: ignore
-            lambda node: isinstance(node, Import), self.current_nodes
-        )
+        yield from filter(lambda node: isinstance(node, Import), self.current_nodes)  # type: ignore
 
     @classmethod
     def get_previous_scope(cls, scope: "Scope") -> "Scope":
         for _scope in cls.scopes:
             if _scope == scope:
                 return _scope
```

### Comparing `unimport-0.9.6/unimport.egg-info/PKG-INFO` & `unimport-1.0.0/src/unimport.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 Metadata-Version: 2.1
 Name: unimport
-Version: 0.9.6
-Summary: A linter, formatter for finding and removing unused import statements.
-Home-page: https://github.com/hakancelik96/unimport
+Version: 1.0.0
+Summary: The ultimate linter and formatter for removing unused import statements in your code.
+Home-page: https://unimport.hakancelik.dev/
 Author: Hakan Çelik
-Author-email: hakancelik96@outlook.com
+Author-email: hakancelikdev@gmail.com
 License: MIT
 Project-URL: Documentation, https://unimport.hakancelik.dev/
-Project-URL: Issues, https://github.com/hakancelik96/unimport/issues
-Project-URL: Changelog, https://unimport.hakancelik.dev/changelog/
-Description: ![unimport](docs/assets/logo/unimport.png)
-        
-        **A linter, formatter for finding and removing unused import statements.**
-        
-        [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hakancelik96/unimport/master.svg)](https://results.pre-commit.ci/latest/github/hakancelik96/unimport/master)
-        ![test](https://github.com/hakancelik96/unimport/workflows/Test/badge.svg)
-        
-        [![Pypi](https://img.shields.io/pypi/v/unimport)](https://pypi.org/project/unimport/)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unimport)
-        [![Downloads](https://static.pepy.tech/personalized-badge/unimport?period=total&units=none&left_color=grey&right_color=red&left_text=downloads)](https://pepy.tech/project/unimport)
-        [![License](https://img.shields.io/github/license/hakancelik96/unimport.svg)](https://github.com/hakancelik96/unimport/blob/master/LICENSE)
-        
-        [![Forks](https://img.shields.io/github/forks/hakancelik96/unimport)](https://github.com/hakancelik96/unimport/fork)
-        [![Issues](https://img.shields.io/github/issues/hakancelik96/unimport)](https://github.com/hakancelik96/unimport/issues)
-        [![Stars](https://img.shields.io/github/stars/hakancelik96/unimport)](https://github.com/hakancelik96/unimport/stargazers)
-        
-        [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ad6385b18b524cf2b100aa646358b89f)](https://www.codacy.com/gh/hakancelik96/unimport/dashboard?utm_source=github.com&utm_medium=referral&utm_content=hakancelik96/unimport&utm_campaign=Badge_Grade)
-        [![Codecov](https://codecov.io/gh/hakancelik96/unimport/branch/master/graph/badge.svg)](https://codecov.io/gh/hakancelik96/unimport)
-        [![Contributors](https://img.shields.io/github/contributors/hakancelik96/unimport)](https://github.com/hakancelik96/unimport/graphs/contributors)
-        [![Last Commit](https://img.shields.io/github/last-commit/hakancelik96/unimport.svg)](https://github.com/hakancelik96/unimport/commits/master)
-        
-        For more information see: https://unimport.hakancelik.dev/
-        
+Project-URL: Issues, https://github.com/hakancelikdev/unimport/issues/
+Project-URL: Changelog, https://unimport.hakancelik.dev/1.0.0/CHANGELOG/
 Keywords: unused,import
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Environment :: Console
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Environment :: Console
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
+![unimport](https://raw.githubusercontent.com/hakancelikdev/unimport/main/docs/assets/logo/unimport.png)
+
+**🚀 The ultimate linter and formatter for removing unused import statements in your
+code.**
+
+Looking for a way to eliminate those pesky unused import statements in your code? Look
+no further than Unimport! This powerful tool serves as both a linter and formatter,
+making it easy to detect and remove any imports that are no longer needed. Say goodbye
+to cluttered, inefficient code and hello to a cleaner, more streamlined development
+process with Unimport.
+
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/hakancelikdev/unimport/main.svg)](https://results.pre-commit.ci/latest/github/hakancelikdev/unimport/main)
+![test](https://github.com/hakancelikdev/unimport/workflows/Test/badge.svg)
+
+[![Pypi](https://img.shields.io/pypi/v/unimport)](https://pypi.org/project/unimport/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unimport)
+[![Downloads](https://static.pepy.tech/personalized-badge/unimport?period=total&units=international_system&left_color=grey&right_color=red&left_text=downloads)](https://pepy.tech/project/unimport)
+[![License](https://img.shields.io/github/license/hakancelikdev/unimport.svg)](https://github.com/hakancelikdev/unimport/blob/main/LICENSE)
+
+[![Forks](https://img.shields.io/github/forks/hakancelikdev/unimport)](https://github.com/hakancelikdev/unimport/fork)
+[![Issues](https://img.shields.io/github/issues/hakancelikdev/unimport)](https://github.com/hakancelikdev/unimport/issues)
+[![Stars](https://img.shields.io/github/stars/hakancelikdev/unimport)](https://github.com/hakancelikdev/unimport/stargazers)
+
+[![Codecov](https://codecov.io/gh/hakancelikdev/unimport/branch/main/graph/badge.svg)](https://codecov.io/gh/hakancelikdev/unimport)
+[![Contributors](https://img.shields.io/github/contributors/hakancelikdev/unimport)](https://github.com/hakancelikdev/unimport/graphs/contributors)
+[![Last Commit](https://img.shields.io/github/last-commit/hakancelikdev/unimport.svg)](https://github.com/hakancelikdev/unimport/commits/main)
+
+For more information see: https://unimport.hakancelik.dev/
+
+Try it out now using the Unimport Playground,
+https://playground-unimport.hakancelik.dev/
```


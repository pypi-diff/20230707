# Comparing `tmp/lithium-reducer-0.6.2.tar.gz` & `tmp/lithium-reducer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lithium-reducer-0.6.2.tar", last modified: Mon Jan 31 22:04:16 2022, max compression
+gzip compressed data, was "lithium-reducer-1.0.0.tar", last modified: Fri Jul  7 17:08:40 2023, max compression
```

## Comparing `lithium-reducer-0.6.2.tar` & `lithium-reducer-1.0.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.285546 lithium-reducer-0.6.2/
--rw-r--r--   0 worker    (1000) worker    (1000)      238 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/.gitattributes
--rw-r--r--   0 worker    (1000) worker    (1000)      416 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/.gitignore
--rw-r--r--   0 worker    (1000) worker    (1000)     1624 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 worker    (1000) worker    (1000)     2775 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/.taskcluster.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      689 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 worker    (1000) worker    (1000)    16725 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/LICENSE
--rw-r--r--   0 worker    (1000) worker    (1000)     7257 2022-01-31 22:04:16.285546 lithium-reducer-0.6.2/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     6302 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/README.md
--rw-r--r--   0 worker    (1000) worker    (1000)      981 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/pyproject.toml
--rw-r--r--   0 worker    (1000) worker    (1000)     1886 2022-01-31 22:04:16.285546 lithium-reducer-0.6.2/setup.cfg
--rwxr-xr-x   0 worker    (1000) worker    (1000)      385 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/setup.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.277546 lithium-reducer-0.6.2/src/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.281546 lithium-reducer-0.6.2/src/lithium/
--rw-r--r--   0 worker    (1000) worker    (1000)      412 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)      296 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/__main__.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.281546 lithium-reducer-0.6.2/src/lithium/docs/
--rw-r--r--   0 worker    (1000) worker    (1000)     6367 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/docs/algorithm.md
--rw-r--r--   0 worker    (1000) worker    (1000)     1484 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/docs/creating-tests.md
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.281546 lithium-reducer-0.6.2/src/lithium/docs/examples/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.281546 lithium-reducer-0.6.2/src/lithium/docs/examples/arithmetic/
--rw-r--r--   0 worker    (1000) worker    (1000)       48 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/docs/examples/arithmetic/11.txt
--rw-r--r--   0 worker    (1000) worker    (1000)     1032 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/docs/examples/arithmetic/product_divides.py
--rw-r--r--   0 worker    (1000) worker    (1000)       50 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/docs/examples/crash.c
--rw-r--r--   0 worker    (1000) worker    (1000)      205 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/docs/related.txt
--rw-r--r--   0 worker    (1000) worker    (1000)     3912 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/docs/using-for-firefox.md
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.281546 lithium-reducer-0.6.2/src/lithium/interestingness/
--rw-r--r--   0 worker    (1000) worker    (1000)      338 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/interestingness/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1448 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/interestingness/crashes.py
--rw-r--r--   0 worker    (1000) worker    (1000)     3435 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/interestingness/diff_test.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1278 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/interestingness/hangs.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2061 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/interestingness/outputs.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2839 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/interestingness/repeat.py
--rw-r--r--   0 worker    (1000) worker    (1000)     5962 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/interestingness/timed_run.py
--rw-r--r--   0 worker    (1000) worker    (1000)     4282 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/interestingness/utils.py
--rw-r--r--   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/py.typed
--rw-r--r--   0 worker    (1000) worker    (1000)    11563 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/reducer.py
--rw-r--r--   0 worker    (1000) worker    (1000)    64166 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/strategies.py
--rw-r--r--   0 worker    (1000) worker    (1000)    18202 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/testcases.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2136 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/src/lithium/util.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.285546 lithium-reducer-0.6.2/src/lithium_reducer.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)     7257 2022-01-31 22:04:16.000000 lithium-reducer-0.6.2/src/lithium_reducer.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     1326 2022-01-31 22:04:16.000000 lithium-reducer-0.6.2/src/lithium_reducer.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2022-01-31 22:04:16.000000 lithium-reducer-0.6.2/src/lithium_reducer.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)      734 2022-01-31 22:04:16.000000 lithium-reducer-0.6.2/src/lithium_reducer.egg-info/entry_points.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2022-01-31 22:04:16.000000 lithium-reducer-0.6.2/src/lithium_reducer.egg-info/not-zip-safe
--rw-r--r--   0 worker    (1000) worker    (1000)       22 2022-01-31 22:04:16.000000 lithium-reducer-0.6.2/src/lithium_reducer.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        8 2022-01-31 22:04:16.000000 lithium-reducer-0.6.2/src/lithium_reducer.egg-info/top_level.txt
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2022-01-31 22:04:16.285546 lithium-reducer-0.6.2/tests/
--rw-r--r--   0 worker    (1000) worker    (1000)     1827 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/tests/conftest.py
--rw-r--r--   0 worker    (1000) worker    (1000)    11776 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/tests/test_interestingness.py
--rw-r--r--   0 worker    (1000) worker    (1000)     3045 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/tests/test_lithium.py
--rw-r--r--   0 worker    (1000) worker    (1000)    10020 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/tests/test_strategies.py
--rw-r--r--   0 worker    (1000) worker    (1000)    16828 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/tests/test_testcases.py
--rw-r--r--   0 worker    (1000) worker    (1000)     4286 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/tests/test_util.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1209 2022-01-31 22:04:04.000000 lithium-reducer-0.6.2/tox.ini
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.279014 lithium-reducer-1.0.0/
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/.gitattributes
+-rw-r--r--   0 worker    (1000) worker    (1000)      416 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/.gitignore
+-rw-r--r--   0 worker    (1000) worker    (1000)     1753 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 worker    (1000) worker    (1000)     2781 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/.taskcluster.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      689 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 worker    (1000) worker    (1000)    16725 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/LICENSE
+-rw-r--r--   0 worker    (1000) worker    (1000)     7010 2023-07-07 17:08:40.279014 lithium-reducer-1.0.0/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     6302 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/README.md
+-rw-r--r--   0 worker    (1000) worker    (1000)      959 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1715 2023-07-07 17:08:40.279014 lithium-reducer-1.0.0/setup.cfg
+-rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/setup.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.267014 lithium-reducer-1.0.0/src/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.271014 lithium-reducer-1.0.0/src/lithium/
+-rw-r--r--   0 worker    (1000) worker    (1000)      397 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      281 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/__main__.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.271014 lithium-reducer-1.0.0/src/lithium/docs/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6367 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/docs/algorithm.md
+-rw-r--r--   0 worker    (1000) worker    (1000)     1484 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/docs/creating-tests.md
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.275014 lithium-reducer-1.0.0/src/lithium/docs/examples/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.275014 lithium-reducer-1.0.0/src/lithium/docs/examples/arithmetic/
+-rw-r--r--   0 worker    (1000) worker    (1000)       48 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/docs/examples/arithmetic/11.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)     1000 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/docs/examples/arithmetic/product_divides.py
+-rw-r--r--   0 worker    (1000) worker    (1000)       50 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/docs/examples/crash.c
+-rw-r--r--   0 worker    (1000) worker    (1000)      205 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/docs/related.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)     3912 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/docs/using-for-firefox.md
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.275014 lithium-reducer-1.0.0/src/lithium/interestingness/
+-rw-r--r--   0 worker    (1000) worker    (1000)      323 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/interestingness/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1433 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/interestingness/crashes.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3403 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/interestingness/diff_test.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1263 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/interestingness/hangs.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2046 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/interestingness/outputs.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2824 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/interestingness/repeat.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     5904 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/interestingness/timed_run.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     4264 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/interestingness/utils.py
+-rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/py.typed
+-rw-r--r--   0 worker    (1000) worker    (1000)    11514 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/reducer.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    63708 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/strategies.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    18226 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/testcases.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2115 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/src/lithium/util.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.279014 lithium-reducer-1.0.0/src/lithium_reducer.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7010 2023-07-07 17:08:40.000000 lithium-reducer-1.0.0/src/lithium_reducer.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     1326 2023-07-07 17:08:40.000000 lithium-reducer-1.0.0/src/lithium_reducer.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-07-07 17:08:40.000000 lithium-reducer-1.0.0/src/lithium_reducer.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)      733 2023-07-07 17:08:40.000000 lithium-reducer-1.0.0/src/lithium_reducer.egg-info/entry_points.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-07-07 17:08:40.000000 lithium-reducer-1.0.0/src/lithium_reducer.egg-info/not-zip-safe
+-rw-r--r--   0 worker    (1000) worker    (1000)       22 2023-07-07 17:08:40.000000 lithium-reducer-1.0.0/src/lithium_reducer.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        8 2023-07-07 17:08:40.000000 lithium-reducer-1.0.0/src/lithium_reducer.egg-info/top_level.txt
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-07-07 17:08:40.279014 lithium-reducer-1.0.0/tests/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1812 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/tests/conftest.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    11761 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/tests/test_interestingness.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3018 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/tests/test_lithium.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     9921 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/tests/test_strategies.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    16807 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/tests/test_testcases.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     4257 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/tests/test_util.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1276 2023-07-07 17:08:31.000000 lithium-reducer-1.0.0/tox.ini
```

### Comparing `lithium-reducer-0.6.2/.pre-commit-config.yaml` & `lithium-reducer-1.0.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 repos:
   - repo: https://github.com/pycqa/isort
-    rev: 5.9.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/yesqa
-    rev: v1.2.3
+    rev: v1.5.0
     hooks:
       - id: yesqa
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.8.0
+    hooks:
+      - id: pyupgrade
+        args: ['--py38-plus']
   - repo: https://github.com/ambv/black
-    rev: 21.6b0
+    rev: 23.3.0
     hooks:
       - id: black
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.4.0
     hooks:
       - id: check-ast
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-symlinks
       - id: debug-statements
@@ -28,24 +33,24 @@
       - id: trailing-whitespace
       - id: check-yaml
       - id: mixed-line-ending
       - id: name-tests-test
         args: ['--django']
       - id: check-json
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.1.0
+    rev: v2.2.5
     hooks:
       - id: codespell
         exclude_types: [json]
   - repo: https://github.com/marco-c/taskcluster_yml_validator
-    rev: v0.0.7
+    rev: v0.0.10
     hooks:
       - id: taskcluster_yml
   - repo: https://github.com/MozillaSecurity/orion
-    rev: v0.0.2
+    rev: v0.0.7
     hooks:
       - id: orion_ci
   - repo: meta
     hooks:
       - id: check-useless-excludes
   - repo: local
     hooks:
```

### Comparing `lithium-reducer-0.6.2/.taskcluster.yml` & `lithium-reducer-1.0.0/.taskcluster.yml`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,30 @@
           key: token
       script:
         - bash
         - '-xec'
         - tox; tox -e codecov
       jobs:
         include:
-          - name: tests python 3.6
-            version: "3.6"
-            env:
-              TOXENV: py36
-          - name: tests python 3.7
-            version: "3.7"
-            env:
-              TOXENV: py37
           - name: tests python 3.8
             version: "3.8"
             env:
               TOXENV: py38
           - name: tests python 3.9
             version: "3.9"
             env:
               TOXENV: py39
+          - name: tests python 3.10
+            version: "3.10"
+            env:
+              TOXENV: py310
+          - name: tests python 3.11
+            version: "3.11"
+            env:
+              TOXENV: py311
           - name: lint
             version: "3.9"
             env:
               TOXENV: lint
             script:
               - tox
           - name: PyPI upload
```

### Comparing `lithium-reducer-0.6.2/CODE_OF_CONDUCT.md` & `lithium-reducer-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-0.6.2/LICENSE` & `lithium-reducer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lithium-reducer-0.6.2/PKG-INFO` & `lithium-reducer-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: lithium-reducer
-Version: 0.6.2
+Version: 1.0.0
 Summary: Lithium is an automated testcase reduction tool
 Home-page: https://github.com/MozillaSecurity/lithium
 Author: Jesse Ruderman
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: fuzz,fuzzing,reduce,reducer,reduction,security,test,testing
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Task Status](https://community-tc.services.mozilla.com/api/github/v1/repository/MozillaSecurity/lithium/master/badge.svg)](https://community-tc.services.mozilla.com/api/github/v1/repository/MozillaSecurity/lithium/master/latest)
 [![codecov](https://codecov.io/gh/MozillaSecurity/lithium/branch/master/graph/badge.svg)](https://codecov.io/gh/MozillaSecurity/lithium)
 [![Matrix](https://img.shields.io/badge/dynamic/json?color=green&label=chat&query=%24.chunk[%3F(%40.canonical_alias%3D%3D%22%23fuzzing%3Amozilla.org%22)].num_joined_members&suffix=%20users&url=https%3A%2F%2Fmozilla.modular.im%2F_matrix%2Fclient%2Fr0%2FpublicRooms&style=flat&logo=matrix)](https://riot.im/app/#/room/#fuzzing:mozilla.org)
@@ -90,9 +85,7 @@
 
 ### Credits
 
 - [Lithium's testcase reduction algorithm](src/lithium/docs/algorithm.md) is a modified version of the "ddmin" algorithm in Andreas Zeller's paper, [Simplifying and Isolating Failure-Inducing Input](https://www.st.cs.uni-saarland.de/papers/tse2002/).
 - The idea of using an external "interestingness test" program came from [Delta](http://delta.tigris.org/), a similar tool that's [used in clever ways by the GCC project](https://gcc.gnu.org/wiki/A_guide_to_testcase_reduction).
 - [timed_run](src/lithium/interestingness/timed_run.py), used by many of the "interestingness test" scripts that come with Lithium, is based on [timed_run.py](https://web.archive.org/web/20071107032840/http://bclary.com/log/2007/03/07/timed_run), which was written by [Chris Cooper](http://coop.deadsquid.com/) and [Bob Clary](https://bclary.com/).
 - The code was significantly cleaned up and modernized by Jesse Schwartzentruber and Gary Kwong in mid-2017.
-
-
```

### Comparing `lithium-reducer-0.6.2/README.md` & `lithium-reducer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-0.6.2/pyproject.toml` & `lithium-reducer-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -27,28 +27,26 @@
 show_error_codes = true
 
 [tool.pylint.format]
 max-line-length = 88
 
 [tool.pylint.messages_control]
 disable = [
-    "C0330",
-    "C0326",
-    "bad-continuation",
     "duplicate-code",
     "fixme",
     "import-error",
     "subprocess-run-check",
     "too-few-public-methods",
     "too-many-arguments",
     "too-many-branches",
     "too-many-instance-attributes",
     "too-many-lines",
     "too-many-locals",
     "too-many-nested-blocks",
     "too-many-statements",
+    "unspecified-encoding",
 ]
 
 [tool.pytest.ini_options]
 log_level = "DEBUG"
 
 [tool.setuptools_scm]
```

### Comparing `lithium-reducer-0.6.2/setup.cfg` & `lithium-reducer-1.0.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 [metadata]
 author = Jesse Ruderman
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.5
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Topic :: Security
 	Topic :: Software Development :: Testing
 description = Lithium is an automated testcase reduction tool
 keywords = 
 	fuzz
 	fuzzing
 	reduce
@@ -31,14 +26,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = 
 	lithium
 	lithium.interestingness
+python_requires = >=3.8
 zip_safe = False
 
 [options.entry_points]
 console_scripts = 
 	lithium = lithium.reducer:main
 lithium_strategies = 
 	check-only = lithium.strategies:CheckOnly
```

### Comparing `lithium-reducer-0.6.2/src/lithium/docs/algorithm.md` & `lithium-reducer-1.0.0/src/lithium/docs/algorithm.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-0.6.2/src/lithium/docs/creating-tests.md` & `lithium-reducer-1.0.0/src/lithium/docs/creating-tests.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-0.6.2/src/lithium/docs/examples/arithmetic/product_divides.py` & `lithium-reducer-1.0.0/src/lithium/docs/examples/arithmetic/product_divides.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 """This tests Lithium's main "minimize" algorithm."""
 
@@ -20,19 +19,19 @@
     Returns:
         True if successful, False otherwise.
     """
     mod = int(args[0])
     filename = args[1]
 
     prod = 1
-    with open(filename, "r") as input_fp:
+    with open(filename) as input_fp:
         for line in input_fp:
             line = line.strip()
             if line.isdigit():
                 prod *= int(line)
 
     if prod % mod == 0:
-        sys.stdout.write("%d is divisible by %d\n" % (prod, mod))
+        sys.stdout.write(f"{prod} is divisible by {mod}\n")
         return True
 
-    sys.stdout.write("%d is not divisible by %d\n" % (prod, mod))
+    sys.stdout.write(f"{prod} is not divisible by {mod}\n")
     return False
```

### Comparing `lithium-reducer-0.6.2/src/lithium/docs/using-for-firefox.md` & `lithium-reducer-1.0.0/src/lithium/docs/using-for-firefox.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-0.6.2/src/lithium/interestingness/crashes.py` & `lithium-reducer-1.0.0/src/lithium/interestingness/hangs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-# coding=utf-8
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-"""Lithium's "crashes" interestingness test to assess whether a binary crashes.
+"""Lithium's "hangs" interestingness test to assess whether a binary hangs.
 
 Example:
-    python -m lithium crashes --timeout=9 <binary> --fuzzing-safe <testcase>
+    python -m lithium hangs --timeout=3 <binary> --fuzzing-safe <testcase>
 """
 
 import logging
 from typing import List
 
 from . import timed_run
 
 
 def interesting(cli_args: List[str], temp_prefix: str) -> bool:
-    """Interesting if the binary causes a crash. (e.g. SIGKILL/SIGTERM/SIGTRAP etc.)
+    """Interesting if the binary causes a hang.
 
     Args:
         cli_args: List of input arguments.
         temp_prefix: Temporary directory prefix, e.g. tmp1/1 or tmp4/1
 
     Returns:
-        True if binary crashes, False otherwise.
+        True if binary causes a hang, False otherwise.
     """
     parser = timed_run.ArgumentParser(
-        prog="crashes",
+        prog="hangs",
         usage="python -m lithium %(prog)s [options] binary [flags] testcase.ext",
     )
     args = parser.parse_args(cli_args)
 
     log = logging.getLogger(__name__)
-    # Run the program with desired flags and look out for crashes.
     runinfo = timed_run.timed_run(args.cmd_with_flags, args.timeout, temp_prefix)
 
-    time_str = " (%.3f seconds)" % runinfo.elapsedtime
-    if runinfo.sta == timed_run.CRASHED:
-        log.info("Exit status: " + runinfo.msg + time_str)
+    if runinfo.sta == timed_run.TIMED_OUT:
+        log.info("Timed out after %.3f seconds", args.timeout)
         return True
 
-    log.info("[Uninteresting] It didn't crash: " + runinfo.msg + time_str)
+    log.info("Exited in %.3f seconds", runinfo.elapsedtime)
     return False
```

### Comparing `lithium-reducer-0.6.2/src/lithium/interestingness/diff_test.py` & `lithium-reducer-1.0.0/src/lithium/interestingness/diff_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 """Lithium's "diff_test" interestingness test to assess whether a binary shows a
 difference in output when different command line arguments are passed in. This can be
@@ -65,20 +64,20 @@
     )
     b_runinfo = timed_run.timed_run(
         args.cmd_with_flags[:1] + args.b_args.split() + args.cmd_with_flags[1:],
         args.timeout,
         temp_prefix + "-b",
     )
     log = logging.getLogger(__name__)
-    time_str = "(1st Run: %.3f seconds) (2nd Run: %.3f seconds)" % (
-        a_runinfo.elapsedtime,
-        b_runinfo.elapsedtime,
+    time_str = (
+        f"(1st Run: {a_runinfo.elapsedtime:.3f} seconds)"
+        f" (2nd Run: {b_runinfo.elapsedtime:.3f} seconds)"
     )
 
-    if a_runinfo.sta != timed_run.TIMED_OUT and b_runinfo.sta != timed_run.TIMED_OUT:
+    if timed_run.TIMED_OUT not in (a_runinfo.sta, b_runinfo.sta):
         if a_runinfo.return_code != b_runinfo.return_code:
             log.info(
                 "[Interesting] Different return code (%d, %d). %s",
                 a_runinfo.return_code,
                 b_runinfo.return_code,
                 time_str,
             )
```

### Comparing `lithium-reducer-0.6.2/src/lithium/interestingness/hangs.py` & `lithium-reducer-1.0.0/src/lithium/interestingness/crashes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-# coding=utf-8
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-"""Lithium's "hangs" interestingness test to assess whether a binary hangs.
+"""Lithium's "crashes" interestingness test to assess whether a binary crashes.
 
 Example:
-    python -m lithium hangs --timeout=3 <binary> --fuzzing-safe <testcase>
+    python -m lithium crashes --timeout=9 <binary> --fuzzing-safe <testcase>
 """
 
 import logging
 from typing import List
 
 from . import timed_run
 
 
 def interesting(cli_args: List[str], temp_prefix: str) -> bool:
-    """Interesting if the binary causes a hang.
+    """Interesting if the binary causes a crash. (e.g. SIGKILL/SIGTERM/SIGTRAP etc.)
 
     Args:
         cli_args: List of input arguments.
         temp_prefix: Temporary directory prefix, e.g. tmp1/1 or tmp4/1
 
     Returns:
-        True if binary causes a hang, False otherwise.
+        True if binary crashes, False otherwise.
     """
     parser = timed_run.ArgumentParser(
-        prog="hangs",
+        prog="crashes",
         usage="python -m lithium %(prog)s [options] binary [flags] testcase.ext",
     )
     args = parser.parse_args(cli_args)
 
     log = logging.getLogger(__name__)
+    # Run the program with desired flags and look out for crashes.
     runinfo = timed_run.timed_run(args.cmd_with_flags, args.timeout, temp_prefix)
 
-    if runinfo.sta == timed_run.TIMED_OUT:
-        log.info("Timed out after %.3f seconds", args.timeout)
+    time_str = f" ({runinfo.elapsedtime:.3f} seconds)"
+    if runinfo.sta == timed_run.CRASHED:
+        log.info("Exit status: " + runinfo.msg + time_str)
         return True
 
-    log.info("Exited in %.3f seconds", runinfo.elapsedtime)
+    log.info("[Uninteresting] It didn't crash: " + runinfo.msg + time_str)
     return False
```

### Comparing `lithium-reducer-0.6.2/src/lithium/interestingness/outputs.py` & `lithium-reducer-1.0.0/src/lithium/interestingness/outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Lithium's "outputs" interestingness test to assess whether an intended message shows
 up.
```

### Comparing `lithium-reducer-0.6.2/src/lithium/interestingness/repeat.py` & `lithium-reducer-1.0.0/src/lithium/interestingness/repeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 """Repeats an interestingness test a given number of times. If "REPEATNUM" is present,
 it is replaced in turn with each number as it increments. This "REPEATNUM" can be
```

### Comparing `lithium-reducer-0.6.2/src/lithium/interestingness/timed_run.py` & `lithium-reducer-1.0.0/src/lithium/interestingness/timed_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Run a subprocess with timeout
 """
 
@@ -132,17 +131,17 @@
         )
     except subprocess.TimeoutExpired:
         child.kill()
         stdout, stderr = child.communicate()
         sta = TIMED_OUT
     except Exception as exc:  # pylint: disable=broad-except
         print("Tried to run:")
-        print("  %r" % cmd_with_args)
+        print(f"  {cmd_with_args!r}")
         print("but got this error:")
-        print("  %s" % exc)
+        print(f"  {exc}")
         sys.exit(2)
     finally:
         if isinstance(child_stderr, BinaryIO) and isinstance(child_stdout, BinaryIO):
             child_stdout.close()
             child_stderr.close()
     elapsed_time = time.time() - start_time
 
@@ -159,18 +158,15 @@
         # The program was terminated by a signal, which usually indicates a crash.
         # Mac/Linux only!
         # XXX: this doesn't work on Windows
         if child.returncode < 0:
             signum = -child.returncode
         else:
             signum = child.returncode
-        msg = "CRASHED signal %d (%s)" % (
-            signum,
-            get_signal_name(signum),
-        )
+        msg = f"CRASHED signal {signum} ({get_signal_name(signum)})"
         sta = CRASHED
 
     return RunData(
         sta,
         child.returncode if sta != TIMED_OUT else None,
         msg,
         elapsed_time,
```

### Comparing `lithium-reducer-0.6.2/src/lithium/interestingness/utils.py` & `lithium-reducer-1.0.0/src/lithium/interestingness/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 """This lets you import an interestingness test given a full path, or given just a
 filename. (assuming it's in the current directory OR in the same directory as utils.py)
@@ -38,15 +37,15 @@
             # rather than print the whole file, print the lines containing the
             # match, up to the surrounding '\n'
             prev_nl = max(file_contents.rfind(b"\n", 0, idx + 1), 0)
             next_nl = idx + len(regex)
             if not regex.endswith(b"\n"):
                 next_nl = max(file_contents.find(b"\n", idx + len(regex)), next_nl)
             match = file_contents[prev_nl:next_nl].decode("utf-8", errors="replace")
-            print("[Found string in: %r]" % (match,), end=" ")
+            print(f"[Found string in: {match!r}]", end=" ")
         return True
     return False
 
 
 def file_contains_regex(
     input_file: Union[Path, str], regex: bytes, verbose: bool = True
 ) -> Tuple[bool, bytes]:
```

### Comparing `lithium-reducer-0.6.2/src/lithium/reducer.py` & `lithium-reducer-1.0.0/src/lithium/reducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """lithium reducer"""
 
 import argparse
 import logging
@@ -24,15 +23,14 @@
 LOG = logging.getLogger(__name__)
 
 
 class Lithium:
     """Lithium reduction object."""
 
     def __init__(self) -> None:
-
         self.strategy: Optional[Strategy] = None
 
         self.condition_script: Optional[ModuleType] = None
         self.condition_args: Optional[List[str]] = None
 
         self.test_count = 0
         self.test_total = 0
@@ -128,18 +126,17 @@
         grp_atoms = grp_opt.add_mutually_exclusive_group()
 
         strategies: Dict[str, Type[Strategy]] = {}
         testcase_types: Dict[str, Type[Testcase]] = {}
         for entry_point in pkg_resources.iter_entry_points("lithium_strategies"):
             try:
                 strategy_cls = entry_point.load()
-                assert (
-                    strategy_cls.name == entry_point.name
-                ), "entry_point name mismatch, check setup.py and %s.name" % (
-                    strategy_cls.__name__,
+                assert strategy_cls.name == entry_point.name, (
+                    "entry_point name mismatch, check setup.py and "
+                    f"{strategy_cls.__name__}.name"
                 )
             except Exception as exc:  # pylint: disable=broad-except
                 LOG.warning("error loading strategy type %s: %s", entry_point.name, exc)
                 continue
             strategies[entry_point.name] = strategy_cls
         assert DEFAULT_STRATEGY in strategies
         for entry_point in pkg_resources.iter_entry_points("lithium_testcases"):
@@ -198,15 +195,15 @@
         )
         # this has already been parsed above, it's only here for the help message
         assert self.strategy is not None
         grp_opt.add_argument(
             "--strategy",
             default=self.strategy.name,
             choices=strategies.keys(),
-            help="reduction strategy to use. default: %s" % DEFAULT_STRATEGY,
+            help=f"reduction strategy to use. default: {DEFAULT_STRATEGY}",
         )
         self.strategy.add_args(parser)
         testcase_types[atom].add_arguments(parser)
         grp_ext = parser.add_argument_group(
             description="Condition, condition options and file-to-reduce"
         )
         grp_ext.add_argument(
@@ -250,26 +247,26 @@
             filename_stem: Basename for the testcase on disk.
             use_number: Prefix filename with the next number in sequence.
 
         Returns:
             Filename to use for the next testcase.
         """
         if use_number:
-            filename_stem = "%d-%s" % (self.temp_file_count, filename_stem)
+            filename_stem = f"{self.temp_file_count}-{filename_stem}"
             self.temp_file_count += 1
         assert self.testcase is not None
         assert self.testcase.extension is not None
         assert self.temp_dir is not None
         return self.temp_dir / (filename_stem + self.testcase.extension)
 
     def create_temp_dir(self) -> None:
         """Create and switch to the next available temporary working folder."""
         i = 1
         while True:
-            temp_dir = Path("tmp%d" % (i,))
+            temp_dir = Path(f"tmp{i}")
             # To avoid race conditions, we use try/except instead of exists/create
             # Hopefully we don't get any errors other than "File exists" :)
             try:
                 temp_dir.mkdir()
             except OSError:
                 i += 1
             else:
```

### Comparing `lithium-reducer-0.6.2/src/lithium/strategies.py` & `lithium-reducer-1.0.0/src/lithium/strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Lithium reduction strategy implementations"""
 
 import abc
 import argparse
@@ -307,15 +306,15 @@
 
 
 class CheckOnly(Strategy):
     """Only check whether the testcase reproduces."""
 
     name = "check-only"
 
-    # pylint: disable=arguments-differ
+    # pylint: disable=arguments-renamed
     @ReductionIterator.wrap  # type: ignore[arg-type]
     def reduce(  # type: ignore[override]
         self, iterator: ReductionIterator
     ) -> Iterator[Testcase]:
         # check doesn't reduce, only checks
         yield from iterator.try_testcase(iterator.testcase, "Check")
 
@@ -370,15 +369,15 @@
             result += divide_rounding_up(length, chunk_size)
             chunk_size = int(chunk_size / 2)
         return int(result)
 
     def add_args(self, parser: argparse.ArgumentParser) -> None:
         super().add_args(parser)
         grp_add = parser.add_argument_group(
-            description="Additional options for the %s strategy" % (self.name,)
+            description=f"Additional options for the {self.name} strategy"
         )
         grp_add.add_argument(
             "--min", type=int, default=1, help="must be a power of two. default: 1"
         )
         grp_add.add_argument(
             "--max",
             type=int,
@@ -428,20 +427,18 @@
         if args.max_run_time:
             self.stop_after_time = args.max_run_time
         if not is_power_of_two(self.minimize_min):
             parser.error("Min must be a power of two.")
         if not is_power_of_two(self.minimize_max):
             parser.error("Max must be a power of two.")
 
-    def _post_round_cb(  # pylint: disable=no-self-use
-        self, iterator: ReductionIterator
-    ) -> Iterator[Testcase]:
+    def _post_round_cb(self, iterator: ReductionIterator) -> Iterator[Testcase]:
         return cast(Iterator[Testcase], [])
 
-    # pylint: disable=arguments-differ
+    # pylint: disable=arguments-renamed
     @ReductionIterator.wrap  # type: ignore[arg-type]
     def reduce(  # type: ignore[override]
         self, iterator: ReductionIterator
     ) -> Iterator[Testcase]:
         chunk_size = min(
             self.minimize_max, largest_power_of_two_smaller_than(len(iterator.testcase))
         )
@@ -471,18 +468,15 @@
 
                 yield from self._post_round_cb(iterator)
 
                 # If the chunk_size is less than or equal to the min_chunk_size and...
                 if chunk_size <= min_chunk_size:
                     # Repeat mode is last or always and at least one chunk was removed
                     # during the last round, repeat
-                    if removed_chunks and (
-                        self.minimize_repeat == "always"
-                        or self.minimize_repeat == "last"
-                    ):
+                    if removed_chunks and self.minimize_repeat in {"always", "last"}:
                         LOG.info("Starting another round of chunk size %d", chunk_size)
                         chunk_end = len(iterator.testcase)
                     # Otherwise, end minimization
                     else:
                         LOG.info(
                             "Lithium result: succeeded, reduced to: %s",
                             quantity(len(iterator.testcase), iterator.testcase.atom),
@@ -509,18 +503,17 @@
 
                     LOG.info("")
                     LOG.info("Reducing chunk size to %d", chunk_size)
 
                 removed_chunks = False
 
             chunk_start = max(0, chunk_end - chunk_size)
-            status = "Removing chunk from %s to %s of %d" % (
-                chunk_start,
-                chunk_end,
-                len(iterator.testcase),
+            status = (
+                f"Removing chunk from {chunk_start} to {chunk_end}"
+                f" of {len(iterator.testcase)}"
             )
             test_to_try = iterator.testcase.copy()
             test_to_try.rmslice(chunk_start, chunk_end)
             for test in iterator.try_testcase(test_to_try, status):
                 yield test
                 if iterator.last_feedback:
                     removed_chunks = True
@@ -603,15 +596,15 @@
 
         if final_chunk_size == 1 and self.minimize_repeat != "never":
             LOG.info(
                 "  Removing any single %s from the final file makes it uninteresting!",
                 iterator.testcase.atom,
             )
 
-    def try_removing_chunks(  # pylint: disable=no-self-use
+    def try_removing_chunks(
         self,
         chunk_size: int,
         stop_after_time: Optional[int],
         iterator: ReductionIterator,
     ) -> Iterator[Testcase]:
         """Make a single run through the testcase, trying to remove chunks of size
         chunk_size.
@@ -648,19 +641,17 @@
 
                 chunk_bef_start = max(0, chunk_start - chunk_size)
                 chunk_bef_end = chunk_start
                 chunk_aft_start = min(len(iterator.testcase), chunk_start + chunk_size)
                 chunk_aft_end = min(
                     len(iterator.testcase), chunk_aft_start + chunk_size
                 )
-                description = "Removing chunk #%d & #%d of %d chunks of size %d" % (
-                    before_chunk_idx,
-                    after_chunk_idx,
-                    num_chunks,
-                    chunk_size,
+                description = (
+                    f"Removing chunk #{before_chunk_idx} & #{after_chunk_idx} of "
+                    f"{num_chunks} chunks of size {chunk_size}"
                 )
 
                 testcase_suggestion = iterator.testcase.copy()
                 testcase_suggestion.rmslice(chunk_aft_start, chunk_aft_end)
                 testcase_suggestion.rmslice(chunk_bef_start, chunk_bef_end)
                 for test in iterator.try_testcase(testcase_suggestion, description):
                     yield test
@@ -748,15 +739,15 @@
     def __init__(self) -> None:
         super().__init__()
         self.use_experimental_move = False
 
     def add_args(self, parser: argparse.ArgumentParser) -> None:
         super().add_args(parser)
         grp_add = parser.add_argument_group(
-            description="Additional options for the %s strategy" % (self.name,)
+            description=f"Additional options for the {self.name} strategy"
         )
         grp_add.add_argument(
             "--with-experimental-move",
             action="store_true",
             help="Moving chunks is still a bit experimental, and it can introduce "
             "reducing loops. Use at own risk!",
         )
@@ -809,18 +800,17 @@
         lhs_chunk_idx = 0
 
         try:
             while chunk_start < len(iterator.testcase):
                 if stop_after_time is not None and time.time() > stop_after_time:
                     return
 
-                description = "chunk #%d of %d chunks of size %d" % (
-                    lhs_chunk_idx,
-                    num_chunks,
-                    chunk_size,
+                description = (
+                    f"chunk #{lhs_chunk_idx} of {num_chunks} chunks of size "
+                    f"{chunk_size}"
                 )
 
                 assert (
                     summary.count("S", 0, lhs_chunk_idx) * chunk_size == chunk_start
                 ), (
                     "the chunk_start should correspond to the lhs_chunk_idx modulo the "
                     "removed chunks."
@@ -884,19 +874,17 @@
                     "S", lhs_chunk_idx, rhs_chunk_idx
                 )
                 chunk_rhs_start = min(len(iterator.testcase), chunk_rhs_start)
                 chunk_rhs_end = min(
                     len(iterator.testcase), chunk_rhs_start + chunk_size
                 )
 
-                description = "chunk #%d & #%d of %d chunks of size %d" % (
-                    lhs_chunk_idx,
-                    rhs_chunk_idx,
-                    num_chunks,
-                    chunk_size,
+                description = (
+                    f"chunk #{lhs_chunk_idx} & #{rhs_chunk_idx} of {num_chunks} chunks "
+                    f"of size {chunk_size}"
                 )
 
                 testcase_suggestion = iterator.testcase.copy()
                 testcase_suggestion.rmslice(chunk_rhs_start, chunk_rhs_end)
                 testcase_suggestion.rmslice(chunk_lhs_start, chunk_lhs_end)
                 worked = False
                 for test in iterator.try_testcase(
@@ -985,18 +973,17 @@
                     assert (
                         summary.count("S", 0, mid_chunk_idx) * chunk_size
                         == chunk_mid_start
                     ), (
                         "the chunk_mid_start should correspond to the mid_chunk_idx "
                         "modulo the removed chunks."
                     )
-                    description = "chunk #%d of %d chunks of size %d" % (
-                        mid_chunk_idx,
-                        num_chunks,
-                        chunk_size,
+                    description = (
+                        f"chunk #{mid_chunk_idx} of {num_chunks} chunks of size "
+                        f"{chunk_size}"
                     )
 
                     parts = _split_parts(
                         iterator.testcase.parts,
                         chunk_size,
                         chunk_lhs_start,
                         chunk_mid_start,
@@ -1268,15 +1255,15 @@
         final_chunk_size = max(self.minimize_min, 1)
 
         # Map words to the chunk indexes in which they are present.
         words = {}
         for chunk, line in enumerate(iterator.testcase.parts):
             if not iterator.testcase.reducible[chunk]:
                 continue
-            for match in re.finditer(br"(?<=[\w\d_])\.(\w+)", line):
+            for match in re.finditer(rb"(?<=[\w\d_])\.(\w+)", line):
                 word = match.group(1)
                 if word not in words:
                     words[word] = [chunk]
                 else:
                     words[word] += [chunk]
 
         # All patterns have been removed successfully.
@@ -1301,26 +1288,24 @@
             for chunk_idx, chunk_starts in chunk_indexes.items():
                 # Unless this is the final size, let's try to remove couple of
                 # prefixes, otherwise wait for the final size to remove each of them
                 # individually.
                 if len(chunk_starts) == 1 and final_chunk_size != chunk_size:
                     continue
 
-                description = "'%s' in chunk #%d of %d chunks of size %d" % (
-                    word.decode("utf-8", "replace"),
-                    chunk_idx,
-                    num_chunks,
-                    chunk_size,
+                description = (
+                    f"'{word.decode('utf-8', 'replace')}' in chunk #{chunk_idx} "
+                    f"of {num_chunks} chunks of size {chunk_size}"
                 )
 
                 maybe_removed = 0
                 new_tc = iterator.testcase.copy()
                 for chunk_start in chunk_starts:
                     subst = re.sub(
-                        br"[\w_.]+\." + word, word, new_tc.parts[chunk_start]
+                        rb"[\w_.]+\." + word, word, new_tc.parts[chunk_start]
                     )
                     maybe_removed += len(new_tc.parts[chunk_start]) - len(subst)
                     new_tc.parts = (
                         new_tc.parts[:chunk_start]
                         + [subst]
                         + new_tc.parts[(chunk_start + 1) :]
                     )
@@ -1393,17 +1378,15 @@
         while True:
             num_removed_arguments = 0
             for maybe_removed, testcase in self.try_arguments_as_globals(iterator):
                 yield testcase
                 if iterator.last_feedback:
                     num_removed_arguments += maybe_removed
 
-            if num_removed_arguments and (
-                self.minimize_repeat == "always" or self.minimize_repeat == "last"
-            ):
+            if num_removed_arguments and self.minimize_repeat in {"always", "last"}:
                 # Repeat with the same chunk size
                 pass
             else:
                 # Done
                 break
 
     @staticmethod
@@ -1418,21 +1401,22 @@
         num_moved_arguments = 0
         num_survived_arguments = 0
 
         # Map words to the chunk indexes in which they are present.
         functions: Dict[bytes, Dict[str, Any]] = {}
         anonymous_queue: List[Dict[str, Any]] = []
         anonymous_stack: List[Dict[str, Any]] = []
+        args: List[bytes]
         for chunk, line in enumerate(iterator.testcase.parts):
             if not iterator.testcase.reducible[chunk]:
                 continue
             # Match function definition with at least one argument.
             for match in re.finditer(
-                br"(?:function\s+(\w+)|(\w+)\s*=\s*function)\s*"
-                br"\((\s*\w+\s*(?:,\s*\w+\s*)*)\)",
+                rb"(?:function\s+(\w+)|(\w+)\s*=\s*function)\s*"
+                rb"\((\s*\w+\s*(?:,\s*\w+\s*)*)\)",
                 line,
             ):
                 fun = match.group(1)
                 if fun is None:
                     fun = match.group(2)
 
                 if match.group(3) == b"":
@@ -1450,26 +1434,26 @@
                 else:
                     functions[fun]["defs"] = args
                     functions[fun]["args_pattern"] = match.group(3)
                     functions[fun]["chunk"] = chunk
 
             # Match anonymous function definition, which are surrounded by parentheses.
             for match in re.finditer(
-                br"\(function\s*\w*\s*\(((?:\s*\w+\s*(?:,\s*\w+\s*)*)?)\)\s*{", line
+                rb"\(function\s*\w*\s*\(((?:\s*\w+\s*(?:,\s*\w+\s*)*)?)\)\s*{", line
             ):
                 if match.group(1) == b"":
                     args = []
                 else:
                     args = match.group(1).split(b",")
                 anonymous_stack += [
                     {"defs": args, "chunk": chunk, "use": None, "use_chunk": 0}
                 ]
 
             # Match calls of anonymous function.
-            for match in re.finditer(br"}\s*\)\s*\(((?:[^()]|\([^,()]*\))*)\)", line):
+            for match in re.finditer(rb"}\s*\)\s*\(((?:[^()]|\([^,()]*\))*)\)", line):
                 if not anonymous_stack:
                     continue
                 anon = anonymous_stack[-1]
                 anonymous_stack = anonymous_stack[:-1]
                 if match.group(1) == b"" and not anon["defs"]:
                     continue
                 if match.group(1) == b"":
@@ -1477,15 +1461,15 @@
                 else:
                     args = match.group(1).split(b",")
                 anon["use"] = args
                 anon["use_chunk"] = chunk
                 anonymous_queue += [anon]
 
             # match function calls. (and some definitions)
-            for match in re.finditer(br"((\w+)\s*\(((?:[^()]|\([^,()]*\))*)\))", line):
+            for match in re.finditer(rb"((\w+)\s*\(((?:[^()]|\([^,()]*\))*)\))", line):
                 pattern = match.group(1)
                 fun = match.group(2)
                 if match.group(3) == b"":
                     args = []
                 else:
                     args = match.group(3).split(b",")
                 if fun not in functions:
@@ -1566,16 +1550,15 @@
                 new_tc.reducible = (
                     new_tc.reducible[:chunk] + [True] + new_tc.reducible[(chunk + 1) :]
                 )
                 maybe_moved_arguments = len(values)
 
                 for test in iterator.try_testcase(
                     new_tc,
-                    "Removing %s at %s #%d"
-                    % (description, iterator.testcase.atom, chunk),
+                    f"Removing {description} at {iterator.testcase.atom} #{chunk}",
                 ):
                     yield maybe_moved_arguments, test
                     if iterator.last_feedback:
                         num_moved_arguments += maybe_moved_arguments
                         break
                 else:
                     num_survived_arguments += maybe_moved_arguments
@@ -1586,17 +1569,17 @@
             maybe_moved_arguments = 0
             new_tc = iterator.testcase.copy()
 
             arg_defs = anon["defs"]
             def_chunk = anon["chunk"]
             values = anon["use"]
             chunk = anon["use_chunk"]
-            description = "arguments of anonymous function at #%s %s" % (
-                iterator.testcase.atom,
-                def_chunk,
+            description = (
+                f"arguments of anonymous function at #{iterator.testcase.atom} "
+                f"{def_chunk}"
             )
             # Remove arguments of the function.
             subst = new_tc.parts[def_chunk].replace(b",".join(arg_defs), b"", 1)
             if new_tc.parts[def_chunk] == subst:
                 noop_changes += 1
             new_tc.parts = (
                 new_tc.parts[:def_chunk] + [subst] + new_tc.parts[(def_chunk + 1) :]
@@ -1672,15 +1655,15 @@
         """Collapse braces separated by whitespace
         Args:
             testcase (Testcase): Testcase to be reduced.
         Returns:
             True if callback was performed successfully, False otherwise.
         """
         raw = b"".join(iterator.testcase.parts)
-        modified = re.sub(br"{\s+}", b"{ }", raw)
+        modified = re.sub(rb"{\s+}", b"{ }", raw)
 
         # Don't update the testcase if no changes were applied
         if raw != modified:
             assert iterator.testcase.filename is not None
             with open(iterator.testcase.filename, "wb") as testf:
                 testf.write(iterator.testcase.before)
                 testf.write(modified)
```

### Comparing `lithium-reducer-0.6.2/src/lithium/testcases.py` & `lithium-reducer-1.0.0/src/lithium/testcases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Lithium Testcase definitions.
 
 A testcase is a file to be reduced, split in a certain way (eg. bytes, lines).
 """
@@ -28,15 +27,15 @@
     """description of the units this testcase splits into"""
 
     def __init__(self) -> None:
         self.before: bytes = b""
         self.after: bytes = b""
         self.parts: List[bytes] = []
         # bool array with same length as `parts`
-        # parts with a matchine `False` in `reducible` should
+        # parts with a matching `False` in `reducible` should
         # not be removed by the Strategy
         self.reducible: List[bool] = []
         self.filename: Optional[str] = None
         self.extension: Optional[str] = None
 
     def __len__(self) -> int:
         """Length of the testcase in terms of parts to be reduced.
@@ -112,14 +111,15 @@
 
         Args:
             path: Location on disk of testcase to read.
 
         Raises:
             LithiumError: DDBEGIN/DDEND token mismatch.
         """
+        # pylint: disable=unnecessary-dunder-call
         self.__init__()  # type: ignore[misc]
         self.filename = str(path)
         self.extension = os.path.splitext(self.filename)[1]
 
         with open(self.filename, "rb") as fileobj:
             text = fileobj.read().decode("utf-8", errors="surrogateescape")
 
@@ -134,16 +134,16 @@
             before.append(line)
             if line.find(b"DDBEGIN") != -1:
                 self.before = b"".join(before)
                 del before
                 break
             if line.find(b"DDEND") != -1:
                 raise LithiumError(
-                    "The testcase (%s) has a line containing 'DDEND' "
-                    "without a line containing 'DDBEGIN' before it." % (self.filename,)
+                    f"The testcase ({self.filename}) has a line containing 'DDEND' "
+                    "without a line containing 'DDBEGIN' before it."
                 )
         else:
             # no DDBEGIN/END, `before` contains the whole testcase
             self.split_parts(b"".join(before))
             return
 
         between = []
@@ -152,16 +152,16 @@
             if line.find(b"DDEND") != -1:
                 self.after = line + b"".join(lines)
                 break
 
             between.append(line)
         else:
             raise LithiumError(
-                "The testcase (%s) has a line containing 'DDBEGIN' "
-                "but no line containing 'DDEND'." % (self.filename,)
+                f"The testcase ({self.filename}) has a line containing 'DDBEGIN' but no"
+                "line containing 'DDEND'."
             )
         self.split_parts(b"".join(between))
 
     @staticmethod
     def add_arguments(parser: argparse.ArgumentParser) -> None:
         """Add any testcase specific arguments.
 
@@ -268,27 +268,27 @@
         chars: List[int] = []
 
         while True:
             last = 0
             while True:
                 if instr:
                     match = re.match(
-                        br"(\\u[0-9A-Fa-f]{4}|\\x[0-9A-Fa-f]{2}|"
-                        br"\\u\{[0-9A-Fa-f]+\}|\\.|.)",
+                        rb"(\\u[0-9A-Fa-f]{4}|\\x[0-9A-Fa-f]{2}|"
+                        rb"\\u\{[0-9A-Fa-f]+\}|\\.|.)",
                         data[last:],
                         re.DOTALL,
                     )
                     if not match:
                         break
                     chars.append(len(self.parts))
                     if match.group(0) == instr:
                         instr = None
                         chars.pop()
                 else:
-                    match = re.search(br"""['"]""", data[last:])
+                    match = re.search(rb"""['"]""", data[last:])
                     if not match:
                         break
                     instr = match.group(0)
                 self.parts.append(data[last : last + match.end(0)])
                 last += match.end(0)
 
             if last != len(data):
@@ -419,16 +419,16 @@
 
 class TestcaseAttrs(Testcase):
     """Testcase file split by anything that looks like an XML attribute."""
 
     atom = "attribute"
     args = ("-a", "--attrs")
     arg_help = "Delimit a file by XML attributes."
-    TAG_PATTERN = br"<\s*[A-Za-z][A-Za-z-]*"
-    ATTR_PATTERN = br"((\s+|^)[A-Za-z][A-Za-z0-9:-]*(=|>|\s)|\s*>)"
+    TAG_PATTERN = rb"<\s*[A-Za-z][A-Za-z-]*"
+    ATTR_PATTERN = rb"((\s+|^)[A-Za-z][A-Za-z0-9:-]*(=|>|\s)|\s*>)"
 
     def split_parts(self, data: bytes) -> None:
         in_tag = False
         while data:
             if in_tag:
                 # we're in what looks like an element definition `<tag ...`
                 # look for attributes, or the end `>`
@@ -476,15 +476,15 @@
                 if data[0:1] in {b"'", b'"'}:
                     # quote delimited string value, look for the end quote
                     attr_parts.append(data[0:1])
                     data = data[1:]
                     end_match = re.search(attr_parts[-1], data)
                     incl_end = True
                 else:
-                    end_match = re.search(br"(\s|>)", data)
+                    end_match = re.search(rb"(\s|>)", data)
                     incl_end = False
                 if end_match is None:
                     # EOF looking for end quote
                     data = b"".join(attr_parts) + data
                     LOG.debug("EOF looking for attr end quote")
                     in_tag = False
                     continue
```

### Comparing `lithium-reducer-0.6.2/src/lithium/util.py` & `lithium-reducer-1.0.0/src/lithium/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Miscellaneous lithium utility functions"""
 
 import logging
 
@@ -70,13 +69,13 @@
     Returns:
         object: A string-able object representing the amount with units,
                 pluralized if necessary.
     """
 
     class _:
         def __str__(self) -> str:
-            result = "%s %s" % (amount, unit)
+            result = f"{amount} {unit}"
             if amount != 1:
                 result += "s"
             return result
 
     return _()
```

### Comparing `lithium-reducer-0.6.2/src/lithium_reducer.egg-info/PKG-INFO` & `lithium-reducer-1.0.0/src/lithium_reducer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: lithium-reducer
-Version: 0.6.2
+Version: 1.0.0
 Summary: Lithium is an automated testcase reduction tool
 Home-page: https://github.com/MozillaSecurity/lithium
 Author: Jesse Ruderman
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: fuzz,fuzzing,reduce,reducer,reduction,security,test,testing
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Task Status](https://community-tc.services.mozilla.com/api/github/v1/repository/MozillaSecurity/lithium/master/badge.svg)](https://community-tc.services.mozilla.com/api/github/v1/repository/MozillaSecurity/lithium/master/latest)
 [![codecov](https://codecov.io/gh/MozillaSecurity/lithium/branch/master/graph/badge.svg)](https://codecov.io/gh/MozillaSecurity/lithium)
 [![Matrix](https://img.shields.io/badge/dynamic/json?color=green&label=chat&query=%24.chunk[%3F(%40.canonical_alias%3D%3D%22%23fuzzing%3Amozilla.org%22)].num_joined_members&suffix=%20users&url=https%3A%2F%2Fmozilla.modular.im%2F_matrix%2Fclient%2Fr0%2FpublicRooms&style=flat&logo=matrix)](https://riot.im/app/#/room/#fuzzing:mozilla.org)
@@ -90,9 +85,7 @@
 
 ### Credits
 
 - [Lithium's testcase reduction algorithm](src/lithium/docs/algorithm.md) is a modified version of the "ddmin" algorithm in Andreas Zeller's paper, [Simplifying and Isolating Failure-Inducing Input](https://www.st.cs.uni-saarland.de/papers/tse2002/).
 - The idea of using an external "interestingness test" program came from [Delta](http://delta.tigris.org/), a similar tool that's [used in clever ways by the GCC project](https://gcc.gnu.org/wiki/A_guide_to_testcase_reduction).
 - [timed_run](src/lithium/interestingness/timed_run.py), used by many of the "interestingness test" scripts that come with Lithium, is based on [timed_run.py](https://web.archive.org/web/20071107032840/http://bclary.com/log/2007/03/07/timed_run), which was written by [Chris Cooper](http://coop.deadsquid.com/) and [Bob Clary](https://bclary.com/).
 - The code was significantly cleaned up and modernized by Jesse Schwartzentruber and Gary Kwong in mid-2017.
-
-
```

### Comparing `lithium-reducer-0.6.2/src/lithium_reducer.egg-info/SOURCES.txt` & `lithium-reducer-1.0.0/src/lithium_reducer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lithium-reducer-0.6.2/src/lithium_reducer.egg-info/entry_points.txt` & `lithium-reducer-1.0.0/src/lithium_reducer.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
 
 [lithium_testcases]
 attributes = lithium.testcases:TestcaseAttrs
 char = lithium.testcases:TestcaseChar
 jsstr-char = lithium.testcases:TestcaseJsStr
 line = lithium.testcases:TestcaseLine
 symbol-delimiter = lithium.testcases:TestcaseSymbol
-
```

### Comparing `lithium-reducer-0.6.2/tests/conftest.py` & `lithium-reducer-1.0.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """lithium unittest fixtures"""
 
 import argparse
 import os
```

### Comparing `lithium-reducer-0.6.2/tests/test_interestingness.py` & `lithium-reducer-1.0.0/tests/test_interestingness.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Lithium interestingness-test tests"""
 
 import logging
 import platform
@@ -419,11 +418,11 @@
         [
             "outputs",
             pattern,
         ]
         + CAT_CMD
         + ["temp.js"]
     )
-    assert result == 0, "%r not found in %r" % (pattern, open("temp.js").read())
+    assert result == 0, f"{pattern!r} not found in {Path('temp.js').read_text()!r}"
     #    assert lith.test_count == 1
     captured = capsys.readouterr()
-    assert "[Found string in: %r]" % (expected,) in captured.out
+    assert f"[Found string in: {expected!r}]" in captured.out
```

### Comparing `lithium-reducer-0.6.2/tests/test_lithium.py` & `lithium-reducer-1.0.0/tests/test_lithium.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Lithium tests"""
 
 import logging
 import shutil
@@ -59,15 +58,15 @@
 def test_empty(caplog) -> None:
     """test lithium with empty input"""
     lith = lithium.Lithium()
     with open("empty.txt", "w"):
         pass
 
     class _Interesting:
-        # pylint: disable=missing-function-docstring,no-self-use
+        # pylint: disable=missing-function-docstring
         def init(self, *_):
             pass
 
         def interesting(self, *_):
             raise RuntimeError("Not expected to be run")
 
         def cleanup(self, *_):
```

### Comparing `lithium-reducer-0.6.2/tests/test_strategies.py` & `lithium-reducer-1.0.0/tests/test_strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Lithium Strategy tests"""
 
 from pathlib import Path
 
@@ -14,15 +13,15 @@
 
 
 def test_minimize(testcase_cls) -> None:
     """test that minimize strategy works"""
     test_path = Path("a.txt")
 
     class _Interesting:
-        # pylint: disable=missing-function-docstring,no-self-use
+        # pylint: disable=missing-function-docstring
         def init(self, condition_args):
             pass
 
         def interesting(self, *_):
             return b"o\n" in test_path.read_bytes()
 
         def cleanup(self, condition_args):
@@ -39,15 +38,15 @@
 
 
 def test_minimize_around(testcase_cls) -> None:
     """test that minimize around strategy works"""
     test_path = Path("a.txt")
 
     class _Interesting:
-        # pylint: disable=missing-function-docstring,no-self-use
+        # pylint: disable=missing-function-docstring
         def init(self, condition_args):
             pass
 
         def interesting(self, *_):
             data = test_path.read_bytes()
             return b"o\n" in data and len(set(data.split(b"o\n"))) == 1
 
@@ -65,15 +64,15 @@
 
 
 def test_minimize_balanced(testcase_cls) -> None:
     """test that minimize balanced strategy works"""
     test_path = Path("a.txt")
 
     class _Interesting:
-        # pylint: disable=missing-function-docstring,no-self-use
+        # pylint: disable=missing-function-docstring
         def init(self, condition_args):
             pass
 
         def interesting(self, *_):
             data = test_path.read_bytes()
             if b"o\n" in data:
                 head, tail = data.split(b"o\n")
@@ -138,15 +137,15 @@
         b"push = function(a) {\n  list.push(a);\n}\n"
         b"Foo.prototype.last = function() {\n  return list.pop();\n}\n",
         expected,
     }
     test_path = Path("a.txt")
 
     class _Interesting:
-        # pylint: disable=missing-function-docstring,no-self-use
+        # pylint: disable=missing-function-docstring
         def init(self, condition_args):
             pass
 
         def interesting(self, *_):
             return test_path.read_bytes() in valid_reductions
 
         def cleanup(self, condition_args):
@@ -179,15 +178,15 @@
         b"function foo(b) {\n  list = a + b;\n}\na = 2;\nfoo(3)\n",
         b"function foo() {\n  list = a + b;\n}\na = 2;\nb = 3;\nfoo(2,3)\n",
         expected,
     }
     test_path = Path("a.txt")
 
     class _Interesting:
-        # pylint: disable=missing-function-docstring,no-self-use
+        # pylint: disable=missing-function-docstring
         def init(self, condition_args) -> None:
             pass
 
         def interesting(self, *_):
             return test_path.read_bytes() in valid_reductions
 
         def cleanup(self, condition_args) -> None:
@@ -217,15 +216,15 @@
     ],
 )
 def test_minimize_collapse_braces(test_type, test_count, expected) -> None:
     """test that collapse-braces strategy eliminates empty braces"""
     test_path = Path("a.txt")
 
     class _Interesting:
-        # pylint: disable=missing-function-docstring,no-self-use
+        # pylint: disable=missing-function-docstring
         def init(self, condition_args) -> None:
             pass
 
         def interesting(self, condition_args, *_):
             data = test_path.read_bytes()
             if condition_args == "NEEDS_BRACE":
                 return data.count(b"{") == 1 and data.count(b"{") == data.count(b"}")
@@ -253,15 +252,15 @@
 
 
 def test_minimize_reducible() -> None:
     """test that minimize works around non-reducible parts in the testcase"""
     test_path = Path("a.txt")
 
     class _Interesting:
-        # pylint: disable=missing-function-docstring,no-self-use
+        # pylint: disable=missing-function-docstring
         def init(self, condition_args) -> None:
             pass
 
         def interesting(self, *_):
             return b"o\n" in test_path.read_bytes()
 
         def cleanup(self, condition_args) -> None:
```

### Comparing `lithium-reducer-0.6.2/tests/test_testcases.py` & `lithium-reducer-1.0.0/tests/test_testcases.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Lithium Testcase* tests"""
 
 from pathlib import Path
 from typing import List
@@ -305,15 +304,15 @@
 def test_errors(data: bytes, error: str) -> None:
     """Test DDBEGIN/END errors"""
     test = lithium.testcases.TestcaseLine()
     test_path = Path("a.txt")
     test_path.write_bytes(data)
     with pytest.raises(
         lithium.LithiumError,
-        match=r"^The testcase \(%s\) has a line containing %s" % (test_path, error),
+        match=rf"^The testcase \({test_path}\) has a line containing {error}",
     ):
         test.load(test_path)
 
 
 def test_reducible_slices() -> None:
     """Test reducible part slicing"""
     # pylint: disable=protected-access
```

### Comparing `lithium-reducer-0.6.2/tests/test_util.py` & `lithium-reducer-1.0.0/tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 """Lithium utility tests"""
 
 import logging
 import math
@@ -24,15 +23,15 @@
         inp: input
 
     Returns:
         result
     """
     assert (
         isinstance(inp, int) or inp.is_integer()
-    ), "ispow2() only works for integers, %r is not an integer" % (inp,)
+    ), f"ispow2() only works for integers, {inp!r} is not an integer"
     assert inp >= 1, "domain error"
     orig = inp
     result = True
     while inp > 1:
         if inp % 2:
             result = False
             break
@@ -43,15 +42,15 @@
         # diff to the next closest integer
         diff = abs(math_result - round(math_result))
         math_result = diff < 10 ** -(
             sys.float_info.dig - 1
         )  # float_info.dig is the # of decimal digits representable
         assert (
             result == math_result
-        ), "ispow2(n) did not match math.log(n)/math.log(2) for n = %d" % (orig,)
+        ), f"ispow2(n) did not match math.log(n)/math.log(2) for n = {orig}"
     return result
 
 
 def _divceil(num: int, den: int) -> int:
     """Simple version of `_divide_rounding_up` for testing and comparison
 
     Args:
@@ -65,15 +64,15 @@
     rem = num % den
     result = quo + (1 if rem else 0)
     # if the inputs are representable as a float, compare the result to math library
     if num <= sys.float_info.max and den <= sys.float_info.max:
         math_result = math.ceil(1.0 * num / den)
         assert (
             result == math_result
-        ), "divceil(n,d) did not match math.ceil(n/d) for n = %d, d = %d" % (num, den)
+        ), f"divceil(n,d) did not match math.ceil(n/d) for n = {num}, d = {den}"
     return result
 
 
 def test_divide_rounding_up() -> None:
     """test `divide_rounding_up`"""
     for _ in range(10000):
         num = random.randint(1, (1 << 64) - 1)
```

### Comparing `lithium-reducer-0.6.2/tox.ini` & `lithium-reducer-1.0.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py{36,37,38,39},lint
+envlist = py{38,39,310,311},lint
 skip_missing_interpreters = true
 tox_pip_extensions_ext_venv_update = true
 
 [testenv]
 commands = pytest -v --cache-clear --cov="{toxinidir}" --cov-config="{toxinidir}/pyproject.toml" --cov-report term-missing --basetemp="{envtmpdir}" {posargs} --disable-pytest-warnings
 deps =
     pytest
@@ -16,52 +16,57 @@
     TRAVIS
     TRAVIS_*
     TWINE_*
 usedevelop = true
 
 [testenv:codecov]
 commands =
-    codecov -X gcov
-deps =
     codecov
+deps =
     coverage[toml]
 skip_install = true
+allowlist_externals =
+    codecov
 
 [testenv:lint]
 commands =
     pre-commit run -a {posargs}
 deps =
     pre-commit
 skip_install = true
 
 [testenv:mypy]
 commands =
     mypy --install-types --non-interactive {posargs}
 deps =
-    mypy==v0.910
+    mypy==v1.3.0
 usedevelop = true
 
 [testenv:pylint]
 commands =
     pylint {posargs}
 deps =
-    pylint==2.8.3
+    pylint==2.17.4
 usedevelop = true
 
 [testenv:pypi]
 commands =
     python setup.py sdist bdist_wheel
     twine upload --skip-existing dist/*
 deps =
     setuptools>=43
     setuptools_scm[toml]>=3.4
     twine
     wheel
 skip_install = true
 
 [flake8]
-extend-ignore = E203
+# E203, W503, and W504 are all black compat
+ignore =
+    E203
+    W503
+enable =
+    W504
 per-file-ignores =
     */__init__.py: F401
 max-line-length = 88
 show-source = true
-statistics = true
```


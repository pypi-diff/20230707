# Comparing `tmp/path-16.6.0.tar.gz` & `tmp/path-16.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "path-16.6.0.tar", last modified: Wed Nov 30 22:47:17 2022, max compression
+gzip compressed data, was "path-16.7.0.tar", last modified: Thu Jul  6 23:27:51 2023, max compression
```

## Comparing `path-16.6.0.tar` & `path-16.7.0.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 22:47:17.048983 path-16.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2022-11-30 22:46:48.000000 path-16.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-30 22:46:48.000000 path-16.6.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      246 2022-11-30 22:46:48.000000 path-16.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-11-30 22:46:48.000000 path-16.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 22:47:17.044983 path-16.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)       20 2022-11-30 22:46:48.000000 path-16.6.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (122)      148 2022-11-30 22:46:48.000000 path-16.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 22:47:17.044983 path-16.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2739 2022-11-30 22:46:48.000000 path-16.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2022-11-30 22:46:48.000000 path-16.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-30 22:46:48.000000 path-16.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      233 2022-11-30 22:46:48.000000 path-16.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    14857 2022-11-30 22:46:48.000000 path-16.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)      167 2022-11-30 22:46:48.000000 path-16.6.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2022-11-30 22:46:48.000000 path-16.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       14 2022-11-30 22:46:48.000000 path-16.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6330 2022-11-30 22:47:17.048983 path-16.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5607 2022-11-30 22:46:48.000000 path-16.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 22:47:17.044983 path-16.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     6765 2022-11-30 22:46:48.000000 path-16.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      233 2022-11-30 22:46:48.000000 path-16.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2022-11-30 22:46:48.000000 path-16.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-30 22:46:48.000000 path-16.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (122)      389 2022-11-30 22:46:48.000000 path-16.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      154 2022-11-30 22:46:48.000000 path-16.6.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 22:47:17.044983 path-16.6.0/path/
--rw-r--r--   0 runner    (1001) docker     (122)    50317 2022-11-30 22:46:48.000000 path-16.6.0/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15317 2022-11-30 22:46:48.000000 path-16.6.0/path/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      663 2022-11-30 22:46:48.000000 path-16.6.0/path/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2022-11-30 22:46:48.000000 path-16.6.0/path/classes.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2221 2022-11-30 22:46:48.000000 path-16.6.0/path/masks.py
--rw-r--r--   0 runner    (1001) docker     (122)      205 2022-11-30 22:46:48.000000 path-16.6.0/path/masks.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1378 2022-11-30 22:46:48.000000 path-16.6.0/path/matchers.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2022-11-30 22:46:48.000000 path-16.6.0/path/matchers.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 22:46:48.000000 path-16.6.0/path/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     4760 2022-11-30 22:46:48.000000 path-16.6.0/path/py37compat.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2022-11-30 22:46:48.000000 path-16.6.0/path/py37compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 22:47:17.048983 path-16.6.0/path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6330 2022-11-30 22:47:17.000000 path-16.6.0/path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      686 2022-11-30 22:47:17.000000 path-16.6.0/path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 22:47:17.000000 path-16.6.0/path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      408 2022-11-30 22:47:17.000000 path-16.6.0/path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-30 22:47:17.000000 path-16.6.0/path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      378 2022-11-30 22:46:48.000000 path-16.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      910 2022-11-30 22:46:48.000000 path-16.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2022-11-30 22:47:17.048983 path-16.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    44622 2022-11-30 22:46:48.000000 path-16.6.0/test_path.py
--rw-r--r--   0 runner    (1001) docker     (122)      732 2022-11-30 22:46:48.000000 path-16.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:27:51.347170 path-16.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-06 23:27:30.000000 path-16.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 23:27:30.000000 path-16.7.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 23:27:30.000000 path-16.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:27:51.343170 path-16.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 23:27:30.000000 path-16.7.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-06 23:27:30.000000 path-16.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:27:51.343170 path-16.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-06 23:27:30.000000 path-16.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 23:27:30.000000 path-16.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 23:27:30.000000 path-16.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 23:27:30.000000 path-16.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-06 23:27:30.000000 path-16.7.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-06 23:27:30.000000 path-16.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 23:27:30.000000 path-16.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-07-06 23:27:30.000000 path-16.7.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-06 23:27:51.347170 path-16.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-06 23:27:30.000000 path-16.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:27:51.343170 path-16.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-06 23:27:30.000000 path-16.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 23:27:30.000000 path-16.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-06 23:27:30.000000 path-16.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 23:27:30.000000 path-16.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 23:27:30.000000 path-16.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 23:27:30.000000 path-16.7.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:27:51.347170 path-16.7.0/path/
+-rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-07-06 23:27:30.000000 path-16.7.0/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-07-06 23:27:30.000000 path-16.7.0/path/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 23:27:30.000000 path-16.7.0/path/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 23:27:30.000000 path-16.7.0/path/classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-06 23:27:30.000000 path-16.7.0/path/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-06 23:27:30.000000 path-16.7.0/path/masks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-06 23:27:30.000000 path-16.7.0/path/matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 23:27:30.000000 path-16.7.0/path/matchers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:27:30.000000 path-16.7.0/path/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:27:51.347170 path-16.7.0/path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-06 23:27:51.000000 path-16.7.0/path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-06 23:27:51.000000 path-16.7.0/path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:27:51.000000 path-16.7.0/path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-06 23:27:51.000000 path-16.7.0/path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 23:27:51.000000 path-16.7.0/path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 23:27:30.000000 path-16.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-06 23:27:30.000000 path-16.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-06 23:27:51.347170 path-16.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    44531 2023-07-06 23:27:30.000000 path-16.7.0/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 23:27:30.000000 path-16.7.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 23:27:30.000000 path-16.7.0/tox.ini
```

### Comparing `path-16.6.0/.github/workflows/main.yml` & `path-16.7.0/.github/workflows/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient.
-  FORCE_COLOR: -106
+  # to a non-empty value is sufficient. For tox, it must be one of
+  # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
+  # in common is "1".
+  FORCE_COLOR: 1
   # MyPy's color enforcement (must be a non-zero number)
   MYPY_FORCE_COLOR: -42
   # Recognized by the `py` package, dependency of `pytest` (must be "1")
   PY_COLORS: 1
   # Make tox-wrapped tools see color requests
   TOX_TESTENV_PASSENV: >-
     FORCE_COLOR
@@ -33,73 +38,87 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
+    continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
+      - name: Install tox
+        run: |
+          python -m pip install tox
+      - name: Run
+        run: tox
+
+  docs:
+    runs-on: ubuntu-latest
+    env:
+      TOXENV: docs
+    steps:
+      - uses: actions/checkout@v3
+      - name: Setup Python
+        uses: actions/setup-python@v4
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
+    - docs
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Release
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `path-16.6.0/CHANGES.rst` & `path-16.7.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v16.7.0
+=======
+
+Features
+--------
+
+- Added ``.permissions`` attribute. (#211)
+- Require Python 3.8 or later.
+
+
 v16.6.0
 -------
 
 - ``.mtime`` and ``.atime`` are now settable.
 
 v16.5.0
 -------
```

### Comparing `path-16.6.0/LICENSE` & `path-16.7.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `path-16.6.0/PKG-INFO` & `path-16.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 Metadata-Version: 2.1
 Name: path
-Version: 16.6.0
+Version: 16.7.0
 Summary: A module wrapper for os.path
 Home-page: https://github.com/jaraco/path
 Author: Jason Orendorff
 Author-email: jason.orendorff@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/path.svg
    :target: https://pypi.org/project/path
 
 .. image:: https://img.shields.io/pypi/pyversions/path.svg
 
 .. image:: https://github.com/jaraco/path/workflows/tests/badge.svg
    :target: https://github.com/jaraco/path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/path/badge/?version=latest
    :target: https://path.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/path
    :target: https://tidelift.com/subscription/pkg/pypi-path?utm_source=pypi-path&utm_medium=readme
 
 
 ``path`` (aka path pie, formerly ``path.py``) implements path
```

### Comparing `path-16.6.0/README.rst` & `path-16.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/path.svg
 
 .. image:: https://github.com/jaraco/path/workflows/tests/badge.svg
    :target: https://github.com/jaraco/path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/path/badge/?version=latest
    :target: https://path.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/path
    :target: https://tidelift.com/subscription/pkg/pypi-path?utm_source=pypi-path&utm_medium=readme
 
 
 ``path`` (aka path pie, formerly ``path.py``) implements path
```

### Comparing `path-16.6.0/docs/Makefile` & `path-16.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `path-16.6.0/docs/conf.py` & `path-16.7.0/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
 extensions = [
     'sphinx.ext.autodoc',
     'jaraco.packaging.sphinx',
 ]
 
 master_doc = "index"
 html_theme = "furo"
 
 pygments_style = "sphinx"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `path-16.6.0/path/__init__.py` & `path-16.7.0/path/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import shutil
 import hashlib
 import errno
 import tempfile
 import functools
 import re
 import contextlib
-import io
 import importlib
 import itertools
 import datetime
 from numbers import Number
 from typing import Union
 
 with contextlib.suppress(ImportError):
@@ -49,15 +48,14 @@
 
 with contextlib.suppress(ImportError):
     import grp
 
 from . import matchers
 from . import masks
 from . import classes
-from .py37compat import best_realpath, lru_cache
 
 
 __all__ = ['Path', 'TempDir']
 
 
 LINESEPS = ['\r\n', '\r', '\n']
 U_LINESEPS = LINESEPS + ['\u0085', '\u2028', '\u2029']
@@ -147,15 +145,15 @@
     def __init__(self, other=''):
         if other is None:
             raise TypeError("Invalid initial value for path: None")
         with contextlib.suppress(AttributeError):
             self._validate()
 
     @classmethod
-    @lru_cache
+    @functools.lru_cache
     def using_module(cls, module):
         subclass_name = cls.__name__ + '_' + module.__name__
         bases = (cls,)
         ns = {'module': module}
         return type(subclass_name, bases, ns)
 
     @classes.ClassProperty
@@ -165,19 +163,19 @@
         What class should be used to construct new instances from this class
         """
         return cls
 
     # --- Special Python methods.
 
     def __repr__(self):
-        return '%s(%s)' % (type(self).__name__, super(Path, self).__repr__())
+        return '{}({})'.format(type(self).__name__, super().__repr__())
 
     # Adding a Path and a string yields a Path.
     def __add__(self, more):
-        return self._next_class(super(Path, self).__add__(more))
+        return self._next_class(super().__add__(more))
 
     def __radd__(self, other):
         return self._next_class(other.__add__(self))
 
     # The / operator joins Paths.
     def __div__(self, rel):
         """fp.__div__(rel) == fp / rel == fp.joinpath(rel)
@@ -235,16 +233,15 @@
 
     def normpath(self):
         """.. seealso:: :func:`os.path.normpath`"""
         return self._next_class(self.module.normpath(self))
 
     def realpath(self):
         """.. seealso:: :func:`os.path.realpath`"""
-        realpath = best_realpath(self.module)
-        return self._next_class(realpath(self))
+        return self._next_class(self.module.realpath(self))
 
     def expanduser(self):
         """.. seealso:: :func:`os.path.expanduser`"""
         return self._next_class(self.module.expanduser(self))
 
     def expandvars(self):
         """.. seealso:: :func:`os.path.expandvars`"""
@@ -294,15 +291,15 @@
 
         >>> Path('filename.ext').with_suffix('zip')
         Traceback (most recent call last):
         ...
         ValueError: Invalid suffix 'zip'
         """
         if not suffix.startswith('.'):
-            raise ValueError("Invalid suffix {suffix!r}".format(**locals()))
+            raise ValueError(f"Invalid suffix {suffix!r}")
 
         return self.stripext() + suffix
 
     @property
     def drive(self):
         """The drive specifier, for example ``'C:'``.
 
@@ -547,16 +544,15 @@
             try:
                 do_traverse = traverse()
             except Exception as exc:
                 errors(f"Unable to access '{child}': {exc}")
                 continue
 
             if do_traverse:
-                for item in child.walk(errors=errors, match=match):
-                    yield item
+                yield from child.walk(errors=errors, match=match)
 
     def walkdirs(self, *args, **kwargs):
         """Iterator over subdirs, recursively."""
         return (item for item in self.walk(*args, **kwargs) if item.isdir())
 
     def walkfiles(self, *args, **kwargs):
         """Iterator over files, recursively."""
@@ -621,15 +617,15 @@
 
     def open(self, *args, **kwargs):
         """Open this file and return a corresponding file object.
 
         Keyword arguments work as in :func:`io.open`.  If the file cannot be
         opened, an :class:`OSError` is raised.
         """
-        return io.open(self, *args, **kwargs)
+        return open(self, *args, **kwargs)
 
     def bytes(self):
         """Open this file, read all bytes, return them as a string."""
         with self.open('rb') as f:
             return f.read()
 
     def chunks(self, size, *args, **kwargs):
@@ -637,22 +633,21 @@
          be read piece by piece with a simple for loop.
 
         Any argument you pass after `size` will be passed to :meth:`open`.
 
         :example:
 
             >>> hash = hashlib.md5()
-            >>> for chunk in Path("CHANGES.rst").chunks(8192, mode='rb'):
+            >>> for chunk in Path("NEWS.rst").chunks(8192, mode='rb'):
             ...     hash.update(chunk)
 
          This will read the file by chunks of 8192 bytes.
         """
         with self.open(*args, **kwargs) as f:
-            for chunk in iter(lambda: f.read(size) or None, None):
-                yield chunk
+            yield from iter(lambda: f.read(size) or None, None)
 
     def write_bytes(self, bytes, append=False):
         """Open this file and write the given bytes to it.
 
         Default behavior is to overwrite any existing file.
         Call ``p.write_bytes(bytes, append=True)`` to append instead.
         """
@@ -991,14 +986,29 @@
         None,
         """ Size of the file, in bytes.
 
         .. seealso:: :meth:`getsize`, :func:`os.path.getsize`
         """,
     )
 
+    @property
+    def permissions(self) -> masks.Permissions:
+        """
+        Permissions.
+
+        >>> perms = Path('.').permissions
+        >>> isinstance(perms, int)
+        True
+        >>> set(perms.symbolic) <= set('rwx-')
+        True
+        >>> perms.symbolic
+        'r...'
+        """
+        return masks.Permissions(self.stat().st_mode)
+
     def access(self, *args, **kwargs):
         """
         Return does the real user have access to this path.
 
         >>> Path('.').access(os.F_OK)
         True
 
@@ -1101,14 +1111,20 @@
         return self
 
     def chmod(self, mode):
         """
         Set the mode. May be the new mode (os.chmod behavior) or a `symbolic
         mode <http://en.wikipedia.org/wiki/Chmod#Symbolic_modes>`_.
 
+        >>> a_file = Path(getfixture('tmp_path')).joinpath('afile.txt').touch()
+        >>> a_file.chmod(0o700)
+        Path(...
+        >>> a_file.chmod('u+x')
+        Path(...
+
         .. seealso:: :func:`os.chmod`
         """
         if isinstance(mode, str):
             mask = masks.compound(mode)
             mode = mask(self.stat().st_mode)
         os.chmod(self, mode)
         return self
@@ -1394,15 +1410,15 @@
             raise ValueError('Only read-only file modes can be used')
 
         # move existing file to backup, create new file with same permissions
         # borrowed extensively from the fileinput module
         backup_fn = self + (backup_extension or os.extsep + 'bak')
         backup_fn.remove_p()
         self.rename(backup_fn)
-        readable = io.open(
+        readable = open(
             backup_fn,
             mode,
             buffering=buffering,
             encoding=encoding,
             errors=errors,
             newline=newline,
         )
@@ -1416,15 +1432,15 @@
                 errors=errors,
                 newline=newline,
             )
         else:
             os_mode = os.O_CREAT | os.O_WRONLY | os.O_TRUNC
             os_mode |= getattr(os, 'O_BINARY', 0)
             fd = os.open(self, os_mode, perm)
-            writable = io.open(
+            writable = open(
                 fd,
                 "w" + mode.replace('r', ''),
                 buffering=buffering,
                 encoding=encoding,
                 errors=errors,
                 newline=newline,
             )
@@ -1548,15 +1564,15 @@
         return self.ResolverScope(self, scope)
 
     def get_dir(self, scope, class_):
         """
         Return the callable function from appdirs, but with the
         result wrapped in self.path_class
         """
-        prop_name = '{scope}_{class_}_dir'.format(**locals())
+        prop_name = f'{scope}_{class_}_dir'
         value = getattr(self.wrapper, prop_name)
         MultiPath = Multi.for_class(self.path_class)
         return MultiPath.detect(value)
 
 
 class Multi:
     """
@@ -1609,15 +1625,15 @@
     @classes.ClassProperty
     @classmethod
     def _next_class(cls):
         return Path
 
     def __new__(cls, *args, **kwargs):
         dirname = tempfile.mkdtemp(*args, **kwargs)
-        return super(TempDir, cls).__new__(cls, dirname)
+        return super().__new__(cls, dirname)
 
     def __init__(self, *args, **kwargs):
         pass
 
     def __enter__(self):
         # TempDir should return a Path version of itself and not itself
         # so that a second context manager does not create a second
```

### Comparing `path-16.6.0/path/__init__.pyi` & `path-16.7.0/path/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import builtins
 import contextlib
 import os
-import shutil
 import sys
 from io import (
     BufferedRandom,
     BufferedReader,
     BufferedWriter,
     FileIO,
     TextIOWrapper,
```

### Comparing `path-16.6.0/path/classes.py` & `path-16.7.0/path/classes.py`

 * *Files identical despite different names*

### Comparing `path-16.6.0/path/matchers.py` & `path-16.7.0/path/matchers.py`

 * *Files identical despite different names*

### Comparing `path-16.6.0/path/matchers.pyi` & `path-16.7.0/path/matchers.pyi`

 * *Files identical despite different names*

### Comparing `path-16.6.0/path.egg-info/PKG-INFO` & `path-16.7.0/path.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 Metadata-Version: 2.1
 Name: path
-Version: 16.6.0
+Version: 16.7.0
 Summary: A module wrapper for os.path
 Home-page: https://github.com/jaraco/path
 Author: Jason Orendorff
 Author-email: jason.orendorff@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/path.svg
    :target: https://pypi.org/project/path
 
 .. image:: https://img.shields.io/pypi/pyversions/path.svg
 
 .. image:: https://github.com/jaraco/path/workflows/tests/badge.svg
    :target: https://github.com/jaraco/path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/path/badge/?version=latest
    :target: https://path.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/path
    :target: https://tidelift.com/subscription/pkg/pypi-path?utm_source=pypi-path&utm_medium=readme
 
 
 ``path`` (aka path pie, formerly ``path.py``) implements path
```

### Comparing `path-16.6.0/setup.cfg` & `path-16.7.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -15,48 +15,48 @@
 	Programming Language :: Python :: 3 :: Only
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
+	pytest-ruff
 	
 	appdirs
 	packaging
 	pywin32; platform_system == "Windows" and python_version < "3.12"
 	
 	pygments
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
+	sphinx-lint
+	
 	jaraco.tidelift >= 1.4
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `path-16.6.0/test_path.py` & `path-16.7.0/test_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 in the issue tracker.
 
 TestScratchDir.test_touch() takes a while to run. It sleeps a few
 seconds to allow some time to pass between calls to check the modify
 time on files.
 """
 
-import io
 import os
 import sys
 import shutil
 import time
 import types
 import ntpath
 import posixpath
@@ -90,15 +89,15 @@
         """
         assert Path(1) == '1'
 
     def test_string_compatibility(self):
         """Test compatibility with ordinary strings."""
         x = Path('xyzzy')
         assert x == 'xyzzy'
-        assert x == str('xyzzy')
+        assert x == 'xyzzy'
 
         # sorting
         items = [Path('fhj'), Path('fgh'), 'E', Path('d'), 'A', Path('B'), 'c']
         items.sort()
         assert items == ['A', 'B', 'E', 'c', 'd', 'fgh', 'fhj']
 
         # Test p1/p1.
@@ -312,15 +311,15 @@
 
 class TestPerformance:
     @staticmethod
     def get_command_time(cmd):
         args = [sys.executable, '-m', 'timeit', '-n', '1', '-r', '1', '-u', 'usec'] + [
             cmd
         ]
-        res = subprocess.check_output(args, universal_newlines=True)
+        res = subprocess.check_output(args, text=True)
         dur = re.search(r'(\d+) usec per loop', res).group(1)
         return datetime.timedelta(microseconds=int(dur))
 
     def test_import_time(self, monkeypatch):
         """
         Import should take less than some limit.
 
@@ -470,15 +469,15 @@
         assert t0 <= f.mtime <= t1
         if hasattr(os.path, 'getctime'):
             ct = f.ctime
             assert t0 <= ct <= t1
 
         time.sleep(threshold * 2)
         fobj = open(f, 'ab')
-        fobj.write('some bytes'.encode('utf-8'))
+        fobj.write(b'some bytes')
         fobj.close()
 
         time.sleep(threshold * 2)
         t2 = time.time() - threshold
         f.touch()
         t3 = time.time() + threshold
 
@@ -546,15 +545,15 @@
         finally:
             for f in files:
                 with contextlib.suppress(Exception):
                     f.remove()
 
     @pytest.fixture
     def bytes_filename(self, tmpdir):
-        name = r'r\xe9\xf1emi'.encode('latin-1')
+        name = br'r\xe9\xf1emi'
         base = str(tmpdir).encode('ascii')
         try:
             with open(os.path.join(base, name), 'wb'):
                 pass
         except Exception as exc:
             raise pytest.skip(f"Invalid encodings disallowed {exc}")
         return name
@@ -735,15 +734,15 @@
             '\n',
             'hanging',
         ]
         clean = ''.join(expectedLines)
         stripped = [line.replace('\n', '') for line in expectedLines]
 
         # write bytes manually to file
-        with io.open(p, 'wb') as strm:
+        with open(p, 'wb') as strm:
             strm.write(given.encode(encoding))
 
         # test all 3 path read-fully functions, including
         # path.lines() in unicode mode.
         assert p.bytes() == given.encode(encoding)
         with pytest.deprecated_call():
             assert p.text(encoding) == clean
@@ -909,26 +908,28 @@
         target = Path(self.subdir_b / self.test_link.name)
         check = target.islink if hasattr(os, 'symlink') else target.isfile
         assert check()
 
     def test_with_nonexisting_dst_kwargs(self):
         self.subdir_a.merge_tree(self.subdir_b, symlinks=True)
         assert self.subdir_b.isdir()
-        expected = set(
-            (self.subdir_b / self.test_file.name, self.subdir_b / self.test_link.name)
-        )
+        expected = {
+            self.subdir_b / self.test_file.name,
+            self.subdir_b / self.test_link.name,
+        }
         assert set(self.subdir_b.listdir()) == expected
         self.check_link()
 
     def test_with_nonexisting_dst_args(self):
         self.subdir_a.merge_tree(self.subdir_b, True)
         assert self.subdir_b.isdir()
-        expected = set(
-            (self.subdir_b / self.test_file.name, self.subdir_b / self.test_link.name)
-        )
+        expected = {
+            self.subdir_b / self.test_file.name,
+            self.subdir_b / self.test_link.name,
+        }
         assert set(self.subdir_b.listdir()) == expected
         self.check_link()
 
     def test_with_existing_dst(self):
         self.subdir_b.rmtree()
         self.subdir_a.copytree(self.subdir_b, True)
 
@@ -937,21 +938,19 @@
         test_new.touch()
         with open(self.test_file, 'w') as f:
             f.write('x' * 5000)
 
         self.subdir_a.merge_tree(self.subdir_b, True)
 
         assert self.subdir_b.isdir()
-        expected = set(
-            (
-                self.subdir_b / self.test_file.name,
-                self.subdir_b / self.test_link.name,
-                self.subdir_b / test_new.name,
-            )
-        )
+        expected = {
+            self.subdir_b / self.test_file.name,
+            self.subdir_b / self.test_link.name,
+            self.subdir_b / test_new.name,
+        }
         assert set(self.subdir_b.listdir()) == expected
         self.check_link()
         assert len(Path(self.subdir_b / self.test_file.name).bytes()) == 5000
 
     def test_copytree_parameters(self):
         """
         merge_tree should accept parameters to copytree, such as 'ignore'
```


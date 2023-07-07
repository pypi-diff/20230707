# Comparing `tmp/read_acq-0.5.0.tar.gz` & `tmp/read_acq-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_acq-0.5.0.tar", last modified: Thu Jun 23 16:57:48 2022, max compression
+gzip compressed data, was "read_acq-0.5.2.tar", last modified: Fri Jul  7 21:48:43 2023, max compression
```

## Comparing `read_acq-0.5.0.tar` & `read_acq-0.5.2.tar`

### file list

```diff
@@ -1,52 +1,48 @@
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.807848 read_acq-0.5.0/
--rw-r--r--   0 smurray   (1096) loco      (1002)    53248 2022-04-07 23:17:13.000000 read_acq-0.5.0/.coverage
--rw-r--r--   0 smurray   (1096) loco      (1002)      607 2022-06-23 16:50:39.000000 read_acq-0.5.0/.coveragerc
--rw-r--r--   0 smurray   (1096) loco      (1002)      702 2021-07-12 16:35:27.000000 read_acq-0.5.0/.flake8
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.623843 read_acq-0.5.0/.github/
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.687845 read_acq-0.5.0/.github/workflows/
--rw-r--r--   0 smurray   (1096) loco      (1002)     1834 2022-06-23 16:56:58.000000 read_acq-0.5.0/.github/workflows/deploy.yaml
--rw-r--r--   0 smurray   (1096) loco      (1002)     2542 2022-06-23 16:50:39.000000 read_acq-0.5.0/.github/workflows/test_suite.yaml
--rw-r--r--   0 smurray   (1096) loco      (1002)       88 2021-07-12 16:35:27.000000 read_acq-0.5.0/.gitignore
--rw-r--r--   0 smurray   (1096) loco      (1002)      229 2022-02-02 00:36:07.000000 read_acq-0.5.0/.isort.cfg
--rw-r--r--   0 smurray   (1096) loco      (1002)     1612 2022-06-23 15:51:27.000000 read_acq-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 smurray   (1096) loco      (1002)     1260 2022-04-07 23:17:10.000000 read_acq-0.5.0/CHANGELOG.md
--rw-r--r--   0 smurray   (1096) loco      (1002)     1053 2022-04-07 23:17:10.000000 read_acq-0.5.0/LICENSE.rst
--rw-r--r--   0 smurray   (1096) loco      (1002)       30 2021-06-03 19:36:39.000000 read_acq-0.5.0/MANIFEST.in
--rw-r--r--   0 smurray   (1096) loco      (1002)     2920 2022-06-23 16:57:48.807848 read_acq-0.5.0/PKG-INFO
--rw-r--r--   0 smurray   (1096) loco      (1002)     1912 2021-07-12 16:35:28.000000 read_acq-0.5.0/README.rst
--rw-r--r--   0 smurray   (1096) loco      (1002)      155 2022-06-23 16:50:39.000000 read_acq-0.5.0/pyproject.toml
--rw-r--r--   0 smurray   (1096) loco      (1002)     1560 2022-06-23 16:57:48.811848 read_acq-0.5.0/setup.cfg
--rw-r--r--   0 smurray   (1096) loco      (1002)      396 2022-06-23 16:56:58.000000 read_acq-0.5.0/setup.py
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.627843 read_acq-0.5.0/src/
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.715845 read_acq-0.5.0/src/read_acq/
--rw-r--r--   0 smurray   (1096) loco      (1002)      461 2021-07-12 16:35:28.000000 read_acq-0.5.0/src/read_acq/__init__.py
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.747846 read_acq-0.5.0/src/read_acq/__pycache__/
--rw-r--r--   0 smurray   (1096) loco      (1002)      609 2022-04-20 05:47:51.000000 read_acq-0.5.0/src/read_acq/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 smurray   (1096) loco      (1002)      611 2021-07-19 20:05:59.000000 read_acq-0.5.0/src/read_acq/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 smurray   (1096) loco      (1002)     2850 2022-04-20 05:47:51.000000 read_acq-0.5.0/src/read_acq/__pycache__/codec.cpython-37.pyc
--rw-r--r--   0 smurray   (1096) loco      (1002)     2874 2022-02-02 00:38:00.000000 read_acq-0.5.0/src/read_acq/__pycache__/codec.cpython-39.pyc
--rw-r--r--   0 smurray   (1096) loco      (1002)    10864 2022-04-20 05:47:51.000000 read_acq-0.5.0/src/read_acq/__pycache__/read_acq.cpython-37.pyc
--rw-r--r--   0 smurray   (1096) loco      (1002)    11133 2022-04-07 23:25:13.000000 read_acq-0.5.0/src/read_acq/__pycache__/read_acq.cpython-39.pyc
--rw-r--r--   0 smurray   (1096) loco      (1002)     2417 2022-04-20 05:47:51.000000 read_acq-0.5.0/src/read_acq/__pycache__/writers.cpython-37.pyc
--rw-r--r--   0 smurray   (1096) loco      (1002)     2423 2022-02-02 00:38:00.000000 read_acq-0.5.0/src/read_acq/__pycache__/writers.cpython-39.pyc
--rw-r--r--   0 smurray   (1096) loco      (1002)      778 2022-02-02 00:36:07.000000 read_acq-0.5.0/src/read_acq/cli.py
--rw-r--r--   0 smurray   (1096) loco      (1002)     2760 2022-02-02 00:36:07.000000 read_acq-0.5.0/src/read_acq/codec.py
--rw-r--r--   0 smurray   (1096) loco      (1002)     3670 2021-06-03 19:36:39.000000 read_acq-0.5.0/src/read_acq/decode.c
--rwxr-xr-x   0 smurray   (1096) loco      (1002)    21776 2022-02-02 00:36:30.000000 read_acq-0.5.0/src/read_acq/decode.cpython-37m-x86_64-linux-gnu.so
--rwxr-xr-x   0 smurray   (1096) loco      (1002)    16360 2022-06-23 15:52:00.000000 read_acq-0.5.0/src/read_acq/decode.cpython-39-x86_64-linux-gnu.so
--rw-r--r--   0 smurray   (1096) loco      (1002)    13290 2022-04-07 23:17:13.000000 read_acq-0.5.0/src/read_acq/read_acq.py
--rw-r--r--   0 smurray   (1096) loco      (1002)     2067 2022-02-02 00:36:07.000000 read_acq-0.5.0/src/read_acq/writers.py
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.735846 read_acq-0.5.0/src/read_acq.egg-info/
--rw-r--r--   0 smurray   (1096) loco      (1002)     2920 2022-06-23 16:57:47.000000 read_acq-0.5.0/src/read_acq.egg-info/PKG-INFO
--rw-r--r--   0 smurray   (1096) loco      (1002)     1184 2022-06-23 16:57:48.000000 read_acq-0.5.0/src/read_acq.egg-info/SOURCES.txt
--rw-r--r--   0 smurray   (1096) loco      (1002)        1 2022-06-23 16:57:47.000000 read_acq-0.5.0/src/read_acq.egg-info/dependency_links.txt
--rw-r--r--   0 smurray   (1096) loco      (1002)       42 2022-06-23 16:57:47.000000 read_acq-0.5.0/src/read_acq.egg-info/entry_points.txt
--rw-r--r--   0 smurray   (1096) loco      (1002)        1 2021-07-19 19:50:19.000000 read_acq-0.5.0/src/read_acq.egg-info/not-zip-safe
--rw-r--r--   0 smurray   (1096) loco      (1002)      110 2022-06-23 16:57:48.000000 read_acq-0.5.0/src/read_acq.egg-info/requires.txt
--rw-r--r--   0 smurray   (1096) loco      (1002)        9 2022-06-23 16:57:48.000000 read_acq-0.5.0/src/read_acq.egg-info/top_level.txt
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.751847 read_acq-0.5.0/tests/
-drwxr-xr-x   0 smurray   (1096) loco      (1002)        0 2022-06-23 16:57:48.751847 read_acq-0.5.0/tests/data/
--rw-r--r--   0 smurray   (1096) loco      (1002)   656907 2021-06-03 19:36:39.000000 read_acq-0.5.0/tests/data/sample.acq
--rw-r--r--   0 smurray   (1096) loco      (1002)      668 2022-02-02 00:36:07.000000 read_acq-0.5.0/tests/test_cli.py
--rw-r--r--   0 smurray   (1096) loco      (1002)     1653 2022-02-02 00:36:07.000000 read_acq-0.5.0/tests/test_encoding.py
--rw-r--r--   0 smurray   (1096) loco      (1002)     1194 2022-02-02 00:36:07.000000 read_acq-0.5.0/tests/test_writing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:48:43.267514 read_acq-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    53248 2023-07-07 21:48:25.000000 read_acq-0.5.2/.coverage
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-07 21:48:25.000000 read_acq-0.5.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-07 21:48:25.000000 read_acq-0.5.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:48:43.255514 read_acq-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:48:43.259513 read_acq-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/workflows/release-draft.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-07 21:48:25.000000 read_acq-0.5.2/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 21:48:25.000000 read_acq-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 21:48:25.000000 read_acq-0.5.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-07 21:48:25.000000 read_acq-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 21:48:25.000000 read_acq-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-07 21:48:25.000000 read_acq-0.5.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-07 21:48:25.000000 read_acq-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 21:48:43.267514 read_acq-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-07 21:48:25.000000 read_acq-0.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 21:48:25.000000 read_acq-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-07 21:48:43.267514 read_acq-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-07 21:48:25.000000 read_acq-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:48:43.251514 read_acq-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:48:43.259513 read_acq-0.5.2/src/read_acq/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-07 21:48:25.000000 read_acq-0.5.2/src/read_acq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-07 21:48:25.000000 read_acq-0.5.2/src/read_acq/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-07 21:48:25.000000 read_acq-0.5.2/src/read_acq/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-07 21:48:25.000000 read_acq-0.5.2/src/read_acq/decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-07 21:48:25.000000 read_acq-0.5.2/src/read_acq/read_acq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-07 21:48:25.000000 read_acq-0.5.2/src/read_acq/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:48:43.263514 read_acq-0.5.2/src/read_acq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 21:48:43.000000 read_acq-0.5.2/src/read_acq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 21:48:43.000000 read_acq-0.5.2/src/read_acq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:48:43.000000 read_acq-0.5.2/src/read_acq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 21:48:43.000000 read_acq-0.5.2/src/read_acq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:48:42.000000 read_acq-0.5.2/src/read_acq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 21:48:43.000000 read_acq-0.5.2/src/read_acq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 21:48:43.000000 read_acq-0.5.2/src/read_acq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:48:43.263514 read_acq-0.5.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:48:43.263514 read_acq-0.5.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   656907 2023-07-07 21:48:25.000000 read_acq-0.5.2/tests/data/sample.acq
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-07 21:48:25.000000 read_acq-0.5.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-07 21:48:25.000000 read_acq-0.5.2/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 21:48:25.000000 read_acq-0.5.2/tests/test_writing.py
```

### Comparing `read_acq-0.5.0/.coverage` & `read_acq-0.5.2/.coverage`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/.coveragerc` & `read_acq-0.5.2/.coveragerc`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # .coveragerc to control coverage.py
 [run]
 branch = True
 source = read_acq
-parallel = True
 # omit = bad_file.py
 
 [paths]
 source =
     src/
     */site-packages/
```

### Comparing `read_acq-0.5.0/.flake8` & `read_acq-0.5.2/.flake8`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 [flake8]
 ignore =
-  E203    # No space before colon
+  # No space before colon
+  E203
   W503
-  N806    # Variable name should be lower case. We have some single-letter variables that make more sense to be caps.
-  A003    # Class attribute shadows a python builtin -- not much chance of that causing a problem
-  D401    # First line should be in imperative mood -- cached_properties don't fit this bill.
-  D101    # Missing docstring in public class -- my docstrings are in the __init__ which seems to fail this ?
+  # Variable name should be lower case. We have some single-letter variables that make more sense to be caps.
+  N806
+  # Class attribute shadows a python builtin -- not much chance of that causing a problem
+  A003
+  # First line should be in imperative mood -- cached_properties don't fit this bill.
+  D401
+  # Missing docstring in public class -- my docstrings are in the __init__ which seems to fail this ?
+  D101
 max-line-length = 88
 max-complexity = 20
 inline-quotes = double
 docstring-convention=numpy
 rst-roles =
   class
   method
```

### Comparing `read_acq-0.5.0/.github/workflows/test_suite.yaml` & `read_acq-0.5.2/.github/workflows/test_suite.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -16,46 +16,54 @@
       OS: ${{ matrix.os }}
     name: Testing
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest]
-        python-version: [3.8, 3.9, "3.10"]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
     steps:
       - uses: actions/checkout@master
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: set PY
         run: echo "PY=$(python -c 'import hashlib, sys;print(hashlib.sha256(sys.version.encode()+sys.executable.encode()).hexdigest())')" >> $GITHUB_ENV
       - name: Setup Environment
         run: |
           pip install -U coverage
           pip install .[dev]
       - name: Run Tests
         run: |
-          python -m pytest --cov-config=.coveragerc --durations=25
+          coverage run --parallel-mode -m pytest
+
+      - name: Upload coverage data
+        uses: actions/upload-artifact@v3
+        with:
+          name: coverage-data
+          path: ".coverage.*"
+          if-no-files-found: error
+
   downstream:
     env:
       PYTHON: 3.8
       OS: ubuntu-latest
     name: Downstream
     runs-on: ubuntu-latest
     strategy:
       matrix:
         package: ['edges-io', 'edges-cal','edges-analysis']
       fail-fast: false
     steps:
       - uses: actions/checkout@master
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ env.PYTHON }}
       - name: set PY
         run: echo "PY=$(python -c 'import hashlib, sys;print(hashlib.sha256(sys.version.encode()+sys.executable.encode()).hexdigest())')" >> $GITHUB_ENV
       - name: Setup Environment
         run: |
           pip install -U coverage
@@ -67,18 +75,50 @@
           cd ${{ matrix.package }}
           pip install .[dev]
       - name: Install ipykernel
         if: matrix.package == 'edges-cal'
         run: python -m ipykernel install --user --name edges --display-name "edges"
       - name: Print Versions
         run: pip freeze | grep -E "edges-|read_acq"
+
       - name: Run Tests
         run: |
-          cd ../${{ matrix.package }}
-          python -m pytest --cov-config=../read_acq/.coveragerc
+          coverage run --parallel-mode -m pytest ../${{ matrix.package}}
+
+      - name: Upload coverage data
+        uses: actions/upload-artifact@v3
+        with:
+          name: coverage-data
+          path: ".coverage.*"
+          if-no-files-found: error
 
   codecov:
     needs: [downstream, tests]
     name: Codecov Reporting
     runs-on: ubuntu-latest
     steps:
-      - uses: codecov/codecov-action@v2
+      - uses: actions/checkout@v3
+
+      - name: Download coverage data.
+        uses: actions/download-artifact@v3
+        with:
+          name: coverage-data
+
+      - uses: actions/setup-python@v4
+        with:
+          python-version: 3.9
+
+      - name: Install coverage
+        run: pip install coverage
+
+      - run: pip install .[dev]
+
+      - name: Combine/Report
+        run: |
+          coverage combine
+          coverage xml
+
+      - uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: true
+          verbose: true
+          file: ./coverage.xml
```

### Comparing `read_acq-0.5.0/.pre-commit-config.yaml` & `read_acq-0.5.2/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 exclude: '^docs/conf.py|^tests/data/'
 
 ci:
   autoupdate_schedule: monthly
 
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
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=no']
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1  # pick a git hash / tag to point to
+  rev: 6.0.0  # pick a git hash / tag to point to
   hooks:
   - id: flake8
     additional_dependencies:
       - flake8-quotes
       - flake8-comprehensions
       - flake8-builtins
       - flake8-eradicate
@@ -32,41 +32,41 @@
       - flake8-pytest
       - flake8-docstrings
       - flake8-rst-docstrings
       - flake8-rst
       - flake8-copyright
 
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.3.0
   hooks:
   - id: black
 - repo: https://github.com/pre-commit/pygrep-hooks
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
     - id: rst-backticks
     - id: rst-directive-colons
     - id: rst-inline-touching-normal
 - repo: https://github.com/Lucas-C/pre-commit-hooks-markup
   rev: v1.0.1
   hooks:
   - id: rst-linter
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.1
+    rev: v3.8.0
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 
 - repo: https://github.com/asottile/setup-cfg-fmt
-  rev: v1.20.1
+  rev: v2.4.0
   hooks:
   -   id: setup-cfg-fmt
 
 - repo: https://github.com/commitizen-tools/commitizen
-  rev: v2.27.1
+  rev: 3.5.2
   hooks:
     - id: commitizen
       stages: [commit-msg]
```

### Comparing `read_acq-0.5.0/CHANGELOG.md` & `read_acq-0.5.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/LICENSE.rst` & `read_acq-0.5.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/PKG-INFO` & `read_acq-0.5.2/src/read_acq.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: read_acq
-Version: 0.5.0
+Name: read-acq
+Version: 0.5.2
 Summary: Read/Write ACQ Spectrum Files
 Home-page: https://github.com/edges-collab/read_acq
 Author: EDGES Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,17 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: h5
 License-File: LICENSE.rst
```

### Comparing `read_acq-0.5.0/README.rst` & `read_acq-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/setup.cfg` & `read_acq-0.5.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 description = Read/Write ACQ Spectrum Files
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/edges-collab/read_acq
 author = EDGES Team
 author_email = steven.g.murray@asu.edu
 license = MIT
-license_file = LICENSE.rst
+license_files = LICENSE.rst
 platforms = any
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Operating System :: Unix
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 install_requires = 
 	click
 	numpy
@@ -47,26 +44,23 @@
 	acq = read_acq.cli:main
 
 [options.extras_require]
 dev = 
 	edges-io
 	pre-commit
 	pytest>=5
-	pytest-cov
-	python-semantic-release
 h5 = 
 	edges-io
 
 [test]
 extras = True
 
 [tool:pytest]
 addopts = 
-	--cov read_acq --cov-report term-missing
-	--verbose
+	--verbose --durations=25
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
 
 [aliases]
```

### Comparing `read_acq-0.5.0/src/read_acq/cli.py` & `read_acq-0.5.2/src/read_acq/cli.py`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/src/read_acq/codec.py` & `read_acq-0.5.2/src/read_acq/codec.py`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/src/read_acq/decode.c` & `read_acq-0.5.2/src/read_acq/decode.c`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/src/read_acq/read_acq.py` & `read_acq-0.5.2/src/read_acq/read_acq.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,19 +68,17 @@
             return None
 
     def _read_header(self, fname):
         out = {}
 
         name_pattern = re.compile(r"[a-zA-Z_]+")
         with open(fname) as fl:
-
             type_order = [int, float, str]
 
             for line in fl.readlines():
-
                 if not line.startswith(self.header_char):
                     break
 
                 if line.startswith("; FASTSPEC"):
                     name = "fastspec_version"
                     val = line.split()[-1]
                 else:
```

### Comparing `read_acq-0.5.0/src/read_acq/writers.py` & `read_acq-0.5.2/src/read_acq/writers.py`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/src/read_acq.egg-info/PKG-INFO` & `read_acq-0.5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: read-acq
-Version: 0.5.0
+Name: read_acq
+Version: 0.5.2
 Summary: Read/Write ACQ Spectrum Files
 Home-page: https://github.com/edges-collab/read_acq
 Author: EDGES Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,17 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: h5
 License-File: LICENSE.rst
```

### Comparing `read_acq-0.5.0/tests/data/sample.acq` & `read_acq-0.5.2/tests/data/sample.acq`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/tests/test_cli.py` & `read_acq-0.5.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/tests/test_encoding.py` & `read_acq-0.5.2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `read_acq-0.5.0/tests/test_writing.py` & `read_acq-0.5.2/tests/test_writing.py`

 * *Files identical despite different names*


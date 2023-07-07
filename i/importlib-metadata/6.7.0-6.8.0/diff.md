# Comparing `tmp/importlib_metadata-6.7.0.tar.gz` & `tmp/importlib_metadata-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.7.0.tar", last modified: Sun Jun 18 21:44:24 2023, max compression
+gzip compressed data, was "importlib_metadata-6.8.0.tar", last modified: Fri Jul  7 16:15:52 2023, max compression
```

## Comparing `importlib_metadata-6.7.0.tar` & `importlib_metadata-6.8.0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.618949 importlib_metadata-6.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.618949 importlib_metadata-6.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.618949 importlib_metadata-6.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.618949 importlib_metadata-6.7.0/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30724 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 21:44:24.000000 importlib_metadata-6.7.0/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.614949 importlib_metadata-6.7.0/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:24.622949 importlib_metadata-6.7.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-18 21:44:05.000000 importlib_metadata-6.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.234363 importlib_metadata-6.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.234363 importlib_metadata-6.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.234363 importlib_metadata-6.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30749 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-07 16:15:52.000000 importlib_metadata-6.8.0/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-07 16:15:52.000000 importlib_metadata-6.8.0/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:15:52.000000 importlib_metadata-6.8.0/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 16:15:52.000000 importlib_metadata-6.8.0/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 16:15:52.000000 importlib_metadata-6.8.0/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.234363 importlib_metadata-6.8.0/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:52.238363 importlib_metadata-6.8.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-07 16:15:29.000000 importlib_metadata-6.8.0/tox.ini
```

### Comparing `importlib_metadata-6.7.0/.github/workflows/main.yml` & `importlib_metadata-6.8.0/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -38,65 +38,56 @@
 
 
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
-        - python: pypy3.9
-          platform: ubuntu-latest
-        - platform: ubuntu-latest
-          python: "3.8"
-        - platform: ubuntu-latest
-          python: "3.9"
+        # disabled for #463
+        # - python: pypy3.9
+        #   platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
         with:
           # fetch all branches and tags (to get tags for versioning)
           # ref actions/checkout#448
           fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
@@ -141,15 +132,15 @@
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
       - name: Release
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `importlib_metadata-6.7.0/CHANGES.rst` & `importlib_metadata-6.8.0/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v6.8.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v6.7.0
 ======
 
 * #453: When inferring top-level names that are importable for
   distributions in ``package_distributions``, now symlinks to
   other directories are honored.
```

### Comparing `importlib_metadata-6.7.0/LICENSE` & `importlib_metadata-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/PKG-INFO` & `importlib_metadata-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.7.0
+Version: 6.8.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: perf
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/importlib_metadata.svg
    :target: https://pypi.org/project/importlib_metadata
 
 .. image:: https://img.shields.io/pypi/pyversions/importlib_metadata.svg
 
 .. image:: https://github.com/python/importlib_metadata/workflows/tests/badge.svg
    :target: https://github.com/python/importlib_metadata/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/importlib-metadata/badge/?version=latest
    :target: https://importlib-metadata.readthedocs.io/en/latest/?badge=latest
```

### Comparing `importlib_metadata-6.7.0/README.rst` & `importlib_metadata-6.8.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/importlib_metadata.svg
 
 .. image:: https://github.com/python/importlib_metadata/workflows/tests/badge.svg
    :target: https://github.com/python/importlib_metadata/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/importlib-metadata/badge/?version=latest
    :target: https://importlib-metadata.readthedocs.io/en/latest/?badge=latest
```

### Comparing `importlib_metadata-6.7.0/conftest.py` & `importlib_metadata-6.8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/docs/conf.py` & `importlib_metadata-6.8.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
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

### Comparing `importlib_metadata-6.7.0/docs/index.rst` & `importlib_metadata-6.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/docs/migration.rst` & `importlib_metadata-6.8.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/docs/using.rst` & `importlib_metadata-6.8.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/exercises.py` & `importlib_metadata-6.8.0/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/importlib_metadata/__init__.py` & `importlib_metadata-6.8.0/importlib_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -869,15 +869,15 @@
         filename, ext = os.path.splitext(stem)
         if ext not in ('.dist-info', '.egg-info'):
             return
         name, sep, rest = filename.partition('-')
         return name
 
 
-def distribution(distribution_name) -> Distribution:
+def distribution(distribution_name: str) -> Distribution:
     """Get the ``Distribution`` instance for the named package.
 
     :param distribution_name: The name of the distribution package as a string.
     :return: A ``Distribution`` instance (or subclass thereof).
     """
     return Distribution.from_name(distribution_name)
 
@@ -886,24 +886,24 @@
     """Get all ``Distribution`` instances in the current environment.
 
     :return: An iterable of ``Distribution`` instances.
     """
     return Distribution.discover(**kwargs)
 
 
-def metadata(distribution_name) -> _meta.PackageMetadata:
+def metadata(distribution_name: str) -> _meta.PackageMetadata:
     """Get the metadata for the named package.
 
     :param distribution_name: The name of the distribution package to query.
     :return: A PackageMetadata containing the parsed metadata.
     """
     return Distribution.from_name(distribution_name).metadata
 
 
-def version(distribution_name) -> str:
+def version(distribution_name: str) -> str:
     """Get the version string for the named package.
 
     :param distribution_name: The name of the distribution package to query.
     :return: The version string for the package as defined in the package's
         "Version" metadata key.
     """
     return distribution(distribution_name).version
@@ -929,24 +929,24 @@
     """
     eps = itertools.chain.from_iterable(
         dist.entry_points for dist in _unique(distributions())
     )
     return EntryPoints(eps).select(**params)
 
 
-def files(distribution_name) -> Optional[List[PackagePath]]:
+def files(distribution_name: str) -> Optional[List[PackagePath]]:
     """Return a list of files for the named package.
 
     :param distribution_name: The name of the distribution package to query.
     :return: List of files composing the distribution.
     """
     return distribution(distribution_name).files
 
 
-def requires(distribution_name) -> Optional[List[str]]:
+def requires(distribution_name: str) -> Optional[List[str]]:
     """
     Return a list of requirements for the named package.
 
     :return: An iterable of requirements, suitable for
         packaging.requirement.Requirement.
     """
     return distribution(distribution_name).requires
```

### Comparing `importlib_metadata-6.7.0/importlib_metadata/_adapters.py` & `importlib_metadata-6.8.0/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/importlib_metadata/_collections.py` & `importlib_metadata-6.8.0/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/importlib_metadata/_compat.py` & `importlib_metadata-6.8.0/importlib_metadata/_compat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 import os
 import sys
 import platform
 
 from typing import Union
 
 
-__all__ = ['install', 'NullFinder', 'Protocol']
-
-
-try:
-    from typing import Protocol
-except ImportError:  # pragma: no cover
-    # Python 3.7 compatibility
-    from typing_extensions import Protocol  # type: ignore
+__all__ = ['install', 'NullFinder']
 
 
 def install(cls):
     """
     Class decorator for installation on sys.meta_path.
 
     Adds the backport DistributionFinder to sys.meta_path and
```

### Comparing `importlib_metadata-6.7.0/importlib_metadata/_functools.py` & `importlib_metadata-6.8.0/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/importlib_metadata/_itertools.py` & `importlib_metadata-6.8.0/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/importlib_metadata/_meta.py` & `importlib_metadata-6.8.0/importlib_metadata/_meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._compat import Protocol
+from typing import Protocol
 from typing import Any, Dict, Iterator, List, Optional, TypeVar, Union, overload
 
 
 _T = TypeVar("_T")
 
 
 class PackageMetadata(Protocol):
```

### Comparing `importlib_metadata-6.7.0/importlib_metadata/_py39compat.py` & `importlib_metadata-6.8.0/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/importlib_metadata/_text.py` & `importlib_metadata-6.8.0/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.8.0/importlib_metadata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.7.0
+Version: 6.8.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: perf
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/importlib_metadata.svg
    :target: https://pypi.org/project/importlib_metadata
 
 .. image:: https://img.shields.io/pypi/pyversions/importlib_metadata.svg
 
 .. image:: https://github.com/python/importlib_metadata/workflows/tests/badge.svg
    :target: https://github.com/python/importlib_metadata/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/importlib-metadata/badge/?version=latest
    :target: https://importlib-metadata.readthedocs.io/en/latest/?badge=latest
```

### Comparing `importlib_metadata-6.7.0/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.8.0/importlib_metadata.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 .coveragerc
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
-CHANGES.rst
 LICENSE
+NEWS.rst
 README.rst
 conftest.py
 exercises.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/__init__.py
 docs/api.rst
 docs/conf.py
```

### Comparing `importlib_metadata-6.7.0/pytest.ini` & `importlib_metadata-6.8.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/setup.cfg` & `importlib_metadata-6.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	zipp>=0.5
 	typing-extensions>=3.6.4; python_version < "3.8"
 
 [options.packages.find]
 exclude = 
 	build*
@@ -33,15 +33,15 @@
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	importlib_resources>=1.3; python_version < "3.9"
 	packaging
 	pyfakefs
 	flufl.flake8
 	pytest-perf >= 0.9.2
```

### Comparing `importlib_metadata-6.7.0/tests/_path.py` & `importlib_metadata-6.8.0/tests/_path.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-# from jaraco.path 3.6
+# from jaraco.path 3.7
 
 import functools
 import pathlib
-from typing import Dict, Union
-
-try:
-    from typing import Protocol, runtime_checkable
-except ImportError:  # pragma: no cover
-    # Python 3.7
-    from typing_extensions import Protocol, runtime_checkable  # type: ignore
+from typing import Dict, Protocol, Union
+from typing import runtime_checkable
 
 
 class Symlink(str):
     """
     A string indicating the target of a symlink.
     """
```

### Comparing `importlib_metadata-6.7.0/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.8.0/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.8.0/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.8.0/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tests/fixtures.py` & `importlib_metadata-6.8.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tests/test_api.py` & `importlib_metadata-6.8.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tests/test_integration.py` & `importlib_metadata-6.8.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tests/test_main.py` & `importlib_metadata-6.8.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tests/test_py39compat.py` & `importlib_metadata-6.8.0/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tests/test_zip.py` & `importlib_metadata-6.8.0/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.7.0/tox.ini` & `importlib_metadata-6.8.0/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
@@ -32,14 +28,24 @@
 deps =
 	diff-cover
 commands =
 	pytest {posargs} --cov-report xml
 	diff-cover coverage.xml --compare-branch=origin/main --html-report diffcov.html
 	diff-cover coverage.xml --compare-branch=origin/main --fail-under=100
 
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
+
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
 passenv =
```


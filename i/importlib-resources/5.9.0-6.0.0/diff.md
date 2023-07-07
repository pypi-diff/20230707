# Comparing `tmp/importlib_resources-5.9.0.tar.gz` & `tmp/importlib_resources-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_resources-5.9.0.tar", last modified: Fri Jul 22 16:46:53 2022, max compression
+gzip compressed data, was "importlib_resources-6.0.0.tar", last modified: Fri Jul  7 18:27:18 2023, max compression
```

## Comparing `importlib_resources-5.9.0.tar` & `importlib_resources-6.0.0.tar`

### file list

```diff
@@ -1,85 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.761731 importlib_resources-5.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.761731 importlib_resources-5.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9150 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5906 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/importlib_resources/
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4202 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/readers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/importlib_resources/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/importlib_resources/tests/data01/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/binary.file
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/data01/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/subdirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/subdirectory/binary.file
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/utf-16.file
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/utf-8.file
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/data02/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/data02/one/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/one/resource1.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/data02/two/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/two/resource2.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/namespacedata01/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/namespacedata01/binary.file
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/namespacedata01/utf-16.file
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/namespacedata01/utf-8.file
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_compatibilty_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_resource.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1417 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/update-zips.py
--rw-r--r--   0 runner    (1001) docker     (121)     5309 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/zipdata01/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/zipdata01/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/zipdata01/ziptestdata.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/zipdata02/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/zipdata02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/zipdata02/ziptestdata.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/importlib_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/docs/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/importlib_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/importlib_resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data01/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/binary.file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data01/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/subdirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/subdirectory/binary.file
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/utf-16.file
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data01/utf-8.file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data02/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data02/one/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/one/resource1.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.857378 importlib_resources-6.0.0/importlib_resources/tests/data02/subdirectory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data02/subdirectory/subsubdir/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/subdirectory/subsubdir/resource.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/data02/two/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/data02/two/resource2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/namespacedata01/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/namespacedata01/binary.file
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/namespacedata01/utf-16.file
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/namespacedata01/utf-8.file
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_compatibilty_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/test_resource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/update-zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/zipdata01/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/zipdata01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/zipdata01/ziptestdata.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/importlib_resources/tests/zipdata02/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/zipdata02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/importlib_resources/tests/zipdata02/ziptestdata.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:27:18.861378 importlib_resources-6.0.0/importlib_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 18:27:18.000000 importlib_resources-6.0.0/importlib_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 18:27:18.865378 importlib_resources-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-07 18:26:57.000000 importlib_resources-6.0.0/tox.ini
```

### Comparing `importlib_resources-5.9.0/.gitignore` & `importlib_resources-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.9.0/CHANGES.rst` & `importlib_resources-6.0.0/NEWS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,80 @@
+v6.0.0
+======
+
+Deprecations and Removals
+-------------------------
+
+- Removed legacy functions deprecated in 5.3. (#80)
+
+
+v5.13.0
+=======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
+v5.12.0
+=======
+
+* #257: ``importlib_resources`` (backport) now gives
+  precedence to built-in readers (file system, zip,
+  namespace packages), providing forward-compatibility
+  of behaviors like ``MultiplexedPath``.
+
+v5.11.1
+=======
+
+v5.10.4
+=======
+
+* #280: Fixed one more ``EncodingWarning`` in test suite.
+
+v5.11.0
+=======
+
+* #265: ``MultiplexedPath`` now honors multiple subdirectories
+  in ``iterdir`` and ``joinpath``.
+
+v5.10.3
+=======
+
+* Packaging refresh, including fixing EncodingWarnings
+  and some tests cleanup.
+
+v5.10.2
+=======
+
+* #274: Prefer ``write_bytes`` to context manager as
+  proposed in gh-100586.
+
+v5.10.1
+=======
+
+* #274: Fixed ``ResourceWarning`` in ``_common``.
+
+v5.10.0
+=======
+
+* #203: Lifted restriction on modules passed to ``files``.
+  Now modules need not be a package and if a non-package
+  module is passed, resources will be resolved adjacent to
+  those modules, even for modules not found in any package.
+  For example, ``files(import_module('mod.py'))`` will
+  resolve resources found at the root. The parameter to
+  files was renamed from 'package' to 'anchor', with a
+  compatibility shim for those passing by keyword.
+
+* #259: ``files`` no longer requires the anchor to be
+  specified and can infer the anchor from the caller's scope
+  (defaults to the caller's module).
+
 v5.9.0
 ======
 
 * #228: ``as_file`` now also supports a ``Traversable``
   representing a directory and (when needed) renders the
   full tree to a temporary directory.
```

### Comparing `importlib_resources-5.9.0/PKG-INFO` & `importlib_resources-6.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: importlib_resources
-Version: 5.9.0
+Version: 6.0.0
 Summary: Read resources from Python packages
 Home-page: https://github.com/python/importlib_resources
 Author: Barry Warsaw
 Author-email: barry@python.org
 Project-URL: Documentation, https://importlib-resources.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/importlib_resources.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/importlib_resources
 
 .. image:: https://img.shields.io/pypi/pyversions/importlib_resources.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/importlib_resources
 
 .. image:: https://github.com/python/importlib_resources/workflows/tests/badge.svg
    :target: https://github.com/python/importlib_resources/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/importlib-resources/badge/?version=latest
    :target: https://importlib-resources.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/importlib-resources
    :target: https://tidelift.com/subscription/pkg/pypi-importlib-resources?utm_source=pypi-importlib-resources&utm_medium=readme
 
 ``importlib_resources`` is a backport of Python standard library
 `importlib.resources
@@ -60,15 +61,17 @@
 were contributed to different versions in the standard library:
 
 .. list-table::
    :header-rows: 1
 
    * - importlib_resources
      - stdlib
-   * - 5.8
+   * - 6.0
+     - 3.13
+   * - 5.12
      - 3.12
    * - 5.7
      - 3.11
    * - 5.0
      - 3.10
    * - 1.3
      - 3.9
```

### Comparing `importlib_resources-5.9.0/README.rst` & `importlib_resources-6.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .. image:: https://img.shields.io/pypi/v/importlib_resources.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/importlib_resources
 
 .. image:: https://img.shields.io/pypi/pyversions/importlib_resources.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/importlib_resources
 
 .. image:: https://github.com/python/importlib_resources/workflows/tests/badge.svg
    :target: https://github.com/python/importlib_resources/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/importlib-resources/badge/?version=latest
    :target: https://importlib-resources.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/importlib-resources
    :target: https://tidelift.com/subscription/pkg/pypi-importlib-resources?utm_source=pypi-importlib-resources&utm_medium=readme
 
 ``importlib_resources`` is a backport of Python standard library
 `importlib.resources
@@ -42,15 +43,17 @@
 were contributed to different versions in the standard library:
 
 .. list-table::
    :header-rows: 1
 
    * - importlib_resources
      - stdlib
-   * - 5.8
+   * - 6.0
+     - 3.13
+   * - 5.12
      - 3.12
    * - 5.7
      - 3.11
    * - 5.0
      - 3.10
    * - 1.3
      - 3.9
```

### Comparing `importlib_resources-5.9.0/docs/index.rst` & `importlib_resources-6.0.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Welcome to |project| documentation!
 ===================================
 
+.. sidebar-links::
+   :home:
+   :pypi:
+
 ``importlib_resources`` is a library which provides for access to *resources*
 in Python packages.  It provides functionality similar to ``pkg_resources``
 `Basic Resource Access`_ API, but without all of the overhead and performance
 problems of ``pkg_resources``.
 
-In our terminology, a *resource* is a file tree that is located within an
-importable `Python package`_.  Resources can live on the file system or in a
+In our terminology, a *resource* is a file tree that is located alongside an
+importable `Python module`_.  Resources can live on the file system or in a
 zip file, with support for other loader_ classes that implement the appropriate
 API for reading resources.
 
 ``importlib_resources`` supplies a backport of :mod:`importlib.resources`,
 enabling early access to features of future Python versions and making
 functionality available for older Python versions. Users are encouraged to
 use the Python standard library where suitable and fall back to
@@ -39,9 +43,9 @@
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
 
 
 .. _`Basic Resource Access`: http://setuptools.readthedocs.io/en/latest/pkg_resources.html#basic-resource-access
-.. _`Python package`: https://docs.python.org/3/reference/import.html#packages
+.. _`Python module`: https://docs.python.org/3/glossary.html#term-module
 .. _loader: https://docs.python.org/3/reference/import.html#finders-and-loaders
```

### Comparing `importlib_resources-5.9.0/docs/migration.rst` & `importlib_resources-6.0.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.9.0/docs/using.rst` & `importlib_resources-6.0.0/docs/using.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 .. _using:
 
 ===========================
  Using importlib_resources
 ===========================
 
 ``importlib_resources`` is a library that leverages Python's import system to
-provide access to *resources* within *packages*.  Given that this library is
-built on top of the import system, it is highly efficient and easy to use.
-This library's philosophy is that, if you can import a package, you can access
-resources within that package.  Resources can be opened or read, in either
-binary or text mode.
+provide access to *resources* within *packages* and alongside *modules*. Given
+that this library is built on top of the import system, it is highly efficient
+and easy to use. This library's philosophy is that, if one can import a
+module, one can access resources associated with that module. Resources can be
+opened or read, in either binary or text mode.
 
 What exactly do we mean by "a resource"?  It's easiest to think about the
 metaphor of files and directories on the file system, though it's important to
 keep in mind that this is just a metaphor.  Resources and packages **do not**
 have to exist as physical files and directories on the file system.
 
 If you have a file system layout such as::
 
     data/
         __init__.py
         one/
             __init__.py
             resource1.txt
+            module1.py
             resources1/
                 resource1.1.txt
         two/
             __init__.py
             resource2.txt
+    standalone.py
+    resource3.txt
 
 then the directories are ``data``, ``data/one``, and ``data/two``.  Each of
 these are also Python packages by virtue of the fact that they all contain
 ``__init__.py`` files.  That means that in Python, all of these import
 statements work::
 
     import data
@@ -44,19 +47,22 @@
 additional attribute, namely a ``__path__`` [#fn1]_.
 
 In this analogy then, resources are just files or directories contained in a
 package directory, so
 ``data/one/resource1.txt`` and ``data/two/resource2.txt`` are both resources,
 as are the ``__init__.py`` files in all the directories.
 
-Resources are always accessed relative to the package that they live in.
-``resource1.txt`` and ``resources1/resource1.1.txt`` are resources within
-the ``data.one`` package, and
-``two/resource2.txt`` is a resource within the
-``data`` package.
+Resources in packages are always accessed relative to the package that they
+live in. ``resource1.txt`` and ``resources1/resource1.1.txt`` are resources
+within the ``data.one`` package, and ``two/resource2.txt`` is a resource
+within the ``data`` package.
+
+Resources may also be referenced relative to another *anchor*, a module in a
+package (``data.one.module1``) or a standalone module (``standalone``). In
+this case, resources are loaded from the same loader that loaded that module.
 
 
 Example
 =======
 
 Let's say you are writing an email parsing library and in your test suite you
 have a sample email message in a file called ``message.eml``.  You would like
@@ -99,72 +105,71 @@
 using ``importlib_resources`` would look like::
 
     from importlib_resources import files
     # Reads contents with UTF-8 encoding and returns str.
     eml = files('email.tests.data').joinpath('message.eml').read_text()
 
 
-Packages or package names
-=========================
+Anchors
+=======
 
-All of the ``importlib_resources`` APIs take a *package* as their first
-parameter, but this can either be a package name (as a ``str``) or an actual
-module object, though the module *must* be a package.  If a string is
-passed in, it must name an importable Python package, and this is first
-imported.  Thus the above example could also be written as::
+The ``importlib_resources`` ``files`` API takes an *anchor* as its first
+parameter, which can either be a package name (as a ``str``) or an actual
+module object.  If a string is passed in, it must name an importable Python
+module, which is imported prior to loading any resources. Thus the above
+example could also be written as::
 
     import email.tests.data
     eml = files(email.tests.data).joinpath('message.eml').read_text()
 
 
+Namespace Packages
+==================
+
+``importlib_resources`` supports namespace packages as anchors just like
+any other package. Similar to modules in a namespace package,
+resources in a namespace package are not allowed to collide by name.
+For example, if two packages both expose ``nspkg/data/foo.txt``, those
+resources are unsupported by this library. The package will also likely
+experience problems due to the collision with installers.
+
+It's perfectly valid, however, for two packages to present different resources
+in the same namespace package, regular package, or subdirectory.
+For example, one package could expose ``nspkg/data/foo.txt`` and another
+expose ``nspkg/data/bar.txt`` and those two packages could be installed
+into separate paths, and the resources should be queryable::
+
+    data = importlib_resources.files('nspkg').joinpath('data')
+    data.joinpath('foo.txt').read_text()
+    data.joinpath('bar.txt').read_text()
+
+
 File system or zip file
 =======================
 
-In general you never have to worry whether your package is on the file system
-or in a zip file, as the ``importlib_resources`` APIs hide those details from
-you.  Sometimes though, you need a path to an actual file on the file system.
+A consumer need not worry whether any given package is on the file system
+or in a zip file, as the ``importlib_resources`` APIs abstracts those details.
+Sometimes though, the user needs a path to an actual file on the file system.
 For example, some SSL APIs require a certificate file to be specified by a
 real file system path, and C's ``dlopen()`` function also requires a real file
 system path.
 
-To support this, ``importlib_resources`` provides an API that will extract the
-resource from a zip file to a temporary file, and return the file system path
-to this temporary file as a :py:class:`pathlib.Path` object.  In order to
-properly clean up this temporary file, what's actually returned is a context
-manager that you can use in a ``with``-statement::
+To support this need, ``importlib_resources`` provides an API to extract the
+resource from a zip file to a temporary file or folder and return the file
+system path to this materialized resource as a :py:class:`pathlib.Path`
+object. In order to properly clean up this temporary file, what's actually
+returned is a context manager for use in a ``with``-statement::
 
     from importlib_resources import files, as_file
 
     source = files(email.tests.data).joinpath('message.eml')
     with as_file(source) as eml:
         third_party_api_requiring_file_system_path(eml)
 
-You can use all the standard :py:mod:`contextlib` APIs to manage this context
-manager.
-
-.. attention::
-
-   There is an odd interaction with Python 3.4, 3.5, and 3.6 regarding adding
-   zip or wheel file paths to ``sys.path``.  Due to limitations in `zipimport
-   <https://docs.python.org/3/library/zipimport.html>`_, which can't be
-   changed without breaking backward compatibility, you **must** use an
-   absolute path to the zip/wheel file.  If you use a relative path, you will
-   not be able to find resources inside these zip files.  E.g.:
-
-   **No**::
-
-       sys.path.append('relative/path/to/foo.whl')
-       files('foo')  # This will fail!
-
-   **Yes**::
-
-       sys.path.append(os.path.abspath('relative/path/to/foo.whl'))
-       files('foo')
-
-Both relative and absolute paths work for Python 3.7 and newer.
+Use all the standard :py:mod:`contextlib` APIs to manage this context manager.
 
 
 Migrating from Legacy
 =====================
 
 Starting with Python 3.9 and ``importlib_resources`` 1.4, this package
 introduced the ``files()`` API, to be preferred over the legacy API,
```

### Comparing `importlib_resources-5.9.0/importlib_resources/_adapters.py` & `importlib_resources-6.0.0/importlib_resources/_adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,15 @@
 
 
 def _io_wrapper(file, mode='r', *args, **kwargs):
     if mode == 'r':
         return TextIOWrapper(file, *args, **kwargs)
     elif mode == 'rb':
         return file
-    raise ValueError(
-        "Invalid mode value '{}', only 'r' and 'rb' are supported".format(mode)
-    )
+    raise ValueError(f"Invalid mode value '{mode}', only 'r' and 'rb' are supported")
 
 
 class CompatibilityFiles:
     """
     Adapter for an existing or non-existent resource reader
     to provide a compatibility .files().
     """
```

### Comparing `importlib_resources-5.9.0/importlib_resources/_common.py` & `importlib_resources-6.0.0/importlib_resources/_common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,66 @@
 import os
 import pathlib
 import tempfile
 import functools
 import contextlib
 import types
 import importlib
+import inspect
+import warnings
+import itertools
 
-from typing import Union, Optional
+from typing import Union, Optional, cast
 from .abc import ResourceReader, Traversable
 
 from ._compat import wrap_spec
 
 Package = Union[types.ModuleType, str]
+Anchor = Package
 
 
-def files(package):
-    # type: (Package) -> Traversable
+def package_to_anchor(func):
     """
-    Get a Traversable resource from a package
+    Replace 'package' parameter as 'anchor' and warn about the change.
+
+    Other errors should fall through.
+
+    >>> files('a', 'b')
+    Traceback (most recent call last):
+    TypeError: files() takes from 0 to 1 positional arguments but 2 were given
+    """
+    undefined = object()
+
+    @functools.wraps(func)
+    def wrapper(anchor=undefined, package=undefined):
+        if package is not undefined:
+            if anchor is not undefined:
+                return func(anchor, package)
+            warnings.warn(
+                "First parameter to files is renamed to 'anchor'",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            return func(package)
+        elif anchor is undefined:
+            return func()
+        return func(anchor)
+
+    return wrapper
+
+
+@package_to_anchor
+def files(anchor: Optional[Anchor] = None) -> Traversable:
+    """
+    Get a Traversable resource for an anchor.
     """
-    return from_package(get_package(package))
+    return from_package(resolve(anchor))
 
 
-def get_resource_reader(package):
-    # type: (types.ModuleType) -> Optional[ResourceReader]
+def get_resource_reader(package: types.ModuleType) -> Optional[ResourceReader]:
     """
     Return the package's loader if it's a ResourceReader.
     """
     # We can't use
     # a issubclass() check here because apparently abc.'s __subclasscheck__()
     # hook wants to create a weak reference to the object, but
     # zipimport.zipimporter does not support weak references, resulting in a
@@ -35,32 +68,47 @@
     spec = package.__spec__
     reader = getattr(spec.loader, 'get_resource_reader', None)  # type: ignore
     if reader is None:
         return None
     return reader(spec.name)  # type: ignore
 
 
-def resolve(cand):
-    # type: (Package) -> types.ModuleType
-    return cand if isinstance(cand, types.ModuleType) else importlib.import_module(cand)
+@functools.singledispatch
+def resolve(cand: Optional[Anchor]) -> types.ModuleType:
+    return cast(types.ModuleType, cand)
+
+
+@resolve.register
+def _(cand: str) -> types.ModuleType:
+    return importlib.import_module(cand)
+
 
+@resolve.register
+def _(cand: None) -> types.ModuleType:
+    return resolve(_infer_caller().f_globals['__name__'])
 
-def get_package(package):
-    # type: (Package) -> types.ModuleType
-    """Take a package name or module object and return the module.
 
-    Raise an exception if the resolved module is not a package.
+def _infer_caller():
     """
-    resolved = resolve(package)
-    if wrap_spec(resolved).submodule_search_locations is None:
-        raise TypeError(f'{package!r} is not a package')
-    return resolved
+    Walk the stack and find the frame of the first caller not in this module.
+    """
+
+    def is_this_file(frame_info):
+        return frame_info.filename == __file__
+
+    def is_wrapper(frame_info):
+        return frame_info.function == 'wrapper'
+
+    not_this_file = itertools.filterfalse(is_this_file, inspect.stack())
+    # also exclude 'wrapper' due to singledispatch in the call stack
+    callers = itertools.filterfalse(is_wrapper, not_this_file)
+    return next(callers).frame
 
 
-def from_package(package):
+def from_package(package: types.ModuleType):
     """
     Return a Traversable object for the given package.
 
     """
     spec = wrap_spec(package)
     reader = spec.loader.get_resource_reader(spec.name)
     return reader.files()
@@ -151,9 +199,9 @@
 def _write_contents(target, source):
     child = target.joinpath(source.name)
     if source.is_dir():
         child.mkdir()
         for item in source.iterdir():
             _write_contents(child, item)
     else:
-        child.open('wb').write(source.read_bytes())
+        child.write_bytes(source.read_bytes())
     return child
```

### Comparing `importlib_resources-5.9.0/importlib_resources/_compat.py` & `importlib_resources-6.0.0/importlib_resources/_compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,27 +68,28 @@
                 path = pathlib.Path(self.path)
             except TypeError:
                 return None
             if path.exists():
                 return readers.FileReader(self)
 
         return (
-            # native reader if it supplies 'files'
-            _native_reader(self.spec)
-            or
             # local ZipReader if a zip module
             _zip_reader(self.spec)
             or
             # local NamespaceReader if a namespace module
             _namespace_reader(self.spec)
             or
             # local FileReader
             _file_reader(self.spec)
+            or
+            # native reader if it supplies 'files'
+            _native_reader(self.spec)
+            or
             # fallback - adapt the spec ResourceReader to TraversableReader
-            or _adapters.CompatibilityFiles(self.spec)
+            _adapters.CompatibilityFiles(self.spec)
         )
 
 
 def wrap_spec(package):
     """
     Construct a package spec with traversable compatibility
     on the spec/loader/reader.
```

### Comparing `importlib_resources-5.9.0/importlib_resources/abc.py` & `importlib_resources-6.0.0/importlib_resources/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,16 @@
         mode may be 'r' or 'rb' to open as text or binary. Return a handle
         suitable for reading (same as pathlib.Path.open).
 
         When opening as text, accepts encoding parameters such as those
         accepted by io.TextIOWrapper.
         """
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def name(self) -> str:
         """
         The base name of this object without any parent references.
         """
 
 
 class TraversableResources(ResourceReader):
```

### Comparing `importlib_resources-5.9.0/importlib_resources/simple.py` & `importlib_resources-6.0.0/importlib_resources/simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,55 +12,74 @@
 
 class SimpleReader(abc.ABC):
     """
     The minimum, low-level interface required from a resource
     provider.
     """
 
-    @abc.abstractproperty
-    def package(self):
-        # type: () -> str
+    @property
+    @abc.abstractmethod
+    def package(self) -> str:
         """
         The name of the package for which this reader loads resources.
         """
 
     @abc.abstractmethod
-    def children(self):
-        # type: () -> List['SimpleReader']
+    def children(self) -> List['SimpleReader']:
         """
         Obtain an iterable of SimpleReader for available
         child containers (e.g. directories).
         """
 
     @abc.abstractmethod
-    def resources(self):
-        # type: () -> List[str]
+    def resources(self) -> List[str]:
         """
         Obtain available named resources for this virtual package.
         """
 
     @abc.abstractmethod
-    def open_binary(self, resource):
-        # type: (str) -> BinaryIO
+    def open_binary(self, resource: str) -> BinaryIO:
         """
         Obtain a File-like for a named resource.
         """
 
     @property
     def name(self):
         return self.package.split('.')[-1]
 
 
+class ResourceContainer(Traversable):
+    """
+    Traversable container for a package's resources via its reader.
+    """
+
+    def __init__(self, reader: SimpleReader):
+        self.reader = reader
+
+    def is_dir(self):
+        return True
+
+    def is_file(self):
+        return False
+
+    def iterdir(self):
+        files = (ResourceHandle(self, name) for name in self.reader.resources)
+        dirs = map(ResourceContainer, self.reader.children())
+        return itertools.chain(files, dirs)
+
+    def open(self, *args, **kwargs):
+        raise IsADirectoryError()
+
+
 class ResourceHandle(Traversable):
     """
     Handle to a named resource in a ResourceReader.
     """
 
-    def __init__(self, parent, name):
-        # type: (ResourceContainer, str) -> None
+    def __init__(self, parent: ResourceContainer, name: str):
         self.parent = parent
         self.name = name  # type: ignore
 
     def is_file(self):
         return True
 
     def is_dir(self):
@@ -72,38 +91,14 @@
             stream = io.TextIOWrapper(*args, **kwargs)
         return stream
 
     def joinpath(self, name):
         raise RuntimeError("Cannot traverse into a resource")
 
 
-class ResourceContainer(Traversable):
-    """
-    Traversable container for a package's resources via its reader.
-    """
-
-    def __init__(self, reader):
-        # type: (SimpleReader) -> None
-        self.reader = reader
-
-    def is_dir(self):
-        return True
-
-    def is_file(self):
-        return False
-
-    def iterdir(self):
-        files = (ResourceHandle(self, name) for name in self.reader.resources)
-        dirs = map(ResourceContainer, self.reader.children())
-        return itertools.chain(files, dirs)
-
-    def open(self, *args, **kwargs):
-        raise IsADirectoryError()
-
-
 class TraversableReader(TraversableResources, SimpleReader):
     """
     A TraversableResources based on SimpleReader. Resource providers
     may derive from this class to provide the TraversableResources
     interface by supplying the SimpleReader interface.
     """
```

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/test_compatibilty_files.py` & `importlib_resources-6.0.0/importlib_resources/tests/test_compatibilty_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,19 +60,21 @@
 
     def test_orphan_path_name(self):
         self.assertEqual((self.files / 'a' / 'b').name, 'b')
         self.assertEqual((self.files / 'a' / 'b' / 'c').name, 'c')
 
     def test_spec_path_open(self):
         self.assertEqual(self.files.read_bytes(), b'Hello, world!')
-        self.assertEqual(self.files.read_text(), 'Hello, world!')
+        self.assertEqual(self.files.read_text(encoding='utf-8'), 'Hello, world!')
 
     def test_child_path_open(self):
         self.assertEqual((self.files / 'a').read_bytes(), b'Hello, world!')
-        self.assertEqual((self.files / 'a').read_text(), 'Hello, world!')
+        self.assertEqual(
+            (self.files / 'a').read_text(encoding='utf-8'), 'Hello, world!'
+        )
 
     def test_orphan_path_open(self):
         with self.assertRaises(FileNotFoundError):
             (self.files / 'a' / 'b').read_bytes()
         with self.assertRaises(FileNotFoundError):
             (self.files / 'a' / 'b' / 'c').read_bytes()
```

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/test_contents.py` & `importlib_resources-6.0.0/importlib_resources/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/test_open.py` & `importlib_resources-6.0.0/importlib_resources/tests/test_open.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,58 +11,62 @@
         with target.open('rb'):
             pass
 
 
 class CommonTextTests(util.CommonTests, unittest.TestCase):
     def execute(self, package, path):
         target = resources.files(package).joinpath(path)
-        with target.open():
+        with target.open(encoding='utf-8'):
             pass
 
 
 class OpenTests:
     def test_open_binary(self):
         target = resources.files(self.data) / 'binary.file'
         with target.open('rb') as fp:
             result = fp.read()
             self.assertEqual(result, b'\x00\x01\x02\x03')
 
     def test_open_text_default_encoding(self):
         target = resources.files(self.data) / 'utf-8.file'
-        with target.open() as fp:
+        with target.open(encoding='utf-8') as fp:
             result = fp.read()
             self.assertEqual(result, 'Hello, UTF-8 world!\n')
 
     def test_open_text_given_encoding(self):
         target = resources.files(self.data) / 'utf-16.file'
         with target.open(encoding='utf-16', errors='strict') as fp:
             result = fp.read()
         self.assertEqual(result, 'Hello, UTF-16 world!\n')
 
     def test_open_text_with_errors(self):
-        # Raises UnicodeError without the 'errors' argument.
+        """
+        Raises UnicodeError without the 'errors' argument.
+        """
         target = resources.files(self.data) / 'utf-16.file'
         with target.open(encoding='utf-8', errors='strict') as fp:
             self.assertRaises(UnicodeError, fp.read)
         with target.open(encoding='utf-8', errors='ignore') as fp:
             result = fp.read()
         self.assertEqual(
             result,
             'H\x00e\x00l\x00l\x00o\x00,\x00 '
             '\x00U\x00T\x00F\x00-\x001\x006\x00 '
             '\x00w\x00o\x00r\x00l\x00d\x00!\x00\n\x00',
         )
 
     def test_open_binary_FileNotFoundError(self):
         target = resources.files(self.data) / 'does-not-exist'
-        self.assertRaises(FileNotFoundError, target.open, 'rb')
+        with self.assertRaises(FileNotFoundError):
+            target.open('rb')
 
     def test_open_text_FileNotFoundError(self):
         target = resources.files(self.data) / 'does-not-exist'
-        self.assertRaises(FileNotFoundError, target.open)
+        with self.assertRaises(FileNotFoundError):
+            target.open(encoding='utf-8')
 
 
 class OpenDiskTests(OpenTests, unittest.TestCase):
     def setUp(self):
         self.data = data01
```

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/test_path.py` & `importlib_resources-6.0.0/importlib_resources/tests/test_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,20 @@
     def execute(self, package, path):
         with resources.as_file(resources.files(package).joinpath(path)):
             pass
 
 
 class PathTests:
     def test_reading(self):
-        # Path should be readable.
-        # Test also implicitly verifies the returned object is a pathlib.Path
-        # instance.
+        """
+        Path should be readable.
+
+        Test also implicitly verifies the returned object is a pathlib.Path
+        instance.
+        """
         target = resources.files(self.data) / 'utf-8.file'
         with resources.as_file(target) as path:
             self.assertTrue(path.name.endswith("utf-8.file"), repr(path))
             # pathlib.Path.read_text() was introduced in Python 3.5.
             with path.open('r', encoding='utf-8') as file:
                 text = file.read()
             self.assertEqual('Hello, UTF-8 world!\n', text)
@@ -49,16 +52,18 @@
         )
         self.data.__spec__.origin = None
         self.data.__spec__.has_location = False
 
 
 class PathZipTests(PathTests, util.ZipSetup, unittest.TestCase):
     def test_remove_in_context_manager(self):
-        # It is not an error if the file that was temporarily stashed on the
-        # file system is removed inside the `with` stanza.
+        """
+        It is not an error if the file that was temporarily stashed on the
+        file system is removed inside the `with` stanza.
+        """
         target = resources.files(self.data) / 'utf-8.file'
         with resources.as_file(target) as path:
             path.unlink()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/test_read.py` & `importlib_resources-6.0.0/importlib_resources/tests/test_read.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,36 +9,42 @@
 class CommonBinaryTests(util.CommonTests, unittest.TestCase):
     def execute(self, package, path):
         resources.files(package).joinpath(path).read_bytes()
 
 
 class CommonTextTests(util.CommonTests, unittest.TestCase):
     def execute(self, package, path):
-        resources.files(package).joinpath(path).read_text()
+        resources.files(package).joinpath(path).read_text(encoding='utf-8')
 
 
 class ReadTests:
     def test_read_bytes(self):
         result = resources.files(self.data).joinpath('binary.file').read_bytes()
         self.assertEqual(result, b'\0\1\2\3')
 
     def test_read_text_default_encoding(self):
-        result = resources.files(self.data).joinpath('utf-8.file').read_text()
+        result = (
+            resources.files(self.data)
+            .joinpath('utf-8.file')
+            .read_text(encoding='utf-8')
+        )
         self.assertEqual(result, 'Hello, UTF-8 world!\n')
 
     def test_read_text_given_encoding(self):
         result = (
             resources.files(self.data)
             .joinpath('utf-16.file')
             .read_text(encoding='utf-16')
         )
         self.assertEqual(result, 'Hello, UTF-16 world!\n')
 
     def test_read_text_with_errors(self):
-        # Raises UnicodeError without the 'errors' argument.
+        """
+        Raises UnicodeError without the 'errors' argument.
+        """
         target = resources.files(self.data) / 'utf-16.file'
         self.assertRaises(UnicodeError, target.read_text, encoding='utf-8')
         result = target.read_text(encoding='utf-8', errors='ignore')
         self.assertEqual(
             result,
             'H\x00e\x00l\x00l\x00o\x00,\x00 '
             '\x00U\x00T\x00F\x00-\x001\x006\x00 '
```

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/test_reader.py` & `importlib_resources-6.0.0/importlib_resources/tests/test_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,14 +77,25 @@
         )
         self.assertEqual(path.joinpath(), path)
 
     def test_join_path_compound(self):
         path = MultiplexedPath(self.folder)
         assert not path.joinpath('imaginary/foo.py').exists()
 
+    def test_join_path_common_subdir(self):
+        prefix = os.path.abspath(os.path.join(__file__, '..'))
+        data01 = os.path.join(prefix, 'data01')
+        data02 = os.path.join(prefix, 'data02')
+        path = MultiplexedPath(data01, data02)
+        self.assertIsInstance(path.joinpath('subdirectory'), MultiplexedPath)
+        self.assertEqual(
+            str(path.joinpath('subdirectory', 'subsubdir'))[len(prefix) + 1 :],
+            os.path.join('data02', 'subdirectory', 'subsubdir'),
+        )
+
     def test_repr(self):
         self.assertEqual(
             repr(MultiplexedPath(self.folder)),
             f"MultiplexedPath('{self.folder}')",
         )
 
     def test_name(self):
```

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/test_resource.py` & `importlib_resources-6.0.0/importlib_resources/tests/test_resource.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import contextlib
 import sys
 import unittest
 import importlib_resources as resources
 import uuid
 import pathlib
 
 from . import data01
 from . import zipdata01, zipdata02
 from . import util
 from importlib import import_module
-from ._compat import import_helper, unlink
+from ._compat import import_helper, os_helper, unlink
 
 
 class ResourceTests:
     # Subclasses are expected to set the `data` attribute.
 
     def test_is_file_exists(self):
         target = resources.files(self.data) / 'binary.file'
@@ -65,18 +66,20 @@
             file=data01, path=data01.__file__, contents=['A', 'B', 'C', 'D/E', 'D/F']
         )
         self.assertFalse(resources.files(package).joinpath('Z').is_file())
 
 
 class ResourceCornerCaseTests(unittest.TestCase):
     def test_package_has_no_reader_fallback(self):
-        # Test odd ball packages which:
+        """
+        Test odd ball packages which:
         # 1. Do not have a ResourceReader as a loader
         # 2. Are not on the file system
         # 3. Are not in a zip file
+        """
         module = util.create_package(
             file=data01, path=data01.__file__, contents=['A', 'B', 'C']
         )
         # Give the module a dummy loader.
         module.__loader__ = object()
         # Give the module a dummy origin.
         module.__file__ = '/path/which/shall/not/be/named'
@@ -134,90 +137,79 @@
         )
         self.assertEqual(
             names(resources.files('ziptestdata.two')),
             {'__init__.py', 'resource2.txt'},
         )
 
 
+@contextlib.contextmanager
+def zip_on_path(dir):
+    data_path = pathlib.Path(zipdata01.__file__)
+    source_zip_path = data_path.parent.joinpath('ziptestdata.zip')
+    zip_path = pathlib.Path(dir) / f'{uuid.uuid4()}.zip'
+    zip_path.write_bytes(source_zip_path.read_bytes())
+    sys.path.append(str(zip_path))
+    import_module('ziptestdata')
+
+    try:
+        yield
+    finally:
+        with contextlib.suppress(ValueError):
+            sys.path.remove(str(zip_path))
+
+        with contextlib.suppress(KeyError):
+            del sys.path_importer_cache[str(zip_path)]
+            del sys.modules['ziptestdata']
+
+        with contextlib.suppress(OSError):
+            unlink(zip_path)
+
+
 class DeletingZipsTest(unittest.TestCase):
     """Having accessed resources in a zip file should not keep an open
     reference to the zip.
     """
 
-    ZIP_MODULE = zipdata01
-
     def setUp(self):
+        self.fixtures = contextlib.ExitStack()
+        self.addCleanup(self.fixtures.close)
+
         modules = import_helper.modules_setup()
         self.addCleanup(import_helper.modules_cleanup, *modules)
 
-        data_path = pathlib.Path(self.ZIP_MODULE.__file__)
-        data_dir = data_path.parent
-        self.source_zip_path = data_dir / 'ziptestdata.zip'
-        self.zip_path = pathlib.Path(f'{uuid.uuid4()}.zip').absolute()
-        self.zip_path.write_bytes(self.source_zip_path.read_bytes())
-        sys.path.append(str(self.zip_path))
-        self.data = import_module('ziptestdata')
-
-    def tearDown(self):
-        try:
-            sys.path.remove(str(self.zip_path))
-        except ValueError:
-            pass
-
-        try:
-            del sys.path_importer_cache[str(self.zip_path)]
-            del sys.modules[self.data.__name__]
-        except KeyError:
-            pass
-
-        try:
-            unlink(self.zip_path)
-        except OSError:
-            # If the test fails, this will probably fail too
-            pass
+        temp_dir = self.fixtures.enter_context(os_helper.temp_dir())
+        self.fixtures.enter_context(zip_on_path(temp_dir))
 
     def test_iterdir_does_not_keep_open(self):
-        c = [item.name for item in resources.files('ziptestdata').iterdir()]
-        self.zip_path.unlink()
-        del c
+        [item.name for item in resources.files('ziptestdata').iterdir()]
 
     def test_is_file_does_not_keep_open(self):
-        c = resources.files('ziptestdata').joinpath('binary.file').is_file()
-        self.zip_path.unlink()
-        del c
+        resources.files('ziptestdata').joinpath('binary.file').is_file()
 
     def test_is_file_failure_does_not_keep_open(self):
-        c = resources.files('ziptestdata').joinpath('not-present').is_file()
-        self.zip_path.unlink()
-        del c
+        resources.files('ziptestdata').joinpath('not-present').is_file()
 
     @unittest.skip("Desired but not supported.")
     def test_as_file_does_not_keep_open(self):  # pragma: no cover
-        c = resources.as_file(resources.files('ziptestdata') / 'binary.file')
-        self.zip_path.unlink()
-        del c
+        resources.as_file(resources.files('ziptestdata') / 'binary.file')
 
     def test_entered_path_does_not_keep_open(self):
-        # This is what certifi does on import to make its bundle
-        # available for the process duration.
-        c = resources.as_file(
-            resources.files('ziptestdata') / 'binary.file'
-        ).__enter__()
-        self.zip_path.unlink()
-        del c
+        """
+        Mimic what certifi does on import to make its bundle
+        available for the process duration.
+        """
+        resources.as_file(resources.files('ziptestdata') / 'binary.file').__enter__()
 
     def test_read_binary_does_not_keep_open(self):
-        c = resources.files('ziptestdata').joinpath('binary.file').read_bytes()
-        self.zip_path.unlink()
-        del c
+        resources.files('ziptestdata').joinpath('binary.file').read_bytes()
 
     def test_read_text_does_not_keep_open(self):
-        c = resources.files('ziptestdata').joinpath('utf-8.file').read_text()
-        self.zip_path.unlink()
-        del c
+        resources.files('ziptestdata').joinpath('utf-8.file').read_text(
+            encoding='utf-8'
+        )
 
 
 class ResourceFromNamespaceTest01(unittest.TestCase):
     site_dir = str(pathlib.Path(__file__).parent)
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/update-zips.py` & `importlib_resources-6.0.0/importlib_resources/tests/update-zips.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/util.py` & `importlib_resources-6.0.0/importlib_resources/tests/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 import importlib
 import io
 import sys
 import types
-from pathlib import Path, PurePath
+import pathlib
 
 from . import data01
 from . import zipdata01
 from ..abc import ResourceReader
 from ._compat import import_helper
 
 
@@ -76,51 +76,52 @@
     def execute(self, package, path):
         """
         Call the pertinent legacy API function (e.g. open_text, path)
         on package and path.
         """
 
     def test_package_name(self):
-        # Passing in the package name should succeed.
+        """
+        Passing in the package name should succeed.
+        """
         self.execute(data01.__name__, 'utf-8.file')
 
     def test_package_object(self):
-        # Passing in the package itself should succeed.
+        """
+        Passing in the package itself should succeed.
+        """
         self.execute(data01, 'utf-8.file')
 
     def test_string_path(self):
-        # Passing in a string for the path should succeed.
+        """
+        Passing in a string for the path should succeed.
+        """
         path = 'utf-8.file'
         self.execute(data01, path)
 
     def test_pathlib_path(self):
-        # Passing in a pathlib.PurePath object for the path should succeed.
-        path = PurePath('utf-8.file')
+        """
+        Passing in a pathlib.PurePath object for the path should succeed.
+        """
+        path = pathlib.PurePath('utf-8.file')
         self.execute(data01, path)
 
     def test_importing_module_as_side_effect(self):
-        # The anchor package can already be imported.
+        """
+        The anchor package can already be imported.
+        """
         del sys.modules[data01.__name__]
         self.execute(data01.__name__, 'utf-8.file')
 
-    def test_non_package_by_name(self):
-        # The anchor package cannot be a module.
-        with self.assertRaises(TypeError):
-            self.execute(__name__, 'utf-8.file')
-
-    def test_non_package_by_package(self):
-        # The anchor package cannot be a module.
-        with self.assertRaises(TypeError):
-            module = sys.modules['importlib_resources.tests.util']
-            self.execute(module, 'utf-8.file')
-
     def test_missing_path(self):
-        # Attempting to open or read or request the path for a
-        # non-existent path should succeed if open_resource
-        # can return a viable data stream.
+        """
+        Attempting to open or read or request the path for a
+        non-existent path should succeed if open_resource
+        can return a viable data stream.
+        """
         bytes_data = io.BytesIO(b'Hello, world!')
         package = create_package(file=bytes_data, path=FileNotFoundError())
         self.execute(package, 'utf-8.file')
         self.assertEqual(package.__loader__._path, 'utf-8.file')
 
     def test_extant_path(self):
         # Attempting to open or read or request the path when the
@@ -140,15 +141,15 @@
 
 
 class ZipSetupBase:
     ZIP_MODULE = None
 
     @classmethod
     def setUpClass(cls):
-        data_path = Path(cls.ZIP_MODULE.__file__)
+        data_path = pathlib.Path(cls.ZIP_MODULE.__file__)
         data_dir = data_path.parent
         cls._zip_path = str(data_dir / 'ziptestdata.zip')
         sys.path.append(cls._zip_path)
         cls.data = importlib.import_module('ziptestdata')
 
     @classmethod
     def tearDownClass(cls):
```

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/zipdata01/ziptestdata.zip` & `importlib_resources-6.0.0/importlib_resources/tests/zipdata01/ziptestdata.zip`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.9.0/importlib_resources/tests/zipdata02/ziptestdata.zip` & `importlib_resources-6.0.0/importlib_resources/tests/zipdata02/ziptestdata.zip`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.9.0/importlib_resources.egg-info/PKG-INFO` & `importlib_resources-6.0.0/importlib_resources.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: importlib-resources
-Version: 5.9.0
+Version: 6.0.0
 Summary: Read resources from Python packages
 Home-page: https://github.com/python/importlib_resources
 Author: Barry Warsaw
 Author-email: barry@python.org
 Project-URL: Documentation, https://importlib-resources.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/importlib_resources.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/importlib_resources
 
 .. image:: https://img.shields.io/pypi/pyversions/importlib_resources.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/importlib_resources
 
 .. image:: https://github.com/python/importlib_resources/workflows/tests/badge.svg
    :target: https://github.com/python/importlib_resources/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/importlib-resources/badge/?version=latest
    :target: https://importlib-resources.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/importlib-resources
    :target: https://tidelift.com/subscription/pkg/pypi-importlib-resources?utm_source=pypi-importlib-resources&utm_medium=readme
 
 ``importlib_resources`` is a backport of Python standard library
 `importlib.resources
@@ -60,15 +61,17 @@
 were contributed to different versions in the standard library:
 
 .. list-table::
    :header-rows: 1
 
    * - importlib_resources
      - stdlib
-   * - 5.8
+   * - 6.0
+     - 3.13
+   * - 5.12
      - 3.12
    * - 5.7
      - 3.11
    * - 5.0
      - 3.10
    * - 1.3
      - 3.9
```

### Comparing `importlib_resources-5.9.0/importlib_resources.egg-info/SOURCES.txt` & `importlib_resources-6.0.0/importlib_resources.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 .coveragerc
 .editorconfig
-.flake8
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
 codecov.yml
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 docs/migration.rst
 docs/using.rst
 importlib_resources/__init__.py
 importlib_resources/_adapters.py
 importlib_resources/_common.py
 importlib_resources/_compat.py
 importlib_resources/_itertools.py
-importlib_resources/_legacy.py
 importlib_resources/abc.py
 importlib_resources/py.typed
 importlib_resources/readers.py
 importlib_resources/simple.py
 importlib_resources.egg-info/PKG-INFO
 importlib_resources.egg-info/SOURCES.txt
 importlib_resources.egg-info/dependency_links.txt
 importlib_resources.egg-info/requires.txt
 importlib_resources.egg-info/top_level.txt
 importlib_resources/tests/__init__.py
 importlib_resources/tests/_compat.py
+importlib_resources/tests/_path.py
 importlib_resources/tests/test_compatibilty_files.py
 importlib_resources/tests/test_contents.py
+importlib_resources/tests/test_custom.py
 importlib_resources/tests/test_files.py
 importlib_resources/tests/test_open.py
 importlib_resources/tests/test_path.py
 importlib_resources/tests/test_read.py
 importlib_resources/tests/test_reader.py
 importlib_resources/tests/test_resource.py
 importlib_resources/tests/update-zips.py
@@ -54,14 +55,15 @@
 importlib_resources/tests/data01/utf-16.file
 importlib_resources/tests/data01/utf-8.file
 importlib_resources/tests/data01/subdirectory/__init__.py
 importlib_resources/tests/data01/subdirectory/binary.file
 importlib_resources/tests/data02/__init__.py
 importlib_resources/tests/data02/one/__init__.py
 importlib_resources/tests/data02/one/resource1.txt
+importlib_resources/tests/data02/subdirectory/subsubdir/resource.txt
 importlib_resources/tests/data02/two/__init__.py
 importlib_resources/tests/data02/two/resource2.txt
 importlib_resources/tests/namespacedata01/binary.file
 importlib_resources/tests/namespacedata01/utf-16.file
 importlib_resources/tests/namespacedata01/utf-8.file
 importlib_resources/tests/zipdata01/__init__.py
 importlib_resources/tests/zipdata01/ziptestdata.zip
```

### Comparing `importlib_resources-5.9.0/setup.cfg` & `importlib_resources-6.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -13,39 +13,42 @@
 	Programming Language :: Python :: 3 :: Only
 project_urls = 
 	Documentation = https://importlib-resources.readthedocs.io/
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	zipp >= 3.1.0; python_version < '3.10'
 
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
-	pytest-flake8
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
+	pytest-ruff
 docs = 
-	sphinx
-	jaraco.packaging >= 9
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
+	
 	jaraco.tidelift >= 1.4
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `importlib_resources-5.9.0/tox.ini` & `importlib_resources-6.0.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
+setenv =
+	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
-extras = testing
+extras =
+	testing
 
 [testenv:docs]
 extras =
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
+	python -m sphinxlint
 
 [testenv:diffcov]
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


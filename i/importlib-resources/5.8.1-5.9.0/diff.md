# Comparing `tmp/importlib_resources-5.8.1.tar.gz` & `tmp/importlib_resources-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_resources-5.8.1.tar", last modified: Fri Jul 22 16:23:25 2022, max compression
+gzip compressed data, was "importlib_resources-5.9.0.tar", last modified: Fri Jul 22 16:46:53 2022, max compression
```

## Comparing `importlib_resources-5.8.1.tar` & `importlib_resources-5.9.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.897757 importlib_resources-5.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.897757 importlib_resources-5.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8983 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.897757 importlib_resources-5.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5906 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/docs/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/readers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/data01/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data01/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data01/binary.file
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/data01/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data01/subdirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data01/subdirectory/binary.file
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data01/utf-16.file
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data01/utf-8.file
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/data02/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data02/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/data02/one/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data02/one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data02/one/resource1.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/data02/two/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data02/two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/data02/two/resource2.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/namespacedata01/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/namespacedata01/binary.file
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/namespacedata01/utf-16.file
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/namespacedata01/utf-8.file
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/test_compatibilty_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8145 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/test_resource.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1417 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/update-zips.py
--rw-r--r--   0 runner    (1001) docker     (121)     5309 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/zipdata01/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/zipdata01/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/zipdata01/ziptestdata.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources/tests/zipdata02/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/zipdata02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/importlib_resources/tests/zipdata02/ziptestdata.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:23:25.901757 importlib_resources-5.8.1/importlib_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-07-22 16:23:25.000000 importlib_resources-5.8.1/importlib_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-07-22 16:23:25.000000 importlib_resources-5.8.1/importlib_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 16:23:25.000000 importlib_resources-5.8.1/importlib_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-07-22 16:23:25.000000 importlib_resources-5.8.1/importlib_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:23:25.000000 importlib_resources-5.8.1/importlib_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-07-22 16:23:25.905757 importlib_resources-5.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-07-22 16:23:01.000000 importlib_resources-5.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.761731 importlib_resources-5.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.761731 importlib_resources-5.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     9150 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5906 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/docs/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/importlib_resources/
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4202 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5128 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/readers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/importlib_resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/importlib_resources/tests/data01/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/binary.file
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/data01/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/subdirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/subdirectory/binary.file
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/utf-16.file
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data01/utf-8.file
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/data02/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/data02/one/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/one/resource1.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/data02/two/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/data02/two/resource2.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/namespacedata01/
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/namespacedata01/binary.file
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/namespacedata01/utf-16.file
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/namespacedata01/utf-8.file
+-rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_compatibilty_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/test_resource.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1417 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/update-zips.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5309 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/zipdata01/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/zipdata01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/zipdata01/ziptestdata.zip
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/importlib_resources/tests/zipdata02/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/zipdata02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/importlib_resources/tests/zipdata02/ziptestdata.zip
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:46:53.765731 importlib_resources-5.9.0/importlib_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-22 16:46:53.000000 importlib_resources-5.9.0/importlib_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-07-22 16:46:53.769731 importlib_resources-5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-07-22 16:46:22.000000 importlib_resources-5.9.0/tox.ini
```

### Comparing `importlib_resources-5.8.1/.github/workflows/main.yml` & `importlib_resources-5.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/.gitignore` & `importlib_resources-5.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/CHANGES.rst` & `importlib_resources-5.9.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v5.9.0
+======
+
+* #228: ``as_file`` now also supports a ``Traversable``
+  representing a directory and (when needed) renders the
+  full tree to a temporary directory.
+
 v5.8.1
 ======
 
 * #253: In ``MultiplexedPath``, restore expectation that
   a compound path with a non-existent directory does not
   raise an exception.
```

### Comparing `importlib_resources-5.8.1/LICENSE` & `importlib_resources-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/PKG-INFO` & `importlib_resources-5.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_resources
-Version: 5.8.1
+Version: 5.9.0
 Summary: Read resources from Python packages
 Home-page: https://github.com/python/importlib_resources
 Author: Barry Warsaw
 Author-email: barry@python.org
 Project-URL: Documentation, https://importlib-resources.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `importlib_resources-5.8.1/README.rst` & `importlib_resources-5.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/docs/conf.py` & `importlib_resources-5.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/docs/index.rst` & `importlib_resources-5.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/docs/migration.rst` & `importlib_resources-5.9.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/docs/using.rst` & `importlib_resources-5.9.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/__init__.py` & `importlib_resources-5.9.0/importlib_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/_adapters.py` & `importlib_resources-5.9.0/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/_compat.py` & `importlib_resources-5.9.0/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/_itertools.py` & `importlib_resources-5.9.0/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/_legacy.py` & `importlib_resources-5.9.0/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/abc.py` & `importlib_resources-5.9.0/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/readers.py` & `importlib_resources-5.9.0/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/simple.py` & `importlib_resources-5.9.0/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/test_compatibilty_files.py` & `importlib_resources-5.9.0/importlib_resources/tests/test_compatibilty_files.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/test_contents.py` & `importlib_resources-5.9.0/importlib_resources/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/test_files.py` & `importlib_resources-5.9.0/importlib_resources/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/test_open.py` & `importlib_resources-5.9.0/importlib_resources/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/test_path.py` & `importlib_resources-5.9.0/importlib_resources/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/test_read.py` & `importlib_resources-5.9.0/importlib_resources/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/test_reader.py` & `importlib_resources-5.9.0/importlib_resources/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/test_resource.py` & `importlib_resources-5.9.0/importlib_resources/tests/test_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,22 @@
 
     def test_submodule_contents_by_name(self):
         self.assertEqual(
             names(resources.files('ziptestdata.subdirectory')),
             {'__init__.py', 'binary.file'},
         )
 
+    def test_as_file_directory(self):
+        with resources.as_file(resources.files('ziptestdata')) as data:
+            assert data.name == 'ziptestdata'
+            assert data.is_dir()
+            assert data.joinpath('subdirectory').is_dir()
+            assert len(list(data.iterdir()))
+        assert not data.parent.exists()
+
 
 class ResourceFromZipsTest02(util.ZipSetupBase, unittest.TestCase):
     ZIP_MODULE = zipdata02  # type: ignore
 
     def test_unrelated_contents(self):
         """
         Test thata zip with two unrelated subpackages return
```

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/update-zips.py` & `importlib_resources-5.9.0/importlib_resources/tests/update-zips.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/util.py` & `importlib_resources-5.9.0/importlib_resources/tests/util.py`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/zipdata01/ziptestdata.zip` & `importlib_resources-5.9.0/importlib_resources/tests/zipdata01/ziptestdata.zip`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources/tests/zipdata02/ziptestdata.zip` & `importlib_resources-5.9.0/importlib_resources/tests/zipdata02/ziptestdata.zip`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/importlib_resources.egg-info/PKG-INFO` & `importlib_resources-5.9.0/importlib_resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-resources
-Version: 5.8.1
+Version: 5.9.0
 Summary: Read resources from Python packages
 Home-page: https://github.com/python/importlib_resources
 Author: Barry Warsaw
 Author-email: barry@python.org
 Project-URL: Documentation, https://importlib-resources.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `importlib_resources-5.8.1/importlib_resources.egg-info/SOURCES.txt` & `importlib_resources-5.9.0/importlib_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/pytest.ini` & `importlib_resources-5.9.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/setup.cfg` & `importlib_resources-5.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_resources-5.8.1/tox.ini` & `importlib_resources-5.9.0/tox.ini`

 * *Files identical despite different names*


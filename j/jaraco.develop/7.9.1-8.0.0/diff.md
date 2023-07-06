# Comparing `tmp/jaraco.develop-7.9.1.tar.gz` & `tmp/jaraco.develop-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.develop-7.9.1.tar", last modified: Wed Mar 23 13:56:17 2022, max compression
+gzip compressed data, was "jaraco.develop-8.0.0.tar", last modified: Thu Jul  6 22:28:16 2023, max compression
```

## Comparing `jaraco.develop-7.9.1.tar` & `jaraco.develop-8.0.0.tar`

### file list

```diff
@@ -1,46 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.347970 jaraco.develop-7.9.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.347970 jaraco.develop-7.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.347970 jaraco.develop-7.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.347970 jaraco.develop-7.9.1/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/jaraco/develop/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/add-github-secret.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/add-github-secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/create-github-release.py
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/github.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/indent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/init-azure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/macos-build-python.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/print-meta.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/pypi.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/remove-namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/jaraco/develop/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/jaraco.develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-03-23 13:56:16.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-03-23 13:56:17.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 13:56:16.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-03-23 13:56:17.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-23 13:56:17.000000 jaraco.develop-7.9.1/jaraco.develop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-23 13:56:17.351970 jaraco.develop-7.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/todo.txt
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-03-23 13:55:55.000000 jaraco.develop-7.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.254268 jaraco.develop-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.242268 jaraco.develop-8.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.242268 jaraco.develop-8.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 22:28:16.254268 jaraco.develop-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.242268 jaraco.develop-8.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.238268 jaraco.develop-8.0.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.254268 jaraco.develop-8.0.0/jaraco/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/add-github-secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/add-github-secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/checkout-all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/create-github-release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/init-azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/macos-build-python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/print-meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/rst-header-replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/rtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/towncrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/jaraco/develop/update-projects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:28:16.242268 jaraco.develop-8.0.0/jaraco.develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 22:28:16.000000 jaraco.develop-8.0.0/jaraco.develop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-06 22:28:16.258268 jaraco.develop-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/todo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-06 22:27:53.000000 jaraco.develop-8.0.0/tox.ini
```

### Comparing `jaraco.develop-7.9.1/CHANGES.rst` & `jaraco.develop-8.0.0/NEWS.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,136 @@
+v8.0.0
+======
+
+Deprecations and Removals
+-------------------------
+
+- Replace ``pep517`` with ``build``. ``repo.get_project_metadata`` no longer includes the ``dist``.
+
+
+v7.25.0
+=======
+
+Features
+--------
+
+- Added counter to update-projects.
+
+
+v7.24.0
+=======
+
+Features
+--------
+
+- Add optional branch parameter to update-projects.
+
+
+v7.23.0
+=======
+
+Features
+--------
+
+- Add ``finalize`` command.
+- Require Python 3.8 or later.
+
+
+v7.22.1
+=======
+
+* Fixed bug in argument handling of ``towncrier``.
+
+v7.22.0
+=======
+
+* Added ``rst-header-replace`` script.
+
+v7.21.0
+=======
+
+* Added ``towncrier.check_changes`` from ``setuptools``'
+  ``finalize``.
+
+v7.20.0
+=======
+
+* Added ``towncrier`` module for invoking towncrier with
+  a version calculated based on towncrier news fragments
+  in service of jaraco/skeleton#83.
+
+v7.19.0
+=======
+
+* Replaced the "skeleton" merge resolver with a "project"
+  merge resolver, based on the changes planned for
+  jaraco/skeleton#70.
+
+v7.18.0
+=======
+
+* ``update-projects`` now accepts a ``tag`` argument.
+* ``update-projects`` now allows overriding the base from
+  which to update.
+
+v7.17.0
+=======
+
+* ``update-projects`` now accepts keyword arguments.
+* Added another conflict resolver to ``merge`` module.
+
+v7.16.1
+=======
+
+* Actually add the merge module, missed in prior release.
+
+v7.16.0
+=======
+
+* Added 'merge' tool toward automatically resolving skeleton changes.
+
+v7.15.0
+=======
+
+* Projects are now loaded from ``PROJECTS_LIST_URL`` instead of
+  from am embedded text file.
+
+v7.14.0
+=======
+
+* ``update-projects`` no longer prompts to edit the commit message.
+
+v7.13.1
+=======
+
+* Declare requirement on Python 3.9.
+* Fixed test failures in CI.
+
+v7.13.0
+=======
+
+* Added performance optimizations on ``update-projects``.
+
+v7.12.0
+=======
+
+* "checkout all" script now checks out more projects and lays them
+  out according to organization.
+* Require Python 3.9 or later.
+
+v7.11.0
+=======
+
+* Added ``checkout-all`` script.
+
+v7.10.0
+=======
+
+* Added ``update-projects`` script.
+
 v7.9.1
 ======
 
 * bpo-46975: Fix error in LDFLAGS building Python on macOS.
 
 v7.9.0
 ======
```

### Comparing `jaraco.develop-7.9.1/LICENSE` & `jaraco.develop-8.0.0/LICENSE`

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

### Comparing `jaraco.develop-7.9.1/PKG-INFO` & `jaraco.develop-8.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.develop
-Version: 7.9.1
+Version: 8.0.0
 Summary: Development utilities by jaraco
 Home-page: https://github.com/jaraco/jaraco.develop
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.develop.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.develop
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.develop.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.develop
 
 .. image:: https://github.com/jaraco/jaraco.develop/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.develop/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracodevelop/badge/?version=latest
    :target: https://jaracodevelop.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
-
-
```

### Comparing `jaraco.develop-7.9.1/README.rst` & `jaraco.develop-8.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.develop.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.develop
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.develop.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.develop
 
 .. image:: https://github.com/jaraco/jaraco.develop/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.develop/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracodevelop/badge/?version=latest
    :target: https://jaracodevelop.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.develop-7.9.1/jaraco/develop/add-github-secrets.py` & `jaraco.develop-8.0.0/jaraco/develop/add-github-secrets.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.1/jaraco/develop/compiler.py` & `jaraco.develop-8.0.0/jaraco/develop/compiler.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.1/jaraco/develop/github.py` & `jaraco.develop-8.0.0/jaraco/develop/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
             Authorization=f'token {cls.load_token()}',
         )
         return session
 
     @staticmethod
     def load_token():
         token = os.environ.get("GITHUB_TOKEN") or keyring.get_password(
-            'Github', getpass.getuser()
+            'Github',
+            username(),
         )
         assert token, "Token not available"
         return token
 
     @classmethod
     def detect(cls):
         return cls(repo.get_project_metadata().project)
@@ -84,9 +85,15 @@
         all = itertools.chain.from_iterable(map(cls.find_secrets, workflows))
         return itertools.filterfalse('GITHUB_TOKEN'.__eq__, all)
 
     @staticmethod
     def find_secrets(file):
         return (
             match.group(1)
-            for match in re.finditer(r'\${{\s*secrets\.(\w+)\s*}}', file.read_text())
+            for match in re.finditer(
+                r'\${{\s*secrets\.(\w+)\s*}}', file.read_text(encoding='utf-8')
+            )
         )
+
+
+def username():
+    return os.environ.get('GITHUB_USERNAME') or getpass.getuser()
```

### Comparing `jaraco.develop-7.9.1/jaraco/develop/indent.py` & `jaraco.develop-8.0.0/jaraco/develop/indent.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.1/jaraco/develop/init-azure.py` & `jaraco.develop-8.0.0/jaraco/develop/init-azure.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.1/jaraco/develop/macos-build-python.py` & `jaraco.develop-8.0.0/jaraco/develop/macos-build-python.py`

 * *Files identical despite different names*

### Comparing `jaraco.develop-7.9.1/jaraco.develop.egg-info/PKG-INFO` & `jaraco.develop-8.0.0/jaraco.develop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.develop
-Version: 7.9.1
+Version: 8.0.0
 Summary: Development utilities by jaraco
 Home-page: https://github.com/jaraco/jaraco.develop
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.develop.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.develop
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.develop.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.develop
 
 .. image:: https://github.com/jaraco/jaraco.develop/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.develop/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracodevelop/badge/?version=latest
    :target: https://jaracodevelop.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
-
-
```

### Comparing `jaraco.develop-7.9.1/setup.cfg` & `jaraco.develop-8.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -11,49 +11,56 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.9
 install_requires = 
 	jaraco.ui
 	jaraco.context
 	jaraco.collections
 	keyring
 	autocommand
 	requests-toolbelt
 	PyNaCl
 	packaging
-	pep517
 	setuptools
+	path
+	jaraco.vcs >= 1.1
+	build
 
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
-	pytest-enabler >= 1.0.1
+	pytest-enabler >= 2.2
+	pytest-ruff
+	
+	pytest-subprocess
+	types-requests
 docs = 
-	sphinx
+	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `jaraco.develop-7.9.1/tox.ini` & `jaraco.develop-8.0.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,41 @@
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
+	# required for github.username()
+	GITHUB_USERNAME = jaraco
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
+
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
 
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
```


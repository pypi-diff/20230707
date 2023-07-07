# Comparing `tmp/trackteroid-0.1.0rc4.tar.gz` & `tmp/trackteroid-0.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackteroid-0.1.0rc4.tar", last modified: Fri Jun 30 12:16:16 2023, max compression
+gzip compressed data, was "trackteroid-0.1.0rc5.tar", last modified: Fri Jul  7 11:18:00 2023, max compression
```

## Comparing `trackteroid-0.1.0rc4.tar` & `trackteroid-0.1.0rc5.tar`

### file list

```diff
@@ -1,80 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/issue--bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/issue--feature-request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.graphics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/.graphics/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.graphics/svg/logo_black.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.graphics/svg/logo_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/sphinx_source/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/sphinx_source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   170890 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/_static/logo_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/sphinx_source/collections/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections/emptycollection.md
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections/entitycollection.md
--rw-r--r--   0 runner    (1001) docker     (123)    26744 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/collections.md
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/entity.md
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/doc/sphinx_source/query/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/query/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/query/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/query.md
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/doc/sphinx_source/session.md
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.620515 trackteroid-0.1.0rc4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/src/trackteroid/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/src/trackteroid/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71990 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/declarations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/declarations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    31930 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/entities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   171659 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/entities.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/relationships_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/entities/schematypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/src/trackteroid/query/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/criteria.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/src/trackteroid/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/src/trackteroid/stubs/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.624515 trackteroid-0.1.0rc4/src/trackteroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 12:16:16.000000 trackteroid-0.1.0rc4/src/trackteroid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:16:16.628515 trackteroid-0.1.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/tests/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-30 12:16:04.000000 trackteroid-0.1.0rc4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.683743 trackteroid-0.1.0rc5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.671743 trackteroid-0.1.0rc5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.671743 trackteroid-0.1.0rc5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/.github/ISSUE_TEMPLATE/issue--bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/.github/ISSUE_TEMPLATE/issue--feature-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.671743 trackteroid-0.1.0rc5/.graphics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/.graphics/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/.graphics/svg/logo_black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/.graphics/svg/logo_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-07-07 11:18:00.683743 trackteroid-0.1.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/doc/sphinx_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/doc/sphinx_source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   170890 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/_static/logo_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/doc/sphinx_source/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/collections/emptycollection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/collections/entitycollection.md
+-rw-r--r--   0 runner    (1001) docker     (123)    27268 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/collections/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/collections/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/entity.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/doc/sphinx_source/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/query/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/query/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/query.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/doc/sphinx_source/session/
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/session/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/doc/sphinx_source/session.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:18:00.683743 trackteroid-0.1.0rc5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.671743 trackteroid-0.1.0rc5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.675743 trackteroid-0.1.0rc5/src/trackteroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.679743 trackteroid-0.1.0rc5/src/trackteroid/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77117 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/entities/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/entities/declarations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/entities/declarations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    31930 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/entities/entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   171659 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/entities/entities.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/entities/relationships_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/entities/schematypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.679743 trackteroid-0.1.0rc5/src/trackteroid/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/query/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/query/criteria.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/query/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14814 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.679743 trackteroid-0.1.0rc5/src/trackteroid/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/src/trackteroid/stubs/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.679743 trackteroid-0.1.0rc5/src/trackteroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-07-07 11:18:00.000000 trackteroid-0.1.0rc5/src/trackteroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-07 11:18:00.000000 trackteroid-0.1.0rc5/src/trackteroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:18:00.000000 trackteroid-0.1.0rc5/src/trackteroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 11:18:00.000000 trackteroid-0.1.0rc5/src/trackteroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 11:18:00.000000 trackteroid-0.1.0rc5/src/trackteroid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.679743 trackteroid-0.1.0rc5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.671743 trackteroid-0.1.0rc5/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:18:00.683743 trackteroid-0.1.0rc5/tests/resources/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tests/resources/session/operations_linux.dbm
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tests/resources/session/operations_windows.dbm.bak
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tests/resources/session/operations_windows.dbm.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tests/resources/session/operations_windows.dbm.dir
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tests/test_authoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-07 11:17:45.000000 trackteroid-0.1.0rc5/tox.ini
```

### Comparing `trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/issue--bug-report.md` & `trackteroid-0.1.0rc5/.github/ISSUE_TEMPLATE/issue--bug-report.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/.github/ISSUE_TEMPLATE/issue--feature-request.md` & `trackteroid-0.1.0rc5/.github/ISSUE_TEMPLATE/issue--feature-request.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/.github/workflows/python-publish.yml` & `trackteroid-0.1.0rc5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/.graphics/svg/logo_black.svg` & `trackteroid-0.1.0rc5/.graphics/svg/logo_black.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/.graphics/svg/logo_white.svg` & `trackteroid-0.1.0rc5/.graphics/svg/logo_white.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/.readthedocs.yaml` & `trackteroid-0.1.0rc5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/LICENSE` & `trackteroid-0.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/PKG-INFO` & `trackteroid-0.1.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackteroid
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: Declarative, object-oriented wrapper for Ftrack queries. Powerful functional-style interactions with resulting collections.
 Author: Rico Koschmitzky, Dennis Weil
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Trixter
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `trackteroid-0.1.0rc4/README.md` & `trackteroid-0.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/Makefile` & `trackteroid-0.1.0rc5/doc/sphinx_source/Makefile`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/_static/favicon.ico` & `trackteroid-0.1.0rc5/doc/sphinx_source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/_static/logo_white.svg` & `trackteroid-0.1.0rc5/doc/sphinx_source/_static/logo_white.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/collections/emptycollection.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/collections/emptycollection.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 The concept of the `EmptyCollection` shares similarities with the [optional type](https://docs.oracle.com/javase/8/docs/api/java/util/Optional.html) found in various programming languages. It serves as a mechanism to handle the absence of values or empty results.
 
 Similar to optional types in other languages, the `EmptyCollection` provides a consistent interface and allows for operations and attribute access without the need for explicit checks for empty or null values. It acts as a container that represents the absence of a value or result.
 
 By utilizing the `EmptyCollection`, developers can write cleaner and more concise code by treating empty results as a valid state without the need for verbose conditional statements. This promotes a more functional programming style, allowing for seamless chaining and composition of operations even in scenarios where the result might be empty.
 
-Just as optional types in different programming languages offer methods or functions to check for presence (_isPresent()_) and provide fallback values (_orElse()_), the `EmptyCollection` provides a simple fallback functionality to handle cases where the collection is empty as it always evaluates to `False`.
+Just as optional types in different programming languages offer methods or functions to check for presence or provide fallback values , the `EmptyCollection` provides a simple fallback functionality to handle cases where the collection is empty as it always evaluates to `False`.
 
 This demonstrates how you can implement a straightforward fallback mechanism using the or operator when retrieving the final data.
 ```{include} collections/examples.md
 :start-after: example fallback1 start
 :end-before: example fallback1 end
 ```
```

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/collections/entitycollection.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/collections/entitycollection.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/collections/examples.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/collections/examples.md`

 * *Files 1% similar despite different names*

```diff
@@ -1041,8 +1041,30 @@
 
 print(
     typedcontext_collection[Folder],
     typedcontext_collection[AssetBuild]
 )
 # EntityCollection[Folder]{4} EntityCollection[AssetBuild]{17}
 ```
-example type filtering2 end
+example type filtering2 end
+
+example delete start
+```python
+from trackteroid import (
+    Query,
+    AssetVersion,
+    SESSION
+)
+
+_id = "405c569e-8bfa-11eb-ae63-c2ffbce28b68"
+
+Query(AssetVersion).by_id(_id).get_one().delete().commit()
+
+SESSION.reconnect()
+
+# will result in error as the entity doesn't exist anymore
+# ftrack_api.exception.NoResultFoundError: 
+# No result found for 'select id, asset.name, version from AssetVersion where (id is "405c569e-8bfa-11eb-ae63-c2ffbce28b68")'
+#
+Query(AssetVersion).by_id(_id).get_one()
+```
+example delete end
```

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/collections/overview.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/collections/overview.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/conf.py` & `trackteroid-0.1.0rc5/doc/sphinx_source/conf.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/configuration.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/configuration.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/index.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/index.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/installation.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/installation.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/make.bat` & `trackteroid-0.1.0rc5/doc/sphinx_source/make.bat`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/query/examples.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/query/examples.md`

 * *Files 4% similar despite different names*

```diff
@@ -124,17 +124,30 @@
 example limiting end
 
 example session start
 ```python
 from trackteroid import (
     AssetVersion,
     Query,
+    SCHEMA,
     SESSION,
 )
-from trackteroid.query import SCHEMA
 
 # same as Query(AssetVersion)
 Query(AssetVersion, session=SESSION, schema=SCHEMA.default)
 ```
 example session end
 
+example session2 start
+```python
+from trackteroid import (
+    Query,
+    AssetVersion,
+    SCHEMA
+)
+from trackteroid.session import Session
+
+session = Session()
 
+Query(AssetVersion, session=session)
+```
+example session2 end
```

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/query/overview.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/query/overview.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 To retrieve data from the Ftrack server, you need to perform queries using the `Query` class. This class serves as the entry point for accessing data and should be initialized with the desired entity type: `Query(<Entity Type>)`.
 
 In the previous example, we wanted to retrieve any `AssetVersion` but only fetched the first result from the server. Any `get_` prefixed method on the `Query` instance we do refer to as **terminators**. 
 These terminators are responsible for executing the resolved query instruction, sending it to the Ftrack server, and fetching the corresponding data. 
 
-The result is returned as a collection, specifically an instance of either EntityCollection or EmptyCollection, depending on the outcome. When printed, the collection is represented as:
+The result is returned as a collection, specifically an instance of either `EntityCollection` or `EmptyCollection`, depending on the outcome. When printed, the collection is represented as:
 
 `EntityCollection[<Entity Type>]{<Number of Results>}` or `EmptyCollection[<Entity Type>]`
 
 If you wish to preview the resolved query without sending it to the server, you can simply print the collection or call str on it.
 
 ```python
+from trackteroid import AssetVersion
+
 print(Query(AssetVersion))
 # output: select id, asset.name, version from AssetVersion
 ```
 
 #### Projections
 
 When accessing data from the resulting collection, it is important to _project_ (specify) the attributes that you will need to access later. 
@@ -25,48 +27,55 @@
 
 Looking back at the previous example, you can observe that the attributes _id_, _asset.name_, and _version_ were included in the resolved query instruction. 
 This was done because these attributes are commonly accessed and can be predefined for certain entity types.
 
 By projecting the necessary attributes in the query, you ensure that the resulting collection includes the specific data you require.
 
 ```python
+from trackteroid import AssetVersion
+
 print(AssetVersion.projections)
 # output: ['id', 'asset.name', 'version']
 ```
 In contrast to the Ftrack Python API, the default Session within Trackteroid disables the auto-population feature. This means that the Session will not automatically fetch missing data when accessing attributes on your collections. Instead, the data is fetched only for the attributes that were explicitly projected in the query.
-This behavior provides a more controlled and optimized approach to data retrieval. By avoiding unnecessary data fetching, disabled auto-population minimizes network requests and might improve performance significantly. 
+This behavior provides a more controlled and optimized approach to data retrieval. By avoiding unnecessary data fetching, disabled auto-population minimizes server requests and might improve performance significantly. 
 
 When working with Trackteroid, it is important to be aware of this behavior and ensure that you project all the attributes you need in your queries. 
 
 ```{include} query/examples.md
 :start-after: example projections1 start
 :end-before: example projections1 end
 ```
-When attempting to access the comment attribute without projecting it, the output contains `Symbol(NOT_SET)`, indicating that the data for the comment attribute was not fetched.
-However, by modifying the query to include the comment attribute in the projections list (projections=["comment"]) and accessing it, the output becomes [u'Hello World'], providing the retrieved value of the comment.
+When attempting to access the _comment_ attribute without projecting it, the output contains `Symbol(NOT_SET)`, indicating that the data for the comment attribute was not fetched.
+However, by modifying the query to include the _comment_ attribute in the projections list (projections=["comment"]) and accessing it, the output becomes [u'Hello World'], providing the retrieved value of the comment.
 
 ```python
+from trackteroid import (
+    Query,
+    AssetVersion
+)
+
 print(
     Query(AssetVersion).get_first(
         projections=["comment", "asset.parent.project.name"]
     ).asset.parent.project.name
 )
 # output: [u'DummyProject']
 ```
-Knowing these relationships and constructing written queries can be challenging, leading to long and complex queries. However, Trackteroid provides a shorter and easier alternative for many relationships
+Knowing these relationships and constructing written queries can be challenging, leading to long and complex queries. However, Trackteroid provides a shorter and easier alternative for many relationships.
 ```{include} query/examples.md
 :start-after: example projections shortcut start
 :end-before: example projections shortcut end
 ```
 
 This concise and intuitive approach simplifies querying and attribute retrieval for complex relationships.
 
 #### Filtering
 
-To ensure optimal performance and avoid fetching unnecessary data, it's recommended to narrow down the query results directly using Query criteria. Criteria methods in Trackteroid follow a `by_` and `not_by_` name prefix convention and can be chained together. While different entity types may have different criteria methods available, many share common ones.
+To ensure optimal performance and avoid fetching unnecessary data, it's recommended to narrow down the query results directly using `Query` criteria. Criteria methods in Trackteroid follow a `by_` and `not_by_` name prefix convention and can be chained together. While different entity types may have different criteria methods available, many share common ones.
 By utilizing criteria methods, you can specify filtering conditions directly in the query construction process, reducing the amount of data retrieved. This approach helps improve code performance and efficiency.
 
 ```{include} query/examples.md
 :start-after: example criteria1 start
 :end-before: example criteria1 end
 ```
 
@@ -78,15 +87,15 @@
 
 Frequently, criteria in the query mechanism involve searching for direct properties of an entity, such as _id_, _name_, or _metadata_. By default, those criteria are associated with the entity type specified in the Query, representing the desired results. However, criteria can also offer the flexibility to define a target, allowing you to specify the entity type for which you want to reference its property instead.
 ```{include} query/examples.md
 :start-after: example criteria target start
 :end-before: example criteria target end
 ```
 
-For criteria that support target specification, you have the option to provide exactly one target as the first positional argument. This target defines the relationship for the property used within the criterion.
+For criteria that support target specification, you have the option to provide **exactly one target as the first positional argument**. This target defines the relationship for the property used within the criterion.
 
 ### Limiting and Ordering
 
 The `get_all` terminator supports limiting and ordering results.
 
 ```{include} query/examples.md
 :start-after: example limiting start
```

### Comparing `trackteroid-0.1.0rc4/doc/sphinx_source/quickstart.md` & `trackteroid-0.1.0rc5/doc/sphinx_source/quickstart.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Quickstart
 
 Eager to get started? This page give some introduction to the core concepts of Trackteroid. 
 Follow [Installation](installation.md) and install Trackteroid first. Ideally you should also have a basic understanding of the [Ftrack Python API](https://ftrack-python-api.readthedocs.io/en/stable/index.html).
 
-The following examples assumes you have [configured the api access for Ftrack](https://ftrack-python-api.readthedocs.io/en/stable/understanding_sessions.html) accordingly.
+The provided examples assume that you have properly configured the [API access for Ftrack](https://ftrack-python-api.readthedocs.io/en/stable/understanding_sessions.html) accordingly.
 
 ## Accessing Data From FTrack
 
 ```{include} query/examples.md
 :start-after: example minimal start
 :end-before: example minimal end
 
@@ -21,32 +21,32 @@
 
 One of the main objectives of Trackteroid is to minimize the need for in-depth knowledge of the underlying database structure when working with queries and resulting collections. This goal is accomplished through two distinct approaches.
 
 Firstly, it automatically derives relationships whenever possible by dynamically inspecting the schema of the current session. This capability allows for seamless handling of relationships without requiring explicit configuration.
 
 However, Ftrack's dynamic nature means that certain entity types may require configuring relationships to align with specific requirements. Trackteroid provides the flexibility to describe and represent contextual relationships for such cases, enabling customization and adaptation to meet individual needs by implementing a [resolver](configuration.md#relationships-resolver).
 
-All communication with an Ftrack server is facilitated through a `Session` object. By default, a Query is constructed using the _SESSION_ singleton and the _default_ schema. Here's an example:
+All communication with an Ftrack server is facilitated through a `Session` object. By default, a `Query` is constructed using the [_SESSION_ singleton](session.md#multiple-sessions) and the _default_ schema. Here's an example:
 
 ```{include} query/examples.md
 :start-after: example session start
 :end-before: example session end
 ```
 
 However, you also have the flexibility to initialize your own `Session` object and provide a different schema. Here's an example:
 
 ```python
 from trackteroid import (
-    AssetVersion,
     Query,
-    SCHEMA
+    SCHEMA,
+    AssetVersion
 )
 from trackteroid.session import Session
 
-my_session = Session(server_url="<some_ftrack_server>")
+my_session = Session()
 
 Query(AssetVersion, session=my_session, schema=SCHEMA.vfx)
 ```
 
 ## Collections
 
 ```{include} collections/overview.md
@@ -66,15 +66,15 @@
 :end-before: example practice end
 ```
 
 The provided code demonstrates some of the capabilities of Trackteroid in handling complex scenarios without the need for explicit loops or excessive conditional statements. 
 Although the code may seem complex at first glance, the following explanations will break it down step by step.
 
 In the first part of the code, a single _TypedContext_ sample is retrieved using the _Query_ class. 
-The limit parameter is set to 1 to fetch only one sample. The projections parameter is used to specify the desired attributes (_Component.name_ and _ComponentLocation.resource_identifier_) to be included in the result.
+The _limit_ parameter is set to 1 to fetch only one sample. The _projections_ parameter is used to specify the desired attributes (_Component.name_ and _ComponentLocation.resource_identifier_) to be included in the result.
 
 Next, the retrieved _TypedContext_ sample is filtered using the _[Shot]_ filter. This filter selects only the subtypes of _TypedContext_ that match the _Shot_ entity and ensures that only _Shot_ entities are considered in the subsequent operations. 
 Since we are limiting the result of the _TypedContext_ query to only one entity, there is a possibility that the retrieved entity may not be a _Shot_. It could be of a different entity type, such as _AssetBuild_, _Sequence_, or _Folder_.
 Following the filter, the _Shot_ sample is further filtered using the _filter_ method. In this case, the filter condition checks if the _Component_ name of any of the _Shot's_ _AssetVersions_ is equal to "main". 
 Finally, the _resource_identifier_ attribute of a single _ComponentLocation_ is accessed. As we are anticipating only one result, the value is accessed using the [0] index. If a value is present, it is utilized; otherwise, the fallback string _"Not existing"_ is used.
 
 The second part of the code follows a similar structure, but this time the limit parameter is set to 10 to retrieve 10 potential _TypedContext_ samples. 
@@ -110,33 +110,33 @@
 :start-after: example custom attribute access start
 :end-before: example custom attribute access end
 ```
 
 #### Transformation Methods
 
 While iterating through loops is a valid approach, leveraging transformations can provide enhanced convenience. 
-The EntityCollection class provides higher-order methods that accept functions as arguments, aligning with the principles of functional programming. 
+The `EntityCollection` class provides [higher-order methods](collections.md#higher-order-methods) that accept functions as arguments, aligning with the principles of functional programming. 
 The presented example highlights a subset of the transformation methods available.
 
 ```{include} collections/examples.md
 :start-after: example transformation methods overview start
 :end-before: example transformation methods overview end
 ```
 
 #### Set Operations
 
-Due to the immutability of collections, it is not possible to directly add or remove entities. However, you can utilize the identical set operations available in Python's `set` class to obtain new collections.
+Due to the immutability of collections, it is not possible to directly add or remove entities. However, you can utilize the identical [set operations](collections.md#set-operations) available in Python's `set` class to obtain new collections.
 ```{include} collections/examples.md
 :start-after: example set operations overview start
 :end-before: example set operations overview end
 ```
 
 #### Fetching Attributes
 
-As Trackteroid's default Sessions disable the _autopolulate_ feature, it is possible to work with unprojected data. In such cases, you may need to fetch missing attributes when required. This can be accomplished using the `fetch_attributes` method on your collection.
+As Trackteroid's default Sessions disable the _auto-polulate_ feature, it is possible to work with unprojected data. In such cases, you may need to fetch missing attributes when required. This can be accomplished using the `fetch_attributes` method on your collection.
 ```{include} collections/examples.md
 :start-after: example fetch attributes1 start
 :end-before: example fetch attributes1 end
 ```
 
 #### Fallback Concept
 
@@ -165,19 +165,19 @@
 
 ```{include} collections/examples.md
 :start-after: example setattr1 start
 :end-before: example setattr1 end
 ```
 The provided code example illustrates the process of assigning values to the _resource_identifier_ attribute of `ComponentLocation` entities associated with an `AssetVersion` collection.
 
-The code demonstrates two scenarios for updating values: single-value and multi-value assignment. In the case of single-value assignment, a string value is assigned to _ComponentLocation[0].resource_identifier_, assuming that we are dealing with a collection containing a single element. This operation is possible when the collection has only one element. On the other hand, in the list assignment scenario, a list of values is assigned to the _ComponentLocation.resource_identifier_ attribute, with each value corresponding to an element in the collection. It is crucial to ensure that the number of elements in the list matches the number of elements in the collection.
+The code demonstrates two scenarios for updating values: single-value and multi-value assignment. In the case of a single-value assignment, a string value is assigned to _ComponentLocation[0].resource_identifier_, assuming that we are dealing with a collection containing a single element. This operation is possible when the collection has only one element. On the other hand, in the list assignment scenario, a list of values is assigned to the _ComponentLocation.resource_identifier_ attribute, with each value corresponding to an element in the collection. It is crucial to ensure that the number of elements in the list matches the number of elements in the collection.
 
 ```{attention}
 It's important to note that updates made to the collection are only stored in the local cache until they are committed. 
-The `commit()` method can be called on any collection and will persist **all recorded operations** from the underlying session to the Ftrack server. To verify the success of the update, the code reconnects the session and retrieves the updated attribute value by executing a new query.
+The `commit()` method can be called on any collection and will commit **all recorded operations** from the underlying session to the Ftrack server. To verify the success of the update in the example, the code reconnects the session and retrieves the updated attribute value by executing a new query.
 ```
 
 ```{tip}
 The [apply](collections.md#apply) method provides a convenient approach when you need to assign a single value or a single-element collection to a collection that has multiple receivers.
 ```
 
 #### Create
@@ -191,15 +191,15 @@
 
 The code example showcases the process of adding a new note to an existing collection of notes within an `AssetVersion` collection. Since collections are immutable and do not allow entities to be added or removed from an existing collection directly, the create method returns a new `Note` collection that solely contains the newly created note.
 
 To preserve the existing notes, the code performs a `union` operation between the original `Note` collection and the newly created collection. This combined collection is then assigned back, ensuring that both the existing notes and the newly created note are included.
 
 ```{attention}
 It's important to note that creation and updates made to the collection are only stored in the local cache until they are committed. 
-The `commit()` method can be called on any collection and will persist **all recorded operations** from the underlying session to the Ftrack server. To verify the success of the update, the code reconnects the session and retrieves the updated attribute value by executing a new query.
+The `commit()` method can be called on any collection and will commit **all recorded operations** from the underlying session to the Ftrack server.
 ```
 
 ##### Linking 
 
 The `AssetVersion` collection offers a convenient way to link entities to each other using the _uses_versions_ and _used_in_versions_ attribute types. Additionally, collections can be easily linked or unlinked from each other by utilizing the following methods:
 - `link_inputs(collection)`
 - `link_outputs(collection)` 
@@ -213,7 +213,20 @@
 ```{include} collections/examples.md
 :start-after: example linking1 start
 :end-before: example linking1 end
 ```
 
 #### Delete
 
+The `delete()` method available on a collection provides the capability to delete entities associated with that collection.
+
+```{include} collections/examples.md
+:start-after: example delete start
+:end-before: example delete end
+```
+
+```{attention}
+It's important to note that of a collection is only stored in the local cache until the changes are committed. 
+The `commit()` method can be called on any collection and will commit **all recorded operations** from the underlying session to the Ftrack server. To verify the success of the deletion in the example, the code reconnects the session and retrieves the updated attribute value by executing a new query.
+```
+
+
```

### Comparing `trackteroid-0.1.0rc4/pyproject.toml` & `trackteroid-0.1.0rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/__init__.py` & `trackteroid-0.1.0rc5/src/trackteroid/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/configuration.py` & `trackteroid-0.1.0rc5/src/trackteroid/configuration.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/constants.py` & `trackteroid-0.1.0rc5/src/trackteroid/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__VERSION__ = "0.1.0rc4"
+__VERSION__ = "0.1.0rc5"
```

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/entities/__init__.py` & `trackteroid-0.1.0rc5/src/trackteroid/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/entities/base.py` & `trackteroid-0.1.0rc5/src/trackteroid/entities/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,18 @@
     OrderedDict,
     defaultdict,
     namedtuple,
 )
 from copy import copy
 import sys
 
+from ftrack_api.attribute import (
+    CollectionAttribute,
+    ReferenceAttribute
+)
 from ftrack_api.symbol import NOT_SET
 
 from .declarations import *
 
 from .schematypes import (
     CUSTOM_ATTRIBUTE_TYPE_COMPATIBILITY,
     AttributeInfo
@@ -196,15 +200,15 @@
                     else:
                         _collection = bool(re.match(r"^(children|ancestors)(\[\w+\])?", attribute_tokens[0]))
 
                     if collection is None:
                         collection = _collection
                     if collection != _collection:
                         raise AttributeError(
-                            "Given relationships '{}' attribute array state is ambigious.".format(
+                            "Given relationships '{}' attribute array state is ambiguous.".format(
                                 relation
                             )
                         )
 
                 self.add(globals()[target_entity_name], relation, collection)
 
     def add(self, target, relation, collection=False):
@@ -330,22 +334,22 @@
             collections.append(self.create(**_attributes))
 
         return EmptyCollection(_type=self._entity).union(*collections)
 
     def union(self, *collections):
         if len(collections) == 1:
             return collections[0]
-        
+
         first = collections[0]
         others = [_ for _ in collections[1:] if _]
         first_type = first.entity_type
         for other_type in (_.entity_type for _ in others if _):
             assert first_type == other_type, "Can't union collections with different types. {} != {}."\
                 .format(first_type, other_type)
-        
+
         return first.union(*others)
 
 
 class EntityCollection(object):
     """ An immutable sorted set of unique Entities of the same entity type.
     """
     MEMBERS = [
@@ -393,21 +397,42 @@
         if isinstance(other, EntityCollection):
             return [_.ftrack_entity for _ in self.values()] == \
                    [_.ftrack_entity for _ in other.values()]
         else:
             return False
 
     def __getattr__(self, item):
+        from .entities import TypedContext, Component
+        coercion_map = {
+            "parent": TypedContext,
+            "children": TypedContext,
+            "ancestors": TypedContext,
+            "descendants": TypedContext,
+            "components": Component
+        }
+
         # TODO: clean after we have tests for this functionality
-        if self and item in list(self.values())[0].ftrack_entity.keys():
+        sample_entity = list(self.values())[0].ftrack_entity
+
+        # Checking if an attribute exists on the ftrack entity via
+        # "item in sample_entity" for some reason triggers the attribute
+        # getter in the entity which in turn triggers a bug on the Ftrack API
+        # that "locks" an NOT_SET attribute via setting an empty collection as
+        # the local value. By checking the attributes schema we can bypass this
+        # behaviour
+        existing_attributes = [x.name for x in sample_entity.attributes]
+
+        if self and item in existing_attributes:
             entities = []
             values = []
             entity_type = None
+
             for entity in self.values():
                 value = entity[item]
+
                 # resolve entities in collections
                 if value.__class__.__name__ == "Collection":
                     for _ in value:
                         # wrap ftrack entity
                         if hasattr(_, "entity_type"):
                             entities.append(Entity.from_entity_type(str(_.entity_type), ftrack_entity=_))
                         else:
@@ -421,30 +446,56 @@
 
                 # wrap ftrack entity
                 elif hasattr(value, "entity_type"):
                     entities.append(Entity.from_entity_type(str(value.entity_type), ftrack_entity=value))
                 else:
                     values.append(value)
 
+            # If all values are NOT_SET means we have not fetched that attribute
+            # that we're trying to retrieve. We must then pick up reference and
+            # collection attributes and properly return them as EmptyCollection
+            # of the proper entity type.
+            if values and all([x is NOT_SET for x in values]):
+                # We get the ftrack attribute type, to check if this attribute is a reference
+                # to any other type of entity
+                ftrack_attribute = sample_entity.attributes.get(item)
+
+                if isinstance(ftrack_attribute, (CollectionAttribute, ReferenceAttribute)):
+
+                    # If it's a collection or a reference attribute, we'll replace NOT_SET with
+                    # an empty collection of the right type, for that we need to determine what
+                    # type of attribute it is via its original Ftrack type schema:
+                    # Find the ftrack type schema
+                    type_schema = [x for x in self._session.schemas if x["id"] == sample_entity.entity_type][0]
+
+                    # Find the attribute schema
+                    attribute_schema = type_schema["properties"][item]
+
+                    # Find the actual reference type
+                    collection_type_name = attribute_schema.get("$ref")
+                    if collection_type_name is None:
+                        collection_type_name = attribute_schema["items"]["$ref"]
+
+                    # Convert it to a trackteroid type and coerce it
+                    entity_type_class = self._session.get_type_class(collection_type_name)
+                    entity_type_class = coercion_map.get(item, entity_type_class)
+
+                    # Finally return the actual emtpy collection
+                    return EmptyCollection(
+                        _type=entity_type_class(),
+                        source=self,
+                        session=self._session
+                    )
+
             if entities:
-                # wrap into lambdas so this will be only requested when needed
-                _to_typedcontext = lambda: getattr(importlib.import_module("..entities", __name__), "TypedContext")
-                _to_component = lambda: getattr(importlib.import_module("..entities", __name__), "Component")
-                _to_original = lambda: lambda collection: collection
-
-                coerce_attributes = {
-                    "parent": _to_typedcontext,
-                    "children": _to_typedcontext,
-                    "ancestors": _to_typedcontext,
-                    "descendants": _to_typedcontext,
-                    "components": _to_component
-                }
-                coercion_type = coerce_attributes.get(item, _to_original)()
+                collection = self.from_entities(entities, source=(item, self))
+                if item in coercion_map:
+                    return coercion_map[item](collection)
 
-                return coercion_type(self.from_entities(entities, source=(item, self)))
+                return collection
 
             elif entity_type:
                 return EmptyCollection(_type=entity_type, source=self, session=self._session)
             return values
 
         elif item == "get":
             return self._get_relatives
@@ -570,26 +621,36 @@
                 # If the attribute access produces a collection
                 # we potentially can not go by key as the attribute
                 # access can be a type based shortcut.
                 # Therefore we need to resolve the collections produced
                 # via the full attribute chain and retain the last attribute
                 # as our key.
                 if not isinstance(attribute_value, list):
-                    key, collection = attribute_value._source
+                    if isinstance(attribute_value, EntityCollection):
+                        key, collection = attribute_value._source
+                    elif isinstance(attribute_value, EmptyCollection):
+                        # TODO: assignment on an EmptyCollection attribute doesn't
+                        #  seem to be handled at the moment anyways.
+                        if attribute_value.depth > 1:
+                            raise EntityCollectionOperationError(
+                                "You are attempting to assign a value to an attribute on an EmptyCollection."
+                            )
+                        collection = attribute_value.source
                 else:
                     collection = self
 
                 compatible, reason = collection._is_attribute_compatible_with_value(key, value)
                 if not compatible:
                     raise TypeError(reason)
 
                 if isinstance(value, (list, tuple, EntityCollection)) \
                         and len(collection) == 1 \
                         and list(collection._entities.values())[0].ftrack_entity[key].__class__.__name__ == "Collection":
                     if isinstance(value, EntityCollection):
+                        self._verify_operability(value)
                         list(collection.values())[0].ftrack_entity[key] = [_.ftrack_entity for _ in value.values()]
                 else:
                     for idx, entity in enumerate(collection.values()):
                         if key.startswith("custom_"):
                             if isinstance(value, (list, tuple, EntityCollection)):
                                 entity.ftrack_entity["custom_attributes"][key.replace("custom_", "")] = value[idx]
                             else:
@@ -605,14 +666,15 @@
                                 if not len(value):
                                     entity.ftrack_entity[key] = value
                                 else:
                                     for _key, _value in value.items():
                                         entity.ftrack_entity[key][_key] = _value
                         else:
                             if isinstance(value, EntityCollection):
+                                self._verify_operability(value)
                                 entity.ftrack_entity[key] = list(value.values())[idx].ftrack_entity
                             elif isinstance(value, (list, tuple)):
                                 entity.ftrack_entity[key] = value[idx]
                             else:
                                 entity.ftrack_entity[key] = value
 
             else:
@@ -682,19 +744,19 @@
         query = self.as_query(use_ids=True)
         query.projections = list(set(projections_).union(query.projections))  # update not override
         return query.get_all(session=session or self._session).children
 
     # TODO: move to avoid circular import
     @staticmethod
     def _make_empty(entity_class, session):
+        from ..query import Query
         # UGLY AS HELL!!!!!
         entitycollection = EntityCollection(_cls=entity_class, entities=OrderedDict())
         # this special import is neccessary to avoid a circular import
-        adhoc_type = getattr(importlib.import_module("...query", __name__), "Query")
-        entitycollection.query = adhoc_type(entity=entity_class, session=session)
+        entitycollection.query = Query(entity=entity_class, session=session)
         entitycollection.query.valid = False
         entitycollection._session = session
         return entitycollection
 
     @property
     def entity_type(self):
         return self._entity.__class__
@@ -871,14 +933,38 @@
         elif property_schema.get("type"):
             attribute_info.types = self._schema_types_map[property_schema["type"]]
         else:
             raise AttributeError("Attribute '{}' not found in schema '{}'.".format(attribute_name, entity_schema["id"]))
 
         return attribute_info
 
+    def _verify_operability(self, *collections):
+        """ verify that an operation can actually work between collections
+
+        Args:
+            *collections (EntityCollection or EmptyCollection instances): collections to operate
+
+        """
+        sessions = [self._session] + [_._session for _ in [__ for __ in collections if __]]
+        unique_sessions = [item for i, item in enumerate(sessions) if item not in sessions[:i]]
+
+        if len(unique_sessions) > 1:
+            raise EntityCollectionOperationError(
+                "Operation can not be performed because collections are using different `Session` objects."
+            )
+
+        schemas = [self.query.schema["name"]] + [_.query.schema["name"] for _ in [__ for __ in collections if __]]
+        unique_schemas = set(schemas)
+
+        if len(unique_schemas) > 1:
+            raise EntityCollectionOperationError(
+                "Operation can not be performed because collections are using different schemas: "
+                f"{', '.join(unique_schemas)}"
+            )
+
     def keys(self):
         return self._entities.keys()
 
     def values(self):
         return self._entities.values()
 
     @property
@@ -1171,14 +1257,16 @@
         Args:
             collections (EntityCollection): EntityCollection object of same type as the current one
 
         Returns:
             EntityCollection:
 
         """
+        self._verify_operability(*collections)
+
         entities = list(self.values())
         for collection in collections:
             if not collection:
                 continue  # avoid merging EmptyCollections
             self._validate_collection_type(collection)
             for entity in collection:
                 if list(entity.values())[0] not in entities:
@@ -1192,14 +1280,16 @@
         Args:
             collections (EntityCollection): EntityCollection object of same type as the current one
 
         Returns:
             EntityCollection:
 
         """
+        self._verify_operability(*collections)
+
         for collection in collections:
             self._validate_collection_type(collection)
 
         intersection = []
         for _id in self.keys():
             if all(_id in collection.keys() for collection in collections):
                 intersection.append(_id)
@@ -1217,14 +1307,17 @@
         Args:
             *collections (EntityCollection): EntityCollection objects of same
              type as the current one
 
         Returns:
             EntityCollection
         """
+        # not necessarily needed as long as union will be called
+        self._verify_operability(*collections)
+
         for collection in collections:
             self._validate_collection_type(collection)
 
         counter = defaultdict(int)
 
         all_collections = [self] + list(collections)
         all_entities = self.union(*collections)
@@ -1241,14 +1334,15 @@
         """ Generates the difference between self and the given collections.
 
         This essentially acts as a "subtraction" operation.
 
         Returns:
             EntityCollection
         """
+        self._verify_operability(*collections)
 
         ids = self.keys()
 
         for collection in collections:
             ids = [_id for _id in ids if _id not in collection.keys()]
 
         return self.filter(lambda x: x.id[0] in ids)
@@ -1346,15 +1440,15 @@
                     for key, value in iterable.items():
                         if len(value.keys()) == 1:
                             # if the child will not branch, we will reset the
                             # hierarchy to not accumulate duplicate levels
                             path = ""
                         _ = __flatten(value, path)
                         if len(_.keys()) == 1:
-                            # if the childs are not branching we extract the values
+                            # if the children are not branching we extract the values
                             # and set them with the correct key
                             flat[key + "." + list(_.keys())[0]] = list(_.values())[0]
                         else:
                             # otherwise we will create a new branch
                             flat[key] = _
                     return flat
                 return flat
@@ -1424,15 +1518,15 @@
         _fetch(self, flat)
 
         return self
 
     def _simple_children_fetch(self, *attributes):
         # this is needed as a special case to avoid an infinite recursion due to
         # fetch_attributes calling getattr and getatrr calling fetch_attributes
-        # (wheh accessing children)
+        # (when accessing children)
         query = self.as_query(use_ids=True)
         # TODO(high): Reimplement the conditional fetching of non-existing projections.
         # Update the projections on the query object accordingly.
         # only perform a query if really necessary
         if set(attributes).union(query.projections) != set(query.projections):
             query.projections = list(set(attributes).union(query.projections))  # update not override
             query.get_all()
@@ -1449,15 +1543,15 @@
             relative_type (Entity): subclass of Entity
             **kwargs ():
 
         Returns:
             Any: whatever the attributes holds, most likely another EntityCollection
         """
 
-        relationship = self.query.entity_type.relationship.get(relative_type, default=TargetRelation()).relation
+        relationship = self.entity_type.relationship.get(relative_type, default=TargetRelation()).relation
         if not relationship:
             raise ValueError("Unknown relationship for relative '{}'".format(relative_type))
 
         if not isinstance(relationship, list):
             relation_projections = [relationship]
         else:
             relation_projections = relationship
@@ -1487,15 +1581,15 @@
         Returns:
 
         """
         # TODO: this definitely needs cleanup
         # make the Query class available
         _Query = getattr(importlib.import_module("...query", __name__), "Query")
 
-        # get the actual entity implemantions not the ForwardDeclare classes
+        # get the actual entity implementations not the ForwardDeclare classes
         _Recipient = getattr(importlib.import_module("..entities", __name__), "Recipient")
         _User = getattr(importlib.import_module("..entities", __name__), "User")
 
         if not ftrack_note_entity.get("author"):
             ftrack_note_entity["author"] = list(_Query(_User, session=self._session).by_name(
                 self._session.api_user).get_one().values())[0].ftrack_entity
 
@@ -1713,20 +1807,25 @@
         self.ftrack_entity = ftrack_entity
         if not _cls:
             self.log = logging.getLogger(
                 "{}.entities.{}".format(self.__class__.__name__, LOGGING_NAMESPACE)
             )
 
     def __getitem__(self, item):
-        return self.ftrack_entity.get(item)
+        # Try/Except against KeyError to keep compatibility with
+        # what it would be "ftrack_entity.get()"
+        try:
+            return self._get_attribute(item)
+        except KeyError:
+            return None
 
     def __getattr__(self, item):
         value = None
         if item in self.ftrack_entity.keys():
-            value = self.ftrack_entity[item]
+            value = self._get_attribute(item)
             if hasattr(value, "entity_type"):
                 return Entity.from_entity_type(str(value.entity_type), ftrack_entity=value)
         return value
 
     def __str__(self):
         return self.__class__.__name__
 
@@ -1753,14 +1852,38 @@
             return 0
         else:
             return 1
 
     def pre_create(self, **kwargs):
         return kwargs
 
+    def _get_attribute(self, attribute_name):
+        """Gets an attribute value of the underlying Ftrack entity. Use
+        this function to bypass the issue with locking attributes in the
+        ftrack api
+
+        Args:
+            attribute_name (str): The attribute name
+
+        Raises:
+            KeyError: If the attribute does not exist
+        """
+
+        attribute = self.ftrack_entity.attributes.get(attribute_name)
+
+        if not attribute:
+            raise KeyError(attribute_name)
+
+        local_value = attribute.get_local_value(self.ftrack_entity)
+
+        if local_value is not NOT_SET:
+            return local_value
+
+        return attribute.get_remote_value(self.ftrack_entity)
+
     @property
     def ftrack_entity(self):
         return self._ftrack_entity
 
     @ftrack_entity.setter
     def ftrack_entity(self, instance):
         self._ftrack_entity = instance
@@ -1784,15 +1907,19 @@
     def create_batch(self, *attributes): pass
     def delete(self): pass
 
     # although there is no logical reason to have multiple filters
     # this is how the query consolidates its criteria
     # having multiple filters allows us the inject criterion multiple times
     # Example:
-    #   Query(Task).inject("parent.parent.name is 'library').by_name(Project, "Foobar").inject("parent.status.name is 'Approved').get_all()
+    #   Query(Task).\
+    #       inject("parent.parent.name is 'library').\
+    #       by_name(Project, "Foobar").\
+    #       inject("parent.status.name is 'Approved').\
+    #       get_all()
     def inject(self, target, *filter):
         if any(re.search(r"^or\s*", _, flags=re.IGNORECASE) for _ in filter):
             raise ValueError(
                 "OR relationships are not supported across multiple criteria or filter.\n"
                 "You can use an 'or' relationship within a single filter string though."
             )
```

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/entities/declarations.py` & `trackteroid-0.1.0rc5/src/trackteroid/entities/declarations.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/entities/declarations.pyi` & `trackteroid-0.1.0rc5/src/trackteroid/entities/declarations.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/entities/entities.py` & `trackteroid-0.1.0rc5/src/trackteroid/entities/entities.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/entities/entities.pyi` & `trackteroid-0.1.0rc5/src/trackteroid/entities/entities.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/entities/relationships_parser.py` & `trackteroid-0.1.0rc5/src/trackteroid/entities/relationships_parser.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/entities/schematypes.py` & `trackteroid-0.1.0rc5/src/trackteroid/entities/schematypes.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/query/__init__.py` & `trackteroid-0.1.0rc5/src/trackteroid/query/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/query/criteria.py` & `trackteroid-0.1.0rc5/src/trackteroid/query/criteria.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         self.target = target
         self.filter = filter
         self.negate = negate
 
     def resolve(self):
         partial_query = self.filter(self.target, *self.args, **self.kwargs)
         if self.negate:
-            partial_query = re.sub("\s+(in|like)\s+", r" not_\1 ", partial_query)
-            partial_query = re.sub("\s+is\s+", " is_not ", partial_query)
+            partial_query = re.sub(r"\s+(in|like)\s+", r" not_\1 ", partial_query)
+            partial_query = re.sub(r"\s+is\s+", " is_not ", partial_query)
 
         return partial_query
 
     # stay compatible - previously we used a namedtuple as Criterion object
     def as_dict(self):
         return {
             "name": self.name,
@@ -67,23 +67,25 @@
             "kwargs": self.kwargs,
             "target": self.target,
             "filter": self.filter,
             "negate": self.negate
         }
 
 
-class Criteria():
+class Criteria:
     """ stubs for filtering (aka query criteria)
 
     This is used to allow proper autocompletion within (some) IDE(s).
     """
 
-    class InvalidArgumentsError(ValueError): pass
-    class CriterionNotImplementedError(NotImplementedError): pass
+    class InvalidArgumentsError(ValueError):
+        pass
 
+    class CriterionNotImplementedError(NotImplementedError):
+        pass
 
     def by_id(self, *ids):
         raise NotImplementedError
 
     def by_location(self, *locations):
         raise NotImplementedError
 
@@ -202,8 +204,8 @@
                         )
 
             # Propagate target as TargetRelation object
             if args[0]:
                 args = [instance.relationship[args[0]]] + list(args[1:])
             return wrapped(*args, **kwargs)
 
-        return wrapper
+        return wrapper
```

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/query/criteria.pyi` & `trackteroid-0.1.0rc5/src/trackteroid/query/criteria.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/query/query.py` & `trackteroid-0.1.0rc5/src/trackteroid/query/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,15 @@
         """ get the result with limit, offset and specific ordering
 
         Notes:
             Compared to the default FTrack behavior our order will reflect the
             actual sorting in the end.
 
         Args:
+            projections (list): attributes you want to project
             limit (int): limited amount of resulting entities
             offset (int): offset
             order (str): "descending" or "ascending"
             order_by (str): field to use for ordering
 
         Returns:
             Entity subclass: the given entity instance
```

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/query/utils.py` & `trackteroid-0.1.0rc5/src/trackteroid/query/utils.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/session.py` & `trackteroid-0.1.0rc5/src/trackteroid/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,22 +113,27 @@
             # so they are all flattened with their relationships removed
             relationship_parser.attributes_blacklist = {"descendants", "ancestors", "status_changes"}
             relationship_parser.extract_all_entity_relations()
             _PARSED_RELATIONSHIPS_CACHE[self._session.server_url] = relationship_parser
 
         return _PARSED_RELATIONSHIPS_CACHE[self._session.server_url]
 
+    def get_type_class(self, type_name):
+        from .entities import entities
+        return getattr(entities, type_name, None)
+
     def get_cached_collections(self):
+        # TODO: Is this function still needed?
         typenames = sorted([str(k) for k, v in self._build_entity_type_classes(self.schemas).items()])
         type_module = importlib.import_module("..entities", __name__)
 
         type_map = {}
         for name in typenames:
             collection = getattr(type_module, "EntityCollection")
-            _type = getattr(type_module, name)
+            _type = getattr(type_module, name, None)
             if _type and issubclass(_type, getattr(type_module, "Entity")):
                 cached_entities = [
                     _type.from_entity_type(name=_type.__name__, ftrack_entity=_) for _ in self._local_cache.values()
                     if _.__class__.__name__ == name
                 ]
                 entitycollection = collection._make_empty(_type, self)
                 type_map[_type] = entitycollection.from_entities(cached_entities)
@@ -270,28 +275,33 @@
         # clear operations temporarily
         deferred = Operations()
         self.recorded_operations = deferred
 
         yield
 
         # sync cache
+        _cache_records = []
         with file_cache._database() as database:
-            for key, value in database.items():
-                entity_data = json.loads(value)
-                for attr, attr_value in entity_data.items():
-                    if isinstance(attr_value, dict):
-                        entity_type = attr_value.get("__entity_type__")
-                        if entity_type:
-                            # if this is an entity we check whether the linked entity is available
-                            # in our filecache
-                            # TODO: eventually we should check for the actual primary key here
-                            #  for our current usecase it seems ok to blindly use the id
-                            cache_key = "('{}', ['{}'])".format(entity_type, attr_value["id"])
-                            if cache_key not in serialised_cache.keys():
-                                serialised_cache.set(cache_key, self._local_cache.get(cache_key))
+            for key in database.keys():
+                value = database[key]
+                _cache_records.append((key, value))
+
+        for key, value in _cache_records:
+            entity_data = json.loads(value)
+            for attr, attr_value in entity_data.items():
+                if isinstance(attr_value, dict):
+                    entity_type = attr_value.get("__entity_type__")
+                    if entity_type:
+                        # if this is an entity we check whether the linked entity is available
+                        # in our filecache
+                        # TODO: eventually we should check for the actual primary key here
+                        #  for our current usecase it seems ok to blindly use the id
+                        cache_key = "('{}', ['{}'])".format(entity_type, attr_value["id"])
+                        if cache_key not in serialised_cache.keys():
+                            serialised_cache.set(cache_key, self._local_cache.get(cache_key))
 
             # serialise operations and store them in the database
             ops = []
             for op in self.recorded_operations:
                 if isinstance(op, CreateEntityOperation):
                     ops.append(
                         {
```

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/stubs/__init__.py` & `trackteroid-0.1.0rc5/src/trackteroid/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid/stubs/stubs.py` & `trackteroid-0.1.0rc5/src/trackteroid/stubs/stubs.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc4/src/trackteroid.egg-info/PKG-INFO` & `trackteroid-0.1.0rc5/src/trackteroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackteroid
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: Declarative, object-oriented wrapper for Ftrack queries. Powerful functional-style interactions with resulting collections.
 Author: Rico Koschmitzky, Dennis Weil
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Trixter
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `trackteroid-0.1.0rc4/src/trackteroid.egg-info/SOURCES.txt` & `trackteroid-0.1.0rc5/src/trackteroid.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.md
 pyproject.toml
 requirements.txt
 tox.ini
 .github/ISSUE_TEMPLATE/issue--bug-report.md
 .github/ISSUE_TEMPLATE/issue--feature-request.md
 .github/workflows/python-publish.yml
+.github/workflows/tox.yml
 .graphics/svg/logo_black.svg
 .graphics/svg/logo_white.svg
 doc/requirements.txt
 doc/sphinx_source/Makefile
 doc/sphinx_source/collections.md
 doc/sphinx_source/conf.py
 doc/sphinx_source/configuration.md
@@ -28,14 +29,15 @@
 doc/sphinx_source/_static/logo_white.svg
 doc/sphinx_source/collections/emptycollection.md
 doc/sphinx_source/collections/entitycollection.md
 doc/sphinx_source/collections/examples.md
 doc/sphinx_source/collections/overview.md
 doc/sphinx_source/query/examples.md
 doc/sphinx_source/query/overview.md
+doc/sphinx_source/session/examples.md
 src/trackteroid/__init__.py
 src/trackteroid/configuration.py
 src/trackteroid/constants.py
 src/trackteroid/session.py
 src/trackteroid.egg-info/PKG-INFO
 src/trackteroid.egg-info/SOURCES.txt
 src/trackteroid.egg-info/dependency_links.txt
@@ -53,8 +55,15 @@
 src/trackteroid/query/criteria.py
 src/trackteroid/query/criteria.pyi
 src/trackteroid/query/query.py
 src/trackteroid/query/query.pyi
 src/trackteroid/query/utils.py
 src/trackteroid/stubs/__init__.py
 src/trackteroid/stubs/stubs.py
-tests/test_placeholder.py
+tests/conftest.py
+tests/test_authoring.py
+tests/test_collection.py
+tests/test_session.py
+tests/resources/session/operations_linux.dbm
+tests/resources/session/operations_windows.dbm.bak
+tests/resources/session/operations_windows.dbm.dat
+tests/resources/session/operations_windows.dbm.dir
```


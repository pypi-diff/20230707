# Comparing `tmp/azure-databricks-sdk-python-0.0.2.tar.gz` & `tmp/azure-databricks-sdk-python-0.0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-databricks-sdk-python-0.0.2.tar", last modified: Fri Oct  2 09:35:31 2020, max compression
+gzip compressed data, was "azure-databricks-sdk-python-0.0.4.dev1.tar", last modified: Fri Jul  7 09:34:19 2023, max compression
```

## Comparing `azure-databricks-sdk-python-0.0.2.tar` & `azure-databricks-sdk-python-0.0.4.dev1.tar`

### file list

```diff
@@ -1,67 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)      603 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.879024 azure-databricks-sdk-python-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.879024 azure-databricks-sdk-python-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2345 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1671 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1077 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (116)      657 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)       47 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (116)      334 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4837 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3358 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/
--rw-r--r--   0 runner    (1001) docker     (116)      147 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8108 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/api.py
--rw-r--r--   0 runner    (1001) docker     (116)     9380 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     8421 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/clusters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1200 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     7197 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/secrets.py
--rw-r--r--   0 runner    (1001) docker     (116)     1987 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/types/
--rw-r--r--   0 runner    (1001) docker     (116)       71 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      837 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/types/auth_methods.py
--rw-r--r--   0 runner    (1001) docker     (116)    15096 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/types/clusters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1714 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/types/secrets.py
--rw-r--r--   0 runner    (1001) docker     (116)      767 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python/types/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4837 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1595 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       47 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (116)       24 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       28 2020-10-02 09:35:31.000000 azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      638 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      799 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)      116 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     3341 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (116)      749 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/_templates/hacks.html
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/_templates/sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/docs/source/_themes/
--rw-r--r--   0 runner    (1001) docker     (116)     4874 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/_themes/flask_theme_support.py
--rw-r--r--   0 runner    (1001) docker     (116)     1083 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3917 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     3466 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      428 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/updates.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/docs/source/user/
--rw-r--r--   0 runner    (1001) docker     (116)     4682 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/user/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1290 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/user/install.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3692 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/docs/source/user/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (116)       92 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      810 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      105 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:31.883024 azure-databricks-sdk-python-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      815 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1841 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5872 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/tests/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (116)     2814 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/tests/test_scopes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1075 2020-10-02 09:35:21.000000 azure-databricks-sdk-python-0.0.2/tests/test_tokens.py
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.574957 azure-databricks-sdk-python-0.0.4.dev1/
+-rw-r--r--   0 god3l      (502) staff       (20)      603 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/.coveragerc
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.547717 azure-databricks-sdk-python-0.0.4.dev1/.github/
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.557060 azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/
+-rw-r--r--   0 god3l      (502) staff       (20)     2345 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 god3l      (502) staff       (20)     1671 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/coverage.yml
+-rw-r--r--   0 god3l      (502) staff       (20)     1077 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/linting.yml
+-rw-r--r--   0 god3l      (502) staff       (20)      657 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/publish.yml
+-rw-r--r--   0 god3l      (502) staff       (20)      125 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/AUTHORS
+-rw-r--r--   0 god3l      (502) staff       (20)     1573 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/ChangeLog
+-rw-r--r--   0 god3l      (502) staff       (20)      334 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/HISTORY.md
+-rw-r--r--   0 god3l      (502) staff       (20)     1072 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/LICENSE
+-rw-r--r--   0 god3l      (502) staff       (20)     4610 2023-07-07 09:34:19.575264 azure-databricks-sdk-python-0.0.4.dev1/PKG-INFO
+-rw-r--r--   0 god3l      (502) staff       (20)     3865 2023-07-07 08:21:41.000000 azure-databricks-sdk-python-0.0.4.dev1/README.md
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.560057 azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/
+-rw-r--r--   0 god3l      (502) staff       (20)     4610 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 god3l      (502) staff       (20)     1092 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 god3l      (502) staff       (20)        1 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 god3l      (502) staff       (20)        1 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/not-zip-safe
+-rw-r--r--   0 god3l      (502) staff       (20)       47 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/pbr.json
+-rw-r--r--   0 god3l      (502) staff       (20)       24 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 god3l      (502) staff       (20)        1 2023-07-07 09:34:19.000000 azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.562010 azure-databricks-sdk-python-0.0.4.dev1/docs/
+-rw-r--r--   0 god3l      (502) staff       (20)      638 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/Makefile
+-rw-r--r--   0 god3l      (502) staff       (20)      799 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/make.bat
+-rw-r--r--   0 god3l      (502) staff       (20)      116 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/requirements-docs.txt
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.564564 azure-databricks-sdk-python-0.0.4.dev1/docs/source/
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.565365 azure-databricks-sdk-python-0.0.4.dev1/docs/source/_static/
+-rw-r--r--   0 god3l      (502) staff       (20)     3341 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/_static/custom.css
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.566737 azure-databricks-sdk-python-0.0.4.dev1/docs/source/_templates/
+-rw-r--r--   0 god3l      (502) staff       (20)      749 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/_templates/hacks.html
+-rw-r--r--   0 god3l      (502) staff       (20)     2178 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/_templates/sidebar.html
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.567317 azure-databricks-sdk-python-0.0.4.dev1/docs/source/_themes/
+-rw-r--r--   0 god3l      (502) staff       (20)     4874 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/_themes/flask_theme_support.py
+-rw-r--r--   0 god3l      (502) staff       (20)     1083 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/api.rst
+-rw-r--r--   0 god3l      (502) staff       (20)     3917 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/conf.py
+-rw-r--r--   0 god3l      (502) staff       (20)     3705 2023-07-07 08:21:18.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/index.rst
+-rw-r--r--   0 god3l      (502) staff       (20)      428 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/updates.rst
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.569879 azure-databricks-sdk-python-0.0.4.dev1/docs/source/user/
+-rw-r--r--   0 god3l      (502) staff       (20)     4682 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/user/advanced.rst
+-rw-r--r--   0 god3l      (502) staff       (20)     1290 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/user/install.rst
+-rw-r--r--   0 god3l      (502) staff       (20)     3692 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/docs/source/user/quickstart.rst
+-rw-r--r--   0 god3l      (502) staff       (20)       92 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/requirements-test.txt
+-rw-r--r--   0 god3l      (502) staff       (20)       23 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/requirements.txt
+-rw-r--r--   0 god3l      (502) staff       (20)      760 2023-07-07 09:34:19.576043 azure-databricks-sdk-python-0.0.4.dev1/setup.cfg
+-rw-r--r--   0 god3l      (502) staff       (20)      105 2023-07-07 09:15:30.000000 azure-databricks-sdk-python-0.0.4.dev1/setup.py
+drwxr-xr-x   0 god3l      (502) staff       (20)        0 2023-07-07 09:34:19.574221 azure-databricks-sdk-python-0.0.4.dev1/tests/
+-rw-r--r--   0 god3l      (502) staff       (20)        0 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/tests/__init__.py
+-rw-r--r--   0 god3l      (502) staff       (20)      815 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/tests/helpers.py
+-rw-r--r--   0 god3l      (502) staff       (20)     1841 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/tests/test_client.py
+-rw-r--r--   0 god3l      (502) staff       (20)     5872 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/tests/test_clusters.py
+-rw-r--r--   0 god3l      (502) staff       (20)     2814 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/tests/test_scopes.py
+-rw-r--r--   0 god3l      (502) staff       (20)     1075 2023-07-07 08:14:01.000000 azure-databricks-sdk-python-0.0.4.dev1/tests/test_tokens.py
```

### Comparing `azure-databricks-sdk-python-0.0.2/.coveragerc` & `azure-databricks-sdk-python-0.0.4.dev1/.coveragerc`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/.github/workflows/codeql-analysis.yml` & `azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/.github/workflows/coverage.yml` & `azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/.github/workflows/linting.yml` & `azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/.github/workflows/publish.yml` & `azure-databricks-sdk-python-0.0.4.dev1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/LICENSE` & `azure-databricks-sdk-python-0.0.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/PKG-INFO` & `azure-databricks-sdk-python-0.0.4.dev1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,107 @@
 Metadata-Version: 2.1
 Name: azure-databricks-sdk-python
-Version: 0.0.2
+Version: 0.0.4.dev1
 Summary: A Python SDK for the Azure Databricks REST API 2.0.
 Home-page: http://github.com/aminekaabachi/azure-databricks-sdk-python
 Author: Amine Kaabachi
 Author-email: ping@kaabachi.io
 Maintainer: Amine Kaabachi
 Maintainer-email: ping@kaabachi.io
 License: MIT
-Description: # Azure Databricks SDK Python
-        
-        [![Workflow Status](https://img.shields.io/github/workflow/status/aminekaabachi/azure-databricks-sdk-python/Unit%20Tests/master?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/actions?query=workflow%3A%22Unit+Tests%22)
-        [![Coveralls github](https://img.shields.io/coveralls/github/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://coveralls.io/github/aminekaabachi/azure-databricks-sdk-python?branch=master)
-        [![PyPI](https://img.shields.io/pypi/v/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
-        [![Downloads](https://img.shields.io/pypi/dm/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
-        [![Docs](https://readthedocs.org/projects/azure-databricks-sdk-python/badge/?version=latest&style=flat-square)](https://azure-databricks-sdk-python.readthedocs.io/en/latest/)
-        [![GitHub](https://img.shields.io/github/license/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/blob/master/LICENSE)
-        
-        
-        **azure-databricks-sdk-python** is a Python SDK for the [`Azure Databricks REST API 2.0`](<https://docs.microsoft.com/en-gb/azure/databricks/dev-tools/api/latest/>).
-        
-        -----------------
-        
-        Easily, perform all the operations as if on the Databricks UI:
-        ```python
-        from azure_databricks_sdk_python import Client
-        from azure_databricks_sdk_python.types.clusters import AutoScale, ClusterAttributes
-        
-        client = Client(databricks_instance="<instance>", personal_access_token="<token>")
-        spark_conf = {'spark.speculation': True}
-        autoscale = AutoScale(min_workers=0, max_workers=1)
-        attributes = ClusterAttributes(cluster_name="my-cluster",
-                                    spark_version="7.2.x-scala2.12",
-                                    node_type_id="Standard_D3_v2",
-                                    spark_conf=spark_conf,
-                                    autoscale=autoscale)
-        created = client.clusters.create(attributes)
-        print(created.cluster_id)
-        ```
-        
-        ## Beloved Features
-        
-        **azure-databricks-sdk-python** is ready for your use-case:
-        
-        - Clear standard to access to APIs.
-        - Contains custom types for the API results and requests.
-        - Support for Personal Access token authentification.
-        - Support for Azure AD authentification.
-        - Support for the use of Azure AD service principals.
-        - Allows free-style API calls with a force mode -(bypass types validation).
-        - Error handeling and proxy support.
-        
-        Officially supports 3.6+, and runs great on PyPy.
-        
-        ## Implementation Progress
-        
-        Please refer to the progress below:
-        
-        | Feature  | Progress |
-        | :--- | :---: | 
-        | Authentification | 100% ✔ |
-        | Custom types | 25% |
-        | API Wrappers | 25% |
-        | Error handling | 80% |
-        | Proxy support | 0% |
-        | Documentation | 20% |
-        
-        As for specific API wrappers:
-        
-        | API  | Progress |
-        | :--- | :---: | 
-        | Clusters API | 100% ✔ |
-        | Secrets API | 100% ✔ |
-        | Token API | 100% ✔ |
-        | Jobs API | 0% |
-        | DBFS API  | 0% |
-        | Groups API  | 0% |
-        | Libraries API | 0% |
-        | Workspace API | 0% |
-        | Clusters Policies API | 0% |
-        | Instance Pools API | 0% |
-        | MLflow API | 0% |
-        | Permissions API | 0% |
-        | SCIM API | 0% |
-        | Token Management API | 0% |
-        
-        ## Documentation
-        
-        Check the documentation on [readthedocs.org](https://azure-databricks-sdk-python.readthedocs.io/en/latest/).
-        
-        ---
-        
-        
 Keywords: azure,databricks
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# Azure Databricks SDK Python
+
+> **Warning**
+> This project has been archived and is no longer actively maintained or supported. We highly recommend migrating to the official Databricks SDK for Python available at https://github.com/databricks/databricks-sdk-py.
+
+[![Workflow Status](https://img.shields.io/github/workflow/status/aminekaabachi/azure-databricks-sdk-python/Unit%20Tests/master?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/actions?query=workflow%3A%22Unit+Tests%22)
+[![Coveralls github](https://img.shields.io/coveralls/github/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://coveralls.io/github/aminekaabachi/azure-databricks-sdk-python?branch=master)
+[![PyPI](https://img.shields.io/pypi/v/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
+[![Downloads](https://img.shields.io/pypi/dm/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
+[![Docs](https://readthedocs.org/projects/azure-databricks-sdk-python/badge/?version=latest&style=flat-square)](https://azure-databricks-sdk-python.readthedocs.io/en/latest/)
+[![GitHub](https://img.shields.io/github/license/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/blob/master/LICENSE)
+
+**azure-databricks-sdk-python** is a Python SDK for the [`Azure Databricks REST API 2.0`](https://docs.microsoft.com/en-gb/azure/databricks/dev-tools/api/latest/).
+
+---
+
+Easily, perform all the operations as if on the Databricks UI:
+
+```python
+from azure_databricks_sdk_python import Client
+from azure_databricks_sdk_python.types.clusters import AutoScale, ClusterAttributes
+
+client = Client(databricks_instance="<instance>", personal_access_token="<token>")
+spark_conf = {'spark.speculation': True}
+autoscale = AutoScale(min_workers=0, max_workers=1)
+attributes = ClusterAttributes(cluster_name="my-cluster",
+                            spark_version="7.2.x-scala2.12",
+                            node_type_id="Standard_D3_v2",
+                            spark_conf=spark_conf,
+                            autoscale=autoscale)
+created = client.clusters.create(attributes)
+print(created.cluster_id)
+```
+
+## Beloved Features
+
+**azure-databricks-sdk-python** is ready for your use-case:
+
+- Clear standard to access to APIs.
+- Contains custom types for the API results and requests.
+- Support for Personal Access token authentification.
+- Support for Azure AD authentification.
+- Support for the use of Azure AD service principals.
+- Allows free-style API calls with a force mode -(bypass types validation).
+- Error handeling and proxy support.
+
+Officially supports 3.6+, and runs great on PyPy.
+
+## Implementation Progress
+
+Please refer to the progress below:
+
+| Feature          | Progress |
+| :--------------- | :------: |
+| Authentification |  100% ✔  |
+| Custom types     |   25%    |
+| API Wrappers     |   25%    |
+| Error handling   |   80%    |
+| Proxy support    |    0%    |
+| Documentation    |   20%    |
+
+As for specific API wrappers:
+
+| API                   | Progress |
+| :-------------------- | :------: |
+| Clusters API          |  100% ✔  |
+| Secrets API           |  100% ✔  |
+| Token API             |  100% ✔  |
+| Jobs API              |    0%    |
+| DBFS API              |    0%    |
+| Groups API            |    0%    |
+| Libraries API         |    0%    |
+| Workspace API         |    0%    |
+| Clusters Policies API |    0%    |
+| Instance Pools API    |    0%    |
+| MLflow API            |    0%    |
+| Permissions API       |    0%    |
+| SCIM API              |    0%    |
+| Token Management API  |    0%    |
+
+## Documentation
+
+Check the documentation on [readthedocs.org](https://azure-databricks-sdk-python.readthedocs.io/en/latest/).
+
+---
+
```

### Comparing `azure-databricks-sdk-python-0.0.2/README.md` & `azure-databricks-sdk-python-0.0.4.dev1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Azure Databricks SDK Python
 
+> **Warning**
+> This project has been archived and is no longer actively maintained or supported. We highly recommend migrating to the official Databricks SDK for Python available at https://github.com/databricks/databricks-sdk-py.
+
 [![Workflow Status](https://img.shields.io/github/workflow/status/aminekaabachi/azure-databricks-sdk-python/Unit%20Tests/master?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/actions?query=workflow%3A%22Unit+Tests%22)
 [![Coveralls github](https://img.shields.io/coveralls/github/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://coveralls.io/github/aminekaabachi/azure-databricks-sdk-python?branch=master)
 [![PyPI](https://img.shields.io/pypi/v/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
 [![Downloads](https://img.shields.io/pypi/dm/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
 [![Docs](https://readthedocs.org/projects/azure-databricks-sdk-python/badge/?version=latest&style=flat-square)](https://azure-databricks-sdk-python.readthedocs.io/en/latest/)
 [![GitHub](https://img.shields.io/github/license/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/blob/master/LICENSE)
 
+**azure-databricks-sdk-python** is a Python SDK for the [`Azure Databricks REST API 2.0`](https://docs.microsoft.com/en-gb/azure/databricks/dev-tools/api/latest/).
 
-**azure-databricks-sdk-python** is a Python SDK for the [`Azure Databricks REST API 2.0`](<https://docs.microsoft.com/en-gb/azure/databricks/dev-tools/api/latest/>).
-
------------------
+---
 
 Easily, perform all the operations as if on the Databricks UI:
+
 ```python
 from azure_databricks_sdk_python import Client
 from azure_databricks_sdk_python.types.clusters import AutoScale, ClusterAttributes
 
 client = Client(databricks_instance="<instance>", personal_access_token="<token>")
 spark_conf = {'spark.speculation': True}
 autoscale = AutoScale(min_workers=0, max_workers=1)
@@ -43,40 +46,40 @@
 
 Officially supports 3.6+, and runs great on PyPy.
 
 ## Implementation Progress
 
 Please refer to the progress below:
 
-| Feature  | Progress |
-| :--- | :---: | 
-| Authentification | 100% ✔ |
-| Custom types | 25% |
-| API Wrappers | 25% |
-| Error handling | 80% |
-| Proxy support | 0% |
-| Documentation | 20% |
+| Feature          | Progress |
+| :--------------- | :------: |
+| Authentification |  100% ✔  |
+| Custom types     |   25%    |
+| API Wrappers     |   25%    |
+| Error handling   |   80%    |
+| Proxy support    |    0%    |
+| Documentation    |   20%    |
 
 As for specific API wrappers:
 
-| API  | Progress |
-| :--- | :---: | 
-| Clusters API | 100% ✔ |
-| Secrets API | 100% ✔ |
-| Token API | 100% ✔ |
-| Jobs API | 0% |
-| DBFS API  | 0% |
-| Groups API  | 0% |
-| Libraries API | 0% |
-| Workspace API | 0% |
-| Clusters Policies API | 0% |
-| Instance Pools API | 0% |
-| MLflow API | 0% |
-| Permissions API | 0% |
-| SCIM API | 0% |
-| Token Management API | 0% |
+| API                   | Progress |
+| :-------------------- | :------: |
+| Clusters API          |  100% ✔  |
+| Secrets API           |  100% ✔  |
+| Token API             |  100% ✔  |
+| Jobs API              |    0%    |
+| DBFS API              |    0%    |
+| Groups API            |    0%    |
+| Libraries API         |    0%    |
+| Workspace API         |    0%    |
+| Clusters Policies API |    0%    |
+| Instance Pools API    |    0%    |
+| MLflow API            |    0%    |
+| Permissions API       |    0%    |
+| SCIM API              |    0%    |
+| Token Management API  |    0%    |
 
 ## Documentation
 
 Check the documentation on [readthedocs.org](https://azure-databricks-sdk-python.readthedocs.io/en/latest/).
 
 ---
```

### Comparing `azure-databricks-sdk-python-0.0.2/azure_databricks_sdk_python.egg-info/PKG-INFO` & `azure-databricks-sdk-python-0.0.4.dev1/azure_databricks_sdk_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,107 @@
 Metadata-Version: 2.1
 Name: azure-databricks-sdk-python
-Version: 0.0.2
+Version: 0.0.4.dev1
 Summary: A Python SDK for the Azure Databricks REST API 2.0.
 Home-page: http://github.com/aminekaabachi/azure-databricks-sdk-python
 Author: Amine Kaabachi
 Author-email: ping@kaabachi.io
 Maintainer: Amine Kaabachi
 Maintainer-email: ping@kaabachi.io
 License: MIT
-Description: # Azure Databricks SDK Python
-        
-        [![Workflow Status](https://img.shields.io/github/workflow/status/aminekaabachi/azure-databricks-sdk-python/Unit%20Tests/master?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/actions?query=workflow%3A%22Unit+Tests%22)
-        [![Coveralls github](https://img.shields.io/coveralls/github/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://coveralls.io/github/aminekaabachi/azure-databricks-sdk-python?branch=master)
-        [![PyPI](https://img.shields.io/pypi/v/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
-        [![Downloads](https://img.shields.io/pypi/dm/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
-        [![Docs](https://readthedocs.org/projects/azure-databricks-sdk-python/badge/?version=latest&style=flat-square)](https://azure-databricks-sdk-python.readthedocs.io/en/latest/)
-        [![GitHub](https://img.shields.io/github/license/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/blob/master/LICENSE)
-        
-        
-        **azure-databricks-sdk-python** is a Python SDK for the [`Azure Databricks REST API 2.0`](<https://docs.microsoft.com/en-gb/azure/databricks/dev-tools/api/latest/>).
-        
-        -----------------
-        
-        Easily, perform all the operations as if on the Databricks UI:
-        ```python
-        from azure_databricks_sdk_python import Client
-        from azure_databricks_sdk_python.types.clusters import AutoScale, ClusterAttributes
-        
-        client = Client(databricks_instance="<instance>", personal_access_token="<token>")
-        spark_conf = {'spark.speculation': True}
-        autoscale = AutoScale(min_workers=0, max_workers=1)
-        attributes = ClusterAttributes(cluster_name="my-cluster",
-                                    spark_version="7.2.x-scala2.12",
-                                    node_type_id="Standard_D3_v2",
-                                    spark_conf=spark_conf,
-                                    autoscale=autoscale)
-        created = client.clusters.create(attributes)
-        print(created.cluster_id)
-        ```
-        
-        ## Beloved Features
-        
-        **azure-databricks-sdk-python** is ready for your use-case:
-        
-        - Clear standard to access to APIs.
-        - Contains custom types for the API results and requests.
-        - Support for Personal Access token authentification.
-        - Support for Azure AD authentification.
-        - Support for the use of Azure AD service principals.
-        - Allows free-style API calls with a force mode -(bypass types validation).
-        - Error handeling and proxy support.
-        
-        Officially supports 3.6+, and runs great on PyPy.
-        
-        ## Implementation Progress
-        
-        Please refer to the progress below:
-        
-        | Feature  | Progress |
-        | :--- | :---: | 
-        | Authentification | 100% ✔ |
-        | Custom types | 25% |
-        | API Wrappers | 25% |
-        | Error handling | 80% |
-        | Proxy support | 0% |
-        | Documentation | 20% |
-        
-        As for specific API wrappers:
-        
-        | API  | Progress |
-        | :--- | :---: | 
-        | Clusters API | 100% ✔ |
-        | Secrets API | 100% ✔ |
-        | Token API | 100% ✔ |
-        | Jobs API | 0% |
-        | DBFS API  | 0% |
-        | Groups API  | 0% |
-        | Libraries API | 0% |
-        | Workspace API | 0% |
-        | Clusters Policies API | 0% |
-        | Instance Pools API | 0% |
-        | MLflow API | 0% |
-        | Permissions API | 0% |
-        | SCIM API | 0% |
-        | Token Management API | 0% |
-        
-        ## Documentation
-        
-        Check the documentation on [readthedocs.org](https://azure-databricks-sdk-python.readthedocs.io/en/latest/).
-        
-        ---
-        
-        
 Keywords: azure,databricks
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# Azure Databricks SDK Python
+
+> **Warning**
+> This project has been archived and is no longer actively maintained or supported. We highly recommend migrating to the official Databricks SDK for Python available at https://github.com/databricks/databricks-sdk-py.
+
+[![Workflow Status](https://img.shields.io/github/workflow/status/aminekaabachi/azure-databricks-sdk-python/Unit%20Tests/master?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/actions?query=workflow%3A%22Unit+Tests%22)
+[![Coveralls github](https://img.shields.io/coveralls/github/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://coveralls.io/github/aminekaabachi/azure-databricks-sdk-python?branch=master)
+[![PyPI](https://img.shields.io/pypi/v/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
+[![Downloads](https://img.shields.io/pypi/dm/azure-databricks-sdk-python?style=flat-square)](https://pypi.org/project/azure-databricks-sdk-python/)
+[![Docs](https://readthedocs.org/projects/azure-databricks-sdk-python/badge/?version=latest&style=flat-square)](https://azure-databricks-sdk-python.readthedocs.io/en/latest/)
+[![GitHub](https://img.shields.io/github/license/aminekaabachi/azure-databricks-sdk-python?style=flat-square)](https://github.com/aminekaabachi/azure-databricks-sdk-python/blob/master/LICENSE)
+
+**azure-databricks-sdk-python** is a Python SDK for the [`Azure Databricks REST API 2.0`](https://docs.microsoft.com/en-gb/azure/databricks/dev-tools/api/latest/).
+
+---
+
+Easily, perform all the operations as if on the Databricks UI:
+
+```python
+from azure_databricks_sdk_python import Client
+from azure_databricks_sdk_python.types.clusters import AutoScale, ClusterAttributes
+
+client = Client(databricks_instance="<instance>", personal_access_token="<token>")
+spark_conf = {'spark.speculation': True}
+autoscale = AutoScale(min_workers=0, max_workers=1)
+attributes = ClusterAttributes(cluster_name="my-cluster",
+                            spark_version="7.2.x-scala2.12",
+                            node_type_id="Standard_D3_v2",
+                            spark_conf=spark_conf,
+                            autoscale=autoscale)
+created = client.clusters.create(attributes)
+print(created.cluster_id)
+```
+
+## Beloved Features
+
+**azure-databricks-sdk-python** is ready for your use-case:
+
+- Clear standard to access to APIs.
+- Contains custom types for the API results and requests.
+- Support for Personal Access token authentification.
+- Support for Azure AD authentification.
+- Support for the use of Azure AD service principals.
+- Allows free-style API calls with a force mode -(bypass types validation).
+- Error handeling and proxy support.
+
+Officially supports 3.6+, and runs great on PyPy.
+
+## Implementation Progress
+
+Please refer to the progress below:
+
+| Feature          | Progress |
+| :--------------- | :------: |
+| Authentification |  100% ✔  |
+| Custom types     |   25%    |
+| API Wrappers     |   25%    |
+| Error handling   |   80%    |
+| Proxy support    |    0%    |
+| Documentation    |   20%    |
+
+As for specific API wrappers:
+
+| API                   | Progress |
+| :-------------------- | :------: |
+| Clusters API          |  100% ✔  |
+| Secrets API           |  100% ✔  |
+| Token API             |  100% ✔  |
+| Jobs API              |    0%    |
+| DBFS API              |    0%    |
+| Groups API            |    0%    |
+| Libraries API         |    0%    |
+| Workspace API         |    0%    |
+| Clusters Policies API |    0%    |
+| Instance Pools API    |    0%    |
+| MLflow API            |    0%    |
+| Permissions API       |    0%    |
+| SCIM API              |    0%    |
+| Token Management API  |    0%    |
+
+## Documentation
+
+Check the documentation on [readthedocs.org](https://azure-databricks-sdk-python.readthedocs.io/en/latest/).
+
+---
+
```

### Comparing `azure-databricks-sdk-python-0.0.2/docs/Makefile` & `azure-databricks-sdk-python-0.0.4.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/make.bat` & `azure-databricks-sdk-python-0.0.4.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/_static/custom.css` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/_templates/hacks.html` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/_templates/hacks.html`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/_templates/sidebar.html` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/_templates/sidebar.html`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/_themes/flask_theme_support.py` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/api.rst` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/conf.py` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/index.rst` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,18 @@
    sphinx-quickstart on Tue Sep 29 21:14:25 2020.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Azure Databricks SDK Python
 ===========================
 
+.. warning::
+    This project has been archived and is no longer actively maintained or supported. 
+    We highly recommend migrating to the official Databricks SDK for Python available at https://github.com/databricks/databricks-sdk-py.
+
 Release v\ |version|. (:ref:`Installation <install>`)
 
 .. image:: https://img.shields.io/github/workflow/status/aminekaabachi/azure-databricks-sdk-python/Unit%20Tests/master?style=flat-square
     :target: https://github.com/aminekaabachi/azure-databricks-sdk-python/actions?query=workflow%3A%22Unit+Tests%22
     
 .. image:: https://img.shields.io/coveralls/github/aminekaabachi/azure-databricks-sdk-python?style=flat-square
     :target: https://coveralls.io/github/aminekaabachi/azure-databricks-sdk-python?branch=master
```

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/user/advanced.rst` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/user/advanced.rst`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/user/install.rst` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/user/install.rst`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/docs/source/user/quickstart.rst` & `azure-databricks-sdk-python-0.0.4.dev1/docs/source/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/setup.cfg` & `azure-databricks-sdk-python-0.0.4.dev1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [metadata]
 name = azure-databricks-sdk-python
+version = 0.0.4
 author = Amine Kaabachi
 author-email = ping@kaabachi.io
 maintainer = Amine Kaabachi
 maintainer-email = ping@kaabachi.io
 summary = A Python SDK for the Azure Databricks REST API 2.0.
 description-file = README.md
 description-content-type = text/markdown
 home-page = http://github.com/aminekaabachi/azure-databricks-sdk-python
 license = MIT
 classifier = 
-	Development Status :: 3 - Alpha
-	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 keywords = azure,databricks
```

### Comparing `azure-databricks-sdk-python-0.0.2/tests/helpers.py` & `azure-databricks-sdk-python-0.0.4.dev1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/tests/test_client.py` & `azure-databricks-sdk-python-0.0.4.dev1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/tests/test_clusters.py` & `azure-databricks-sdk-python-0.0.4.dev1/tests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/tests/test_scopes.py` & `azure-databricks-sdk-python-0.0.4.dev1/tests/test_scopes.py`

 * *Files identical despite different names*

### Comparing `azure-databricks-sdk-python-0.0.2/tests/test_tokens.py` & `azure-databricks-sdk-python-0.0.4.dev1/tests/test_tokens.py`

 * *Files identical despite different names*


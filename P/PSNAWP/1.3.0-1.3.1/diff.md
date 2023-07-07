# Comparing `tmp/PSNAWP-1.3.0.tar.gz` & `tmp/PSNAWP-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSNAWP-1.3.0.tar", last modified: Sun Jul  2 05:18:28 2023, max compression
+gzip compressed data, was "PSNAWP-1.3.1.tar", last modified: Fri Jul  7 03:22:18 2023, max compression
```

## Comparing `PSNAWP-1.3.0.tar` & `PSNAWP-1.3.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.178672 PSNAWP-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.178672 PSNAWP-1.3.0/src/PSNAWP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/core/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/core/psnawp_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/game_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/models/listing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/listing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/listing/listing_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/listing/pagination_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/title_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/models/trophies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/psnawp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/utils/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/utils/request_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.134695 PSNAWP-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-07-07 03:22:18.134695 PSNAWP-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-07 03:22:18.134695 PSNAWP-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.126695 PSNAWP-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.130695 PSNAWP-1.3.1/src/PSNAWP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-07-07 03:22:18.000000 PSNAWP-1.3.1/src/PSNAWP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-07 03:22:18.000000 PSNAWP-1.3.1/src/PSNAWP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:22:18.000000 PSNAWP-1.3.1/src/PSNAWP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:22:18.000000 PSNAWP-1.3.1/src/PSNAWP.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-07 03:22:18.000000 PSNAWP-1.3.1/src/PSNAWP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 03:22:18.000000 PSNAWP-1.3.1/src/PSNAWP.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.130695 PSNAWP-1.3.1/src/psnawp_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.130695 PSNAWP-1.3.1/src/psnawp_api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/core/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/core/psnawp_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.130695 PSNAWP-1.3.1/src/psnawp_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/game_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.130695 PSNAWP-1.3.1/src/psnawp_api/models/listing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/listing/listing_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/listing/pagination_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/title_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.130695 PSNAWP-1.3.1/src/psnawp_api/models/trophies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/trophies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/trophies/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/psnawp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:18.134695 PSNAWP-1.3.1/src/psnawp_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/utils/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-07 03:22:07.000000 PSNAWP-1.3.1/src/psnawp_api/utils/request_builder.py
```

### Comparing `PSNAWP-1.3.0/LICENSE.md` & `PSNAWP-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/PKG-INFO` & `PSNAWP-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PSNAWP
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python API Wrapper for PlayStation Network API
 Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount)
 Author-email: trevorphillips@gmx.us
 License: MIT
 Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/issues
 Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/master/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PSNAWP Version: 1.3.0 Summary: Python API Wrapper
+Metadata-Version: 2.1 Name: PSNAWP Version: 1.3.1 Summary: Python API Wrapper
 for PlayStation Network API Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount) Author-email: trevorphillips@gmx.us
 License: MIT Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/
 issues Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/
 master/CHANGELOG.md Project-URL: Source Code, https://github.com/isFakeAccount/
 psnawp Project-URL: Documentation, https://psnawp.readthedocs.io/en/latest/
 Keywords: PSN API Platform: any Classifier: Development Status :: 4 - Beta
```

### Comparing `PSNAWP-1.3.0/README.md` & `PSNAWP-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/pyproject.toml` & `PSNAWP-1.3.1/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
 [tool.black]
-line-length = 160
+line-length = 160
```

### Comparing `PSNAWP-1.3.0/requirements.txt` & `PSNAWP-1.3.1/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile
 #
-attrs==22.2.0
+attrs==23.1.0
     # via PSNAWP (setup.py)
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   PSNAWP (setup.py)
     #   requests
 chardet==5.1.0
     # via PSNAWP (setup.py)
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via
     #   PSNAWP (setup.py)
     #   requests
 idna==3.4
     # via
     #   PSNAWP (setup.py)
     #   requests
-requests==2.28.2
+requests==2.31.0
     # via PSNAWP (setup.py)
-urllib3==1.26.14
+urllib3==1.26.16
     # via
     #   PSNAWP (setup.py)
     #   requests
```

### Comparing `PSNAWP-1.3.0/requirements_dev.txt` & `PSNAWP-1.3.1/requirements_dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,179 +1,180 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --output-file=requirements_dev.txt --resolver=backtracking requirements_dev.in
 #
 alabaster==0.7.13
     # via sphinx
-attrs==22.2.0
-    # via
-    #   -r requirements_dev.in
-    #   pytest
-babel==2.11.0
+attrs==23.1.0
+    # via -r requirements_dev.in
+babel==2.12.1
     # via sphinx
 bleach==6.0.0
     # via readme-renderer
 build==0.10.0
     # via
     #   -r requirements_dev.in
     #   pip-tools
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -r requirements_dev.in
     #   requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 chardet==5.1.0
     # via -r requirements_dev.in
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
-click==8.1.3
+click==8.1.4
     # via pip-tools
-coverage[toml]==7.1.0
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==39.0.1
+cryptography==41.0.1
     # via secretstorage
 distlib==0.3.6
     # via virtualenv
-docutils==0.18.1
+docutils==0.20.1
     # via
     #   myst-parser
     #   readme-renderer
     #   sphinx
-exceptiongroup==1.1.0
+exceptiongroup==1.1.2
     # via pytest
-filelock==3.9.0
+filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via -r requirements_dev.in
-identify==2.5.17
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   -r requirements_dev.in
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.0.0
+importlib-metadata==6.7.0
     # via
     #   keyring
+    #   sphinx
     #   twine
+importlib-resources==5.12.0
+    # via keyring
 iniconfig==2.0.0
     # via pytest
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
     # via
     #   myst-parser
     #   sphinx
-keyring==23.13.1
+keyring==24.2.0
     # via twine
-markdown-it-py==2.1.0
+markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
     #   rich
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 mccabe==0.7.0
     # via flake8
-mdit-py-plugins==0.3.3
+mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via jaraco-classes
 multidict==6.0.4
     # via yarl
-mypy==1.0.0
+mypy==1.4.1
     # via -r requirements_dev.in
 mypy-extensions==1.0.0
     # via mypy
-myst-parser==0.18.1
+myst-parser==2.0.0
     # via -r requirements_dev.in
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via
     #   build
     #   pytest
     #   sphinx
-pip-tools==6.12.2
+pip-tools==6.14.0
     # via -r requirements_dev.in
 pkginfo==1.9.6
     # via twine
-platformdirs==3.0.0
+platformdirs==3.8.1
     # via virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-pre-commit==3.0.4
+pre-commit==3.3.3
     # via -r requirements_dev.in
 pycodestyle==2.10.0
     # via flake8
 pycparser==2.21
     # via cffi
 pyflakes==3.0.1
     # via flake8
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
     #   sphinx
 pyproject-hooks==1.0.0
     # via build
-pytest==7.2.1
+pytest==7.4.0
     # via
     #   -r requirements_dev.in
     #   pytest-cov
     #   pytest-vcr
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via -r requirements_dev.in
 pytest-vcr==1.0.2
     # via -r requirements_dev.in
-python-dotenv==0.21.1
+python-dotenv==1.0.0
     # via -r requirements_dev.in
-pytz==2022.7.1
+pytz==2023.3
     # via babel
 pyyaml==6.0
     # via
     #   myst-parser
     #   pre-commit
     #   vcrpy
-readme-renderer==37.3
+readme-renderer==40.0
     # via twine
-requests==2.28.2
+requests==2.31.0
     # via
     #   -r requirements_dev.in
     #   requests-toolbelt
     #   sphinx
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.1
+rich==13.4.2
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via
     #   bleach
     #   vcrpy
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==5.3.0
+sphinx==7.0.1
     # via
     #   -r requirements_dev.in
     #   myst-parser
 sphinx-materialdesign-theme==0.1.11
     # via -r requirements_dev.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
@@ -188,46 +189,50 @@
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 tomli==2.0.1
     # via
     #   build
     #   coverage
     #   mypy
+    #   pip-tools
     #   pyproject-hooks
     #   pytest
 twine==4.0.2
     # via -r requirements_dev.in
 types-attrs==19.1.0
     # via -r requirements_dev.in
-types-requests==2.28.11.12
+types-requests==2.31.0.1
     # via -r requirements_dev.in
-types-urllib3==1.26.25.5
+types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.4.0
+typing-extensions==4.7.1
     # via
     #   mypy
-    #   myst-parser
-urllib3==1.26.14
+    #   rich
+urllib3==1.26.16
     # via
     #   -r requirements_dev.in
     #   requests
     #   twine
-vcrpy==4.2.1
+    #   vcrpy
+vcrpy==5.0.0
     # via
     #   -r requirements_dev.in
     #   pytest-vcr
-virtualenv==20.19.0
+virtualenv==20.23.1
     # via pre-commit
 webencodings==0.5.1
     # via bleach
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
-wrapt==1.14.1
+wrapt==1.15.0
     # via vcrpy
-yarl==1.8.2
+yarl==1.9.2
     # via vcrpy
-zipp==3.13.0
-    # via importlib-metadata
+zipp==3.15.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `PSNAWP-1.3.0/setup.cfg` & `PSNAWP-1.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PSNAWP
-version = 1.3.0
+version = 1.3.1
 author = Yoshikage Kira (@isFakeAccount)
 author_email = trevorphillips@gmx.us
 url = https://github.com/isFakeAccount/psnawp
 description = Python API Wrapper for PlayStation Network API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `PSNAWP-1.3.0/src/PSNAWP.egg-info/PKG-INFO` & `PSNAWP-1.3.1/src/PSNAWP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PSNAWP
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python API Wrapper for PlayStation Network API
 Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount)
 Author-email: trevorphillips@gmx.us
 License: MIT
 Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/issues
 Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/master/CHANGELOG.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PSNAWP Version: 1.3.0 Summary: Python API Wrapper
+Metadata-Version: 2.1 Name: PSNAWP Version: 1.3.1 Summary: Python API Wrapper
 for PlayStation Network API Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount) Author-email: trevorphillips@gmx.us
 License: MIT Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/
 issues Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/
 master/CHANGELOG.md Project-URL: Source Code, https://github.com/isFakeAccount/
 psnawp Project-URL: Documentation, https://psnawp.readthedocs.io/en/latest/
 Keywords: PSN API Platform: any Classifier: Development Status :: 4 - Beta
```

### Comparing `PSNAWP-1.3.0/src/PSNAWP.egg-info/SOURCES.txt` & `PSNAWP-1.3.1/src/PSNAWP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/PSNAWP.egg-info/requires.txt` & `PSNAWP-1.3.1/src/PSNAWP.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,98 +1,99 @@
-attrs==22.2.0
-certifi==2022.12.7
+attrs==23.1.0
+certifi==2023.5.7
 chardet==5.1.0
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
 idna==3.4
-requests==2.28.2
-urllib3==1.26.14
+requests==2.31.0
+urllib3==1.26.16
 
 [docs]
 sphinx==7.0.1
 sphinx-materialdesign-theme==0.1.11
 
 [testing]
 alabaster==0.7.13
-attrs==22.2.0
-babel==2.11.0
+attrs==23.1.0
+babel==2.12.1
 bleach==6.0.0
 build==0.10.0
-certifi==2022.12.7
+certifi==2023.5.7
 cffi==1.15.1
 cfgv==3.3.1
 chardet==5.1.0
-charset-normalizer==3.0.1
-click==8.1.3
-coverage[toml]==7.1.0
-cryptography==39.0.1
+charset-normalizer==3.1.0
+click==8.1.4
+coverage[toml]==7.2.7
+cryptography==41.0.1
 distlib==0.3.6
-docutils==0.18.1
-exceptiongroup==1.1.0
-filelock==3.9.0
+docutils==0.20.1
+exceptiongroup==1.1.2
+filelock==3.12.2
 flake8==6.0.0
-identify==2.5.17
+identify==2.5.24
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.0.0
+importlib-metadata==6.7.0
+importlib-resources==5.12.0
 iniconfig==2.0.0
 jaraco-classes==3.2.3
 jeepney==0.8.0
 jinja2==3.1.2
-keyring==23.13.1
-markdown-it-py==2.1.0
-markupsafe==2.1.2
+keyring==24.2.0
+markdown-it-py==3.0.0
+markupsafe==2.1.3
 mccabe==0.7.0
-mdit-py-plugins==0.3.3
+mdit-py-plugins==0.4.0
 mdurl==0.1.2
-more-itertools==9.0.0
+more-itertools==9.1.0
 multidict==6.0.4
-mypy==1.0.0
+mypy==1.4.1
 mypy-extensions==1.0.0
-myst-parser==0.18.1
-nodeenv==1.7.0
-packaging==23.0
-pip-tools==6.12.2
+myst-parser==2.0.0
+nodeenv==1.8.0
+packaging==23.1
+pip-tools==6.14.0
 pkginfo==1.9.6
-platformdirs==3.0.0
-pluggy==1.0.0
-pre-commit==3.0.4
+platformdirs==3.8.1
+pluggy==1.2.0
+pre-commit==3.3.3
 pycodestyle==2.10.0
 pycparser==2.21
 pyflakes==3.0.1
-pygments==2.14.0
+pygments==2.15.1
 pyproject-hooks==1.0.0
-pytest==7.2.1
-pytest-cov==4.0.0
+pytest==7.4.0
+pytest-cov==4.1.0
 pytest-vcr==1.0.2
-python-dotenv==0.21.1
-pytz==2022.7.1
+python-dotenv==1.0.0
+pytz==2023.3
 pyyaml==6.0
-readme-renderer==37.3
-requests==2.28.2
-requests-toolbelt==0.10.1
+readme-renderer==40.0
+requests==2.31.0
+requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.3.1
+rich==13.4.2
 secretstorage==3.3.3
 six==1.16.0
 snowballstemmer==2.2.0
-sphinx==5.3.0
+sphinx==7.0.1
 sphinx-materialdesign-theme==0.1.11
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 tomli==2.0.1
 twine==4.0.2
 types-attrs==19.1.0
-types-requests==2.28.11.12
-types-urllib3==1.26.25.5
-typing-extensions==4.4.0
-urllib3==1.26.14
-vcrpy==4.2.1
-virtualenv==20.19.0
+types-requests==2.31.0.1
+types-urllib3==1.26.25.13
+typing-extensions==4.7.1
+urllib3==1.26.16
+vcrpy==5.0.0
+virtualenv==20.23.1
 webencodings==0.5.1
-wheel==0.38.4
-wrapt==1.14.1
-yarl==1.8.2
-zipp==3.13.0
+wheel==0.40.0
+wrapt==1.15.0
+yarl==1.9.2
+zipp==3.15.0
```

### Comparing `PSNAWP-1.3.0/src/psnawp_api/core/authenticator.py` & `PSNAWP-1.3.1/src/psnawp_api/core/authenticator.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/core/psnawp_exceptions.py` & `PSNAWP-1.3.1/src/psnawp_api/core/psnawp_exceptions.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/client.py` & `PSNAWP-1.3.1/src/psnawp_api/models/client.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/game_title.py` & `PSNAWP-1.3.1/src/psnawp_api/models/game_title.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/group.py` & `PSNAWP-1.3.1/src/psnawp_api/models/group.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/listing/listing_generator.py` & `PSNAWP-1.3.1/src/psnawp_api/models/listing/listing_generator.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/listing/pagination_arguments.py` & `PSNAWP-1.3.1/src/psnawp_api/models/listing/pagination_arguments.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/search.py` & `PSNAWP-1.3.1/src/psnawp_api/models/search.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/title_stats.py` & `PSNAWP-1.3.1/src/psnawp_api/models/title_stats.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy.py` & `PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_constants.py` & `PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy_constants.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_group.py` & `PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy_group.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_summary.py` & `PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy_summary.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_titles.py` & `PSNAWP-1.3.1/src/psnawp_api/models/trophies/trophy_titles.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/models/user.py` & `PSNAWP-1.3.1/src/psnawp_api/models/user.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/psnawp.py` & `PSNAWP-1.3.1/src/psnawp_api/psnawp.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/utils/endpoints.py` & `PSNAWP-1.3.1/src/psnawp_api/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/utils/misc.py` & `PSNAWP-1.3.1/src/psnawp_api/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.3.0/src/psnawp_api/utils/request_builder.py` & `PSNAWP-1.3.1/src/psnawp_api/utils/request_builder.py`

 * *Files identical despite different names*


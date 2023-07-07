# Comparing `tmp/bchmnn.poodle-0.0.8.tar.gz` & `tmp/bchmnn.poodle-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bchmnn.poodle-0.0.8.tar", last modified: Fri Jul  7 15:54:43 2023, max compression
+gzip compressed data, was "bchmnn.poodle-0.0.9.tar", last modified: Fri Jul  7 16:01:28 2023, max compression
```

## Comparing `bchmnn.poodle-0.0.8.tar` & `bchmnn.poodle-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:54:43.661221 bchmnn.poodle-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.653221 bchmnn.poodle-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/src/bchmnn.poodle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-07-07 15:54:43.000000 bchmnn.poodle-0.0.8/src/bchmnn.poodle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-07 15:54:43.000000 bchmnn.poodle-0.0.8/src/bchmnn.poodle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:54:43.000000 bchmnn.poodle-0.0.8/src/bchmnn.poodle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 15:54:43.000000 bchmnn.poodle-0.0.8/src/bchmnn.poodle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 15:54:43.000000 bchmnn.poodle-0.0.8/src/bchmnn.poodle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/src/poodle/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/src/poodle/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/src/poodle/auth/handler/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/auth/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/auth/handler/abstract_sso_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/auth/handler/browser_sso_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/src/poodle/auth/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/auth/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/auth/provider/cli_credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/auth/provider/credential_provider_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/auth/provider/generic_credential_provider_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/corews.py
--rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/poodle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/src/poodle/types/
--rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/courses.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/jsonable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/site.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/types/ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:54:43.657221 bchmnn.poodle-0.0.8/src/poodle/util/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/util/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/util/parse_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/util/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/util/url_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-07 15:54:22.000000 bchmnn.poodle-0.0.8/src/poodle/util/win_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.265920 bchmnn.poodle-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-07-07 16:01:28.265920 bchmnn.poodle-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:01:28.265920 bchmnn.poodle-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.261920 bchmnn.poodle-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.261920 bchmnn.poodle-0.0.9/src/bchmnn.poodle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-07-07 16:01:28.000000 bchmnn.poodle-0.0.9/src/bchmnn.poodle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-07 16:01:28.000000 bchmnn.poodle-0.0.9/src/bchmnn.poodle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:01:28.000000 bchmnn.poodle-0.0.9/src/bchmnn.poodle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 16:01:28.000000 bchmnn.poodle-0.0.9/src/bchmnn.poodle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 16:01:28.000000 bchmnn.poodle-0.0.9/src/bchmnn.poodle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.261920 bchmnn.poodle-0.0.9/src/poodle/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.261920 bchmnn.poodle-0.0.9/src/poodle/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.261920 bchmnn.poodle-0.0.9/src/poodle/auth/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/auth/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/auth/handler/abstract_sso_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/auth/handler/browser_sso_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.261920 bchmnn.poodle-0.0.9/src/poodle/auth/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/auth/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/auth/provider/cli_credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/auth/provider/credential_provider_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/auth/provider/generic_credential_provider_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/corews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/poodle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.265920 bchmnn.poodle-0.0.9/src/poodle/types/
+-rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/courses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/jsonable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/types/ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:01:28.265920 bchmnn.poodle-0.0.9/src/poodle/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/util/parse_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/util/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/util/url_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-07 16:01:01.000000 bchmnn.poodle-0.0.9/src/poodle/util/win_registry.py
```

### Comparing `bchmnn.poodle-0.0.8/LICENSE` & `bchmnn.poodle-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/PKG-INFO` & `bchmnn.poodle-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bchmnn.poodle
-Version: 0.0.8
+Version: 0.0.9
 Summary: Moodle SDK for python
 Author-email: Jacob Bachmann <jacob.bachmann@posteo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bchmnn.poodle-0.0.8/README.md` & `bchmnn.poodle-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/pyproject.toml` & `bchmnn.poodle-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bchmnn.poodle"
-version = "0.0.8"
+version = "0.0.9"
 description = "Moodle SDK for python"
 readme = "README.md"
 authors = [{ name = "Jacob Bachmann", email = "jacob.bachmann@posteo.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "pip-tools", "bumpver", "build", "twine"]
 
 [project.urls]
 Homepage = "https://github.com/bchmnn/poodle"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "feat: release v{new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `bchmnn.poodle-0.0.8/src/bchmnn.poodle.egg-info/PKG-INFO` & `bchmnn.poodle-0.0.9/src/bchmnn.poodle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bchmnn.poodle
-Version: 0.0.8
+Version: 0.0.9
 Summary: Moodle SDK for python
 Author-email: Jacob Bachmann <jacob.bachmann@posteo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bchmnn.poodle-0.0.8/src/bchmnn.poodle.egg-info/SOURCES.txt` & `bchmnn.poodle-0.0.9/src/bchmnn.poodle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/auth/handler/abstract_sso_handler.py` & `bchmnn.poodle-0.0.9/src/poodle/auth/handler/abstract_sso_handler.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/auth/handler/browser_sso_handler.py` & `bchmnn.poodle-0.0.9/src/poodle/auth/handler/browser_sso_handler.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/auth/provider/cli_credential_provider.py` & `bchmnn.poodle-0.0.9/src/poodle/auth/provider/cli_credential_provider.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/auth/provider/credential_provider_interface.py` & `bchmnn.poodle-0.0.9/src/poodle/auth/provider/credential_provider_interface.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/auth/provider/generic_credential_provider_interface.py` & `bchmnn.poodle-0.0.9/src/poodle/auth/provider/generic_credential_provider_interface.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/corews.py` & `bchmnn.poodle-0.0.9/src/poodle/corews.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/poodle.py` & `bchmnn.poodle-0.0.9/src/poodle/poodle.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/types/assign.py` & `bchmnn.poodle-0.0.9/src/poodle/types/assign.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/types/course.py` & `bchmnn.poodle-0.0.9/src/poodle/types/course.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/types/courses.py` & `bchmnn.poodle-0.0.9/src/poodle/types/courses.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/types/exception.py` & `bchmnn.poodle-0.0.9/src/poodle/types/exception.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/types/site.py` & `bchmnn.poodle-0.0.9/src/poodle/types/site.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/types/tag.py` & `bchmnn.poodle-0.0.9/src/poodle/types/tag.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/types/ws.py` & `bchmnn.poodle-0.0.9/src/poodle/types/ws.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/util/cache.py` & `bchmnn.poodle-0.0.9/src/poodle/util/cache.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/util/logging.py` & `bchmnn.poodle-0.0.9/src/poodle/util/logging.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/util/parse_form.py` & `bchmnn.poodle-0.0.9/src/poodle/util/parse_form.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/util/tokens.py` & `bchmnn.poodle-0.0.9/src/poodle/util/tokens.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/util/url_protocol.py` & `bchmnn.poodle-0.0.9/src/poodle/util/url_protocol.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.0.8/src/poodle/util/win_registry.py` & `bchmnn.poodle-0.0.9/src/poodle/util/win_registry.py`

 * *Files identical despite different names*


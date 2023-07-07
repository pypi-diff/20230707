# Comparing `tmp/ngmapi-0.0.1.tar.gz` & `tmp/ngmapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmapi-0.0.1.tar", last modified: Fri Jul  7 09:35:53 2023, max compression
+gzip compressed data, was "ngmapi-0.0.2.tar", last modified: Fri Jul  7 10:03:21 2023, max compression
```

## Comparing `ngmapi-0.0.1.tar` & `ngmapi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 09:35:53.048875 ngmapi-0.0.1/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 09:35:53.048649 ngmapi-0.0.1/PKG-INFO
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 09:35:53.045494 ngmapi-0.0.1/ngmapi/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 06:42:48.000000 ngmapi-0.0.1/ngmapi/__init__.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      258 2023-07-07 09:02:42.000000 ngmapi-0.0.1/ngmapi/__main__.py
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 09:35:53.048356 ngmapi-0.0.1/ngmapi.egg-info/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 09:35:53.000000 ngmapi-0.0.1/ngmapi.egg-info/PKG-INFO
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      234 2023-07-07 09:35:53.000000 ngmapi-0.0.1/ngmapi.egg-info/SOURCES.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-07-07 09:35:53.000000 ngmapi-0.0.1/ngmapi.egg-info/dependency_links.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       40 2023-07-07 09:35:53.000000 ngmapi-0.0.1/ngmapi.egg-info/entry_points.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       16 2023-07-07 09:35:53.000000 ngmapi-0.0.1/ngmapi.egg-info/requires.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        7 2023-07-07 09:35:53.000000 ngmapi-0.0.1/ngmapi.egg-info/top_level.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      527 2023-07-07 09:33:05.000000 ngmapi-0.0.1/pyproject.toml
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-07-07 09:35:53.048938 ngmapi-0.0.1/setup.cfg
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:03:21.201709 ngmapi-0.0.2/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 10:03:21.201410 ngmapi-0.0.2/PKG-INFO
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:03:21.198073 ngmapi-0.0.2/ngmapi/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 06:42:48.000000 ngmapi-0.0.2/ngmapi/__init__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      258 2023-07-07 09:46:14.000000 ngmapi-0.0.2/ngmapi/app.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       32 2023-07-07 09:46:31.000000 ngmapi-0.0.2/ngmapi/func.py
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:03:21.200476 ngmapi-0.0.2/ngmapi.egg-info/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      375 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      262 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       40 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/entry_points.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       24 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/requires.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        7 2023-07-07 10:03:21.000000 ngmapi-0.0.2/ngmapi.egg-info/top_level.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      542 2023-07-07 10:01:41.000000 ngmapi-0.0.2/pyproject.toml
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-07-07 10:03:21.201800 ngmapi-0.0.2/setup.cfg
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-07-07 10:03:21.200850 ngmapi-0.0.2/tests/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      285 2023-07-07 09:46:42.000000 ngmapi-0.0.2/tests/test_add.py
```

### Comparing `ngmapi-0.0.1/pyproject.toml` & `ngmapi-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "ngmapi"
-version = "0.0.1"
+version = "0.0.2"
 description = "Just a demo project"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["flask", "project"]
 dependencies = [
-    "requests",
-    "psutil"
+    "Flask",
+    "Jinja2",
+    "MarkupSafe"
 ]
 
 [project.urls]
 Homepage = "https://github.com/ngmaibulat/training-flask"
 Documentation = "https://github.com/ngmaibulat/training-flask"
 Changes = "https://github.com/ngmaibulat/training-flask"
```


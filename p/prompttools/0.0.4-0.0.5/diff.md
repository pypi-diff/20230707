# Comparing `tmp/prompttools-0.0.4.tar.gz` & `tmp/prompttools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompttools-0.0.4.tar", last modified: Thu Jul  6 17:06:43 2023, max compression
+gzip compressed data, was "prompttools-0.0.5.tar", last modified: Thu Jul  6 22:49:45 2023, max compression
```

## Comparing `prompttools-0.0.4.tar` & `prompttools-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 17:06:43.259367 prompttools-0.0.4/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:51:56.000000 prompttools-0.0.4/LICENSE
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5109 2023-07-06 17:06:43.259026 prompttools-0.0.4/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4508 2023-07-05 23:52:26.000000 prompttools-0.0.4/README.md
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 17:06:43.258366 prompttools-0.0.4/prompttools.egg-info/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5109 2023-07-06 17:06:43.000000 prompttools-0.0.4/prompttools.egg-info/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      278 2023-07-06 17:06:43.000000 prompttools-0.0.4/prompttools.egg-info/SOURCES.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 17:06:43.000000 prompttools-0.0.4/prompttools.egg-info/dependency_links.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-04 19:41:18.000000 prompttools-0.0.4/prompttools.egg-info/not-zip-safe
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-06 17:06:43.000000 prompttools-0.0.4/prompttools.egg-info/requires.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 17:06:43.000000 prompttools-0.0.4/prompttools.egg-info/top_level.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      698 2023-07-06 17:06:05.000000 prompttools-0.0.4/pyproject.toml
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-05 21:42:59.000000 prompttools-0.0.4/requirements.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-06 17:06:43.259477 prompttools-0.0.4/setup.cfg
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3737 2023-07-06 17:06:33.000000 prompttools-0.0.4/setup.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-06 17:05:54.000000 prompttools-0.0.4/version.txt
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 22:49:45.693602 prompttools-0.0.5/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:51:56.000000 prompttools-0.0.5/LICENSE
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5109 2023-07-06 22:49:45.693301 prompttools-0.0.5/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4508 2023-07-05 23:52:26.000000 prompttools-0.0.5/README.md
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 22:49:45.692923 prompttools-0.0.5/prompttools.egg-info/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5109 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      278 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/SOURCES.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/dependency_links.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-04 19:41:18.000000 prompttools-0.0.5/prompttools.egg-info/not-zip-safe
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/requires.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 22:49:45.000000 prompttools-0.0.5/prompttools.egg-info/top_level.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      698 2023-07-06 22:48:41.000000 prompttools-0.0.5/pyproject.toml
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-05 21:42:59.000000 prompttools-0.0.5/requirements.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-06 22:49:45.693707 prompttools-0.0.5/setup.cfg
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3737 2023-07-06 22:49:34.000000 prompttools-0.0.5/setup.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-06 22:48:45.000000 prompttools-0.0.5/version.txt
```

### Comparing `prompttools-0.0.4/LICENSE` & `prompttools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.4/PKG-INFO` & `prompttools-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompttools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for LLM prompt testing and experimentation
 Home-page: https://github.com/hegelai/prompttools
 Author: Hegel AI
 Author-email: Hegel AI <team@hegel-ai.com>
 License: Proprietary
 Project-URL: Homepage, https://github.com/hegelai/prompttools
 Project-URL: Bug Tracker, https://github.com/hegelai/prompttools
```

### Comparing `prompttools-0.0.4/README.md` & `prompttools-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `prompttools-0.0.4/prompttools.egg-info/PKG-INFO` & `prompttools-0.0.5/prompttools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompttools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for LLM prompt testing and experimentation
 Home-page: https://github.com/hegelai/prompttools
 Author: Hegel AI
 Author-email: Hegel AI <team@hegel-ai.com>
 License: Proprietary
 Project-URL: Homepage, https://github.com/hegelai/prompttools
 Project-URL: Bug Tracker, https://github.com/hegelai/prompttools
```

### Comparing `prompttools-0.0.4/pyproject.toml` & `prompttools-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prompttools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Hegel AI", email="team@hegel-ai.com" },
 ]
 description = "Tools for LLM prompt testing and experimentation"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `prompttools-0.0.4/setup.py` & `prompttools-0.0.5/setup.py`

 * *Files identical despite different names*


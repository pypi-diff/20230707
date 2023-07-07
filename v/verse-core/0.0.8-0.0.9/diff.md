# Comparing `tmp/verse-core-0.0.8.tar.gz` & `tmp/verse-core-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verse-core-0.0.8.tar", last modified: Sun May 21 06:11:09 2023, max compression
+gzip compressed data, was "verse-core-0.0.9.tar", last modified: Sat Jul  1 07:20:03 2023, max compression
```

## Comparing `verse-core-0.0.8.tar` & `verse-core-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 06:11:09.883575 verse-core-0.0.8/
--rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verse-core-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      593 2023-05-21 06:11:09.882581 verse-core-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-26 23:13:54.000000 verse-core-0.0.8/README.md
--rw-rw-rw-   0        0        0      660 2023-05-21 06:10:43.000000 verse-core-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 06:11:09.884573 verse-core-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 06:11:09.828720 verse-core-0.0.8/verse/
-drwxrwxrwx   0        0        0        0 2023-05-21 06:11:09.860637 verse-core-0.0.8/verse/core/
--rw-rw-rw-   0        0        0      127 2023-05-21 06:09:26.000000 verse-core-0.0.8/verse/core/__init__.py
--rw-rw-rw-   0        0        0      162 2023-04-26 23:17:00.000000 verse-core-0.0.8/verse/core/_async_helper.py
--rw-rw-rw-   0        0        0      402 2023-04-26 23:17:08.000000 verse-core-0.0.8/verse/core/_import_helper.py
--rw-rw-rw-   0        0        0      463 2023-05-08 23:41:13.000000 verse-core-0.0.8/verse/core/_model.py
--rw-rw-rw-   0        0        0      430 2023-05-19 03:25:38.000000 verse-core-0.0.8/verse/core/decorators.py
--rw-rw-rw-   0        0        0      296 2023-05-19 03:25:19.000000 verse-core-0.0.8/verse/core/exceptions.py
--rw-rw-rw-   0        0        0       26 2023-05-11 01:27:41.000000 verse-core-0.0.8/verse/core/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-21 06:11:09.881578 verse-core-0.0.8/verse_core.egg-info/
--rw-rw-rw-   0        0        0      593 2023-05-21 06:11:09.000000 verse-core-0.0.8/verse_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-21 06:11:09.000000 verse-core-0.0.8/verse_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 06:11:09.000000 verse-core-0.0.8/verse_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 06:11:09.000000 verse-core-0.0.8/verse_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 07:20:03.176278 verse-core-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verse-core-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      593 2023-07-01 07:20:03.175280 verse-core-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-26 23:13:54.000000 verse-core-0.0.9/README.md
+-rw-rw-rw-   0        0        0      660 2023-07-01 07:12:49.000000 verse-core-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 07:20:03.176278 verse-core-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 07:20:03.148352 verse-core-0.0.9/verse/
+-rw-rw-rw-   0        0        0      134 2023-07-01 07:14:55.000000 verse-core-0.0.9/verse/__init__.py
+-rw-rw-rw-   0        0        0      390 2023-06-29 22:27:59.000000 verse-core-0.0.9/verse/_action.py
+-rw-rw-rw-   0        0        0      564 2023-07-01 07:16:11.000000 verse-core-0.0.9/verse/_helpers.py
+-rw-rw-rw-   0        0        0      463 2023-05-08 23:41:13.000000 verse-core-0.0.9/verse/_model.py
+-rw-rw-rw-   0        0        0      992 2023-07-01 03:20:25.000000 verse-core-0.0.9/verse/_provider.py
+-rw-rw-rw-   0        0        0      217 2023-06-30 20:39:30.000000 verse-core-0.0.9/verse/_verse.py
+-rw-rw-rw-   0        0        0      430 2023-07-01 07:18:23.000000 verse-core-0.0.9/verse/decorators.py
+-rw-rw-rw-   0        0        0      296 2023-05-19 03:25:19.000000 verse-core-0.0.9/verse/exceptions.py
+-rw-rw-rw-   0        0        0       26 2023-05-11 01:27:41.000000 verse-core-0.0.9/verse/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-01 07:20:03.173287 verse-core-0.0.9/verse_core.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-07-01 07:20:03.000000 verse-core-0.0.9/verse_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-01 07:20:03.000000 verse-core-0.0.9/verse_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 07:20:03.000000 verse-core-0.0.9/verse_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-01 07:20:03.000000 verse-core-0.0.9/verse_core.egg-info/top_level.txt
```

### Comparing `verse-core-0.0.8/LICENSE` & `verse-core-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `verse-core-0.0.8/PKG-INFO` & `verse-core-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: verse-core
-Version: 0.0.8
+Version: 0.0.9
 Summary: Core Verse package shared by all Verse packages
-Author-email: Rapidverse <admin@rapidverse.com>
+Author-email: rapidverse <admin@rapidverse.com>
 Project-URL: Homepage, https://github.com/rapidverse/verse
 Project-URL: Bug Tracker, https://github.com/rapidverse/verse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `verse-core-0.0.8/pyproject.toml` & `verse-core-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "verse-core"
-version = "0.0.8"
-authors = [{ name = "Rapidverse", email = "admin@rapidverse.com" }]
+version = "0.0.9"
+authors = [{ name = "rapidverse", email = "admin@rapidverse.com" }]
 description = "Core Verse package shared by all Verse packages"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `verse-core-0.0.8/verse_core.egg-info/PKG-INFO` & `verse-core-0.0.9/verse_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: verse-core
-Version: 0.0.8
+Version: 0.0.9
 Summary: Core Verse package shared by all Verse packages
-Author-email: Rapidverse <admin@rapidverse.com>
+Author-email: rapidverse <admin@rapidverse.com>
 Project-URL: Homepage, https://github.com/rapidverse/verse
 Project-URL: Bug Tracker, https://github.com/rapidverse/verse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```


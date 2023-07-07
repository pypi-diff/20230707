# Comparing `tmp/ecallisto_ng-0.0.1.tar.gz` & `tmp/ecallisto_ng-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.0.1.tar", last modified: Thu Jul  6 20:20:21 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.0.2.tar", last modified: Thu Jul  6 21:10:54 2023, max compression
```

## Comparing `ecallisto_ng-0.0.1.tar` & `ecallisto_ng-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 20:20:21.848362 ecallisto_ng-0.0.1/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.1/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      595 2023-07-06 20:20:21.848362 ecallisto_ng-0.0.1/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       14 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.1/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      808 2023-07-06 18:07:47.000000 ecallisto_ng-0.0.1/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-06 20:20:21.848362 ecallisto_ng-0.0.1/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 20:20:21.848362 ecallisto_ng-0.0.1/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 20:20:21.848362 ecallisto_ng-0.0.1/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.1/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 20:20:21.848362 ecallisto_ng-0.0.1/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      946 2023-07-06 18:09:17.000000 ecallisto_ng-0.0.1/src/ecallisto_ng/data_fetching/get_data.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 20:20:21.848362 ecallisto_ng-0.0.1/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2172 2023-07-06 18:11:00.000000 ecallisto_ng-0.0.1/src/ecallisto_ng/plotting/plotting_utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 20:20:21.848362 ecallisto_ng-0.0.1/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      595 2023-07-06 20:20:21.000000 ecallisto_ng-0.0.1/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      347 2023-07-06 20:20:21.000000 ecallisto_ng-0.0.1/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-06 20:20:21.000000 ecallisto_ng-0.0.1/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       92 2023-07-06 20:20:21.000000 ecallisto_ng-0.0.1/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-06 20:20:21.000000 ecallisto_ng-0.0.1/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 21:10:54.455347 ecallisto_ng-0.0.2/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.0.2/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1615 2023-07-06 21:10:54.455347 ecallisto_ng-0.0.2/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1035 2023-07-06 20:56:31.000000 ecallisto_ng-0.0.2/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      808 2023-07-06 21:10:50.000000 ecallisto_ng-0.0.2/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-06 21:10:54.455347 ecallisto_ng-0.0.2/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 21:10:54.455347 ecallisto_ng-0.0.2/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 21:10:54.455347 ecallisto_ng-0.0.2/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.0.2/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 21:10:54.455347 ecallisto_ng-0.0.2/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      946 2023-07-06 18:09:17.000000 ecallisto_ng-0.0.2/src/ecallisto_ng/data_fetching/get_data.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 21:10:54.455347 ecallisto_ng-0.0.2/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2172 2023-07-06 18:11:00.000000 ecallisto_ng-0.0.2/src/ecallisto_ng/plotting/plotting_utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 21:10:54.455347 ecallisto_ng-0.0.2/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1615 2023-07-06 21:10:54.000000 ecallisto_ng-0.0.2/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      347 2023-07-06 21:10:54.000000 ecallisto_ng-0.0.2/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-06 21:10:54.000000 ecallisto_ng-0.0.2/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       92 2023-07-06 21:10:54.000000 ecallisto_ng-0.0.2/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-06 21:10:54.000000 ecallisto_ng-0.0.2/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.0.1/LICENSE` & `ecallisto_ng-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.1/pyproject.toml` & `ecallisto_ng-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.0.1/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.0.2/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.0.1/src/ecallisto_ng/plotting/plotting_utils.py` & `ecallisto_ng-0.0.2/src/ecallisto_ng/plotting/plotting_utils.py`

 * *Files identical despite different names*


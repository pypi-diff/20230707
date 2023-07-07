# Comparing `tmp/rateToolsAC4RM-0.42.tar.gz` & `tmp/rateToolsAC4RM-0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rateToolsAC4RM-0.42.tar", last modified: Fri Jul  7 21:27:22 2023, max compression
+gzip compressed data, was "rateToolsAC4RM-0.43.tar", last modified: Fri Jul  7 21:30:30 2023, max compression
```

## Comparing `rateToolsAC4RM-0.42.tar` & `rateToolsAC4RM-0.43.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:27:22.810855 rateToolsAC4RM-0.42/
--rw-r--r--   0 tleitch1   (501) staff       (20)      190 2023-07-07 21:27:22.810987 rateToolsAC4RM-0.42/PKG-INFO
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:27:22.807572 rateToolsAC4RM-0.42/rateToolsAC4RM/
--rw-rw-r--   0 tleitch1   (501) staff       (20)      412 2023-07-07 21:26:35.000000 rateToolsAC4RM-0.42/rateToolsAC4RM/__init__.py
--rw-r--r--   0 tleitch1   (501) staff       (20)     6789 2023-07-07 21:26:54.000000 rateToolsAC4RM-0.42/rateToolsAC4RM/rateTools.py
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:27:22.810504 rateToolsAC4RM-0.42/rateToolsAC4RM.egg-info/
--rw-r--r--   0 tleitch1   (501) staff       (20)      190 2023-07-07 21:27:22.000000 rateToolsAC4RM-0.42/rateToolsAC4RM.egg-info/PKG-INFO
--rw-r--r--   0 tleitch1   (501) staff       (20)      262 2023-07-07 21:27:22.000000 rateToolsAC4RM-0.42/rateToolsAC4RM.egg-info/SOURCES.txt
--rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-07-07 21:27:22.000000 rateToolsAC4RM-0.42/rateToolsAC4RM.egg-info/dependency_links.txt
--rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 03:42:27.000000 rateToolsAC4RM-0.42/rateToolsAC4RM.egg-info/not-zip-safe
--rw-r--r--   0 tleitch1   (501) staff       (20)       15 2023-07-07 21:27:22.000000 rateToolsAC4RM-0.42/rateToolsAC4RM.egg-info/top_level.txt
--rw-rw-r--   0 tleitch1   (501) staff       (20)       38 2023-07-07 21:27:22.811724 rateToolsAC4RM-0.42/setup.cfg
--rw-rw-r--   0 tleitch1   (501) staff       (20)      227 2023-07-07 21:26:46.000000 rateToolsAC4RM-0.42/setup.py
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:30:30.906724 rateToolsAC4RM-0.43/
+-rw-r--r--   0 tleitch1   (501) staff       (20)      190 2023-07-07 21:30:30.906854 rateToolsAC4RM-0.43/PKG-INFO
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:30:30.903058 rateToolsAC4RM-0.43/rateToolsAC4RM/
+-rw-rw-r--   0 tleitch1   (501) staff       (20)      442 2023-07-07 21:29:40.000000 rateToolsAC4RM-0.43/rateToolsAC4RM/__init__.py
+-rw-r--r--   0 tleitch1   (501) staff       (20)     6789 2023-07-07 21:26:54.000000 rateToolsAC4RM-0.43/rateToolsAC4RM/rateTools.py
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:30:30.906373 rateToolsAC4RM-0.43/rateToolsAC4RM.egg-info/
+-rw-r--r--   0 tleitch1   (501) staff       (20)      190 2023-07-07 21:30:30.000000 rateToolsAC4RM-0.43/rateToolsAC4RM.egg-info/PKG-INFO
+-rw-r--r--   0 tleitch1   (501) staff       (20)      262 2023-07-07 21:30:30.000000 rateToolsAC4RM-0.43/rateToolsAC4RM.egg-info/SOURCES.txt
+-rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-07-07 21:30:30.000000 rateToolsAC4RM-0.43/rateToolsAC4RM.egg-info/dependency_links.txt
+-rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 03:42:27.000000 rateToolsAC4RM-0.43/rateToolsAC4RM.egg-info/not-zip-safe
+-rw-r--r--   0 tleitch1   (501) staff       (20)       15 2023-07-07 21:30:30.000000 rateToolsAC4RM-0.43/rateToolsAC4RM.egg-info/top_level.txt
+-rw-rw-r--   0 tleitch1   (501) staff       (20)       38 2023-07-07 21:30:30.907650 rateToolsAC4RM-0.43/setup.cfg
+-rw-rw-r--   0 tleitch1   (501) staff       (20)      227 2023-07-07 21:29:55.000000 rateToolsAC4RM-0.43/setup.py
```

### Comparing `rateToolsAC4RM-0.42/rateToolsAC4RM/rateTools.py` & `rateToolsAC4RM-0.43/rateToolsAC4RM/rateTools.py`

 * *Files identical despite different names*


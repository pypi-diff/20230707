# Comparing `tmp/ncs-uml-1.0.1.tar.gz` & `tmp/ncs-uml-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncs-uml-1.0.1.tar", last modified: Fri Jun 30 21:49:16 2023, max compression
+gzip compressed data, was "ncs-uml-1.0.2.tar", last modified: Fri Jul  7 01:15:57 2023, max compression
```

## Comparing `ncs-uml-1.0.1.tar` & `ncs-uml-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 21:49:16.440384 ncs-uml-1.0.1/
--rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.0.1/LICENSE
--rw-r--r--   0 kkotari    (501) staff       (20)       75 2023-06-23 13:29:14.000000 ncs-uml-1.0.1/MANIFEST.in
--rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 21:49:16.440209 ncs-uml-1.0.1/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)        9 2023-06-23 13:12:35.000000 ncs-uml-1.0.1/README.md
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 21:49:16.438707 ncs-uml-1.0.1/ncs_uml/
--rw-r--r--   0 kkotari    (501) staff       (20)      248 2023-06-30 21:33:18.000000 ncs-uml-1.0.1/ncs_uml/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5545 2023-06-30 21:41:35.000000 ncs-uml-1.0.1/ncs_uml/main.py
--rw-r--r--   0 kkotari    (501) staff       (20)      960 2023-06-30 21:48:39.000000 ncs-uml-1.0.1/ncs_uml/run.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5981 2023-06-30 20:08:47.000000 ncs-uml-1.0.1/ncs_uml/utils.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 21:49:16.439977 ncs-uml-1.0.1/ncs_uml.egg-info/
--rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)      311 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/SOURCES.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/dependency_links.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       71 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/entry_points.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/requires.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/top_level.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.0.1/requirements.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-06-30 21:49:16.440439 ncs-uml-1.0.1/setup.cfg
--rw-r--r--   0 kkotari    (501) staff       (20)     1683 2023-06-30 20:23:16.000000 ncs-uml-1.0.1/setup.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-07 01:15:57.543233 ncs-uml-1.0.2/
+-rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.0.2/LICENSE
+-rw-r--r--   0 kkotari    (501) staff       (20)       75 2023-06-23 13:29:14.000000 ncs-uml-1.0.2/MANIFEST.in
+-rw-r--r--   0 kkotari    (501) staff       (20)    15076 2023-07-07 01:15:57.543012 ncs-uml-1.0.2/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)    14086 2023-07-07 01:13:56.000000 ncs-uml-1.0.2/README.md
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-07 01:15:57.541606 ncs-uml-1.0.2/ncs_uml/
+-rw-r--r--   0 kkotari    (501) staff       (20)      248 2023-07-07 01:15:08.000000 ncs-uml-1.0.2/ncs_uml/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5545 2023-06-30 21:41:35.000000 ncs-uml-1.0.2/ncs_uml/main.py
+-rw-r--r--   0 kkotari    (501) staff       (20)      960 2023-06-30 21:48:39.000000 ncs-uml-1.0.2/ncs_uml/run.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5981 2023-06-30 20:08:47.000000 ncs-uml-1.0.2/ncs_uml/utils.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-07 01:15:57.542766 ncs-uml-1.0.2/ncs_uml.egg-info/
+-rw-r--r--   0 kkotari    (501) staff       (20)    15076 2023-07-07 01:15:57.000000 ncs-uml-1.0.2/ncs_uml.egg-info/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)      311 2023-07-07 01:15:57.000000 ncs-uml-1.0.2/ncs_uml.egg-info/SOURCES.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-07-07 01:15:57.000000 ncs-uml-1.0.2/ncs_uml.egg-info/dependency_links.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       71 2023-07-07 01:15:57.000000 ncs-uml-1.0.2/ncs_uml.egg-info/entry_points.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-07-07 01:15:57.000000 ncs-uml-1.0.2/ncs_uml.egg-info/requires.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-07-07 01:15:57.000000 ncs-uml-1.0.2/ncs_uml.egg-info/top_level.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.0.2/requirements.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-07-07 01:15:57.543295 ncs-uml-1.0.2/setup.cfg
+-rw-r--r--   0 kkotari    (501) staff       (20)     1683 2023-06-30 20:23:16.000000 ncs-uml-1.0.2/setup.py
```

### Comparing `ncs-uml-1.0.1/LICENSE` & `ncs-uml-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.0.1/ncs_uml/main.py` & `ncs-uml-1.0.2/ncs_uml/main.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.0.1/ncs_uml/run.py` & `ncs-uml-1.0.2/ncs_uml/run.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.0.1/ncs_uml/utils.py` & `ncs-uml-1.0.2/ncs_uml/utils.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.0.1/setup.py` & `ncs-uml-1.0.2/setup.py`

 * *Files identical despite different names*


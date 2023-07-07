# Comparing `tmp/pyciactions-1.0.7.tar.gz` & `tmp/pyciactions-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyciactions-1.0.7.tar", last modified: Fri Jul  7 04:35:39 2023, max compression
+gzip compressed data, was "pyciactions-1.0.8.tar", last modified: Fri Jul  7 04:36:52 2023, max compression
```

## Comparing `pyciactions-1.0.7.tar` & `pyciactions-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:35:39.466953 pyciactions-1.0.7/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:35:39.464682 pyciactions-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:35:39.389610 pyciactions-1.0.7/pyciactions/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.7/pyciactions/IWorkflow.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-07-07 04:35:29.000000 pyciactions-1.0.7/pyciactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.7/pyciactions/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:35:39.452223 pyciactions-1.0.7/pyciactions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:35:39.000000 pyciactions-1.0.7/pyciactions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 04:35:39.000000 pyciactions-1.0.7/pyciactions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 04:35:39.000000 pyciactions-1.0.7/pyciactions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 04:35:39.000000 pyciactions-1.0.7/pyciactions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 04:35:39.000000 pyciactions-1.0.7/pyciactions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 04:35:39.467988 pyciactions-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      476 2023-07-07 04:35:35.000000 pyciactions-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:36:52.813140 pyciactions-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:36:52.810661 pyciactions-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:36:52.724533 pyciactions-1.0.8/pyciactions/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.8/pyciactions/IWorkflow.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-07 04:36:45.000000 pyciactions-1.0.8/pyciactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.8/pyciactions/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:36:52.797479 pyciactions-1.0.8/pyciactions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:36:52.000000 pyciactions-1.0.8/pyciactions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 04:36:52.000000 pyciactions-1.0.8/pyciactions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 04:36:52.000000 pyciactions-1.0.8/pyciactions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 04:36:52.000000 pyciactions-1.0.8/pyciactions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 04:36:52.000000 pyciactions-1.0.8/pyciactions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 04:36:52.814248 pyciactions-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-07 04:36:50.000000 pyciactions-1.0.8/setup.py
```

### Comparing `pyciactions-1.0.7/LICENSE` & `pyciactions-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.7/PKG-INFO` & `pyciactions-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.7
+Version: 1.0.8
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```

### Comparing `pyciactions-1.0.7/README.md` & `pyciactions-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.7/pyciactions.egg-info/PKG-INFO` & `pyciactions-1.0.8/pyciactions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.7
+Version: 1.0.8
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```


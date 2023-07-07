# Comparing `tmp/pyciactions-1.0.8a4.tar.gz` & `tmp/pyciactions-1.0.8a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyciactions-1.0.8a4.tar", last modified: Fri Jul  7 05:37:50 2023, max compression
+gzip compressed data, was "pyciactions-1.0.8a5.tar", last modified: Fri Jul  7 05:41:32 2023, max compression
```

## Comparing `pyciactions-1.0.8a4.tar` & `pyciactions-1.0.8a5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:37:50.326395 pyciactions-1.0.8a4/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.8a4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:37:50.324186 pyciactions-1.0.8a4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.8a4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:37:50.231192 pyciactions-1.0.8a4/pyciactions/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.8a4/pyciactions/IWorkflow.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-07 05:37:41.000000 pyciactions-1.0.8a4/pyciactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.8a4/pyciactions/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:37:50.309535 pyciactions-1.0.8a4/pyciactions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:37:50.000000 pyciactions-1.0.8a4/pyciactions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 05:37:50.000000 pyciactions-1.0.8a4/pyciactions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 05:37:50.000000 pyciactions-1.0.8a4/pyciactions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 05:37:50.000000 pyciactions-1.0.8a4/pyciactions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 05:37:50.000000 pyciactions-1.0.8a4/pyciactions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 05:37:50.326907 pyciactions-1.0.8a4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      483 2023-07-07 05:37:47.000000 pyciactions-1.0.8a4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:41:32.328534 pyciactions-1.0.8a5/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.8a5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:41:32.324865 pyciactions-1.0.8a5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.8a5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:41:32.225186 pyciactions-1.0.8a5/pyciactions/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.8a5/pyciactions/IWorkflow.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-07 05:41:22.000000 pyciactions-1.0.8a5/pyciactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.8a5/pyciactions/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:41:32.309471 pyciactions-1.0.8a5/pyciactions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:41:32.000000 pyciactions-1.0.8a5/pyciactions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 05:41:32.000000 pyciactions-1.0.8a5/pyciactions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 05:41:32.000000 pyciactions-1.0.8a5/pyciactions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 05:41:32.000000 pyciactions-1.0.8a5/pyciactions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 05:41:32.000000 pyciactions-1.0.8a5/pyciactions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 05:41:32.330173 pyciactions-1.0.8a5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      483 2023-07-07 05:41:27.000000 pyciactions-1.0.8a5/setup.py
```

### Comparing `pyciactions-1.0.8a4/LICENSE` & `pyciactions-1.0.8a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.8a4/PKG-INFO` & `pyciactions-1.0.8a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.8a4
+Version: 1.0.8a5
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```

### Comparing `pyciactions-1.0.8a4/README.md` & `pyciactions-1.0.8a5/README.md`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.8a4/pyciactions.egg-info/PKG-INFO` & `pyciactions-1.0.8a5/pyciactions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.8a4
+Version: 1.0.8a5
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```


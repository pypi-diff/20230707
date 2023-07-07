# Comparing `tmp/pyciactions-1.0.4.tar.gz` & `tmp/pyciactions-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyciactions-1.0.4.tar", last modified: Fri Jul  7 04:26:24 2023, max compression
+gzip compressed data, was "pyciactions-1.0.5.tar", last modified: Fri Jul  7 04:29:30 2023, max compression
```

## Comparing `pyciactions-1.0.4.tar` & `pyciactions-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:26:24.562614 pyciactions-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:26:24.560389 pyciactions-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:26:24.470350 pyciactions-1.0.4/pyciactions/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.4/pyciactions/IWorkflow.py
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-07 04:20:29.000000 pyciactions-1.0.4/pyciactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.4/pyciactions/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:26:24.546283 pyciactions-1.0.4/pyciactions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:26:24.000000 pyciactions-1.0.4/pyciactions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 04:26:24.000000 pyciactions-1.0.4/pyciactions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 04:26:24.000000 pyciactions-1.0.4/pyciactions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 04:26:24.000000 pyciactions-1.0.4/pyciactions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 04:26:24.000000 pyciactions-1.0.4/pyciactions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 04:26:24.563652 pyciactions-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      476 2023-07-07 04:21:22.000000 pyciactions-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:29:30.726329 pyciactions-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:29:30.723531 pyciactions-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:29:30.628951 pyciactions-1.0.5/pyciactions/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.5/pyciactions/IWorkflow.py
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-07 04:29:03.000000 pyciactions-1.0.5/pyciactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.5/pyciactions/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:29:30.708761 pyciactions-1.0.5/pyciactions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 04:29:30.727381 pyciactions-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-07 04:29:28.000000 pyciactions-1.0.5/setup.py
```

### Comparing `pyciactions-1.0.4/LICENSE` & `pyciactions-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.4/PKG-INFO` & `pyciactions-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.4
+Version: 1.0.5
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```

### Comparing `pyciactions-1.0.4/README.md` & `pyciactions-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.4/pyciactions.egg-info/PKG-INFO` & `pyciactions-1.0.5/pyciactions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.4
+Version: 1.0.5
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```


# Comparing `tmp/pyciactions-1.0.5.tar.gz` & `tmp/pyciactions-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyciactions-1.0.5.tar", last modified: Fri Jul  7 04:29:30 2023, max compression
+gzip compressed data, was "pyciactions-1.0.6.tar", last modified: Fri Jul  7 04:33:52 2023, max compression
```

## Comparing `pyciactions-1.0.5.tar` & `pyciactions-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:29:30.726329 pyciactions-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:29:30.723531 pyciactions-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:29:30.628951 pyciactions-1.0.5/pyciactions/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.5/pyciactions/IWorkflow.py
--rw-r--r--   0 root         (0) root         (0)       78 2023-07-07 04:29:03.000000 pyciactions-1.0.5/pyciactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.5/pyciactions/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:29:30.708761 pyciactions-1.0.5/pyciactions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 04:29:30.000000 pyciactions-1.0.5/pyciactions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 04:29:30.727381 pyciactions-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      476 2023-07-07 04:29:28.000000 pyciactions-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:33:52.911568 pyciactions-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:33:52.909559 pyciactions-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:33:52.806914 pyciactions-1.0.6/pyciactions/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.6/pyciactions/IWorkflow.py
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-07 04:33:42.000000 pyciactions-1.0.6/pyciactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.6/pyciactions/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 04:33:52.893301 pyciactions-1.0.6/pyciactions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-07 04:33:52.000000 pyciactions-1.0.6/pyciactions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 04:33:52.000000 pyciactions-1.0.6/pyciactions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 04:33:52.000000 pyciactions-1.0.6/pyciactions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 04:33:52.000000 pyciactions-1.0.6/pyciactions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 04:33:52.000000 pyciactions-1.0.6/pyciactions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 04:33:52.913466 pyciactions-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-07 04:33:49.000000 pyciactions-1.0.6/setup.py
```

### Comparing `pyciactions-1.0.5/LICENSE` & `pyciactions-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.5/PKG-INFO` & `pyciactions-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.5
+Version: 1.0.6
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```

### Comparing `pyciactions-1.0.5/README.md` & `pyciactions-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.5/pyciactions.egg-info/PKG-INFO` & `pyciactions-1.0.6/pyciactions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.5
+Version: 1.0.6
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```


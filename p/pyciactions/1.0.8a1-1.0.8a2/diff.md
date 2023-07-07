# Comparing `tmp/pyciactions-1.0.8a1.tar.gz` & `tmp/pyciactions-1.0.8a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyciactions-1.0.8a1.tar", last modified: Fri Jul  7 05:33:42 2023, max compression
+gzip compressed data, was "pyciactions-1.0.8a2.tar", last modified: Fri Jul  7 05:35:46 2023, max compression
```

## Comparing `pyciactions-1.0.8a1.tar` & `pyciactions-1.0.8a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:33:42.918409 pyciactions-1.0.8a1/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.8a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:33:42.916115 pyciactions-1.0.8a1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.8a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:33:42.835705 pyciactions-1.0.8a1/pyciactions/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.8a1/pyciactions/IWorkflow.py
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-07 05:32:56.000000 pyciactions-1.0.8a1/pyciactions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.8a1/pyciactions/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:33:42.902114 pyciactions-1.0.8a1/pyciactions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:33:42.000000 pyciactions-1.0.8a1/pyciactions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 05:33:42.000000 pyciactions-1.0.8a1/pyciactions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 05:33:42.000000 pyciactions-1.0.8a1/pyciactions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 05:33:42.000000 pyciactions-1.0.8a1/pyciactions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 05:33:42.000000 pyciactions-1.0.8a1/pyciactions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 05:33:42.919451 pyciactions-1.0.8a1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      483 2023-07-07 05:33:39.000000 pyciactions-1.0.8a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:35:46.745762 pyciactions-1.0.8a2/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-07 06:32:23.000000 pyciactions-1.0.8a2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:35:46.743309 pyciactions-1.0.8a2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-07 04:20:01.000000 pyciactions-1.0.8a2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:35:46.663138 pyciactions-1.0.8a2/pyciactions/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 06:26:08.000000 pyciactions-1.0.8a2/pyciactions/IWorkflow.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-07 05:35:34.000000 pyciactions-1.0.8a2/pyciactions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-07 05:48:28.000000 pyciactions-1.0.8a2/pyciactions/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 05:35:46.729132 pyciactions-1.0.8a2/pyciactions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-07-07 05:35:46.000000 pyciactions-1.0.8a2/pyciactions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-07 05:35:46.000000 pyciactions-1.0.8a2/pyciactions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 05:35:46.000000 pyciactions-1.0.8a2/pyciactions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-07 05:35:46.000000 pyciactions-1.0.8a2/pyciactions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-07 05:35:46.000000 pyciactions-1.0.8a2/pyciactions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 05:35:46.746884 pyciactions-1.0.8a2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      483 2023-07-07 05:35:44.000000 pyciactions-1.0.8a2/setup.py
```

### Comparing `pyciactions-1.0.8a1/LICENSE` & `pyciactions-1.0.8a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.8a1/PKG-INFO` & `pyciactions-1.0.8a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.8a1
+Version: 1.0.8a2
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```

### Comparing `pyciactions-1.0.8a1/README.md` & `pyciactions-1.0.8a2/README.md`

 * *Files identical despite different names*

### Comparing `pyciactions-1.0.8a1/pyciactions.egg-info/PKG-INFO` & `pyciactions-1.0.8a2/pyciactions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyciactions
-Version: 1.0.8a1
+Version: 1.0.8a2
 Summary: Declarative builder for Github Action Scripts
 Home-page: https://github.com/JBongars/pyciactions
 Author: Julien Bongars
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Python CI Workflow Documentation
```


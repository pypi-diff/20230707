# Comparing `tmp/lokzzpylib-0.2.dev8.tar.gz` & `tmp/lokzzpylib-0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylib-0.2.dev8.tar", last modified: Mon Jul  3 10:05:37 2023, max compression
+gzip compressed data, was "lokzzpylib-0.2.dev9.tar", last modified: Mon Jul  3 10:10:27 2023, max compression
```

## Comparing `lokzzpylib-0.2.dev8.tar` & `lokzzpylib-0.2.dev9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:05:37.161278 lokzzpylib-0.2.dev8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:05:37.161278 lokzzpylib-0.2.dev8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:05:37.161278 lokzzpylib-0.2.dev8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 10:05:16.000000 lokzzpylib-0.2.dev8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 10:05:16.000000 lokzzpylib-0.2.dev8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 10:05:16.000000 lokzzpylib-0.2.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 10:05:37.161278 lokzzpylib-0.2.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 10:05:16.000000 lokzzpylib-0.2.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:05:37.161278 lokzzpylib-0.2.dev8/lokzzpylib/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-03 10:05:16.000000 lokzzpylib-0.2.dev8/lokzzpylib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:05:37.161278 lokzzpylib-0.2.dev8/lokzzpylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 10:05:37.000000 lokzzpylib-0.2.dev8/lokzzpylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 10:05:37.000000 lokzzpylib-0.2.dev8/lokzzpylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:05:37.000000 lokzzpylib-0.2.dev8/lokzzpylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 10:05:37.000000 lokzzpylib-0.2.dev8/lokzzpylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 10:05:37.000000 lokzzpylib-0.2.dev8/lokzzpylib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 10:05:16.000000 lokzzpylib-0.2.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:05:37.161278 lokzzpylib-0.2.dev8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.950512 lokzzpylib-0.2.dev9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.946512 lokzzpylib-0.2.dev9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.946512 lokzzpylib-0.2.dev9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 10:10:27.950512 lokzzpylib-0.2.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.946512 lokzzpylib-0.2.dev9/lokzzpylib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/lokzzpylib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:10:27.946512 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 10:10:27.000000 lokzzpylib-0.2.dev9/lokzzpylib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 10:10:03.000000 lokzzpylib-0.2.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:10:27.950512 lokzzpylib-0.2.dev9/setup.cfg
```

### Comparing `lokzzpylib-0.2.dev8/.github/workflows/python-publish.yml` & `lokzzpylib-0.2.dev9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lokzzpylib-0.2.dev8/lokzzpylib/__init__.py` & `lokzzpylib-0.2.dev9/lokzzpylib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from clint.textui import puts, colored, indent
 from os import system, name
 from pick import pick
 
-global enabledebugP
-
 class Choice(object):
     def __init__(self, index, option):
         self.index = index
         self.option = option
 
 def choose_from_list(title, options):
     option, index = pick(options, title)
@@ -41,16 +39,16 @@
         sep =+ sepC
         with indent(BegL, quote=Beg):
             if not f:
                 puts(colored.blue(n) + sep + d)
             else:
                 puts(colored.blue(d) + sep + n)
 
-def printd(n, d = '', f = False, sepL = 0, sepC = ' ', Beg = colored.red('>>|'), BegL = 4):
-    if enabledebugP == True:
+def printd(n, d = '', f = False, A = False, sepL = 0, sepC = ' ', Beg = colored.red('>>|'), BegL = 4):
+    if A == True:
         sep = ''
         for i in range(sepL):
             sep =+ sepC
             with indent(BegL, quote=Beg):
                 if not f:
                     puts(colored.blue(n) + sep + d)
                 else:
```

### Comparing `lokzzpylib-0.2.dev8/pyproject.toml` & `lokzzpylib-0.2.dev9/pyproject.toml`

 * *Files identical despite different names*


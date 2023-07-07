# Comparing `tmp/SocketUI-0.0.1.tar.gz` & `tmp/SocketUI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SocketUI-0.0.1.tar", last modified: Thu Jul  6 14:18:23 2023, max compression
+gzip compressed data, was "SocketUI-0.0.2.tar", last modified: Fri Jul  7 05:32:44 2023, max compression
```

## Comparing `SocketUI-0.0.1.tar` & `SocketUI-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 14:18:23.943329 SocketUI-0.0.1/
--rw-r--r--   0 meo       (1000) meo       (1000)      412 2023-07-06 14:18:23.943329 SocketUI-0.0.1/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)       16 2023-07-06 13:43:41.000000 SocketUI-0.0.1/README.md
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 14:18:23.943329 SocketUI-0.0.1/SocketUI/
--rw-r--r--   0 meo       (1000) meo       (1000)     3862 2023-07-06 14:05:00.000000 SocketUI-0.0.1/SocketUI/__init__.py
--rw-r--r--   0 meo       (1000) meo       (1000)     2588 2023-07-06 11:22:37.000000 SocketUI-0.0.1/SocketUI/ui.py
-drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-06 14:18:23.943329 SocketUI-0.0.1/SocketUI.egg-info/
--rw-r--r--   0 meo       (1000) meo       (1000)      412 2023-07-06 14:18:23.000000 SocketUI-0.0.1/SocketUI.egg-info/PKG-INFO
--rw-r--r--   0 meo       (1000) meo       (1000)      248 2023-07-06 14:18:23.000000 SocketUI-0.0.1/SocketUI.egg-info/SOURCES.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-06 14:18:23.000000 SocketUI-0.0.1/SocketUI.egg-info/dependency_links.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       43 2023-07-06 14:18:23.000000 SocketUI-0.0.1/SocketUI.egg-info/entry_points.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        6 2023-07-06 14:18:23.000000 SocketUI-0.0.1/SocketUI.egg-info/requires.txt
--rw-r--r--   0 meo       (1000) meo       (1000)        9 2023-07-06 14:18:23.000000 SocketUI-0.0.1/SocketUI.egg-info/top_level.txt
--rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-06 14:18:23.943329 SocketUI-0.0.1/setup.cfg
--rw-r--r--   0 meo       (1000) meo       (1000)      958 2023-07-06 14:18:10.000000 SocketUI-0.0.1/setup.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-07 05:32:44.232240 SocketUI-0.0.2/
+-rw-r--r--   0 meo       (1000) meo       (1000)      484 2023-07-07 05:32:44.232240 SocketUI-0.0.2/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)       87 2023-07-06 14:42:29.000000 SocketUI-0.0.2/README.md
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-07 05:32:44.232240 SocketUI-0.0.2/SocketUI/
+-rw-r--r--   0 meo       (1000) meo       (1000)     4957 2023-07-07 05:29:02.000000 SocketUI-0.0.2/SocketUI/__init__.py
+-rw-r--r--   0 meo       (1000) meo       (1000)     3566 2023-07-07 05:29:40.000000 SocketUI-0.0.2/SocketUI/ui.py
+drwxr-xr-x   0 meo       (1000) meo       (1000)        0 2023-07-07 05:32:44.232240 SocketUI-0.0.2/SocketUI.egg-info/
+-rw-r--r--   0 meo       (1000) meo       (1000)      484 2023-07-07 05:32:44.000000 SocketUI-0.0.2/SocketUI.egg-info/PKG-INFO
+-rw-r--r--   0 meo       (1000) meo       (1000)      248 2023-07-07 05:32:44.000000 SocketUI-0.0.2/SocketUI.egg-info/SOURCES.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        1 2023-07-07 05:32:44.000000 SocketUI-0.0.2/SocketUI.egg-info/dependency_links.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       42 2023-07-07 05:32:44.000000 SocketUI-0.0.2/SocketUI.egg-info/entry_points.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        6 2023-07-07 05:32:44.000000 SocketUI-0.0.2/SocketUI.egg-info/requires.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)        9 2023-07-07 05:32:44.000000 SocketUI-0.0.2/SocketUI.egg-info/top_level.txt
+-rw-r--r--   0 meo       (1000) meo       (1000)       38 2023-07-07 05:32:44.232240 SocketUI-0.0.2/setup.cfg
+-rw-r--r--   0 meo       (1000) meo       (1000)      957 2023-07-07 05:11:53.000000 SocketUI-0.0.2/setup.py
```

### Comparing `SocketUI-0.0.1/setup.py` & `SocketUI-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 PROJ_NAME = "SocketUI"
 setup(
     name         =  PROJ_NAME,
     author       =  "miaobuao",
     url          =  "https://github.com/miaobuao/SocketUI",
     description  =  desc,
-    version      =  '0.0.1',
+    version      =  '0.0.2',
     license      =  "MIT License",
     author_email =  "miaobuao@outlook.com",
     packages     = find_packages(),
     include_package_data = True,
     long_description     = desc,
     long_description_content_type="text/markdown",
     classifiers=[
@@ -25,11 +25,11 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "pyqt5"
     ],
     entry_points={
         'console_scripts': [
-            f'socket-ui = {PROJ_NAME}:run',
+            f'socketui = {PROJ_NAME}:run',
         ],
     },
 )
```


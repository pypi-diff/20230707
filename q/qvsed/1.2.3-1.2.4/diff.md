# Comparing `tmp/qvsed-1.2.3.tar.gz` & `tmp/qvsed-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.2.3.tar", last modified: Fri Jul  7 18:59:52 2023, max compression
+gzip compressed data, was "qvsed-1.2.4.tar", last modified: Fri Jul  7 19:21:01 2023, max compression
```

## Comparing `qvsed-1.2.3.tar` & `qvsed-1.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 18:59:52.499447 qvsed-1.2.3/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0       57 2023-07-07 18:58:49.000000 qvsed-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-07 18:59:52.497262 qvsed-1.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 18:59:52.463488 qvsed-1.2.3/QVSED/
--rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 qvsed-1.2.3/QVSED/QVSED.ui
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.2.3/QVSED/__init__.py
--rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 qvsed-1.2.3/QVSED/config.py
--rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 qvsed-1.2.3/QVSED/config_default.py
--rw-rw-rw-   0        0        0    11290 2023-07-07 18:52:58.000000 qvsed-1.2.3/QVSED/qvsed.py
--rw-rw-rw-   0        0        0     5751 2023-07-07 12:20:45.000000 qvsed-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 18:59:52.496254 qvsed-1.2.3/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-07 18:59:52.000000 qvsed-1.2.3/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-07-07 18:59:52.000000 qvsed-1.2.3/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:59:52.000000 qvsed-1.2.3/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-07 18:59:52.000000 qvsed-1.2.3/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 18:59:52.000000 qvsed-1.2.3/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 18:59:52.000000 qvsed-1.2.3/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 18:59:52.499447 qvsed-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-07-07 18:59:29.000000 qvsed-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:21:01.060086 qvsed-1.2.4/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-07-07 19:12:44.000000 qvsed-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-07 19:21:01.060086 qvsed-1.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 19:21:01.043844 qvsed-1.2.4/QVSED/
+-rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 qvsed-1.2.4/QVSED/QVSED.ui
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.2.4/QVSED/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 qvsed-1.2.4/QVSED/config.py
+-rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 qvsed-1.2.4/QVSED/config_default.py
+-rw-rw-rw-   0        0        0    11290 2023-07-07 18:52:58.000000 qvsed-1.2.4/QVSED/qvsed.py
+-rw-rw-rw-   0        0        0     5751 2023-07-07 12:20:45.000000 qvsed-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 19:21:01.058264 qvsed-1.2.4/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-07 19:21:00.000000 qvsed-1.2.4/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-07-07 19:21:00.000000 qvsed-1.2.4/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 19:21:00.000000 qvsed-1.2.4/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-07 19:21:00.000000 qvsed-1.2.4/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 19:21:00.000000 qvsed-1.2.4/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 19:21:00.000000 qvsed-1.2.4/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 19:21:01.062599 qvsed-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-07-07 19:20:15.000000 qvsed-1.2.4/setup.py
```

### Comparing `qvsed-1.2.3/LICENSE.txt` & `qvsed-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.2.3/PKG-INFO` & `qvsed-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.2.3
+Version: 1.2.4
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.2.3/QVSED/QVSED.ui` & `qvsed-1.2.4/QVSED/QVSED.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.2.3/QVSED/qvsed.py` & `qvsed-1.2.4/QVSED/qvsed.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.2.3/README.md` & `qvsed-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.2.3/qvsed.egg-info/PKG-INFO` & `qvsed-1.2.4/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.2.3
+Version: 1.2.4
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.2.3/setup.py` & `qvsed-1.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.2.3',
+    version='1.2.4',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```


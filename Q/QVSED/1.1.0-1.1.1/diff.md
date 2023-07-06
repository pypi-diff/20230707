# Comparing `tmp/QVSED-1.1.0.tar.gz` & `tmp/QVSED-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QVSED-1.1.0.tar", last modified: Thu Jul  6 21:59:38 2023, max compression
+gzip compressed data, was "QVSED-1.1.1.tar", last modified: Thu Jul  6 22:04:12 2023, max compression
```

## Comparing `QVSED-1.1.0.tar` & `QVSED-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 21:59:38.004628 QVSED-1.1.0/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 QVSED-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 QVSED-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      710 2023-07-06 21:59:38.004628 QVSED-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 21:59:37.990412 QVSED-1.1.0/QVSED/
--rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 QVSED-1.1.0/QVSED/QVSED.ui
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 QVSED-1.1.0/QVSED/__init__.py
--rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 QVSED-1.1.0/QVSED/config.py
--rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 QVSED-1.1.0/QVSED/config_default.py
--rw-rw-rw-   0        0        0     8334 2023-07-06 21:57:59.000000 QVSED-1.1.0/QVSED/qvsed.py
-drwxrwxrwx   0        0        0        0 2023-07-06 21:59:38.001394 QVSED-1.1.0/QVSED.egg-info/
--rw-rw-rw-   0        0        0      710 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2037 2023-07-06 21:43:09.000000 QVSED-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 21:59:38.004628 QVSED-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-07-06 21:58:47.000000 QVSED-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:04:12.357448 QVSED-1.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 QVSED-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 QVSED-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      710 2023-07-06 22:04:12.357448 QVSED-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 22:04:12.345494 QVSED-1.1.1/QVSED/
+-rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 QVSED-1.1.1/QVSED/QVSED.ui
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 QVSED-1.1.1/QVSED/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 QVSED-1.1.1/QVSED/config.py
+-rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 QVSED-1.1.1/QVSED/config_default.py
+-rw-rw-rw-   0        0        0     8334 2023-07-06 21:57:59.000000 QVSED-1.1.1/QVSED/qvsed.py
+drwxrwxrwx   0        0        0        0 2023-07-06 22:04:12.353865 QVSED-1.1.1/QVSED.egg-info/
+-rw-rw-rw-   0        0        0      710 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2037 2023-07-06 21:43:09.000000 QVSED-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 22:04:12.357448 QVSED-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-07-06 22:03:16.000000 QVSED-1.1.1/setup.py
```

### Comparing `QVSED-1.1.0/LICENSE.txt` & `QVSED-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QVSED-1.1.0/PKG-INFO` & `QVSED-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QVSED
-Version: 1.1.0
+Version: 1.1.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.
```

### Comparing `QVSED-1.1.0/QVSED/QVSED.ui` & `QVSED-1.1.1/QVSED/QVSED.ui`

 * *Files identical despite different names*

### Comparing `QVSED-1.1.0/QVSED/qvsed.py` & `QVSED-1.1.1/QVSED/qvsed.py`

 * *Files identical despite different names*

### Comparing `QVSED-1.1.0/QVSED.egg-info/PKG-INFO` & `QVSED-1.1.1/QVSED.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QVSED
-Version: 1.1.0
+Version: 1.1.1
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.
```

### Comparing `QVSED-1.1.0/README.md` & `QVSED-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `QVSED-1.1.0/setup.py` & `QVSED-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='QVSED',
-    version='1.1.0',
+    version='1.1.1',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description='QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.',
     packages=find_packages(),
     license="GPL-3.0-or-later",
     url='https://github.com/That1M8Head/QVSED/',
     include_package_data=True,
     install_requires=[
         'PyQt5'
     ],
     entry_points={
-        'console_scripts': [
+        'gui_scripts': [
             'qvsed = QVSED.qvsed:main',
         ],
     },
     package_data={'QVSED': ['QVSED.ui']},
 )
```


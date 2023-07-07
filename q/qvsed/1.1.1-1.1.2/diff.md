# Comparing `tmp/QVSED-1.1.1.tar.gz` & `tmp/qvsed-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QVSED-1.1.1.tar", last modified: Thu Jul  6 22:04:12 2023, max compression
+gzip compressed data, was "qvsed-1.1.2.tar", last modified: Fri Jul  7 11:23:00 2023, max compression
```

## Comparing `QVSED-1.1.1.tar` & `qvsed-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 22:04:12.357448 QVSED-1.1.1/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 QVSED-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 QVSED-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      710 2023-07-06 22:04:12.357448 QVSED-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 22:04:12.345494 QVSED-1.1.1/QVSED/
--rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 QVSED-1.1.1/QVSED/QVSED.ui
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 QVSED-1.1.1/QVSED/__init__.py
--rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 QVSED-1.1.1/QVSED/config.py
--rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 QVSED-1.1.1/QVSED/config_default.py
--rw-rw-rw-   0        0        0     8334 2023-07-06 21:57:59.000000 QVSED-1.1.1/QVSED/qvsed.py
-drwxrwxrwx   0        0        0        0 2023-07-06 22:04:12.353865 QVSED-1.1.1/QVSED.egg-info/
--rw-rw-rw-   0        0        0      710 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 22:04:12.000000 QVSED-1.1.1/QVSED.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2037 2023-07-06 21:43:09.000000 QVSED-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 22:04:12.357448 QVSED-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-07-06 22:03:16.000000 QVSED-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:23:00.670728 qvsed-1.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 qvsed-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      710 2023-07-07 11:23:00.669717 qvsed-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 11:23:00.649248 qvsed-1.1.2/QVSED/
+-rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 qvsed-1.1.2/QVSED/QVSED.ui
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 qvsed-1.1.2/QVSED/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 qvsed-1.1.2/QVSED/config.py
+-rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 qvsed-1.1.2/QVSED/config_default.py
+-rw-rw-rw-   0        0        0     8334 2023-07-07 11:18:15.000000 qvsed-1.1.2/QVSED/qvsed.py
+-rw-rw-rw-   0        0        0     4080 2023-07-07 11:19:56.000000 qvsed-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 11:23:00.664726 qvsed-1.1.2/qvsed.egg-info/
+-rw-rw-rw-   0        0        0      710 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 11:23:00.000000 qvsed-1.1.2/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:23:00.671740 qvsed-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-07-07 11:22:20.000000 qvsed-1.1.2/setup.py
```

### Comparing `QVSED-1.1.1/LICENSE.txt` & `qvsed-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QVSED-1.1.1/PKG-INFO` & `qvsed-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: QVSED
-Version: 1.1.1
+Name: qvsed
+Version: 1.1.2
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.
```

### Comparing `QVSED-1.1.1/QVSED/QVSED.ui` & `qvsed-1.1.2/QVSED/QVSED.ui`

 * *Files identical despite different names*

### Comparing `QVSED-1.1.1/QVSED/qvsed.py` & `qvsed-1.1.2/QVSED/qvsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def echo_area_update(self, message):
         echo_area = self.findChild(QLineEdit, "echoArea")
         echo_area.setText(message)
 
     def load_ui_file(self):
         current_dir = os.path.dirname(os.path.abspath(__file__))
-        ui_file = os.path.join(current_dir, 'QVSED.ui')
+        ui_file = os.path.join(current_dir, 'qvsed.ui')
         loadUi(ui_file, self)
 
     def generate_config(self):
         current_dir = os.path.dirname(os.path.abspath(__file__))
         config_default = os.path.join(current_dir, 'config_default.py')
         
         if os.name == 'nt': # Windows
```

### Comparing `QVSED-1.1.1/QVSED.egg-info/PKG-INFO` & `qvsed-1.1.2/qvsed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: QVSED
-Version: 1.1.1
+Name: qvsed
+Version: 1.1.2
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.
```

### Comparing `QVSED-1.1.1/setup.py` & `qvsed-1.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='QVSED',
-    version='1.1.1',
+    name='qvsed',
+    version='1.1.2',
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
         'gui_scripts': [
-            'qvsed = QVSED.qvsed:main',
+            'qvsed = qvsed.qvsed:main',
         ],
     },
-    package_data={'QVSED': ['QVSED.ui']},
+    package_data={'qvsed': ['qvsed.ui']},
 )
```


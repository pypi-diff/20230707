# Comparing `tmp/QVSED-1.0.3.tar.gz` & `tmp/QVSED-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QVSED-1.0.3.tar", last modified: Thu Jul  6 21:40:02 2023, max compression
+gzip compressed data, was "QVSED-1.1.0.tar", last modified: Thu Jul  6 21:59:38 2023, max compression
```

## Comparing `QVSED-1.0.3.tar` & `QVSED-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 21:40:02.359702 QVSED-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 QVSED-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 QVSED-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      710 2023-07-06 21:40:02.359702 QVSED-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 21:40:02.336837 QVSED-1.0.3/QVSED/
--rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 QVSED-1.0.3/QVSED/QVSED.ui
--rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 QVSED-1.0.3/QVSED/__init__.py
--rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 QVSED-1.0.3/QVSED/config.py
--rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 QVSED-1.0.3/QVSED/config_default.py
--rw-rw-rw-   0        0        0     7480 2023-07-06 21:07:16.000000 QVSED-1.0.3/QVSED/qvsed.py
-drwxrwxrwx   0        0        0        0 2023-07-06 21:40:02.358264 QVSED-1.0.3/QVSED.egg-info/
--rw-rw-rw-   0        0        0      710 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 21:40:02.000000 QVSED-1.0.3/QVSED.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2040 2023-07-06 21:39:45.000000 QVSED-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 21:40:02.359702 QVSED-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-07-06 21:39:53.000000 QVSED-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:59:38.004628 QVSED-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 QVSED-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       51 2023-07-06 21:31:44.000000 QVSED-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      710 2023-07-06 21:59:38.004628 QVSED-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 21:59:37.990412 QVSED-1.1.0/QVSED/
+-rw-rw-rw-   0        0        0    20071 2023-07-06 21:04:23.000000 QVSED-1.1.0/QVSED/QVSED.ui
+-rw-rw-rw-   0        0        0       50 2023-07-06 20:42:20.000000 QVSED-1.1.0/QVSED/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-07-06 19:49:30.000000 QVSED-1.1.0/QVSED/config.py
+-rw-rw-rw-   0        0        0      261 2023-07-06 20:11:25.000000 QVSED-1.1.0/QVSED/config_default.py
+-rw-rw-rw-   0        0        0     8334 2023-07-06 21:57:59.000000 QVSED-1.1.0/QVSED/qvsed.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:59:38.001394 QVSED-1.1.0/QVSED.egg-info/
+-rw-rw-rw-   0        0        0      710 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 21:59:37.000000 QVSED-1.1.0/QVSED.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2037 2023-07-06 21:43:09.000000 QVSED-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 21:59:38.004628 QVSED-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-07-06 21:58:47.000000 QVSED-1.1.0/setup.py
```

### Comparing `QVSED-1.0.3/LICENSE.txt` & `QVSED-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QVSED-1.0.3/PKG-INFO` & `QVSED-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QVSED
-Version: 1.0.3
+Version: 1.1.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.
```

### Comparing `QVSED-1.0.3/QVSED/QVSED.ui` & `QVSED-1.1.0/QVSED/QVSED.ui`

 * *Files identical despite different names*

### Comparing `QVSED-1.0.3/QVSED/qvsed.py` & `QVSED-1.1.0/QVSED/qvsed.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 QVSED - Qt-Based Volatile Small Editor
 A cross-platform simple and volatile text editor by Arsalan Kazmi
 See README.md or "Get Help" inside QVSED for more info
 """
 
 import os
 import shutil
-import pkg_resources
+import configparser
+import importlib.util
 from PyQt5.QtWidgets import (
     QApplication, QMainWindow, QPushButton, QVBoxLayout, QWidget,
     QFileDialog, QPlainTextEdit, QLineEdit, QAction, QShortcut
 )
 from PyQt5.QtGui import QKeySequence, QFont
 from PyQt5.uic import loadUi
 
@@ -41,36 +42,53 @@
 
     def load_ui_file(self):
         current_dir = os.path.dirname(os.path.abspath(__file__))
         ui_file = os.path.join(current_dir, 'QVSED.ui')
         loadUi(ui_file, self)
 
     def generate_config(self):
-        self.echo_area_update("Welcome to QVSED! Config file config.py created.")
-
         current_dir = os.path.dirname(os.path.abspath(__file__))
         config_default = os.path.join(current_dir, 'config_default.py')
-        shutil.copyfile(config_default, "QVSED/config.py")
-    
+        
+        if os.name == 'nt': # Windows
+            user_config_dir = os.path.join(os.environ['APPDATA'], 'QVSED')
+        else: # *nix
+            user_config_dir = os.path.expanduser("~") + "/.config/QVSED"
+        
+        if not os.path.exists(user_config_dir):
+            os.makedirs(user_config_dir)
+        user_config_file = os.path.join(user_config_dir, 'config.py')
+        
+        shutil.copyfile(config_default, user_config_file)
+
         # Update the first line of config.py
-        with open("config.py", "r+") as config_file:
+        with open(user_config_file, "r+") as config_file:
             lines = config_file.readlines()
             if lines:
                 lines[0] = "# This is QVSED's config file, you can change its options here.\n"
                 config_file.seek(0)
                 config_file.writelines(lines)
                 config_file.truncate()
+                
+        self.echo_area_update(f"Config generated at {user_config_file}.")
 
     def load_config(self):
-        config_file = "config.py"
+        if os.name == 'nt': # Windows
+            user_config_dir = os.path.join(os.environ['APPDATA'], 'QVSED')
+        else: # *nix
+            user_config_dir = os.path.expanduser("~") + "/.config/QVSED"
+        
+        user_config_file = os.path.join(user_config_dir, 'config.py')
 
-        if not os.path.isfile(config_file):
+        if not os.path.isfile(user_config_file):
             self.generate_config()
         
-        import config as qvsed_config
+        spec = importlib.util.spec_from_file_location("qvsed_config", user_config_file)
+        qvsed_config = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(qvsed_config)
 
         self.font_family = qvsed_config.font_family
         self.font_size = qvsed_config.font_size
 
     def set_up_fonts(self):
         font = QFont()
         font.setFamilies(self.font_family)
```

### Comparing `QVSED-1.0.3/QVSED.egg-info/PKG-INFO` & `QVSED-1.1.0/QVSED.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QVSED
-Version: 1.0.3
+Version: 1.1.0
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.
```

### Comparing `QVSED-1.0.3/README.md` & `QVSED-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 QVSED is licensed under the GNU General Public License version 3 or later.
 
 ## The window
 
 QVSED is broken up into three parts - the Action Deck, the Text Area and the Echo Area.
 
-![QVSED screenshot, editing its own source code](qsved_screenie.png)
+![QVSED screenshot, showing the help message](qsved_screenie.png)
 
 The Action Deck includes the commands Clear Text, Open File, Save File, Get Help and Quit QVSED. These can be activated by clicking on them or entering their keyboard shortcut.
 
 The Text Area is where the actual text editing takes place. This is straightforward so I won't say anything more.
 
 The Echo Area is a small bar at the bottom of the QSMED window that prints information, for example, when a file is opened, it prints its path.
```

### Comparing `QVSED-1.0.3/setup.py` & `QVSED-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='QVSED',
-    version='1.0.3',
+    version='1.1.0',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description='QVSED is a volatile text editor, meaning that there are no restrictions against unsaved work or bad files. QVSED is a PyQt5 rewrite of my older project, ASMED (Another SMol EDitor), which was written using Windows Forms, and was quite obviously only for Windows. QVSED seeks to replace ASMED by being cross-platform, and it will bring over the benefits of such a lightweight editor without the overhead of .NET. QVSED is licensed under the GNU General Public License version 3 or later.',
     packages=find_packages(),
     license="GPL-3.0-or-later",
     url='https://github.com/That1M8Head/QVSED/',
     include_package_data=True,
```


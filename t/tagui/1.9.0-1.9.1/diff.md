# Comparing `tmp/tagui-1.9.0.tar.gz` & `tmp/tagui-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tagui-1.9.0.tar", last modified: Mon Jul 15 01:39:02 2019, max compression
+gzip compressed data, was "dist/tagui-1.9.1.tar", last modified: Mon Jul 15 02:25:12 2019, max compression
```

## Comparing `tagui-1.9.0.tar` & `tagui-1.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kensoh     (501) staff       (20)        0 2019-07-15 01:39:02.000000 tagui-1.9.0/
--rw-r--r--   0 kensoh     (501) staff       (20)      995 2019-07-15 01:39:02.000000 tagui-1.9.0/PKG-INFO
--rw-r--r--   0 kensoh     (501) staff       (20)    50955 2019-07-15 01:17:22.000000 tagui-1.9.0/tagui.py
-drwxr-xr-x   0 kensoh     (501) staff       (20)        0 2019-07-15 01:39:02.000000 tagui-1.9.0/tagui.egg-info/
--rw-r--r--   0 kensoh     (501) staff       (20)      995 2019-07-15 01:39:02.000000 tagui-1.9.0/tagui.egg-info/PKG-INFO
--rw-r--r--   0 kensoh     (501) staff       (20)      177 2019-07-15 01:39:02.000000 tagui-1.9.0/tagui.egg-info/SOURCES.txt
--rw-r--r--   0 kensoh     (501) staff       (20)        6 2019-07-15 01:39:02.000000 tagui-1.9.0/tagui.egg-info/top_level.txt
--rw-r--r--   0 kensoh     (501) staff       (20)        1 2019-07-15 01:39:02.000000 tagui-1.9.0/tagui.egg-info/dependency_links.txt
--rw-------   0 kensoh     (501) staff       (20)       56 2019-06-11 12:42:13.000000 tagui-1.9.0/MANIFEST.in
--rw-r--r--   0 kensoh     (501) staff       (20)     9172 2019-07-14 11:31:58.000000 tagui-1.9.0/README.md
--rw-r--r--   0 kensoh     (501) staff       (20)     1082 2019-07-14 11:31:30.000000 tagui-1.9.0/setup.py
--rw-r--r--   0 kensoh     (501) staff       (20)     2568 2019-07-14 11:40:24.000000 tagui-1.9.0/sample.py
--rw-r--r--   0 kensoh     (501) staff       (20)       59 2019-07-15 01:39:02.000000 tagui-1.9.0/setup.cfg
--rw-r--r--   0 kensoh     (501) staff       (20)    11364 2019-06-11 12:43:16.000000 tagui-1.9.0/LICENSE.txt
+drwxr-xr-x   0 kensoh     (501) staff       (20)        0 2019-07-15 02:25:12.000000 tagui-1.9.1/
+-rw-r--r--   0 kensoh     (501) staff       (20)      995 2019-07-15 02:25:12.000000 tagui-1.9.1/PKG-INFO
+-rw-r--r--   0 kensoh     (501) staff       (20)    51330 2019-07-15 02:15:50.000000 tagui-1.9.1/tagui.py
+drwxr-xr-x   0 kensoh     (501) staff       (20)        0 2019-07-15 02:25:12.000000 tagui-1.9.1/tagui.egg-info/
+-rw-r--r--   0 kensoh     (501) staff       (20)      995 2019-07-15 02:25:12.000000 tagui-1.9.1/tagui.egg-info/PKG-INFO
+-rw-r--r--   0 kensoh     (501) staff       (20)      177 2019-07-15 02:25:12.000000 tagui-1.9.1/tagui.egg-info/SOURCES.txt
+-rw-r--r--   0 kensoh     (501) staff       (20)        6 2019-07-15 02:25:12.000000 tagui-1.9.1/tagui.egg-info/top_level.txt
+-rw-r--r--   0 kensoh     (501) staff       (20)        1 2019-07-15 02:25:12.000000 tagui-1.9.1/tagui.egg-info/dependency_links.txt
+-rw-------   0 kensoh     (501) staff       (20)       56 2019-06-11 12:42:13.000000 tagui-1.9.1/MANIFEST.in
+-rw-r--r--   0 kensoh     (501) staff       (20)     9172 2019-07-14 11:31:58.000000 tagui-1.9.1/README.md
+-rw-r--r--   0 kensoh     (501) staff       (20)     1082 2019-07-15 02:15:59.000000 tagui-1.9.1/setup.py
+-rw-r--r--   0 kensoh     (501) staff       (20)     2568 2019-07-14 11:40:24.000000 tagui-1.9.1/sample.py
+-rw-r--r--   0 kensoh     (501) staff       (20)       59 2019-07-15 02:25:12.000000 tagui-1.9.1/setup.cfg
+-rw-r--r--   0 kensoh     (501) staff       (20)    11364 2019-06-11 12:43:16.000000 tagui-1.9.1/LICENSE.txt
```

### Comparing `tagui-1.9.0/PKG-INFO` & `tagui-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tagui
-Version: 1.9.0
+Version: 1.9.1
 Summary: TagUI for Python is a Python package for digital process automation (RPA)
 Home-page: https://github.com/tebelorg/TagUI-Python
 Author: Ken Soh
 Author-email: opensource@tebel.org
 License: Apache License 2.0
 Description: TagUI for Python homepage - https://github.com/tebelorg/TagUI-Python
 Platform: UNKNOWN
```

### Comparing `tagui-1.9.0/tagui.py` & `tagui-1.9.1/tagui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """INTEGRATION ENGINE FOR TAGUI PYTHON PACKAGE ~ TEBEL.ORG"""
 __author__ = 'Ken Soh <opensource@tebel.org>'
-__version__ = '1.9.0'
+__version__ = '1.9.1'
 
 import subprocess
 import os
 import sys
 import time
 import platform
 
@@ -634,14 +634,20 @@
         # send 'done' instruction to terminate live mode and exit tagui
         _tagui_write('echo "[TAGUI][FINISHED]"\n')
         _tagui_write('done\n')
 
         # loop until tagui process has closed before returning control
         while _process.poll() is None: pass
 
+        # remove again generated tagui flow, js code and custom functions files
+        if os.path.isfile('tagui_python'): os.remove('tagui_python')
+        if os.path.isfile('tagui_python.js'): os.remove('tagui_python.js')
+        if os.path.isfile('tagui_python.raw'): os.remove('tagui_python.raw')
+        if os.path.isfile('tagui_local.js'): os.remove('tagui_local.js')
+
         # remove generated tagui log and data files if not in debug mode
         if not debug():
             if os.path.isfile('tagui_python.log'): os.remove('tagui_python.log')
             if os.path.isfile('tagui_python.txt'): os.remove('tagui_python.txt')
 
         _tagui_visual = False
         _tagui_chrome = False
```

### Comparing `tagui-1.9.0/tagui.egg-info/PKG-INFO` & `tagui-1.9.1/tagui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tagui
-Version: 1.9.0
+Version: 1.9.1
 Summary: TagUI for Python is a Python package for digital process automation (RPA)
 Home-page: https://github.com/tebelorg/TagUI-Python
 Author: Ken Soh
 Author-email: opensource@tebel.org
 License: Apache License 2.0
 Description: TagUI for Python homepage - https://github.com/tebelorg/TagUI-Python
 Platform: UNKNOWN
```

### Comparing `tagui-1.9.0/README.md` & `tagui-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tagui-1.9.0/setup.py` & `tagui-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tagui',
-    version='1.9.0',
+    version='1.9.1',
     py_modules=['tagui'],
     author='Ken Soh',
     author_email='opensource@tebel.org',
     license='Apache License 2.0',
     url='https://github.com/tebelorg/TagUI-Python',
     description='TagUI for Python is a Python package for digital process automation (RPA)',
     long_description='TagUI for Python homepage - https://github.com/tebelorg/TagUI-Python',
```

### Comparing `tagui-1.9.0/sample.py` & `tagui-1.9.1/sample.py`

 * *Files identical despite different names*

### Comparing `tagui-1.9.0/LICENSE.txt` & `tagui-1.9.1/LICENSE.txt`

 * *Files identical despite different names*


# Comparing `tmp/Tashriethon-0.0.1.tar.gz` & `tmp/Tashriethon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tashriethon-0.0.1.tar", last modified: Mon Jul  3 05:58:17 2023, max compression
+gzip compressed data, was "Tashriethon-0.0.2.tar", last modified: Fri Jul  7 06:35:12 2023, max compression
```

## Comparing `Tashriethon-0.0.1.tar` & `Tashriethon-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 05:58:17.963626 Tashriethon-0.0.1/
--rw-rw-rw-   0        0        0    35149 2023-05-28 06:43:53.000000 Tashriethon-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1943 2023-07-03 05:58:17.964582 Tashriethon-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1158 2023-06-28 23:40:07.000000 Tashriethon-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-03 05:58:17.924690 Tashriethon-0.0.1/Tashriethon.egg-info/
--rw-rw-rw-   0        0        0     1943 2023-07-03 05:58:17.000000 Tashriethon-0.0.1/Tashriethon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-07-03 05:58:17.000000 Tashriethon-0.0.1/Tashriethon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 05:58:17.000000 Tashriethon-0.0.1/Tashriethon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-07-03 05:58:17.000000 Tashriethon-0.0.1/Tashriethon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-03 05:58:17.000000 Tashriethon-0.0.1/Tashriethon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 05:58:17.960594 Tashriethon-0.0.1/ethon/
--rw-rw-rw-   0        0        0    12360 2023-05-28 06:43:53.000000 Tashriethon-0.0.1/ethon/FasterTg.py
--rw-rw-rw-   0        0        0        1 2023-05-28 06:43:53.000000 Tashriethon-0.0.1/ethon/__init__.py
--rw-rw-rw-   0        0        0      869 2023-06-28 23:43:42.000000 Tashriethon-0.0.1/ethon/mystarts.py
--rw-rw-rw-   0        0        0     3649 2023-06-28 23:46:03.000000 Tashriethon-0.0.1/ethon/pyfunc.py
--rw-rw-rw-   0        0        0     1118 2023-06-28 23:47:45.000000 Tashriethon-0.0.1/ethon/pyutils.py
--rw-rw-rw-   0        0        0     4166 2023-06-28 23:48:47.000000 Tashriethon-0.0.1/ethon/telefunc.py
--rw-rw-rw-   0        0        0      808 2023-06-28 23:49:32.000000 Tashriethon-0.0.1/ethon/teleutils.py
--rw-rw-rw-   0        0        0     2761 2023-05-28 06:43:53.000000 Tashriethon-0.0.1/ethon/uploader.py
--rw-rw-rw-   0        0        0       86 2023-07-03 05:58:17.966579 Tashriethon-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1153 2023-07-03 05:57:14.000000 Tashriethon-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 06:35:12.495732 Tashriethon-0.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-05-28 06:43:53.000000 Tashriethon-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1941 2023-07-07 06:35:12.496072 Tashriethon-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1158 2023-06-28 23:40:07.000000 Tashriethon-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-07 06:35:12.157120 Tashriethon-0.0.2/Tashriethon.egg-info/
+-rw-rw-rw-   0        0        0     1941 2023-07-07 06:35:08.000000 Tashriethon-0.0.2/Tashriethon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-07 06:35:09.000000 Tashriethon-0.0.2/Tashriethon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 06:35:08.000000 Tashriethon-0.0.2/Tashriethon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-07-07 06:35:08.000000 Tashriethon-0.0.2/Tashriethon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 06:35:08.000000 Tashriethon-0.0.2/Tashriethon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 06:35:12.466924 Tashriethon-0.0.2/ethon/
+-rw-rw-rw-   0        0        0    12360 2023-05-28 06:43:53.000000 Tashriethon-0.0.2/ethon/FasterTg.py
+-rw-rw-rw-   0        0        0        1 2023-05-28 06:43:53.000000 Tashriethon-0.0.2/ethon/__init__.py
+-rw-rw-rw-   0        0        0      869 2023-06-28 23:43:42.000000 Tashriethon-0.0.2/ethon/mystarts.py
+-rw-rw-rw-   0        0        0     3649 2023-06-28 23:46:03.000000 Tashriethon-0.0.2/ethon/pyfunc.py
+-rw-rw-rw-   0        0        0     1118 2023-06-28 23:47:45.000000 Tashriethon-0.0.2/ethon/pyutils.py
+-rw-rw-rw-   0        0        0     4190 2023-07-07 06:32:09.000000 Tashriethon-0.0.2/ethon/telefunc.py
+-rw-rw-rw-   0        0        0      808 2023-06-28 23:49:32.000000 Tashriethon-0.0.2/ethon/teleutils.py
+-rw-rw-rw-   0        0        0     2761 2023-05-28 06:43:53.000000 Tashriethon-0.0.2/ethon/uploader.py
+-rw-rw-rw-   0        0        0       86 2023-07-07 06:35:12.500067 Tashriethon-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2023-07-07 06:30:49.000000 Tashriethon-0.0.2/setup.py
```

### Comparing `Tashriethon-0.0.1/LICENSE.txt` & `Tashriethon-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Tashriethon-0.0.1/PKG-INFO` & `Tashriethon-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Tashriethon
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package containing basic functions to build telegram bots.
-Home-page: https://github.com/vasusen-code/ethon
+Home-page: https://github.com/Tashri2342/ethon
 Author: Tashri-Code
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Tashriethon-0.0.1/README.rst` & `Tashriethon-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `Tashriethon-0.0.1/Tashriethon.egg-info/PKG-INFO` & `Tashriethon-0.0.2/Tashriethon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Tashriethon
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package containing basic functions to build telegram bots.
-Home-page: https://github.com/vasusen-code/ethon
+Home-page: https://github.com/Tashri2342/ethon
 Author: Tashri-Code
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Tashriethon-0.0.1/ethon/FasterTg.py` & `Tashriethon-0.0.2/ethon/FasterTg.py`

 * *Files identical despite different names*

### Comparing `Tashriethon-0.0.1/ethon/mystarts.py` & `Tashriethon-0.0.2/ethon/mystarts.py`

 * *Files identical despite different names*

### Comparing `Tashriethon-0.0.1/ethon/pyfunc.py` & `Tashriethon-0.0.2/ethon/pyfunc.py`

 * *Files identical despite different names*

### Comparing `Tashriethon-0.0.1/ethon/pyutils.py` & `Tashriethon-0.0.2/ethon/pyutils.py`

 * *Files identical despite different names*

### Comparing `Tashriethon-0.0.1/ethon/telefunc.py` & `Tashriethon-0.0.2/ethon/telefunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,21 @@
     now = time.time()
     diff = now - start
     if round(diff % 10.00) == 0 or current == total:
         percentage = current * 100 / total
         speed = current / diff
         time_to_completion = round((total - current) / speed) * 1000
         progress_str = "**[{0}{1}]** `| {2}%`\n\n".format(
-            "".join(["█" for i in range(math.floor(percentage / 5))]),
-            "".join(["" for i in range(20 - math.floor(percentage / 5))]),
+            "".join(["🟩" for i in range(math.floor(percentage / 5))]),
+            "".join(["⬜️" for i in range(20 - math.floor(percentage / 5))]),
             round(percentage, 2),
         )
         tmp = (
             progress_str
-            + "GROSS: {0} of {1}\n\nSpeed: {2}/s\n\nETA: {3}\n\n".format(
+            + "📦 GROSS: {0} of {1}\n\n🚀 Speed: {2}/s\n\n⏱️ ETA: {3}\n\n".format(
                 hbs(current),
                 hbs(total),
                 hbs(speed),
                 time_formatter(time_to_completion),
             )
         )
         if file:
```

### Comparing `Tashriethon-0.0.1/ethon/teleutils.py` & `Tashriethon-0.0.2/ethon/teleutils.py`

 * *Files identical despite different names*

### Comparing `Tashriethon-0.0.1/ethon/uploader.py` & `Tashriethon-0.0.2/ethon/uploader.py`

 * *Files identical despite different names*

### Comparing `Tashriethon-0.0.1/setup.py` & `Tashriethon-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 import os
 import setuptools
 
-ver = 'v0.0.1'
+ver = 'v0.0.2'
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_desc = fh.read()
 
 desc = "Package containing basic functions to build telegram bots."
 GPL = "GNU AFFERO GENERAL PUBLIC LICENSE (v3)"
-git = "https://github.com/vasusen-code/ethon"
+git = "https://github.com/Tashri2342/ethon"
 classify = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```


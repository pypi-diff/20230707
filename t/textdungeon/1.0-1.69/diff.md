# Comparing `tmp/textdungeon-1.0.tar.gz` & `tmp/textdungeon-1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdungeon-1.0.tar", max compression
+gzip compressed data, was "textdungeon-1.69.tar", max compression
```

## Comparing `textdungeon-1.0.tar` & `textdungeon-1.69.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      519 2023-07-07 13:24:39.147514 textdungeon-1.0/README.md
--rw-r--r--   0        0        0      633 2023-07-07 16:26:05.135569 textdungeon-1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 16:10:57.492927 textdungeon-1.0/textdungeon/__init__.py
--rw-r--r--   0        0        0     2289 2023-07-07 16:10:57.492927 textdungeon-1.0/textdungeon/color.py
--rw-r--r--   0        0        0    52294 2023-07-07 16:10:57.492927 textdungeon-1.0/textdungeon/dungeon.py
--rw-r--r--   0        0        0    47828 2023-07-07 16:10:57.492927 textdungeon-1.0/textdungeon/entities.py
--rw-r--r--   0        0        0     3151 2023-07-07 16:10:57.492927 textdungeon-1.0/textdungeon/extra.py
--rw-r--r--   0        0        0    53849 2023-07-07 16:10:57.492927 textdungeon-1.0/textdungeon/items.py
--rw-r--r--   0        0        0     8763 2023-07-07 16:23:09.334246 textdungeon-1.0/textdungeon/main.py
--rw-r--r--   0        0        0     1318 1970-01-01 00:00:00.000000 textdungeon-1.0/PKG-INFO
+-rw-r--r--   0        0        0      430 2023-07-07 18:32:23.535816 textdungeon-1.69/README.md
+-rw-r--r--   0        0        0      776 2023-07-07 18:40:03.206882 textdungeon-1.69/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 16:10:57.492927 textdungeon-1.69/textdungeon/__init__.py
+-rw-r--r--   0        0        0     2289 2023-07-07 16:10:57.492927 textdungeon-1.69/textdungeon/color.py
+-rw-r--r--   0        0        0    52294 2023-07-07 16:10:57.492927 textdungeon-1.69/textdungeon/dungeon.py
+-rw-r--r--   0        0        0    47828 2023-07-07 16:10:57.492927 textdungeon-1.69/textdungeon/entities.py
+-rw-r--r--   0        0        0     3151 2023-07-07 16:10:57.492927 textdungeon-1.69/textdungeon/extra.py
+-rw-r--r--   0        0        0    53849 2023-07-07 16:10:57.492927 textdungeon-1.69/textdungeon/items.py
+-rw-r--r--   0        0        0     8763 2023-07-07 16:23:09.334246 textdungeon-1.69/textdungeon/main.py
+-rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 textdungeon-1.69/PKG-INFO
```

### Comparing `textdungeon-1.0/textdungeon/color.py` & `textdungeon-1.69/textdungeon/color.py`

 * *Files identical despite different names*

### Comparing `textdungeon-1.0/textdungeon/dungeon.py` & `textdungeon-1.69/textdungeon/dungeon.py`

 * *Files identical despite different names*

### Comparing `textdungeon-1.0/textdungeon/entities.py` & `textdungeon-1.69/textdungeon/entities.py`

 * *Files identical despite different names*

### Comparing `textdungeon-1.0/textdungeon/extra.py` & `textdungeon-1.69/textdungeon/extra.py`

 * *Files identical despite different names*

### Comparing `textdungeon-1.0/textdungeon/items.py` & `textdungeon-1.69/textdungeon/items.py`

 * *Files identical despite different names*

### Comparing `textdungeon-1.0/textdungeon/main.py` & `textdungeon-1.69/textdungeon/main.py`

 * *Files identical despite different names*

### Comparing `textdungeon-1.0/PKG-INFO` & `textdungeon-1.69/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdungeon
-Version: 1.0
+Version: 1.69
 Summary: suffer alone in your terminal!
 Home-page: https://github.com/Masbender/text-dungeon
 License: MIT
 Keywords: text,dungeon,game
 Author: Matthew Bender
 Author-email: matthewbender65@gmail.com
 Maintainer: Noah Dinan
@@ -20,24 +20,22 @@
 Project-URL: Repository, https://github.com/Masbender/text-dungeon
 Description-Content-Type: text/markdown
 
 <div align=center>
   <img src="https://github.com/Masbender/text-dungeon/assets/91911303/63d96f62-a73d-4d79-ae93-347dd9906034">
   <h1 align=center>Text Dungeon: suffer alone in your terminal!</h1>
 </div>
-
 ---
 ## Installation
-### Linux
+### Python Pip
+```sh
+pip install textdungeon
+```
+then simply run with:
 ```sh
-curl https://shinysocks.net/install.sh | bash
+textdungeon
 ```
-Installs in working directory and generates desktop entry.
 
 ### Windows
 Download text-dungeon.exe from [latest](https://github.com/Masbender/text-dungeon/releases/latest)
 
-### Python PIP [WIP]
-```sh
-pip install text-dungeon
-```
```


# Comparing `tmp/textureminer-1.0.0.tar.gz` & `tmp/textureminer-1.1.0.tar.gz`

## Comparing `textureminer-1.0.0.tar` & `textureminer-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 textureminer-1.0.0/requirements.txt
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 textureminer-1.0.0/.vscode/tasks.json
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/__init__.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/__main__.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/bedrock.py
--rw-r--r--   0        0        0     7721 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/common.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/java.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 textureminer-1.0.0/src/textureminer/texts.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 textureminer-1.0.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 textureminer-1.0.0/LICENSE
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 textureminer-1.0.0/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 textureminer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 textureminer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 textureminer-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 textureminer-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 textureminer-1.1.0/.vscode/tasks.json
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 textureminer-1.1.0/src/textureminer/__init__.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 textureminer-1.1.0/src/textureminer/__main__.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 textureminer-1.1.0/src/textureminer/bedrock.py
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 textureminer-1.1.0/src/textureminer/common.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 textureminer-1.1.0/src/textureminer/java.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 textureminer-1.1.0/src/textureminer/texts.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 textureminer-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 textureminer-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 textureminer-1.1.0/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 textureminer-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 textureminer-1.1.0/PKG-INFO
```

### Comparing `textureminer-1.0.0/src/textureminer/__main__.py` & `textureminer-1.1.0/src/textureminer/__main__.py`

 * *Files identical despite different names*

### Comparing `textureminer-1.0.0/src/textureminer/bedrock.py` & `textureminer-1.1.0/src/textureminer/bedrock.py`

 * *Files identical despite different names*

### Comparing `textureminer-1.0.0/src/textureminer/common.py` & `textureminer-1.1.0/src/textureminer/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from enum import Enum
 import os
 import re
 from shutil import copytree, rmtree
 import stat
 import tempfile
+from PIL import Image as pil_image
 from forfiles import image, file as f
 from textureminer import texts
 
 HOME_DIR = os.path.expanduser('~').replace('\\', '/')
 TEMP_PATH = f'{tempfile.gettempdir()}/texture_miner'.replace('\\', '/')
 
-DEFAULT_OUTPUT_DIR = f'{HOME_DIR}/Downloads/textures'
+DEFAULT_OUTPUT_DIR = os.path.normpath(f'{HOME_DIR}/Downloads/textures')
 DEFAULT_SCALE_FACTOR = 100
 
 REGEX_BEDROCK_RELEASE = r'^v1\.[0-9]{2}\.[0-9]{1,2}\.[0-9]{1,2}$'
 REGEX_BEDROCK_PREVIEW = r'^v1\.[0-9]{2}\.[0-9]{1,2}\.[0-9]{1,2}-preview$'
 
 REGEX_JAVA_SNAPSHOT = r'^[0-9]{2}w[0-9]{2}[a-z]$'
 REGEX_JAVA_PRE = r'^[0-9]\.[0-9]+\.?[0-9]+-pre[0-9]?$'
@@ -189,39 +190,45 @@
     rmtree(block_folder)
     copytree(item_folder, output_dir, dirs_exist_ok=True)
     rmtree(item_folder)
 
 
 def scale_textures(path: str,
                    scale_factor: int = 100,
-                   do_merge: bool = True) -> str:
+                   do_merge: bool = True,
+                   crop: bool = True) -> str:
     """Scales textures within a directory by a factor
 
     Args:
         path (string): path of the textures that will be scaled
         scale_factor (int): factor that the textures will be scaled by
         do_merge (bool): whether to merge block and item texture files into a single directory
+        crop (bool): whether to crop non-square textures to be square
 
     Returns:
         string: path of the scaled textures
     """
 
     if do_merge:
         merge_dirs(path, path)
     tabbed_print(texts.TEXTURES_FILTERING)
     for subdir, _, files in os.walk(path):
         f.filter(f'{os.path.abspath(subdir)}', ['.png'])
 
-        if scale_factor == 1:
-            continue
-
-        if len(files) > 0:
+        if scale_factor != 1 and len(files) > 0:
             tabbed_print(
                 texts.TEXTURES_RESIZING_AMOUNT.format(texture_amount=len(files))
                 if do_merge else texts.TEXTURES_RESISING_AMOUNT_IN_DIR.
                 format(len(files), os.path.basename(subdir)))
 
         for fil in files:
-            image.scale(f"{os.path.abspath(subdir)}/{fil}", scale_factor,
-                        scale_factor)
+            image_path = os.path.normpath(f"{os.path.abspath(subdir)}/{fil}")
+            if crop:
+                with pil_image.open(image_path) as img:
+                    if img.size[0] > 16 or img.size[1] > 16:
+                        img = img.crop((0, 0, 16, 16))
+                        img.save(image_path)
+
+            if scale_factor != 1:
+                image.scale(image_path, scale_factor, scale_factor)
 
     return path
```

### Comparing `textureminer-1.0.0/src/textureminer/java.py` & `textureminer-1.1.0/src/textureminer/java.py`

 * *Files identical despite different names*

### Comparing `textureminer-1.0.0/src/textureminer/texts.py` & `textureminer-1.1.0/src/textureminer/texts.py`

 * *Files identical despite different names*

### Comparing `textureminer-1.0.0/.gitignore` & `textureminer-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `textureminer-1.0.0/LICENSE` & `textureminer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textureminer-1.0.0/README.md` & `textureminer-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `textureminer-1.0.0/pyproject.toml` & `textureminer-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "textureminer"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="4MBL" },
 ]
 description = "Script that allows you to extract and scale Minecraft's item and block textures."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.11"
```

### Comparing `textureminer-1.0.0/PKG-INFO` & `textureminer-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textureminer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Script that allows you to extract and scale Minecraft's item and block textures.
 Project-URL: Homepage, https://github.com/4MBL/texture-miner
 Project-URL: Bug Tracker, https://github.com/4MBL/texture-miner/issues
 Author: 4MBL
 License: MIT License
         
         Copyright (c) 2023 4MBL
```


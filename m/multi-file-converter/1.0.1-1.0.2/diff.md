# Comparing `tmp/multi_file_converter-1.0.1.tar.gz` & `tmp/multi_file_converter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_file_converter-1.0.1.tar", last modified: Tue Jul  4 14:13:09 2023, max compression
+gzip compressed data, was "multi_file_converter-1.0.2.tar", last modified: Fri Jul  7 11:15:43 2023, max compression
```

## Comparing `multi_file_converter-1.0.1.tar` & `multi_file_converter-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:13:09.947441 multi_file_converter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-04 14:13:09.947441 multi_file_converter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:13:09.947441 multi_file_converter-1.0.1/file_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/docx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:13:09.947441 multi_file_converter-1.0.1/file_converter/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/jpg.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/png.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:13:09.947441 multi_file_converter-1.0.1/file_converter/types/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/file_converter/types/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:13:09.947441 multi_file_converter-1.0.1/multi_file_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-04 14:13:09.000000 multi_file_converter-1.0.1/multi_file_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-04 14:13:09.000000 multi_file_converter-1.0.1/multi_file_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:13:09.000000 multi_file_converter-1.0.1/multi_file_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 14:13:09.000000 multi_file_converter-1.0.1/multi_file_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 14:13:09.000000 multi_file_converter-1.0.1/multi_file_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:13:09.947441 multi_file_converter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-04 14:12:59.000000 multi_file_converter-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:15:43.091063 multi_file_converter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 11:15:43.091063 multi_file_converter-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:15:43.087063 multi_file_converter-1.0.2/file_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/docx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:15:43.087063 multi_file_converter-1.0.2/file_converter/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/jpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/png.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:15:43.087063 multi_file_converter-1.0.2/file_converter/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/file_converter/types/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:15:43.091063 multi_file_converter-1.0.2/multi_file_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 11:15:43.000000 multi_file_converter-1.0.2/multi_file_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 11:15:43.000000 multi_file_converter-1.0.2/multi_file_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:15:43.000000 multi_file_converter-1.0.2/multi_file_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 11:15:43.000000 multi_file_converter-1.0.2/multi_file_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 11:15:43.000000 multi_file_converter-1.0.2/multi_file_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:15:43.091063 multi_file_converter-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-07 11:15:33.000000 multi_file_converter-1.0.2/setup.py
```

### Comparing `multi_file_converter-1.0.1/PKG-INFO` & `multi_file_converter-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi_file_converter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple way to convert files to another formats
 Home-page: https://github.com/DAKExDUCK/FileConverter
 Author: dake_duck
 Author-email: arsengabdulin228@gmail.com
 Project-URL: GutHub, https://github.com/DAKExDUCK/FileConverter
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `multi_file_converter-1.0.1/README.md` & `multi_file_converter-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.1/file_converter/jpg.py` & `multi_file_converter-1.0.2/file_converter/jpg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import BytesIO
 
 from PIL import Image
 
-from file_converter.types.image import Img, Imgs
+from .types.image import Img, Imgs
 
 
 class JPG(Img):
     can_converts_to = [
         'pdf',
         'png',
         'bmp',
```

### Comparing `multi_file_converter-1.0.1/file_converter/types/document.py` & `multi_file_converter-1.0.2/file_converter/types/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import subprocess
 from io import BytesIO
 
-from file_converter.exceptions import ErrorConvertFile
-from file_converter.utils.tmp_file_manager import TmpFileManager as TFM
+from ..exceptions import ErrorConvertFile
+from ..utils.tmp_file_manager import TmpFileManager as TFM
 
 
 class Document:
     can_converts_to: list
     format: str
     doc: BytesIO
```

### Comparing `multi_file_converter-1.0.1/file_converter/types/image.py` & `multi_file_converter-1.0.2/file_converter/types/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from copy import deepcopy
 from io import BytesIO
 from PIL import Image
 
-from file_converter.exceptions import ErrorConvertFile
+from ..exceptions import ErrorConvertFile
 
 
 class Img:
     can_converts_to: list
     format: str
     img: Image.Image
```

### Comparing `multi_file_converter-1.0.1/multi_file_converter.egg-info/PKG-INFO` & `multi_file_converter-1.0.2/multi_file_converter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-file-converter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple way to convert files to another formats
 Home-page: https://github.com/DAKExDUCK/FileConverter
 Author: dake_duck
 Author-email: arsengabdulin228@gmail.com
 Project-URL: GutHub, https://github.com/DAKExDUCK/FileConverter
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `multi_file_converter-1.0.1/setup.py` & `multi_file_converter-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='multi_file_converter',
-  version='1.0.1',
+  version='1.0.2',
   author='dake_duck',
   author_email='arsengabdulin228@gmail.com',
   description='Simple way to convert files to another formats',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/DAKExDUCK/FileConverter',
   packages=find_packages(),
```


# Comparing `tmp/PyNihongo-0.0.1.dev2.tar.gz` & `tmp/PyNihongo-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNihongo-0.0.1.dev2.tar", last modified: Fri Jun 16 18:03:40 2023, max compression
+gzip compressed data, was "PyNihongo-0.0.1.dev3.tar", last modified: Fri Jul  7 12:50:16 2023, max compression
```

## Comparing `PyNihongo-0.0.1.dev2.tar` & `PyNihongo-0.0.1.dev3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:40.258369 PyNihongo-0.0.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 18:03:26.000000 PyNihongo-0.0.1.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-16 18:03:40.258369 PyNihongo-0.0.1.dev2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:40.254369 PyNihongo-0.0.1.dev2/PyNihongo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-16 18:03:40.000000 PyNihongo-0.0.1.dev2/PyNihongo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-16 18:03:40.000000 PyNihongo-0.0.1.dev2/PyNihongo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:03:40.000000 PyNihongo-0.0.1.dev2/PyNihongo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 18:03:40.000000 PyNihongo-0.0.1.dev2/PyNihongo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-16 18:03:26.000000 PyNihongo-0.0.1.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:40.254369 PyNihongo-0.0.1.dev2/pynihongo/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-16 18:03:26.000000 PyNihongo-0.0.1.dev2/pynihongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-16 18:03:26.000000 PyNihongo-0.0.1.dev2/pynihongo/kana.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 18:03:26.000000 PyNihongo-0.0.1.dev2/pynihongo/method.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:03:40.258369 PyNihongo-0.0.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-16 18:03:26.000000 PyNihongo-0.0.1.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 12:50:16.000000 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-07 12:50:16.000000 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:50:16.000000 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 12:50:16.000000 PyNihongo-0.0.1.dev3/PyNihongo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/pynihongo/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/pynihongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/pynihongo/kana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/pynihongo/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:50:16.633996 PyNihongo-0.0.1.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-07 12:49:56.000000 PyNihongo-0.0.1.dev3/setup.py
```

### Comparing `PyNihongo-0.0.1.dev2/LICENSE` & `PyNihongo-0.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNihongo-0.0.1.dev2/PKG-INFO` & `PyNihongo-0.0.1.dev3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNihongo
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: A Python package about japanese.
 Author: Koushoken
 Author-email: kskjcx-dev@yahoo.co.jp
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynihongo
```

### Comparing `PyNihongo-0.0.1.dev2/PyNihongo.egg-info/PKG-INFO` & `PyNihongo-0.0.1.dev3/PyNihongo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNihongo
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: A Python package about japanese.
 Author: Koushoken
 Author-email: kskjcx-dev@yahoo.co.jp
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynihongo
```

### Comparing `PyNihongo-0.0.1.dev2/README.md` & `PyNihongo-0.0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `PyNihongo-0.0.1.dev2/pynihongo/__init__.py` & `PyNihongo-0.0.1.dev3/pynihongo/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,21 +4,29 @@
 @Author: KouShoken
 
 This is an open source project that uses the MIT protocol. 
 While I don't make any demands, But　I think respecting copyright 
 maybe is a basic morality.
 """
 from .kana import Kana
-from .method import Method
+from .method import *
 
 
 class Get:
+    """
+
+    """
+
+    '''仮名'''
     __kana = Kana()
     gojyuon_table = __kana.gojyuon_table
 
     # 仮名（戦前の仮名も含む, 清音のみ）
     hiragana_list = __kana.hiragana_list
     katagana_list = __kana.katagana_list
     romaji_list = __kana.romaji_list
 
     # 現代仮名（戦前の仮名はない, 清音のみ）
     kendai_hiragana_list = []
+
+    '''地理'''
+    todofuken = JapanCountries()
```

### Comparing `PyNihongo-0.0.1.dev2/pynihongo/kana.py` & `PyNihongo-0.0.1.dev3/pynihongo/kana.py`

 * *Files identical despite different names*

### Comparing `PyNihongo-0.0.1.dev2/setup.py` & `PyNihongo-0.0.1.dev3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 maybe is a basic morality.
 """
 import functools
 from datetime import datetime
 
 from setuptools import setup
 
-with open("./README.md", "r") as f:
-    long_description = f.read()
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     long_description=long_description,
     long_description_content_type='text/markdown',
     name='PyNihongo',
-    version='0.0.1dev2',
+    version='0.0.1dev3',
     author='Koushoken',
     author_email='kskjcx-dev@yahoo.co.jp',
     description='A Python package about japanese.',
     packages=['pynihongo'],
     install_requires=[
     ],
 )
```


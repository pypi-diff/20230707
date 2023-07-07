# Comparing `tmp/zen_han_converter-1.0.0.tar.gz` & `tmp/zen_han_converter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen_han_converter-1.0.0.tar", last modified: Mon Jul  3 13:17:41 2023, max compression
+gzip compressed data, was "zen_han_converter-1.0.1.tar", last modified: Fri Jul  7 15:50:52 2023, max compression
```

## Comparing `zen_han_converter-1.0.0.tar` & `zen_han_converter-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:17:41.511515 zen_han_converter-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-03 13:17:41.510227 zen_han_converter-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      446 2023-07-02 04:22:16.000000 zen_han_converter-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 13:17:41.512106 zen_han_converter-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      529 2023-07-03 13:09:09.000000 zen_han_converter-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:17:41.476081 zen_han_converter-1.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-18 16:22:01.000000 zen_han_converter-1.0.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-18 16:22:01.000000 zen_han_converter-1.0.0/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-07-02 13:07:35.000000 zen_han_converter-1.0.0/tests/test_zen_han_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:17:41.489533 zen_han_converter-1.0.0/zen_han_converter/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 13:11:53.000000 zen_han_converter-1.0.0/zen_han_converter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1401 2023-07-02 13:07:35.000000 zen_han_converter-1.0.0/zen_han_converter/han_to_zen_table.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-07-02 13:07:35.000000 zen_han_converter-1.0.0/zen_han_converter/zen_han_convter.py
--rw-r--r--   0 root         (0) root         (0)     1401 2023-07-02 13:07:35.000000 zen_han_converter-1.0.0/zen_han_converter/zen_to_han_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:17:41.506415 zen_han_converter-1.0.0/zen_han_converter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      770 2023-07-03 13:17:41.000000 zen_han_converter-1.0.0/zen_han_converter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      393 2023-07-03 13:17:41.000000 zen_han_converter-1.0.0/zen_han_converter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 13:17:41.000000 zen_han_converter-1.0.0/zen_han_converter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-03 13:17:41.000000 zen_han_converter-1.0.0/zen_han_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/tests/test_zen_han_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/zen_han_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/zen_han_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/zen_han_converter/han_to_zen_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/zen_han_converter/zen_han_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 15:50:40.000000 zen_han_converter-1.0.1/zen_han_converter/zen_to_han_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:52.988296 zen_han_converter-1.0.1/zen_han_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-07 15:50:52.000000 zen_han_converter-1.0.1/zen_han_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-07 15:50:52.000000 zen_han_converter-1.0.1/zen_han_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:50:52.000000 zen_han_converter-1.0.1/zen_han_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 15:50:52.000000 zen_han_converter-1.0.1/zen_han_converter.egg-info/top_level.txt
```

### Comparing `zen_han_converter-1.0.0/PKG-INFO` & `zen_han_converter-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: zen_han_converter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Converts full-width and half-width characters.
 Home-page: https://github.com/n4cl/zen_han_converter.git
 Author: n4cl
 Author-email: devn4cl@gmail.com
 License: MIT
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 zen_han_converter
 ===
 
 # Description
```

### Comparing `zen_han_converter-1.0.0/setup.py` & `zen_han_converter-1.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="zen_han_converter",
-    version="1.0.0",
+    version="1.0.1",
     author="n4cl",
     author_email="devn4cl@gmail.com",
     description="Converts full-width and half-width characters.",
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/n4cl/zen_han_converter.git",
     license='MIT',
     packages=find_packages(),
+    package_dir={"zen_han_converter": "zen_han_converter"},
     classifiers=[
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11"
     ]
 )
```

### Comparing `zen_han_converter-1.0.0/tests/test_zen_han_converter.py` & `zen_han_converter-1.0.1/tests/test_zen_han_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from zen_han_converter.zen_han_convter import ZenToHan, HanToZen
+from zen_han_converter.zen_han_converter import ZenToHan, HanToZen
 
 
 def test_ZenToHan():
     zen_to_han = ZenToHan(alphabet_table=True, number_table=True, ascii_symbol_table=True)
     assert zen_to_han.convert('ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ') == 'abcdefghijklmnopqrstuvwxyz'
     assert zen_to_han.convert('abcdefghijklmnopqrstuvwxyz') == 'abcdefghijklmnopqrstuvwxyz'
     assert zen_to_han.convert('０１２３４５６７８９') == '0123456789'
```

### Comparing `zen_han_converter-1.0.0/zen_han_converter/han_to_zen_table.py` & `zen_han_converter-1.0.1/zen_han_converter/han_to_zen_table.py`

 * *Files identical despite different names*

### Comparing `zen_han_converter-1.0.0/zen_han_converter/zen_han_convter.py` & `zen_han_converter-1.0.1/zen_han_converter/zen_han_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from han_to_zen_table import LATIN_ALPHABET as HAN2ZEN_LATIN_ALPHABET, \
+from .han_to_zen_table import LATIN_ALPHABET as HAN2ZEN_LATIN_ALPHABET, \
                              ARABIC_NUMERALS as HAN2ZEN_ARABIC_NUMERALS, \
                              ASCII_SYMBOL as HAN2ZEN_ASCII_SYMBOL
-from zen_to_han_table import LATIN_ALPHABET as ZEN2HAN_LATIN_ALPHABET, \
+from .zen_to_han_table import LATIN_ALPHABET as ZEN2HAN_LATIN_ALPHABET, \
                              ARABIC_NUMERALS as ZEN2HAN_ARABIC_NUMERALS, \
                              ASCII_SYMBOL as ZEN2HAN_ASCII_SYMBOL
 
 
 class BaseConverter:
     """
     コンバーターの基底クラス
```

### Comparing `zen_han_converter-1.0.0/zen_han_converter/zen_to_han_table.py` & `zen_han_converter-1.0.1/zen_han_converter/zen_to_han_table.py`

 * *Files identical despite different names*

### Comparing `zen_han_converter-1.0.0/zen_han_converter.egg-info/PKG-INFO` & `zen_han_converter-1.0.1/zen_han_converter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: zen-han-converter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Converts full-width and half-width characters.
 Home-page: https://github.com/n4cl/zen_han_converter.git
 Author: n4cl
 Author-email: devn4cl@gmail.com
 License: MIT
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 zen_han_converter
 ===
 
 # Description
```


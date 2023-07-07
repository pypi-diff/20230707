# Comparing `tmp/woofy-0.1.0.tar.gz` & `tmp/woofy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woofy-0.1.0.tar", max compression
+gzip compressed data, was "woofy-1.0.0.tar", max compression
```

## Comparing `woofy-0.1.0.tar` & `woofy-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1086 2023-07-07 11:50:47.481091 woofy-0.1.0/LICENSE
--rw-r--r--   0        0        0      917 2023-07-07 11:56:31.086826 woofy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      592 2023-07-07 11:59:28.633255 woofy-0.1.0/README.md
--rw-r--r--   0        0        0      183 2023-07-07 11:58:14.218216 woofy-0.1.0/src/woofy/__init__.py
--rw-r--r--   0        0        0      282 2023-07-07 11:56:55.865237 woofy-0.1.0/src/woofy/client.py
--rw-r--r--   0        0        0        6 2023-07-07 11:57:23.681233 woofy-0.1.0/src/woofy/manager/__init__.py
--rw-r--r--   0        0        0      444 2023-07-07 11:57:44.372577 woofy-0.1.0/src/woofy/manager/image.py
--rw-r--r--   0        0        0        6 2023-07-07 11:57:21.004450 woofy-0.1.0/src/woofy/struct/__init__.py
--rw-r--r--   0        0        0      114 2023-07-07 11:57:57.114858 woofy-0.1.0/src/woofy/struct/image.py
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 woofy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-07 11:50:47.481091 woofy-1.0.0/LICENSE
+-rw-r--r--   0        0        0      917 2023-07-07 12:01:05.326692 woofy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      592 2023-07-07 12:00:49.712214 woofy-1.0.0/README.md
+-rw-r--r--   0        0        0      183 2023-07-07 11:58:14.218216 woofy-1.0.0/src/woofy/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-07 11:56:55.865237 woofy-1.0.0/src/woofy/client.py
+-rw-r--r--   0        0        0        6 2023-07-07 11:57:23.681233 woofy-1.0.0/src/woofy/manager/__init__.py
+-rw-r--r--   0        0        0      444 2023-07-07 11:57:44.372577 woofy-1.0.0/src/woofy/manager/image.py
+-rw-r--r--   0        0        0        6 2023-07-07 11:57:21.004450 woofy-1.0.0/src/woofy/struct/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-07 11:57:57.114858 woofy-1.0.0/src/woofy/struct/image.py
+-rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 woofy-1.0.0/PKG-INFO
```

### Comparing `woofy-0.1.0/LICENSE` & `woofy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `woofy-0.1.0/pyproject.toml` & `woofy-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "woofy"
-version = "0.1.0"
+version = "1.0.0"
 description = "🐶 An unofficial The Dog API wrapper for Python"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/elaresai/woofy"
 repository = "https://github.com/elaresai/woofy"
```

### Comparing `woofy-0.1.0/README.md` & `woofy-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [_examples/basic.py_](https://github.com/elaresai/woofy/blob/main/examples/basic.py)
 
 ```py
 import woofy
 
 
-client = meowy.Client()
+client = woofy.Client()
 
 # Let's search for 10 images at once
 for _ in range(10):
     print(client.images.search())
 ```
 
 # ✨ Links
```

### Comparing `woofy-0.1.0/PKG-INFO` & `woofy-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woofy
-Version: 0.1.0
+Version: 1.0.0
 Summary: 🐶 An unofficial The Dog API wrapper for Python
 Home-page: https://github.com/elaresai/woofy
 License: MIT
 Author: elaresai
 Author-email: elaresai@gmail.com
 Maintainer: elaresai
 Maintainer-email: elaresai@gmail.com
@@ -38,15 +38,15 @@
 
 [_examples/basic.py_](https://github.com/elaresai/woofy/blob/main/examples/basic.py)
 
 ```py
 import woofy
 
 
-client = meowy.Client()
+client = woofy.Client()
 
 # Let's search for 10 images at once
 for _ in range(10):
     print(client.images.search())
 ```
 
 # ✨ Links
```


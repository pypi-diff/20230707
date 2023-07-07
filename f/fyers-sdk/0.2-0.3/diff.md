# Comparing `tmp/fyers_sdk-0.2.tar.gz` & `tmp/fyers_sdk-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-0.2.tar", last modified: Fri Jul  7 09:05:00 2023, max compression
+gzip compressed data, was "fyers_sdk-0.3.tar", last modified: Fri Jul  7 09:14:27 2023, max compression
```

## Comparing `fyers_sdk-0.2.tar` & `fyers_sdk-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:05:00.530386 fyers_sdk-0.2/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-06-30 14:05:35.000000 fyers_sdk-0.2/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 09:05:00.530386 fyers_sdk-0.2/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10390 2023-07-03 07:06:42.000000 fyers_sdk-0.2/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:05:00.510388 fyers_sdk-0.2/fyersAPI/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       18 2023-07-07 07:45:48.000000 fyers_sdk-0.2/fyersAPI/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      923 2023-06-30 09:29:39.000000 fyers_sdk-0.2/fyersAPI/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    28056 2023-07-03 09:38:05.000000 fyers_sdk-0.2/fyersAPI/fyers_api.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-03 12:46:12.000000 fyers_sdk-0.2/fyersAPI/fyers_logger.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15032 2023-06-30 13:16:29.000000 fyers_sdk-0.2/fyersAPI/order_ws.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:05:00.530386 fyers_sdk-0.2/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 09:04:59.000000 fyers_sdk-0.2/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      303 2023-07-07 09:05:00.000000 fyers_sdk-0.2/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-07 09:05:00.000000 fyers_sdk-0.2/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       96 2023-07-07 09:05:00.000000 fyers_sdk-0.2/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        9 2023-07-07 09:05:00.000000 fyers_sdk-0.2/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-07 09:05:00.530386 fyers_sdk-0.2/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)      804 2023-07-07 09:04:44.000000 fyers_sdk-0.2/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:27.890970 fyers_sdk-0.3/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-06-30 14:05:35.000000 fyers_sdk-0.3/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 09:14:27.890970 fyers_sdk-0.3/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10390 2023-07-03 07:06:42.000000 fyers_sdk-0.3/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:27.862971 fyers_sdk-0.3/fyersAPI/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:06.000000 fyers_sdk-0.3/fyersAPI/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      923 2023-06-30 09:29:39.000000 fyers_sdk-0.3/fyersAPI/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    28056 2023-07-03 09:38:05.000000 fyers_sdk-0.3/fyersAPI/fyers_api.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-03 12:46:12.000000 fyers_sdk-0.3/fyersAPI/fyers_logger.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15032 2023-06-30 13:16:29.000000 fyers_sdk-0.3/fyersAPI/order_ws.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:27.890970 fyers_sdk-0.3/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 09:14:27.000000 fyers_sdk-0.3/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      303 2023-07-07 09:14:27.000000 fyers_sdk-0.3/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-07 09:14:27.000000 fyers_sdk-0.3/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       96 2023-07-07 09:14:27.000000 fyers_sdk-0.3/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        9 2023-07-07 09:14:27.000000 fyers_sdk-0.3/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-07 09:14:27.890970 fyers_sdk-0.3/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      804 2023-07-07 09:14:12.000000 fyers_sdk-0.3/setup.py
```

### Comparing `fyers_sdk-0.2/LICENSE.txt` & `fyers_sdk-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-0.2/PKG-INFO` & `fyers_sdk-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 0.2
+Version: 0.3
 Summary: Fyers trading APIs.
 Home-page: https://github.com/
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fyers_sdk-0.2/README.md` & `fyers_sdk-0.3/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-0.2/fyersAPI/defines.py` & `fyers_sdk-0.3/fyersAPI/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-0.2/fyersAPI/fyers_api.py` & `fyers_sdk-0.3/fyersAPI/fyers_api.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-0.2/fyersAPI/fyers_logger.py` & `fyers_sdk-0.3/fyersAPI/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-0.2/fyersAPI/order_ws.py` & `fyers_sdk-0.3/fyersAPI/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-0.2/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-0.3/fyers_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 0.2
+Version: 0.3
 Summary: Fyers trading APIs.
 Home-page: https://github.com/
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fyers_sdk-0.2/setup.py` & `fyers_sdk-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='0.2',
+     version='0.3',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/",
      packages=setuptools.find_packages(),
```


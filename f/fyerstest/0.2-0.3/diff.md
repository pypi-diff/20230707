# Comparing `tmp/fyerstest-0.2.tar.gz` & `tmp/fyerstest-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyerstest-0.2.tar", last modified: Fri Jul  7 09:39:54 2023, max compression
+gzip compressed data, was "fyerstest-0.3.tar", last modified: Fri Jul  7 10:24:50 2023, max compression
```

## Comparing `fyerstest-0.2.tar` & `fyerstest-0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:39:54.057102 fyerstest-0.2/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-06-30 14:05:35.000000 fyerstest-0.2/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 09:39:54.057102 fyerstest-0.2/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10390 2023-07-03 07:06:42.000000 fyerstest-0.2/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:39:54.033103 fyerstest-0.2/fyerstest/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:06.000000 fyerstest-0.2/fyerstest/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    54530 2023-07-07 09:39:30.000000 fyerstest-0.2/fyerstest/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      923 2023-06-30 09:29:39.000000 fyerstest-0.2/fyerstest/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    28056 2023-07-03 09:38:05.000000 fyerstest-0.2/fyerstest/fyers_api.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-03 12:46:12.000000 fyerstest-0.2/fyerstest/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:39:54.053103 fyerstest-0.2/fyerstest.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 09:39:53.000000 fyerstest-0.2/fyerstest.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      307 2023-07-07 09:39:53.000000 fyerstest-0.2/fyerstest.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-07 09:39:53.000000 fyerstest-0.2/fyerstest.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      126 2023-07-07 09:39:53.000000 fyerstest-0.2/fyerstest.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-07 09:39:53.000000 fyerstest-0.2/fyerstest.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-07 09:39:54.057102 fyerstest-0.2/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)      849 2023-07-07 09:39:40.000000 fyerstest-0.2/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 10:24:50.086278 fyerstest-0.3/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-06-30 14:05:35.000000 fyerstest-0.3/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 10:24:50.086278 fyerstest-0.3/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10390 2023-07-03 07:06:42.000000 fyerstest-0.3/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 10:24:50.066279 fyerstest-0.3/fyerstest/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:06.000000 fyerstest-0.3/fyerstest/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    54530 2023-07-07 09:39:30.000000 fyerstest-0.3/fyerstest/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      923 2023-06-30 09:29:39.000000 fyerstest-0.3/fyerstest/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    28056 2023-07-03 09:38:05.000000 fyerstest-0.3/fyerstest/fyers_api.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-03 12:46:12.000000 fyerstest-0.3/fyerstest/fyers_logger.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-03 06:30:48.000000 fyerstest-0.3/fyerstest/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15032 2023-06-30 13:16:29.000000 fyerstest-0.3/fyerstest/order_ws.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 10:24:50.086278 fyerstest-0.3/fyerstest.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 10:24:49.000000 fyerstest-0.3/fyerstest.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      348 2023-07-07 10:24:50.000000 fyerstest-0.3/fyerstest.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-07 10:24:49.000000 fyerstest-0.3/fyerstest.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      126 2023-07-07 10:24:49.000000 fyerstest-0.3/fyerstest.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-07 10:24:49.000000 fyerstest-0.3/fyerstest.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-07 10:24:50.086278 fyerstest-0.3/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      957 2023-07-07 10:24:40.000000 fyerstest-0.3/setup.py
```

### Comparing `fyerstest-0.2/LICENSE.txt` & `fyerstest-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyerstest-0.2/PKG-INFO` & `fyerstest-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyerstest
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

### Comparing `fyerstest-0.2/README.md` & `fyerstest-0.3/README.md`

 * *Files identical despite different names*

### Comparing `fyerstest-0.2/fyerstest/data_ws.py` & `fyerstest-0.3/fyerstest/data_ws.py`

 * *Files identical despite different names*

### Comparing `fyerstest-0.2/fyerstest/defines.py` & `fyerstest-0.3/fyerstest/defines.py`

 * *Files identical despite different names*

### Comparing `fyerstest-0.2/fyerstest/fyers_api.py` & `fyerstest-0.3/fyerstest/fyers_api.py`

 * *Files identical despite different names*

### Comparing `fyerstest-0.2/fyerstest/fyers_logger.py` & `fyerstest-0.3/fyerstest/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyerstest-0.2/fyerstest.egg-info/PKG-INFO` & `fyerstest-0.3/fyerstest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyerstest
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

### Comparing `fyerstest-0.2/setup.py` & `fyerstest-0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyerstest',  
-     version='0.2',
+     version='0.3',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/",
      packages=setuptools.find_packages(),
+     package_data={
+         'fyerstest': ['/home/vinay/Documents/SDK/fyersSdk/fyerstest/map.json']
+     },
      install_requires=[
             'aiohttp==3.8.4',
             'Requests==2.31.0',
             'websocket_client==1.2.1',
             'websocket_client==1.2.1',
             'websockets==8.1',
             'aws_lambda_powertools==2.19.0'
```


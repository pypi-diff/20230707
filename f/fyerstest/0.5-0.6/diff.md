# Comparing `tmp/fyerstest-0.5.tar.gz` & `tmp/fyerstest-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyerstest-0.5.tar", last modified: Fri Jul  7 10:32:39 2023, max compression
+gzip compressed data, was "fyerstest-0.6.tar", last modified: Fri Jul  7 12:02:45 2023, max compression
```

## Comparing `fyerstest-0.5.tar` & `fyerstest-0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 10:32:39.693120 fyerstest-0.5/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-06-30 14:05:35.000000 fyerstest-0.5/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 10:32:39.693120 fyerstest-0.5/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10390 2023-07-03 07:06:42.000000 fyerstest-0.5/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 10:32:39.669119 fyerstest-0.5/fyerstest/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:06.000000 fyerstest-0.5/fyerstest/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    54575 2023-07-07 10:32:10.000000 fyerstest-0.5/fyerstest/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      923 2023-06-30 09:29:39.000000 fyerstest-0.5/fyerstest/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    28056 2023-07-03 09:38:05.000000 fyerstest-0.5/fyerstest/fyers_api.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-03 12:46:12.000000 fyerstest-0.5/fyerstest/fyers_logger.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-03 06:30:48.000000 fyerstest-0.5/fyerstest/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15032 2023-06-30 13:16:29.000000 fyerstest-0.5/fyerstest/order_ws.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 10:32:39.693120 fyerstest-0.5/fyerstest.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 10:32:39.000000 fyerstest-0.5/fyerstest.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      348 2023-07-07 10:32:39.000000 fyerstest-0.5/fyerstest.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-07 10:32:39.000000 fyerstest-0.5/fyerstest.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      126 2023-07-07 10:32:39.000000 fyerstest-0.5/fyerstest.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-07 10:32:39.000000 fyerstest-0.5/fyerstest.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-07 10:32:39.693120 fyerstest-0.5/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)      957 2023-07-07 10:32:25.000000 fyerstest-0.5/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 12:02:45.840663 fyerstest-0.6/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-06-30 14:05:35.000000 fyerstest-0.6/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 12:02:45.840663 fyerstest-0.6/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10390 2023-07-03 07:06:42.000000 fyerstest-0.6/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 12:02:45.816663 fyerstest-0.6/fyerstest/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:06.000000 fyerstest-0.6/fyerstest/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    54637 2023-07-07 12:02:13.000000 fyerstest-0.6/fyerstest/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      923 2023-06-30 09:29:39.000000 fyerstest-0.6/fyerstest/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    28056 2023-07-03 09:38:05.000000 fyerstest-0.6/fyerstest/fyers_api.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-03 12:46:12.000000 fyerstest-0.6/fyerstest/fyers_logger.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-03 06:30:48.000000 fyerstest-0.6/fyerstest/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15032 2023-06-30 13:16:29.000000 fyerstest-0.6/fyerstest/order_ws.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 12:02:45.840663 fyerstest-0.6/fyerstest.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 12:02:45.000000 fyerstest-0.6/fyerstest.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      348 2023-07-07 12:02:45.000000 fyerstest-0.6/fyerstest.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-07 12:02:45.000000 fyerstest-0.6/fyerstest.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      126 2023-07-07 12:02:45.000000 fyerstest-0.6/fyerstest.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-07 12:02:45.000000 fyerstest-0.6/fyerstest.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-07 12:02:45.840663 fyerstest-0.6/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      957 2023-07-07 12:02:25.000000 fyerstest-0.6/setup.py
```

### Comparing `fyerstest-0.5/LICENSE.txt` & `fyerstest-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyerstest-0.5/PKG-INFO` & `fyerstest-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyerstest
-Version: 0.5
+Version: 0.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fyerstest-0.5/README.md` & `fyerstest-0.6/README.md`

 * *Files identical despite different names*

### Comparing `fyerstest-0.5/fyerstest/data_ws.py` & `fyerstest-0.6/fyerstest/data_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         """
         try:
             symbols = ",".join(symbols)
             fyers = FyersModelv3(token=self.access_token, is_async=False)
             quote_data = fyers.quotes({"symbols": symbols})
             datadict = {}
             values = {}
-            with open("fyerstest/map.json", "r") as file:
+            with open("/home/vinay/Documents/SDK/fyersSdk/fyerstest/map.json", "r") as file:
                 # Load the JSON data into a Python object
                 mapper = json.load(file)
             index_dict = mapper["index_dict"]
             exch_seg_dict = mapper["exch_seg_dict"]
             wrong_symbol = []
             if "d" in quote_data:
                 for data in quote_data["d"]:
@@ -162,14 +162,15 @@
         self.channels = []
         self.running_channels = set()
         self.data_type = None
         self.OnMessage = OnMessage
         self.OnError = OnError
         self.OnOpen = OnOpen
         self.OnClose = OnClose
+        self.ack_count = 0
         self.__ws_run = None
         self.write_to_file = write_to_file
         self.background_flag = False
         self.update_count = 0
         self.literesp = {}
         self.channel_symbol = []
         self.symbol_dict = {}
```

### Comparing `fyerstest-0.5/fyerstest/defines.py` & `fyerstest-0.6/fyerstest/defines.py`

 * *Files identical despite different names*

### Comparing `fyerstest-0.5/fyerstest/fyers_api.py` & `fyerstest-0.6/fyerstest/fyers_api.py`

 * *Files identical despite different names*

### Comparing `fyerstest-0.5/fyerstest/fyers_logger.py` & `fyerstest-0.6/fyerstest/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyerstest-0.5/fyerstest/map.json` & `fyerstest-0.6/fyerstest/map.json`

 * *Files identical despite different names*

### Comparing `fyerstest-0.5/fyerstest/order_ws.py` & `fyerstest-0.6/fyerstest/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyerstest-0.5/fyerstest.egg-info/PKG-INFO` & `fyerstest-0.6/fyerstest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyerstest
-Version: 0.5
+Version: 0.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fyerstest-0.5/setup.py` & `fyerstest-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyerstest',  
-     version='0.5',
+     version='0.6',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/",
      packages=setuptools.find_packages(),
```


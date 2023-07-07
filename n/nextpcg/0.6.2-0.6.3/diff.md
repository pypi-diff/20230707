# Comparing `tmp/nextpcg-0.6.2.tar.gz` & `tmp/nextpcg-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.6.2.tar", last modified: Fri Jul  7 02:26:44 2023, max compression
+gzip compressed data, was "nextpcg-0.6.3.tar", last modified: Fri Jul  7 02:44:20 2023, max compression
```

## Comparing `nextpcg-0.6.2.tar` & `nextpcg-0.6.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.856495 nextpcg-0.6.2/
--rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-07-07 02:26:44.855494 nextpcg-0.6.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.819364 nextpcg-0.6.2/common/
--rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.2/common/__init__.py
--rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.2/common/nextpcg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.833376 nextpcg-0.6.2/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.2/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.850490 nextpcg-0.6.2/pypapi/
--rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.2/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.2/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.2/pypapi/const.py
--rw-rw-rw-   0        0        0     5658 2023-07-04 09:17:13.000000 nextpcg-0.6.2/pypapi/dispatch.py
--rw-rw-rw-   0        0        0     2124 2023-06-30 08:13:29.000000 nextpcg-0.6.2/pypapi/dson.py
--rw-rw-rw-   0        0        0     9235 2023-07-07 02:25:39.000000 nextpcg-0.6.2/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.2/pypapi/dson_field.py
--rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.2/pypapi/dson_geo.py
--rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.6.2/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.2/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.853492 nextpcg-0.6.2/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.6.2/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-07-03 07:47:15.000000 nextpcg-0.6.2/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.6.2/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-07-07 02:26:44.856495 nextpcg-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     2468 2023-07-07 02:26:33.000000 nextpcg-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.124362 nextpcg-0.6.3/
+-rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-07-07 02:44:20.123361 nextpcg-0.6.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.089797 nextpcg-0.6.3/common/
+-rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.3/common/__init__.py
+-rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.3/common/nextpcg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.102135 nextpcg-0.6.3/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.3/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.118357 nextpcg-0.6.3/pypapi/
+-rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.3/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.3/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.3/pypapi/const.py
+-rw-rw-rw-   0        0        0     5658 2023-07-04 09:17:13.000000 nextpcg-0.6.3/pypapi/dispatch.py
+-rw-rw-rw-   0        0        0     2124 2023-06-30 08:13:29.000000 nextpcg-0.6.3/pypapi/dson.py
+-rw-rw-rw-   0        0        0     8592 2023-07-07 02:43:28.000000 nextpcg-0.6.3/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.3/pypapi/dson_field.py
+-rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.3/pypapi/dson_geo.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.3/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.121360 nextpcg-0.6.3/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.6.3/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-07-03 07:47:15.000000 nextpcg-0.6.3/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2972 2023-07-07 02:43:08.000000 nextpcg-0.6.3/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:44:20.124362 nextpcg-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     2468 2023-07-07 02:43:58.000000 nextpcg-0.6.3/setup.py
```

### Comparing `nextpcg-0.6.2/PKG-INFO` & `nextpcg-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.6.2
+Version: 0.6.3
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.6.2/common/nextpcg.py` & `nextpcg-0.6.3/common/nextpcg.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.2/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.6.3/nextpcg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.6.2
+Version: 0.6.3
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.6.2/nextpcg.egg-info/SOURCES.txt` & `nextpcg-0.6.3/nextpcg.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,12 +13,11 @@
 pypapi/__main__.py
 pypapi/const.py
 pypapi/dispatch.py
 pypapi/dson.py
 pypapi/dson_create.py
 pypapi/dson_field.py
 pypapi/dson_geo.py
-pypapi/macro.py
 pypapi/meta_helper.py
 pypapi/plugin_protocol.py
 pypapi/pantry/dson_config.yaml
 pypapi/pantry/dson_generator.py
```

### Comparing `nextpcg-0.6.2/pypapi/__main__.py` & `nextpcg-0.6.3/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.2/pypapi/dispatch.py` & `nextpcg-0.6.3/pypapi/dispatch.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.2/pypapi/dson.py` & `nextpcg-0.6.3/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.2/pypapi/dson_create.py` & `nextpcg-0.6.3/pypapi/dson_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 import os
 import json
 import logging
 
 import common.nextpcg as nextpcg
 
 from pypapi.dispatch import Dispatcher
-from pypapi.plugin_protocol import module_send_done
+from pypapi.plugin_protocol import module_send_done, setup_logger
 
 """
     # load necessary modules or classes to dson_main_import
     dson_main_import = ''
     try:
         for module in dson_config['modules']:
             if isinstance(module, str):
@@ -142,45 +142,23 @@
                     dson_main_import = dson_main_import[:-1]
     except Exception as e:
         print(e)
         exit(1)
     # main function to dson_main_function
     dson_main_function = f"""
 
-def set_up_logger(logger, logger_path):
-    logFormatter = logging.Formatter('%(levelname)s:%(name)s:[%(asctime)s]: %(message)s')
-
-    if not os.path.exists(logger_path):
-        os.makedirs(logger_path)
-
-    logfile_path = os.path.join(logger_path, 'nextpcgpython.log')
-    # delete old log file
-    try:
-        os.remove(logfile_path)
-    except OSError:
-        pass
-
-    fileHandler = logging.FileHandler(logfile_path)
-    fileHandler.setFormatter(logFormatter)
-
-    consoleHandler = logging.StreamHandler()
-    consoleHandler.setFormatter(logFormatter)
-
-    logger.addHandler(fileHandler)
-    logger.addHandler(consoleHandler)
-
 
 if __name__ == '__main__':
     dson_plugin_name = '{dson_plugin_name}'
     logger = logging.getLogger('pypapi_'+dson_plugin_name)
     
     current_path = os.path.split(os.path.realpath(__file__))[0] # path to dosn_path.py
     dot_nextpcg_path = os.path.join(current_path, '.nextpcg')
 
-    set_up_logger(logger, dot_nextpcg_path)
+    setup_logger(logger, dot_nextpcg_path)
     
     module_send_done()
     while(True):
         json_file_name, work_path = input().split()
         json_error_data = {{}}
         try:
             with open(json_file_name, 'r') as f:
```

### Comparing `nextpcg-0.6.2/pypapi/dson_field.py` & `nextpcg-0.6.3/pypapi/dson_field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.2/pypapi/dson_geo.py` & `nextpcg-0.6.3/pypapi/dson_geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.2/pypapi/meta_helper.py` & `nextpcg-0.6.3/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.2/pypapi/pantry/dson_generator.py` & `nextpcg-0.6.3/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.2/pypapi/plugin_protocol.py` & `nextpcg-0.6.3/pypapi/plugin_protocol.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,50 @@
 # -*- coding: utf-8 -*-
 """simple protocol for dispatch to user defined plugin
 Author  : NextPCG
 """
 
 import os
 import json
+import logging
 import threading
 import asyncio
 from concurrent.futures import Future, ThreadPoolExecutor
 
-PROTOCOL_DONE = "s8xc32ds5f" # abitray code
+# magic code
+PROTOCOL_DONE = "s8xc32ds5f"
 
 
 def module_send_done():
     print(PROTOCOL_DONE)
 
 
+def setup_logger(logger, logger_path):
+    logFormatter = logging.Formatter('%(levelname)s:%(name)s:[%(asctime)s]: %(message)s')
+
+    if not os.path.exists(logger_path):
+        os.makedirs(logger_path)
+
+    logfile_path = os.path.join(logger_path, 'nextpcgpython.log')
+    # delete old log file
+    try:
+        os.remove(logfile_path)
+    except OSError:
+        pass
+
+    fileHandler = logging.FileHandler(logfile_path)
+    fileHandler.setFormatter(logFormatter)
+
+    consoleHandler = logging.StreamHandler()
+    consoleHandler.setFormatter(logFormatter)
+
+    logger.addHandler(fileHandler)
+    logger.addHandler(consoleHandler)
+
+
 async def server_check_done(proc, logger):
     """check whether task is done
     
     Args:
         proc(subprocess.Popen): process running dson_main.py """
     a = await run_as_daemon(proc.stdout.readline)
     while not PROTOCOL_DONE in a:
```

### Comparing `nextpcg-0.6.2/setup.py` & `nextpcg-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.6.2',
+    version='0.6.3',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```


# Comparing `tmp/nextpcg-0.6.1.tar.gz` & `tmp/nextpcg-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.6.1.tar", last modified: Fri Jul  7 02:22:27 2023, max compression
+gzip compressed data, was "nextpcg-0.6.2.tar", last modified: Fri Jul  7 02:26:44 2023, max compression
```

## Comparing `nextpcg-0.6.1.tar` & `nextpcg-0.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.877229 nextpcg-0.6.1/
--rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-07-07 02:22:27.876206 nextpcg-0.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.839537 nextpcg-0.6.1/common/
--rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.1/common/__init__.py
--rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.1/common/nextpcg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.851599 nextpcg-0.6.1/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.1/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.870550 nextpcg-0.6.1/pypapi/
--rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.1/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.1/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.1/pypapi/const.py
--rw-rw-rw-   0        0        0     5658 2023-07-04 09:17:13.000000 nextpcg-0.6.1/pypapi/dispatch.py
--rw-rw-rw-   0        0        0     2124 2023-06-30 08:13:29.000000 nextpcg-0.6.1/pypapi/dson.py
--rw-rw-rw-   0        0        0     9233 2023-07-07 02:20:55.000000 nextpcg-0.6.1/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.1/pypapi/dson_field.py
--rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.1/pypapi/dson_geo.py
--rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.6.1/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.1/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.874138 nextpcg-0.6.1/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.6.1/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-07-03 07:47:15.000000 nextpcg-0.6.1/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.6.1/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-07-07 02:22:27.877229 nextpcg-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     2468 2023-07-07 02:22:04.000000 nextpcg-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.856495 nextpcg-0.6.2/
+-rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-07-07 02:26:44.855494 nextpcg-0.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.819364 nextpcg-0.6.2/common/
+-rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.2/common/__init__.py
+-rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.2/common/nextpcg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.833376 nextpcg-0.6.2/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 02:26:44.000000 nextpcg-0.6.2/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.2/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.850490 nextpcg-0.6.2/pypapi/
+-rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.2/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.2/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.2/pypapi/const.py
+-rw-rw-rw-   0        0        0     5658 2023-07-04 09:17:13.000000 nextpcg-0.6.2/pypapi/dispatch.py
+-rw-rw-rw-   0        0        0     2124 2023-06-30 08:13:29.000000 nextpcg-0.6.2/pypapi/dson.py
+-rw-rw-rw-   0        0        0     9235 2023-07-07 02:25:39.000000 nextpcg-0.6.2/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.2/pypapi/dson_field.py
+-rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.2/pypapi/dson_geo.py
+-rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.6.2/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.2/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:26:44.853492 nextpcg-0.6.2/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.6.2/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-07-03 07:47:15.000000 nextpcg-0.6.2/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.6.2/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:26:44.856495 nextpcg-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     2468 2023-07-07 02:26:33.000000 nextpcg-0.6.2/setup.py
```

### Comparing `nextpcg-0.6.1/PKG-INFO` & `nextpcg-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.6.1
+Version: 0.6.2
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.6.1/common/nextpcg.py` & `nextpcg-0.6.2/common/nextpcg.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.6.2/nextpcg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.6.1
+Version: 0.6.2
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.6.1/nextpcg.egg-info/SOURCES.txt` & `nextpcg-0.6.2/nextpcg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/pypapi/__main__.py` & `nextpcg-0.6.2/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/pypapi/dispatch.py` & `nextpcg-0.6.2/pypapi/dispatch.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/pypapi/dson.py` & `nextpcg-0.6.2/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/pypapi/dson_create.py` & `nextpcg-0.6.2/pypapi/dson_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         json_error_data = {{}}
         try:
             with open(json_file_name, 'r') as f:
                 json_data = json.load(f)
             if not json_data:
                 print("didn't get dson data")
                 module_send_done()
-            dispatcher.run_func(json_data, logger, work_path, nextpcg.pson_system_tag, json_error_data)
+            Dispatcher().run_func(json_data, logger, work_path, nextpcg.pson_system_tag, json_error_data)
             json_data_error_file_name = os.path.join(work_path, 'error.json').replace("\\\\",'/')
             # write back json_data
             with open(json_file_name, 'w') as f:
                 json.dump(json_data, f)
         except Exception as e:
             json_error_data['Error_Tag'] = 'plugin {dson_plugin_name} error in main loop'
             json_error_data['Error_Info'] = str(e)
```

### Comparing `nextpcg-0.6.1/pypapi/dson_field.py` & `nextpcg-0.6.2/pypapi/dson_field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/pypapi/dson_geo.py` & `nextpcg-0.6.2/pypapi/dson_geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/pypapi/meta_helper.py` & `nextpcg-0.6.2/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/pypapi/pantry/dson_generator.py` & `nextpcg-0.6.2/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/pypapi/plugin_protocol.py` & `nextpcg-0.6.2/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.1/setup.py` & `nextpcg-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.6.1',
+    version='0.6.2',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```


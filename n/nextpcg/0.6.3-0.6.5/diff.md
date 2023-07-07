# Comparing `tmp/nextpcg-0.6.3.tar.gz` & `tmp/nextpcg-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.6.3.tar", last modified: Fri Jul  7 02:44:20 2023, max compression
+gzip compressed data, was "nextpcg-0.6.5.tar", last modified: Fri Jul  7 02:51:52 2023, max compression
```

## Comparing `nextpcg-0.6.3.tar` & `nextpcg-0.6.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.124362 nextpcg-0.6.3/
--rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-07-07 02:44:20.123361 nextpcg-0.6.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.089797 nextpcg-0.6.3/common/
--rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.3/common/__init__.py
--rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.3/common/nextpcg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.102135 nextpcg-0.6.3/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 02:44:20.000000 nextpcg-0.6.3/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.3/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.118357 nextpcg-0.6.3/pypapi/
--rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.3/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.3/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.3/pypapi/const.py
--rw-rw-rw-   0        0        0     5658 2023-07-04 09:17:13.000000 nextpcg-0.6.3/pypapi/dispatch.py
--rw-rw-rw-   0        0        0     2124 2023-06-30 08:13:29.000000 nextpcg-0.6.3/pypapi/dson.py
--rw-rw-rw-   0        0        0     8592 2023-07-07 02:43:28.000000 nextpcg-0.6.3/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.3/pypapi/dson_field.py
--rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.3/pypapi/dson_geo.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.3/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:44:20.121360 nextpcg-0.6.3/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.6.3/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-07-03 07:47:15.000000 nextpcg-0.6.3/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2972 2023-07-07 02:43:08.000000 nextpcg-0.6.3/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-07-07 02:44:20.124362 nextpcg-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     2468 2023-07-07 02:43:58.000000 nextpcg-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:51:52.807913 nextpcg-0.6.5/
+-rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-07-07 02:51:52.806913 nextpcg-0.6.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 02:51:52.772203 nextpcg-0.6.5/common/
+-rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.5/common/__init__.py
+-rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.5/common/nextpcg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:51:52.785285 nextpcg-0.6.5/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-07-07 02:51:52.000000 nextpcg-0.6.5/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-07-07 02:51:52.000000 nextpcg-0.6.5/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:51:52.000000 nextpcg-0.6.5/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-07 02:51:52.000000 nextpcg-0.6.5/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 02:51:52.000000 nextpcg-0.6.5/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 02:51:52.000000 nextpcg-0.6.5/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.5/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-07 02:51:52.802909 nextpcg-0.6.5/pypapi/
+-rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.5/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.5/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.5/pypapi/const.py
+-rw-rw-rw-   0        0        0     5658 2023-07-04 09:17:13.000000 nextpcg-0.6.5/pypapi/dispatch.py
+-rw-rw-rw-   0        0        0     2124 2023-06-30 08:13:29.000000 nextpcg-0.6.5/pypapi/dson.py
+-rw-rw-rw-   0        0        0     8590 2023-07-07 02:50:00.000000 nextpcg-0.6.5/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.5/pypapi/dson_field.py
+-rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.5/pypapi/dson_geo.py
+-rw-rw-rw-   0        0        0      160 2023-07-07 02:49:18.000000 nextpcg-0.6.5/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.5/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:51:52.804910 nextpcg-0.6.5/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.6.5/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-07-03 07:47:15.000000 nextpcg-0.6.5/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2972 2023-07-07 02:43:08.000000 nextpcg-0.6.5/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:51:52.808914 nextpcg-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     2468 2023-07-07 02:50:07.000000 nextpcg-0.6.5/setup.py
```

### Comparing `nextpcg-0.6.3/PKG-INFO` & `nextpcg-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.6.3
+Version: 0.6.5
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.6.3/common/nextpcg.py` & `nextpcg-0.6.5/common/nextpcg.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.6.5/nextpcg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.6.3
+Version: 0.6.5
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.6.3/nextpcg.egg-info/SOURCES.txt` & `nextpcg-0.6.5/nextpcg.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 pypapi/__main__.py
 pypapi/const.py
 pypapi/dispatch.py
 pypapi/dson.py
 pypapi/dson_create.py
 pypapi/dson_field.py
 pypapi/dson_geo.py
+pypapi/macro.py
 pypapi/meta_helper.py
 pypapi/plugin_protocol.py
 pypapi/pantry/dson_config.yaml
 pypapi/pantry/dson_generator.py
```

### Comparing `nextpcg-0.6.3/pypapi/__main__.py` & `nextpcg-0.6.5/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/pypapi/dispatch.py` & `nextpcg-0.6.5/pypapi/dispatch.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/pypapi/dson.py` & `nextpcg-0.6.5/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/pypapi/dson_create.py` & `nextpcg-0.6.5/pypapi/dson_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
                     dson_main_import = dson_main_import[:-1]
     except Exception as e:
         print(e)
         exit(1)
     # main function to dson_main_function
     dson_main_function = f"""
 
-
 if __name__ == '__main__':
     dson_plugin_name = '{dson_plugin_name}'
     logger = logging.getLogger('pypapi_'+dson_plugin_name)
     
     current_path = os.path.split(os.path.realpath(__file__))[0] # path to dosn_path.py
     dot_nextpcg_path = os.path.join(current_path, '.nextpcg')
```

### Comparing `nextpcg-0.6.3/pypapi/dson_field.py` & `nextpcg-0.6.5/pypapi/dson_field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/pypapi/dson_geo.py` & `nextpcg-0.6.5/pypapi/dson_geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/pypapi/meta_helper.py` & `nextpcg-0.6.5/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/pypapi/pantry/dson_generator.py` & `nextpcg-0.6.5/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/pypapi/plugin_protocol.py` & `nextpcg-0.6.5/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.3/setup.py` & `nextpcg-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.6.3',
+    version='0.6.5',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```


# Comparing `tmp/nextpcg-0.6.6.tar.gz` & `tmp/nextpcg-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.6.6.tar", last modified: Fri Jul  7 03:09:28 2023, max compression
+gzip compressed data, was "nextpcg-0.6.7.tar", last modified: Fri Jul  7 03:33:50 2023, max compression
```

## Comparing `nextpcg-0.6.6.tar` & `nextpcg-0.6.7.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 03:09:28.339390 nextpcg-0.6.6/
--rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-07-07 03:09:28.338389 nextpcg-0.6.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 03:09:28.302563 nextpcg-0.6.6/common/
--rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.6/common/__init__.py
--rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.6/common/nextpcg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:09:28.314806 nextpcg-0.6.6/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-07-07 03:09:28.000000 nextpcg-0.6.6/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-07-07 03:09:28.000000 nextpcg-0.6.6/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 03:09:28.000000 nextpcg-0.6.6/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-07 03:09:28.000000 nextpcg-0.6.6/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 03:09:28.000000 nextpcg-0.6.6/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-07 03:09:28.000000 nextpcg-0.6.6/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.6/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-07-07 03:09:28.333385 nextpcg-0.6.6/pypapi/
--rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.6/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.6/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.6/pypapi/const.py
--rw-rw-rw-   0        0        0     5658 2023-07-04 09:17:13.000000 nextpcg-0.6.6/pypapi/dispatch.py
--rw-rw-rw-   0        0        0     2124 2023-06-30 08:13:29.000000 nextpcg-0.6.6/pypapi/dson.py
--rw-rw-rw-   0        0        0     8590 2023-07-07 02:50:00.000000 nextpcg-0.6.6/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.6/pypapi/dson_field.py
--rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.6/pypapi/dson_geo.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.6/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:09:28.336388 nextpcg-0.6.6/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.6.6/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-07-03 07:47:15.000000 nextpcg-0.6.6/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2972 2023-07-07 02:43:08.000000 nextpcg-0.6.6/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-07-07 03:09:28.339390 nextpcg-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     2468 2023-07-07 03:08:55.000000 nextpcg-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:33:50.594995 nextpcg-0.6.7/
+-rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-07-07 03:33:50.593994 nextpcg-0.6.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 03:33:50.562034 nextpcg-0.6.7/common/
+-rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.7/common/__init__.py
+-rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.7/common/nextpcg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:33:50.574045 nextpcg-0.6.7/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-07-07 03:33:50.000000 nextpcg-0.6.7/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-07-07 03:33:50.000000 nextpcg-0.6.7/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 03:33:50.000000 nextpcg-0.6.7/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-07 03:33:50.000000 nextpcg-0.6.7/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 03:33:50.000000 nextpcg-0.6.7/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 03:33:50.000000 nextpcg-0.6.7/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.7/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-07 03:33:50.591992 nextpcg-0.6.7/pypapi/
+-rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.7/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.7/pypapi/__main__.py
+-rw-rw-rw-   0        0        0     2129 2023-07-07 03:27:03.000000 nextpcg-0.6.7/pypapi/dson.py
+-rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.7/pypapi/dson_const.py
+-rw-rw-rw-   0        0        0     8602 2023-07-07 03:29:19.000000 nextpcg-0.6.7/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0     5663 2023-07-07 03:23:47.000000 nextpcg-0.6.7/pypapi/dson_dispatch.py
+-rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.7/pypapi/dson_field.py
+-rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.7/pypapi/dson_geo.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.7/pypapi/meta_helper.py
+-rw-rw-rw-   0        0        0     2972 2023-07-07 02:43:08.000000 nextpcg-0.6.7/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 03:33:50.594995 nextpcg-0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     2468 2023-07-07 03:19:50.000000 nextpcg-0.6.7/setup.py
```

### Comparing `nextpcg-0.6.6/PKG-INFO` & `nextpcg-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.6.6
+Version: 0.6.7
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.6.6/common/nextpcg.py` & `nextpcg-0.6.7/common/nextpcg.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.6/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.6.7/nextpcg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.6.6
+Version: 0.6.7
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.6.6/pypapi/__main__.py` & `nextpcg-0.6.7/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.6/pypapi/dispatch.py` & `nextpcg-0.6.7/pypapi/dson_dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Author  : NextPCG
 """
 
 import os
 import logging
 from typing import Dict, List, Union, Tuple
 
-from .const import *
 from .dson import DsonMetaInfo, DsonManager
+from .dson_const import *
 from .dson_field import FieldManager, Field, FieldDesc
 from .meta_helper import Singleton
 
 
 class Dispatcher(metaclass=Singleton):
     def __init__(self):
         pass
```

### Comparing `nextpcg-0.6.6/pypapi/dson.py` & `nextpcg-0.6.7/pypapi/dson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Author  : NextPCG
 """
 
 from .meta_helper import Singleton
-from .const import *
+from .dson_const import *
 
 
 class nextpcgmethod(staticmethod):
     def __init__(self, function):
         super(nextpcgmethod, self).__init__(function)
```

### Comparing `nextpcg-0.6.6/pypapi/dson_create.py` & `nextpcg-0.6.7/pypapi/dson_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 import os
 import json
 import logging
 
 from inspect import signature, Signature
 from functools import wraps
 from typing import *
-from .const import *
+
 from .dson import DsonMetaInfo, DsonManager, nextpcgmethod
+from .dson_const import *
 from .dson_field import Field, FieldCategory
 
 
 def create_dson_from_pda(func: Callable, tag, dson_meta_info: DsonMetaInfo) -> Dict:
     cda_json = {}
     try:
         func_sig = signature(func)
@@ -118,15 +119,15 @@
 import sys
 import os
 import json
 import logging
 
 import common.nextpcg as nextpcg
 
-from pypapi.dispatch import Dispatcher
+from pypapi.dson_dispatch import Dispatcher
 from pypapi.plugin_protocol import module_send_done, setup_logger
 
 """
     # load necessary modules or classes to dson_main_import
     dson_main_import = ''
     try:
         for module in dson_config['modules']:
```

### Comparing `nextpcg-0.6.6/pypapi/dson_field.py` & `nextpcg-0.6.7/pypapi/dson_field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.6/pypapi/dson_geo.py` & `nextpcg-0.6.7/pypapi/dson_geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.6/pypapi/meta_helper.py` & `nextpcg-0.6.7/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.6/pypapi/plugin_protocol.py` & `nextpcg-0.6.7/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.6.6/setup.py` & `nextpcg-0.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.6.6',
+    version='0.6.7',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```


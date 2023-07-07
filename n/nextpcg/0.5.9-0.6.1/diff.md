# Comparing `tmp/nextpcg-0.5.9.tar.gz` & `tmp/nextpcg-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.5.9.tar", last modified: Fri Jun 30 07:05:33 2023, max compression
+gzip compressed data, was "nextpcg-0.6.1.tar", last modified: Fri Jul  7 02:22:27 2023, max compression
```

## Comparing `nextpcg-0.5.9.tar` & `nextpcg-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:05:33.769843 nextpcg-0.5.9/
--rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-06-30 07:05:33.768842 nextpcg-0.5.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 07:05:33.741819 nextpcg-0.5.9/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.9/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-06-30 07:05:33.762837 nextpcg-0.5.9/pypapi/
--rw-rw-rw-   0        0        0       15 2023-06-30 03:01:10.000000 nextpcg-0.5.9/pypapi/__init__.py
--rw-rw-rw-   0        0        0     1995 2023-06-30 06:47:27.000000 nextpcg-0.5.9/pypapi/__main__.py
--rw-rw-rw-   0        0        0     2129 2023-06-30 06:48:26.000000 nextpcg-0.5.9/pypapi/dson.py
--rw-rw-rw-   0        0        0      470 2023-06-30 06:47:02.000000 nextpcg-0.5.9/pypapi/dson_const.py
--rw-rw-rw-   0        0        0     8624 2023-06-30 06:48:46.000000 nextpcg-0.5.9/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    17451 2023-06-30 03:18:15.000000 nextpcg-0.5.9/pypapi/dson_field.py
--rw-rw-rw-   0        0        0    38443 2023-06-30 03:10:42.000000 nextpcg-0.5.9/pypapi/dson_geo.py
--rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.9/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.9/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:05:33.766841 nextpcg-0.5.9/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.9/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.9/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.9/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-06-30 07:05:33.770844 nextpcg-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-06-30 07:05:20.000000 nextpcg-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.877229 nextpcg-0.6.1/
+-rw-rw-rw-   0        0        0      167 2023-07-04 11:07:37.000000 nextpcg-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-07-07 02:22:27.876206 nextpcg-0.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.839537 nextpcg-0.6.1/common/
+-rw-rw-rw-   0        0        0      127 2023-02-10 06:47:34.000000 nextpcg-0.6.1/common/__init__.py
+-rw-rw-rw-   0        0        0    18764 2023-06-13 02:35:36.000000 nextpcg-0.6.1/common/nextpcg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.851599 nextpcg-0.6.1/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-07 02:22:27.000000 nextpcg-0.6.1/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.6.1/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.870550 nextpcg-0.6.1/pypapi/
+-rw-rw-rw-   0        0        0       15 2023-07-03 08:28:35.000000 nextpcg-0.6.1/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-30 08:13:29.000000 nextpcg-0.6.1/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-06-30 08:13:29.000000 nextpcg-0.6.1/pypapi/const.py
+-rw-rw-rw-   0        0        0     5658 2023-07-04 09:17:13.000000 nextpcg-0.6.1/pypapi/dispatch.py
+-rw-rw-rw-   0        0        0     2124 2023-06-30 08:13:29.000000 nextpcg-0.6.1/pypapi/dson.py
+-rw-rw-rw-   0        0        0     9233 2023-07-07 02:20:55.000000 nextpcg-0.6.1/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    17451 2023-07-03 08:28:35.000000 nextpcg-0.6.1/pypapi/dson_field.py
+-rw-rw-rw-   0        0        0    38443 2023-07-03 08:28:35.000000 nextpcg-0.6.1/pypapi/dson_geo.py
+-rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.6.1/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.6.1/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:22:27.874138 nextpcg-0.6.1/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.6.1/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-07-03 07:47:15.000000 nextpcg-0.6.1/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.6.1/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:22:27.877229 nextpcg-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2468 2023-07-07 02:22:04.000000 nextpcg-0.6.1/setup.py
```

### Comparing `nextpcg-0.5.9/PKG-INFO` & `nextpcg-0.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.9
+Version: 0.6.1
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.9/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.6.1/nextpcg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.9
+Version: 0.6.1
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.9/pypapi/__main__.py` & `nextpcg-0.6.1/pypapi/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 import argparse
 import os
 import yaml
 import shutil
 from importlib_resources import files, as_file
 
-
 def entry():
     parser = argparse.ArgumentParser(prog = 'nextpcg')
     subparsers = parser.add_subparsers(
         title='These are common NextPCG Dson commands used in various situations',
         metavar='command'
     )
 
@@ -57,10 +56,12 @@
         yaml.safe_dump(dson_config, f, sort_keys=False)
         f.close()
     
     source = files('pypapi').joinpath('pantry').joinpath('dson_generator.py')
     with as_file(source) as source_path:
         shutil.copyfile(source_path,os.path.join(plugin_path, 'dson_generator.py'))
 
+    
+
 
 if __name__ == '__main__':
     entry()
```

### Comparing `nextpcg-0.5.9/pypapi/dson.py` & `nextpcg-0.6.1/pypapi/dson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Author  : NextPCG
 """
 
 from .meta_helper import Singleton
-from .dson_const import *
+from .const import *
 
 
 class nextpcgmethod(staticmethod):
     def __init__(self, function):
         super(nextpcgmethod, self).__init__(function)
```

### Comparing `nextpcg-0.5.9/pypapi/dson_create.py` & `nextpcg-0.6.1/pypapi/dson_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import os
 import json
 import logging
 
 from inspect import signature, Signature
 from functools import wraps
 from typing import *
+from .const import *
 from .dson import DsonMetaInfo, DsonManager, nextpcgmethod
-from .dson_const import *
 from .dson_field import Field, FieldCategory
 
 
 def create_dson_from_pda(func: Callable, tag, dson_meta_info: DsonMetaInfo) -> Dict:
     cda_json = {}
     try:
         func_sig = signature(func)
@@ -29,104 +29,134 @@
         cda_json = {func_name + "." + tag: cda_json_cda}
     except Exception as e:
         logging.exception(e)
     finally:
         return cda_json
 
 
-def generate_dson_files(plugin_name, dson_path):
+def generate_dson_files(base_path, dson_config):
     index = 0
+    dson_path = os.path.join(base_path, "dson")
+    dson_plugin_name = dson_config['name']
+    dson_modules = dson_config['modules']
+
+    # get all dson class
+    for module in dson_modules:
+        if isinstance(module, str):
+            # only module name
+            try:
+                __import__(module, globals(), locals(), [], 0)
+            except Exception as e:
+                print(e)
+                exit(1)
+        else:
+            for module_name in module:
+                # if has class name
+                try:
+                    __import__(module_name, globals(), locals(), module[module_name], 0)
+                except Exception as e:
+                    print(e)
+                    exit(1)
+
+    # path prepare
     if not os.path.exists(dson_path):
         os.makedirs(dson_path, exist_ok=True)
+
+    # generate dson file
     for cls_name, cls in DsonManager().dsonMap.items():
         for name, value in vars(cls).items():
             if isinstance(value, nextpcgmethod):
                 func = value.__func__
-                dson_meta_info = DsonMetaInfo(cls_name, cls.if_in_server, plugin_name)
+                dson_meta_info = DsonMetaInfo(cls_name, cls.if_in_server, dson_plugin_name)
                 json_data = create_dson_from_pda(func, cls.label, dson_meta_info)
                 file_name = name + '.dson'
                 file_path = os.path.join(dson_path, file_name).replace('\\', '/')
                 fp = open(file_path, "w")
                 json.dump(json_data, fp)
                 index += 1
 
 
-def generate_dson_init_script(nextpcg_path, conda_env):
+def generate_dson_init_script(base_path, dson_config):
+    # data prepare
+    conda_env = dson_config['conda_env']
+    # create bat
     if os.name != 'posix':
         # windows
         script_name = 'dson_init.bat'
-        script_string = f"""@echo off
-                        cd %~dp0 
-                        cd ..
-                        call conda activate {conda_env}
-                        @REM call conda env list
-                        python dson_main.py
-                        """
+        script_string = f"""
+@echo off
+cd %~dp0 
+cd ..
+call conda activate {conda_env}
+@REM call conda env list
+python dson_main.py
+"""
     else:
         # linux
         script_name = 'dson_init.sh'
-        script_string = f"""#! /usr/bin/bash
-                        source ~/.bash_profile # get conda into env
-                        BASEDIR=$(dirname $(readlink -f "$0"))
-                        cd "$BASEDIR"
-                        cd ..
-                        eval "$(conda shell.bash hook)"
-                        conda activate {conda_env}
-                        python dson_main.py
-                        """
+        script_string = f"""
+#! /usr/bin/bash
+source ~/.bash_profile # get conda into env
+BASEDIR=$(dirname $(readlink -f "$0"))
+cd "$BASEDIR"
+cd ..
+eval "$(conda shell.bash hook)"
+conda activate {conda_env}
+python dson_main.py
+"""
+    nextpcg_path = os.path.join(base_path, '.nextpcg')
     if not os.path.exists(nextpcg_path):
         os.makedirs(nextpcg_path, exist_ok=True)
     with open(os.path.join(nextpcg_path, script_name), 'w', encoding='utf-8') as f:
         f.write(script_string)
 
 
-def generate_dson_main(base_path, dson_plugin_name, dson_config):
-    # import info
-    dsonmain_string1 = """
-from pypapi.dispatch import Dispatcher
-from pypapi.plugin_protocol import module_send_done
+def generate_dson_main(base_path, dson_config):
+    # data prepare
+    dson_plugin_name = dson_config['name']
+    # import info to dson_main_head
+    dson_main_head = f"""
 import sys
 import os
 import json
 import logging
 
+import common.nextpcg as nextpcg
+
+from pypapi.dispatch import Dispatcher
+from pypapi.plugin_protocol import module_send_done
+
 """
-    # dsonmain_import contains code used to load necessary modules or classes
-    dsonmain_import = ''
-    for module in dson_config['modules']:
-        if isinstance(module, str):
-            # only module name
-            try:
-                dsonmain_import += 'import ' + module + '\n'
-            except Exception as e:
-                print(e)
-                exit(1)
-        else:
-            for module_name in module:
-                # if has class name
-                dsonmain_import += 'from ' + module_name + ' import  '
-                for class_name in module[module_name]:
-                    dsonmain_import += class_name + ','
-                dsonmain_import = dsonmain_import[:-1]
-    # code
-    dsonmain_string2 = f"""
-
-dson_plugin_name = '{dson_plugin_name}'
-dispatcher = Dispatcher()
-logger = logging.getLogger('pypapi_'+dson_plugin_name)
-current_path = os.path.split(os.path.realpath(__file__))[0] # path to dosn_path.py
-dot_nextpcg_path = os.path.join(current_path, '.nextpcg')
+    # load necessary modules or classes to dson_main_import
+    dson_main_import = ''
+    try:
+        for module in dson_config['modules']:
+            if isinstance(module, str):
+                # only module name
+                dson_main_import += 'import ' + module + '\n'
+            else:
+                # has class name
+                for module_name in module:
+                    dson_main_import += 'from ' + module_name + ' import  '
+                    for class_name in module[module_name]:
+                        dson_main_import += class_name + ','
+                    dson_main_import = dson_main_import[:-1]
+    except Exception as e:
+        print(e)
+        exit(1)
+    # main function to dson_main_function
+    dson_main_function = f"""
 
-def set_up_logger():
+def set_up_logger(logger, logger_path):
     logFormatter = logging.Formatter('%(levelname)s:%(name)s:[%(asctime)s]: %(message)s')
 
-    if not os.path.exists(dot_nextpcg_path):
-        os.makedirs(dot_nextpcg_path)
+    if not os.path.exists(logger_path):
+        os.makedirs(logger_path)
 
-    logfile_path = os.path.join(current_path, '.nextpcg', 'nextpcgpython.log')
+    logfile_path = os.path.join(logger_path, 'nextpcgpython.log')
     # delete old log file
     try:
         os.remove(logfile_path)
     except OSError:
         pass
 
     fileHandler = logging.FileHandler(logfile_path)
@@ -134,58 +164,58 @@
 
     consoleHandler = logging.StreamHandler()
     consoleHandler.setFormatter(logFormatter)
 
     logger.addHandler(fileHandler)
     logger.addHandler(consoleHandler)
 
-class Tee:
-    def __init__(self, *files):
-        self.files = files
-
-    def write(self, obj):
-        for f in self.files:
-            f.write(obj)
-            f.flush()
-
-    def flush(self):
-        for f in self.files:
-            f.flush()
 
 if __name__ == '__main__':
-    set_up_logger()
-    ferr = open(os.path.join(dot_nextpcg_path, 'err.txt'), 'w')
-    sys.stderr = Tee(sys.stderr,ferr)
+    dson_plugin_name = '{dson_plugin_name}'
+    logger = logging.getLogger('pypapi_'+dson_plugin_name)
+    
+    current_path = os.path.split(os.path.realpath(__file__))[0] # path to dosn_path.py
+    dot_nextpcg_path = os.path.join(current_path, '.nextpcg')
+
+    set_up_logger(logger, dot_nextpcg_path)
+    
     module_send_done()
     while(True):
         json_file_name, work_path = input().split()
         json_error_data = {{}}
         try:
             with open(json_file_name, 'r') as f:
                 json_data = json.load(f)
             if not json_data:
                 print("didn't get dson data")
                 module_send_done()
-            dispatcher.run_func(json_data, logger, work_path, json_error_data)
+            dispatcher.run_func(json_data, logger, work_path, nextpcg.pson_system_tag, json_error_data)
             json_data_error_file_name = os.path.join(work_path, 'error.json').replace("\\\\",'/')
             # write back json_data
             with open(json_file_name, 'w') as f:
                 json.dump(json_data, f)
         except Exception as e:
             json_error_data['Error_Tag'] = 'plugin {dson_plugin_name} error in main loop'
             json_error_data['Error_Info'] = str(e)
             logger.exception(e)
         finally:
             with open(json_data_error_file_name, 'w') as f:
                 json_error_data = json.dump(json_error_data, f)
         module_send_done()
 """
-    dsonmain_string = dsonmain_string1 + dsonmain_import + dsonmain_string2
+    # merge
+    dson_main_string = dson_main_head + dson_main_import + dson_main_function
     with open(os.path.join(base_path, 'dson_main.py'), 'w', encoding='utf-8') as f:
-        f.write(dsonmain_string)
+        f.write(dson_main_string)
+
+
+def generate(base_path, dson_config):
+    generate_dson_files(base_path, dson_config)
+    generate_dson_init_script(base_path, dson_config)
+    generate_dson_main(base_path, dson_config)
 
 
 def get_inputs(sig: Signature):
     inputs = {}
     params = {}
     input_index = 0
     for param in sig.parameters.values():
```

### Comparing `nextpcg-0.5.9/pypapi/dson_field.py` & `nextpcg-0.6.1/pypapi/dson_field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.9/pypapi/dson_geo.py` & `nextpcg-0.6.1/pypapi/dson_geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.9/pypapi/meta_helper.py` & `nextpcg-0.6.1/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.9/pypapi/pantry/dson_generator.py` & `nextpcg-0.6.1/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.9/pypapi/plugin_protocol.py` & `nextpcg-0.6.1/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.9/setup.py` & `nextpcg-0.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.5.9',
+    version='0.6.1',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced 
@@ -17,19 +17,21 @@
     In addition, the pypapi module makes it easy to create programs and applications that are compatible with 
     different platforms and operating systems, ensuring that users can deploy their creations on a variety of platforms. 
     All in all, the pypapi module in NextPCG is a great tool for developers who want to quickly and easily create 
     complex applications.''',
     author_email='cheneyshen@tencent.com',
     url='https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4',
 
+    include_package_data=True,
+
     # packages=setuptools.find_packages(exclude=["dson_test", "dson_generator", "dispatch"]),
     # packages=setuptools.find_packages(where=['pypapi']),
-    packages=['pypapi', 'pypapi.pantry'],
-    package_dir={'pypapi':'pypapi'},
-    package_data={'pypapi.pantry':['*']},
+    packages=['pypapi', 'common'],
+    # package_dir={'pypapi':'pypapi'},
+    # package_data={'pypapi.pantry':['*']},
 
     entry_points={
         'console_scripts':[
             'nextpcg = pypapi.__main__:entry'
         ]
     },
     install_requires=[
```


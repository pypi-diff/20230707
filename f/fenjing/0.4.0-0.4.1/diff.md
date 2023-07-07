# Comparing `tmp/fenjing-0.4.0.tar.gz` & `tmp/fenjing-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.0.tar", last modified: Thu Jul  6 16:03:29 2023, max compression
+gzip compressed data, was "fenjing-0.4.1.tar", last modified: Fri Jul  7 07:20:27 2023, max compression
```

## Comparing `fenjing-0.4.0.tar` & `fenjing-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-06 16:03:19.000000 fenjing-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-06 16:03:19.000000 fenjing-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-06 16:03:29.234401 fenjing-0.4.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-07-06 16:03:19.000000 fenjing-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 16:03:19.000000 fenjing-0.4.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5246 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    31714 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-06 16:03:19.000000 fenjing-0.4.0/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 16:03:29.000000 fenjing-0.4.0/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 16:03:19.000000 fenjing-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:03:29.234401 fenjing-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 16:03:19.000000 fenjing-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:03:29.234401 fenjing-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-06 16:03:19.000000 fenjing-0.4.0/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-06 16:03:19.000000 fenjing-0.4.0/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:27.248086 fenjing-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-07 07:20:17.000000 fenjing-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 07:20:17.000000 fenjing-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-07 07:20:27.248086 fenjing-0.4.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6120 2023-07-07 07:20:17.000000 fenjing-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 07:20:17.000000 fenjing-0.4.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:27.248086 fenjing-0.4.1/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5246 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31730 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:27.248086 fenjing-0.4.1/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-07-07 07:20:17.000000 fenjing-0.4.1/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:27.248086 fenjing-0.4.1/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-07 07:20:27.000000 fenjing-0.4.1/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-07 07:20:27.000000 fenjing-0.4.1/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:20:27.000000 fenjing-0.4.1/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 07:20:27.000000 fenjing-0.4.1/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 07:20:27.000000 fenjing-0.4.1/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 07:20:17.000000 fenjing-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 07:20:27.248086 fenjing-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 07:20:17.000000 fenjing-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:20:27.248086 fenjing-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-07 07:20:17.000000 fenjing-0.4.1/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-07 07:20:17.000000 fenjing-0.4.1/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.0/LICENSE` & `fenjing-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/PKG-INFO` & `fenjing-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.0/README.md` & `fenjing-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/cli.py` & `fenjing-0.4.1/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/colorize.py` & `fenjing-0.4.1/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/config_payload.py` & `fenjing-0.4.1/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/const.py` & `fenjing-0.4.1/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/context_vars.py` & `fenjing-0.4.1/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/form.py` & `fenjing-0.4.1/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/form_cracker.py` & `fenjing-0.4.1/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/full_payload_gen.py` & `fenjing-0.4.1/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/payload_gen.py` & `fenjing-0.4.1/fenjing/payload_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections import defaultdict
 from typing import Callable, DefaultDict, List, Dict, Union, Any
 import re
 import time
 import logging
-import typing
 from typing import Callable, Any, Dict, Tuple
 from .colorize import colored
 from .const import *
 
 ContextVariable = Dict[str, Any]
 ReqGenRequirement = Tuple
 
@@ -43,15 +42,15 @@
         callback: Union[Callable[[str, Dict], None], None] = None
     ):
         self.waf_func = waf_func
         self.context = context if context else {}
         self.cache = {}
         self.generate_funcs: List[Tuple[
             Callable[[ReqGenRequirement], bool],
-            Callable[[ReqGenRequirement], ReqGenResult | None]
+            Callable[[ReqGenRequirement], Union[ReqGenResult, None]]
         ]]
         self.generate_funcs = [
             (
                 (lambda gen_req: gen_req[0] == LITERAL),
                 (lambda gen_req: (gen_req[1], {}))
             ),
             (
@@ -72,15 +71,15 @@
             )
         ]
             # LITERAL: self.literal_generate,
             # UNSATISFIED: self.unsatisfied_generate
         
         self.callback = callback if callback else (lambda x, y: None)
 
-    def generate_by_list(self, req_list: List[ReqGenRequirement]) -> ReqGenResult | None:
+    def generate_by_list(self, req_list: List[ReqGenRequirement]) -> Union[ReqGenResult, None]:
         str_result, used_context = "", {}
         for req in req_list:
             for checker, runner in self.generate_funcs:
                 if not checker(req):
                     continue
                 result = runner(req)
                 if result is None:
@@ -93,15 +92,15 @@
                 break
             else:
                 raise Exception("it shouldn't runs this line")
         if not self.waf_func(str_result):
             return None
         return str_result, used_context
 
-    def common_generate(self, gen_req: ReqGenRequirement) -> ReqGenResult | None:
+    def common_generate(self, gen_req: ReqGenRequirement) -> Union[ReqGenResult, None]:
 
         gen_type: str
         gen_type, *args = gen_req
         if gen_type not in req_gens or len(req_gens[gen_type]) == 0:
             logger.error("Unknown type: %s", gen_type)
             return None
 
@@ -144,24 +143,24 @@
             failed=colored("red", "failed"),
             gen_type=gen_type,
             args_repl=", ".join(repr(arg) for arg in args),
         ))
         return None
 
 
-    def generate(self, gen_type, *args) ->  str | None:
+    def generate(self, gen_type, *args) ->  Union[str, None]:
         result = self.generate_by_list([
             (gen_type, *args)
         ])
         if result is None:
             return None
         s, c = result
         return s
 
-    def generate_with_used_context(self, gen_type, *args) ->  ReqGenResult | None:
+    def generate_with_used_context(self, gen_type, *args) ->  Union[ReqGenResult, None]:
         result = self.generate_by_list([
             (gen_type, *args)
         ])
         if result is None:
             return None
         s, c = result
         return s, c
```

### Comparing `fenjing-0.4.0/fenjing/requester.py` & `fenjing-0.4.1/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/scan_url.py` & `fenjing-0.4.1/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/shell_payload.py` & `fenjing-0.4.1/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/templates/index.html` & `fenjing-0.4.1/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/waf_func_gen.py` & `fenjing-0.4.1/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/fenjing/webui.py` & `fenjing-0.4.1/fenjing/webui.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         will_print_msg = "其会产生回显。" if data["will_print"] else "其不会产生回显。"
         self.messages.append(
             testsuccess_msg + will_print_msg
         )
 
     def __call__(self, callback_type, data):
         def default_handler(data):
-            return logger.warning(f"{callback_type=} not found")
+            return logger.warning(f"callback_type={callback_type} not found")
         return {
             CALLBACK_PREPARE_FULLPAYLOADGEN: self.callback_prepare_fullpayloadgen,
             CALLBACK_GENERATE_FULLPAYLOAD: self.callback_generate_fullpayload,
             CALLBACK_GENERATE_PAYLOAD: self.callback_generate_payload,
             CALLBACK_SUBMIT: self.callback_submit,
             CALLBACK_TEST_FORM_INPUT: self.callback_test_form_input
         }.get(callback_type, default_handler)(data)
```

### Comparing `fenjing-0.4.0/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.1/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.0/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.1/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/setup.py` & `fenjing-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/tests/test_full_payload_gen.py` & `fenjing-0.4.1/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.0/tests/test_payload_gen.py` & `fenjing-0.4.1/tests/test_payload_gen.py`

 * *Files identical despite different names*


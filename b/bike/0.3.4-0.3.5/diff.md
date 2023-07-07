# Comparing `tmp/bike-0.3.4.tar.gz` & `tmp/bike-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bike-0.3.4.tar", max compression
+gzip compressed data, was "bike-0.3.5.tar", max compression
```

## Comparing `bike-0.3.4.tar` & `bike-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.4/LICENSE
--rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.4/README.md
--rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.4/bike/__init__.py
--rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.4/bike/controllers.py
--rw-r--r--   0        0        0     3086 2023-07-06 18:04:51.285877 bike-0.3.4/bike/fields.py
--rw-r--r--   0        0        0     8564 2023-07-06 11:13:29.712411 bike-0.3.4/bike/models.py
--rw-r--r--   0        0        0      495 2023-07-06 18:18:37.320701 bike-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.5/README.md
+-rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.5/bike/__init__.py
+-rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.5/bike/controllers.py
+-rw-r--r--   0        0        0     3086 2023-07-06 18:04:51.285877 bike-0.3.5/bike/fields.py
+-rw-r--r--   0        0        0     8609 2023-07-07 09:34:46.693316 bike-0.3.5/bike/models.py
+-rw-r--r--   0        0        0      495 2023-07-07 09:34:46.681316 bike-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.5/PKG-INFO
```

### Comparing `bike-0.3.4/LICENSE` & `bike-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bike-0.3.4/README.md` & `bike-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bike-0.3.4/bike/controllers.py` & `bike-0.3.5/bike/controllers.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.4/bike/fields.py` & `bike-0.3.5/bike/fields.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.4/bike/models.py` & `bike-0.3.5/bike/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import inspect
 import json
-from typing import Set, Any
-
+from typing import Set
 import bike
 from .fields import Field
 
 
 __validators__ = {}
 types_default = {
     'str': '""',
@@ -41,15 +40,15 @@
                 params_required_txt = f'{params_required_txt}, {param}' if params_required_txt else param
         else:
             default = field.default or types_default.get(field.type.__name__, "None")
             param = f'{param} = {default}'
             params_optional_txt = f'{params_optional_txt}, {param}' if params_optional_txt else param
         statement = f'self.{k} = {name}'
         body_fn += f'\t{statement}\n'
-    params_txt = f'*, {params_required_txt}, {params_optional_txt}'
+    params_txt = ', '.join([arg for arg in (params_required_txt, params_optional_txt, '*args', '**kwargs') if arg])
     init_fn = f'def __init__(self, {params_txt}):\n{body_fn}'
     ns = {}
     exec(init_fn, None, ns)
     return ns['__init__']
 
 
 def prepare_db_config(cls, table: str, pk: str = ''):
@@ -254,11 +253,11 @@
         func.__validator_pre__ = pre
         return func
     return wrapper
 
 
 def model(
         alias_load: bool = True
-) -> Model:
+) -> callable:
     def wrapper(cls) -> Model:
         return prepare_fields(cls, alias_load=alias_load)
     return wrapper
```

### Comparing `bike-0.3.4/PKG-INFO` & `bike-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bike
-Version: 0.3.4
+Version: 0.3.5
 Summary: A lightweight model validator for modern projects.
 Home-page: https://github.com/manasseslima/bike
 License: MIT
 Author: Manasses Lima
 Author-email: manasseslima@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


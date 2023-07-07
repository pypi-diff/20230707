# Comparing `tmp/aitomatic-1.2.8.tar.gz` & `tmp/aitomatic-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aitomatic-1.2.8.tar", last modified: Mon Jun 26 07:26:32 2023, max compression
+gzip compressed data, was "aitomatic-1.2.9.tar", last modified: Tue Jun 27 03:07:08 2023, max compression
```

## Comparing `aitomatic-1.2.8.tar` & `aitomatic-1.2.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.383148 aitomatic-1.2.8/
--rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.2.8/LICENSE
--rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.2.8/MANIFEST.in
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-06-26 07:26:32.383542 aitomatic-1.2.8/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.2.8/README.md
--rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.2.8/pyproject.toml
--rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.2.8/requirements.txt
--rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-06-26 07:26:32.384819 aitomatic-1.2.8/setup.cfg
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.356311 aitomatic-1.2.8/src/
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.364301 aitomatic-1.2.8/src/aitomatic/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/__init__.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.375019 aitomatic-1.2.8/src/aitomatic/api/
--rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/api/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8843 2023-06-26 07:24:53.000000 aitomatic-1.2.8/src/aitomatic/api/build.py
--rw-r--r--   0 hungvo     (501) staff       (20)     6120 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/api/client.py
--rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/api/exceptions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/api/model_params.py
--rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/api/tuning_utils.py
--rw-r--r--   0 hungvo     (501) staff       (20)    15820 2023-06-26 07:24:20.000000 aitomatic-1.2.8/src/aitomatic/api/web_model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.379384 aitomatic-1.2.8/src/aitomatic/dsl/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/dsl/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/dsl/arl_conclusions.py
--rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/dsl/arl_features.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/dsl/arl_handler.py
--rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.2.8/src/aitomatic/dsl/arl_rules.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.2.8/src/aitomatic/dsl/utils.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.382213 aitomatic-1.2.8/src/aitomatic/objects/
--rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.2.8/src/aitomatic/objects/__init__.py
--rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/objects/dataset.py
--rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.2.8/src/aitomatic/objects/model.py
-drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-26 07:26:32.367013 aitomatic-1.2.8/src/aitomatic.egg-info/
--rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/PKG-INFO
--rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/SOURCES.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/dependency_links.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/requires.txt
--rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-06-26 07:26:32.000000 aitomatic-1.2.8/src/aitomatic.egg-info/top_level.txt
--rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-06-26 07:25:05.000000 aitomatic-1.2.8/version.txt
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.819754 aitomatic-1.2.9/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1065 2023-02-15 03:11:17.000000 aitomatic-1.2.9/LICENSE
+-rw-r--r--   0 hungvo     (501) staff       (20)       36 2023-02-24 03:49:01.000000 aitomatic-1.2.9/MANIFEST.in
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-06-27 03:07:08.819897 aitomatic-1.2.9/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)     4051 2023-05-08 07:01:50.000000 aitomatic-1.2.9/README.md
+-rw-r--r--   0 hungvo     (501) staff       (20)       85 2023-02-15 03:11:17.000000 aitomatic-1.2.9/pyproject.toml
+-rw-r--r--   0 hungvo     (501) staff       (20)       87 2023-05-08 07:01:50.000000 aitomatic-1.2.9/requirements.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)      714 2023-06-27 03:07:08.820703 aitomatic-1.2.9/setup.cfg
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.801855 aitomatic-1.2.9/src/
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.806798 aitomatic-1.2.9/src/aitomatic/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/__init__.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.813218 aitomatic-1.2.9/src/aitomatic/api/
+-rw-r--r--   0 hungvo     (501) staff       (20)     1203 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/api/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     8843 2023-06-26 07:24:53.000000 aitomatic-1.2.9/src/aitomatic/api/build.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     6890 2023-06-27 03:06:50.000000 aitomatic-1.2.9/src/aitomatic/api/client.py
+-rw-r--r--   0 hungvo     (501) staff       (20)       54 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/api/exceptions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     7673 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/api/model_params.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     4333 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/api/tuning_utils.py
+-rw-r--r--   0 hungvo     (501) staff       (20)    15820 2023-06-26 07:24:20.000000 aitomatic-1.2.9/src/aitomatic/api/web_model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.817371 aitomatic-1.2.9/src/aitomatic/dsl/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/dsl/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3778 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/dsl/arl_conclusions.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     8933 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/dsl/arl_features.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3690 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/dsl/arl_handler.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     3463 2023-02-24 03:49:01.000000 aitomatic-1.2.9/src/aitomatic/dsl/arl_rules.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1040 2023-05-16 01:46:06.000000 aitomatic-1.2.9/src/aitomatic/dsl/utils.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.819238 aitomatic-1.2.9/src/aitomatic/objects/
+-rw-r--r--   0 hungvo     (501) staff       (20)        0 2023-04-25 08:41:40.000000 aitomatic-1.2.9/src/aitomatic/objects/__init__.py
+-rw-r--r--   0 hungvo     (501) staff       (20)      531 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/objects/dataset.py
+-rw-r--r--   0 hungvo     (501) staff       (20)     1563 2023-05-04 14:19:17.000000 aitomatic-1.2.9/src/aitomatic/objects/model.py
+drwxr-xr-x   0 hungvo     (501) staff       (20)        0 2023-06-27 03:07:08.809302 aitomatic-1.2.9/src/aitomatic.egg-info/
+-rw-r--r--   0 hungvo     (501) staff       (20)     4587 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/PKG-INFO
+-rw-r--r--   0 hungvo     (501) staff       (20)      799 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        1 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       78 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/requires.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)       10 2023-06-27 03:07:08.000000 aitomatic-1.2.9/src/aitomatic.egg-info/top_level.txt
+-rw-r--r--   0 hungvo     (501) staff       (20)        6 2023-06-27 03:06:53.000000 aitomatic-1.2.9/version.txt
```

### Comparing `aitomatic-1.2.8/LICENSE` & `aitomatic-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/PKG-INFO` & `aitomatic-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.2.8
+Version: 1.2.9
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.2.8/README.md` & `aitomatic-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/setup.cfg` & `aitomatic-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/api/__init__.py` & `aitomatic-1.2.9/src/aitomatic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/api/build.py` & `aitomatic-1.2.9/src/aitomatic/api/build.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/api/client.py` & `aitomatic-1.2.9/src/aitomatic/api/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import requests
-import json
 import os
+import json
+import requests
+from tqdm import tqdm
 from aitomatic.dsl.arl_handler import ARLHandler
 from aitomatic.objects.model import Model
 from aitomatic.objects.dataset import Dataset
 
 
 MODEL_API_ROOT = {
     'local': 'http://localhost:8000/',
@@ -65,28 +66,37 @@
             project_id = get_project_id(project_name, api_token=api_token)
 
         self.project_name = project_name
         self.project_id = project_id
         self.headers = {
             'accept': 'application/json',
             'authorization': api_token,
-            'conent-type': 'application/json',
+            'Content-Type': 'application/json',
         }
         self.init_endpoints()
 
     def init_endpoints(self):
         _, self.API_ROOT = get_api_root()
         self.KNOWLEDGE_LIST = f'{self.API_ROOT}/{self.project_id}/knowledges'
         self.KNOWLEDGE_DETAIL = lambda id_: f'{self.API_ROOT}/knowledges/' + id_
         self.MODELS_LIST = f'{self.API_ROOT}/{self.project_id}/models'
         self.MODEL_DETAIL = lambda id_: f'{self.API_ROOT}/models/' + id_
+        self.MODEL_DELETE = f'{self.API_ROOT}/models/delete'
         self.MODEL_BUILD = f'{self.API_ROOT}/models'
         self.DATA_LIST = f'{self.API_ROOT}/{self.project_id}/data'
         self.DATA_DETAIL = lambda id_: f'{self.API_ROOT}/data/' + id_
 
+    def get_model_list(self):
+        resp = self.make_request('get', self.MODELS_LIST)
+        if resp:
+            models = []
+            for m in resp:
+                models.append(Model(m))
+            return models
+
     def get_model_info(self, model_name: str):
         id_ = self.get_model_id(model_name)
         resp = self.make_request('get', self.MODEL_DETAIL(id_))
         if resp:
             model = Model(resp)
             return model
 
@@ -151,14 +161,26 @@
         dataset_metadata = dataset.metadata
         for key in schema_mapping:
             if dataset_metadata.get(schema_mapping.get(key)):
                 result[key] = dataset_metadata.get(schema_mapping.get(key))
 
         return result
 
+    def delete_model_by_model_name(self, model_name):
+        data = {
+            'project': self.project_name,
+            'model_name': model_name
+        }
+        self.headers["Accept-Language"] = "en-US,en;q=0.9,vi;q=0.8,es;q=0.7"
+        make_request('post', self.MODEL_DELETE, headers=self.headers, json=data)
+
+    def delete_models(self, model_names):
+        for model_name in tqdm(model_names):
+            self.delete_model_by_model_name(model_name)
+
 
 def make_request(request_type: str, url: str, **kwargs):
     func = getattr(requests, request_type)
     if func is None:
         raise ValueError(
             f'Invalid request type {request_type}. ' f'Must be get, post or put'
         )
```

### Comparing `aitomatic-1.2.8/src/aitomatic/api/model_params.py` & `aitomatic-1.2.9/src/aitomatic/api/model_params.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/api/tuning_utils.py` & `aitomatic-1.2.9/src/aitomatic/api/tuning_utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/api/web_model.py` & `aitomatic-1.2.9/src/aitomatic/api/web_model.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/dsl/arl_conclusions.py` & `aitomatic-1.2.9/src/aitomatic/dsl/arl_conclusions.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/dsl/arl_features.py` & `aitomatic-1.2.9/src/aitomatic/dsl/arl_features.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/dsl/arl_handler.py` & `aitomatic-1.2.9/src/aitomatic/dsl/arl_handler.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/dsl/arl_rules.py` & `aitomatic-1.2.9/src/aitomatic/dsl/arl_rules.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/dsl/utils.py` & `aitomatic-1.2.9/src/aitomatic/dsl/utils.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/objects/dataset.py` & `aitomatic-1.2.9/src/aitomatic/objects/dataset.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic/objects/model.py` & `aitomatic-1.2.9/src/aitomatic/objects/model.py`

 * *Files identical despite different names*

### Comparing `aitomatic-1.2.8/src/aitomatic.egg-info/PKG-INFO` & `aitomatic-1.2.9/src/aitomatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aitomatic
-Version: 1.2.8
+Version: 1.2.9
 Summary: aitomatic library to interact with Aitomatic product
 Home-page: https://github.com/aitomatic/aitomatic-cli
 Author: Pham Hoang Tuan
 Author-email: tuan@aitomatic.com
 Project-URL: Bug Tracker, https://github.com/aitomatic/aitomatic-cli/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aitomatic-1.2.8/src/aitomatic.egg-info/SOURCES.txt` & `aitomatic-1.2.9/src/aitomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*


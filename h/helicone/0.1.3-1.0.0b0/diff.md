# Comparing `tmp/helicone-0.1.3.tar.gz` & `tmp/helicone-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicone-0.1.3.tar", max compression
+gzip compressed data, was "helicone-1.0.0b0.tar", max compression
```

## Comparing `helicone-0.1.3.tar` & `helicone-1.0.0b0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-04-30 18:04:13.152472 helicone-0.1.3/LICENSE
--rw-r--r--   0        0        0     9111 2023-05-12 15:45:01.033497 helicone-0.1.3/helicone/__init__.py
--rw-r--r--   0        0        0       20 2023-04-30 16:18:51.491845 helicone-0.1.3/helicone/requirements.txt
--rw-r--r--   0        0        0     7694 2023-05-12 15:45:01.103847 helicone-0.1.3/helicone/test.py
--rw-r--r--   0        0        0        0 2023-04-26 11:31:06.381002 helicone-0.1.3/helicone/utils.py
--rw-r--r--   0        0        0     1027 2023-05-12 15:45:00.986595 helicone-0.1.3/helicone/wrapper.py
--rw-r--r--   0        0        0      386 2023-05-11 21:09:58.962659 helicone-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 helicone-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.0b0/LICENSE
+-rw-r--r--   0        0        0        1 2023-07-06 18:54:19.040110 helicone-1.0.0b0/helicone/async_logger/__init__.py
+-rw-r--r--   0        0        0     2993 2023-07-06 18:54:19.040496 helicone-1.0.0b0/helicone/async_logger/async_logger.py
+-rw-r--r--   0        0        0       52 2023-07-06 18:54:19.040834 helicone-1.0.0b0/helicone/globals/__init__.py
+-rw-r--r--   0        0        0      883 2023-07-06 22:10:20.407271 helicone-1.0.0b0/helicone/globals/helicone.py
+-rw-r--r--   0        0        0       36 2023-07-06 18:54:19.041222 helicone-1.0.0b0/helicone/openai/__init__.py
+-rw-r--r--   0        0        0     8256 2023-07-06 22:10:01.218294 helicone-1.0.0b0/helicone/openai/openai_injector.py
+-rw-r--r--   0        0        0    10392 2023-07-06 18:54:19.042076 helicone-1.0.0b0/helicone/openai_proxy/__init__.py
+-rw-r--r--   0        0        0       20 2023-07-03 21:17:48.000891 helicone-1.0.0b0/helicone/requirements.txt
+-rw-r--r--   0        0        0    11232 2023-07-03 21:17:48.000970 helicone-1.0.0b0/helicone/test.py
+-rw-r--r--   0        0        0      381 2023-07-07 05:21:31.861028 helicone-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 helicone-1.0.0b0/PKG-INFO
```

### Comparing `helicone-0.1.3/LICENSE` & `helicone-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `helicone-0.1.3/helicone/__init__.py` & `helicone-1.0.0b0/helicone/openai_proxy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,46 +10,31 @@
     Completion,
     Edit,
     Embedding,
     Image,
     Moderation,
 )
 import logging
+import threading
 
 logger = logging.getLogger(__name__)
 
 api_key = os.environ.get("HELICONE_API_KEY", None)
 if (api_key is None):
     warnings.warn("Helicone API key is not set as an environment variable.")
 
 proxy_url = os.environ.get("HELICONE_PROXY_URL", "https://oai.hconeai.com/v1")
 
+global_headers = {}
 
-def normalize_data_type(data_type):
-    if isinstance(data_type, str):
-        data_type = data_type.lower()
 
-    if data_type in (str, "str", "string"):
-        return "string"
-    elif data_type in (bool, "bool", "boolean"):
-        return "boolean"
-    elif data_type in (float, int, "float", "int", "numerical"):
-        return "numerical"
-    elif data_type in (object, "object", "categorical"):
-        return "categorical"
-    else:
-        raise ValueError(
-            "Invalid data_type provided. Please use a valid data type or string.")
-
-
-api_key = os.environ.get("HELICONE_API_KEY", None)
-if (api_key is None):
-    warnings.warn("Helicone API key is not set as an environment variable.")
-
-proxy_url = os.environ.get("HELICONE_PROXY_URL", "https://oai.hconeai.com/v1")
+class AttributeDict(dict):
+    def __init__(self, *args, **kwargs):
+        super(AttributeDict, self).__init__(*args, **kwargs)
+        self.__dict__ = self
 
 
 def normalize_data_type(data_type):
     if isinstance(data_type, str):
         data_type = data_type.lower()
 
     if data_type in (str, "str", "string"):
@@ -81,14 +66,15 @@
     return original_api_base, kwargs
 
 
 class Helicone:
     def __init__(self):
         self.openai = openai
         self.apply_helicone_auth()
+        self.headers_store = {}
 
     @property
     def api_key(self):
         global api_key
         return api_key
 
     @api_key.setter
@@ -153,36 +139,50 @@
         headers.update(self._get_rate_limit_policy_headers(
             kwargs.pop("rate_limit_policy", None)))
 
         kwargs["headers"] = headers
 
         return helicone_request_id, kwargs
 
+    def update_response_headers(self, result, helicone_request_id):
+        headers = self.headers_store.get(helicone_request_id, {})
+        result["helicone"] = AttributeDict(
+            id=headers.get("Helicone-Id"),
+            status=headers.get("Helicone-Status"),
+            cache=headers.get("Helicone-Cache"),
+            rate_limit=AttributeDict(
+                limit=headers.get("Helicone-RateLimit-Limit"),
+                remaining=headers.get("Helicone-RateLimit-Remaining"),
+                reset=headers.get("Helicone-RateLimit-Reset"),
+                policy=headers.get("Helicone-RateLimit-Policy"),
+            ) if headers.get("Helicone-RateLimit-Policy") else None,
+        )
+
     def _modify_result(self, result, helicone_request_id):
         def result_with_helicone():
             for r in result:
-                r["helicone"] = {"id": helicone_request_id}
+                self.update_response_headers(r, helicone_request_id)
                 yield r
 
         if inspect.isgenerator(result):
             return result_with_helicone()
         else:
-            result["helicone"] = {"id": helicone_request_id}
+            self.update_response_headers(result, helicone_request_id)
             return result
 
     async def _modify_result_async(self, result, helicone_request_id):
         async def result_with_helicone_async():
             async for r in result:
-                r["helicone"] = {"id": helicone_request_id}
+                self.update_response_headers(r, helicone_request_id)
                 yield r
 
         if inspect.isasyncgen(result):
             return result_with_helicone_async()
         else:
-            result["helicone"] = {"id": helicone_request_id}
+            self.update_response_headers(result, helicone_request_id)
             return result
 
     def _with_helicone_auth(self, func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             helicone_request_id, kwargs = self._prepare_headers(**kwargs)
             original_api_base, kwargs = prepare_api_base(**kwargs)
@@ -245,29 +245,51 @@
                     policy += f';s={rate_limit_policy["segment"]}'
             else:
                 raise TypeError(
                     "rate_limit_policy must be either a string or a dictionary")
             return {"Helicone-RateLimit-Policy": policy}
         return {}
 
-    def apply_helicone_auth(self):
+    def apply_helicone_auth(self_parent):
+        def request_raw_patched(self, *args, **kwargs):
+            helicone_id = kwargs["supplied_headers"]["helicone-request-id"]
+            response = original_request_raw(self, *args, **kwargs)
+            if helicone_id:
+                with threading.Lock():
+                    self_parent.headers_store[helicone_id] = response.headers
+            return response
+
+        async def arequest_raw_patched(self, *args, **kwargs):
+            helicone_id = kwargs["supplied_headers"]["helicone-request-id"]
+            response = await original_arequest_raw(self, *args, **kwargs)
+            if helicone_id:
+                with threading.Lock():
+                    self_parent.headers_store[helicone_id] = response.headers
+            return response
+
+        original_request_raw = openai.api_requestor.APIRequestor.request_raw
+        openai.api_requestor.APIRequestor.request_raw = request_raw_patched
+
+        original_arequest_raw = openai.api_requestor.APIRequestor.arequest_raw
+        openai.api_requestor.APIRequestor.arequest_raw = arequest_raw_patched
+
         api_resources_classes = [
             (ChatCompletion, "create", "acreate"),
             (Completion, "create", "acreate"),
             (Edit, "create", "acreate"),
             (Embedding, "create", "acreate"),
             (Image, "create", "acreate"),
             (Moderation, "create", "acreate"),
         ]
 
         for api_resource_class, method, async_method in api_resources_classes:
             create_method = getattr(api_resource_class, method)
             setattr(api_resource_class, method,
-                    self._with_helicone_auth(create_method))
+                    self_parent._with_helicone_auth(create_method))
 
             async_create_method = getattr(api_resource_class, async_method)
             setattr(api_resource_class, async_method,
-                    self._with_helicone_auth_async(async_create_method))
+                    self_parent._with_helicone_auth_async(async_create_method))
 
 
-helicone = Helicone()
-log_feedback = helicone.log_feedback
+# helicone = Helicone()
+# log_feedback = helicone.log_feedback
```

### Comparing `helicone-0.1.3/PKG-INFO` & `helicone-1.0.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helicone
-Version: 0.1.3
+Version: 1.0.0b0
 Summary: A Python wrapper for the OpenAI API that logs all requests to Helicone.
 Home-page: https://www.helicone.ai
 License: Apache-2.0
 Author: Helicone, Inc.
 Author-email: help@helicone.ai
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: Apache Software License
```


# Comparing `tmp/service_now_api_sdk-0.0.20.tar.gz` & `tmp/service_now_api_sdk-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_now_api_sdk-0.0.20.tar", max compression
+gzip compressed data, was "service_now_api_sdk-0.0.21.tar", max compression
```

## Comparing `service_now_api_sdk-0.0.20.tar` & `service_now_api_sdk-0.0.21.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0     1083 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/LICENSE
--rw-r--r--   0        0        0     6564 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/README.md
--rw-r--r--   0        0        0      708 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/__init__.py
--rw-r--r--   0        0        0       43 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/exceptions.py
--rw-r--r--   0        0        0      140 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/attachments/__init__.py
--rw-r--r--   0        0        0     7114 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/attachments/client.py
--rw-r--r--   0        0        0      227 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/attachments/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/client.py
--rw-r--r--   0        0        0    10869 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py
--rw-r--r--   0        0        0        0 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/__init__.py
--rw-r--r--   0        0        0    15486 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/client.py
--rw-r--r--   0        0        0      818 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/exceptions.py
--rw-r--r--   0        0        0      255 2023-06-15 19:26:26.737149 service_now_api_sdk-0.0.20/service_now_api_sdk/settings.py
--rw-r--r--   0        0        0     7205 1970-01-01 00:00:00.000000 service_now_api_sdk-0.0.20/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/LICENSE
+-rw-r--r--   0        0        0     7072 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/README.md
+-rw-r--r--   0        0        0      708 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/exceptions.py
+-rw-r--r--   0        0        0      200 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/attachments/__init__.py
+-rw-r--r--   0        0        0     7114 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/attachments/client.py
+-rw-r--r--   0        0        0      227 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/attachments/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/helpers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/helpers/client.py
+-rw-r--r--   0        0        0    10869 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/table/__init__.py
+-rw-r--r--   0        0        0    15486 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/table/client.py
+-rw-r--r--   0        0        0      818 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/table/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/utils/__init__.py
+-rw-r--r--   0        0        0     4245 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/utils/aux_functions.py
+-rw-r--r--   0        0        0      117 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/utils/constants.py
+-rw-r--r--   0        0        0      255 2023-07-07 17:52:19.841669 service_now_api_sdk-0.0.21/service_now_api_sdk/settings.py
+-rw-r--r--   0        0        0     7698 1970-01-01 00:00:00.000000 service_now_api_sdk-0.0.21/PKG-INFO
```

### Comparing `service_now_api_sdk-0.0.20/LICENSE` & `service_now_api_sdk-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.20/README.md` & `service_now_api_sdk-0.0.21/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -115,14 +115,29 @@
 }
 
 producer_catalog = ProducerServiceCatalog()
 
 result = producer_catalog.store(catalog_id=survey_catalog_id, variables=variables)
 
 ```
+## Get ticket plataform URL by query or ticket number
+To get ticket plataform URL by query or ticket number, you can use ``aux_functions`` function.
+```python
+from service_now_api_sdk.sdk import aux_functions
+
+query = QueryBuilder().field('number').starts_with("RIT")
+
+url = aux_functions.make_platform_url_list_view(table_name="sc_req_item", query=query, interface="list_view")
+
+print(url)
+
+Output:
+    https://stone.service-now.com/sc_req_item_list.do?sysparm_query=numberSTARTSWITHRIT
+
+```
 # Query params
 
 ### field(field)
 Define the field to operate
 
 **parameters**: field – field (str) to operate
```

### Comparing `service_now_api_sdk-0.0.20/pyproject.toml` & `service_now_api_sdk-0.0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "service_now_api_sdk"
-version = "0.0.20"
+version = "0.0.21"
 description = "Service Now API SDK is used to facilitate integrations, automations and also code reuse"
 authors = ["stone_people_analytics <systems-techpeople@stone.com.br>"]
 maintainers = [
     "guilherme_lsilva <manager.guilherme.silva@gmail.com>",
     "diogo56 <diogo.amorim2001@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/attachments/client.py` & `service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/attachments/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/client.py` & `service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/helpers/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py` & `service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/helpers/query_builder.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/client.py` & `service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/table/client.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.20/service_now_api_sdk/sdk/servicenow/table/exceptions.py` & `service_now_api_sdk-0.0.21/service_now_api_sdk/sdk/servicenow/table/exceptions.py`

 * *Files identical despite different names*

### Comparing `service_now_api_sdk-0.0.20/PKG-INFO` & `service_now_api_sdk-0.0.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: service-now-api-sdk
-Version: 0.0.20
+Version: 0.0.21
 Summary: Service Now API SDK is used to facilitate integrations, automations and also code reuse
 Home-page: https://github.com/people-analytics-tech/ service-now-api-sdk
 License: MIT
 Author: stone_people_analytics
 Author-email: systems-techpeople@stone.com.br
 Maintainer: guilherme_lsilva
 Maintainer-email: manager.guilherme.silva@gmail.com
@@ -135,14 +135,29 @@
 }
 
 producer_catalog = ProducerServiceCatalog()
 
 result = producer_catalog.store(catalog_id=survey_catalog_id, variables=variables)
 
 ```
+## Get ticket plataform URL by query or ticket number
+To get ticket plataform URL by query or ticket number, you can use ``aux_functions`` function.
+```python
+from service_now_api_sdk.sdk import aux_functions
+
+query = QueryBuilder().field('number').starts_with("RIT")
+
+url = aux_functions.make_platform_url_list_view(table_name="sc_req_item", query=query, interface="list_view")
+
+print(url)
+
+Output:
+    https://stone.service-now.com/sc_req_item_list.do?sysparm_query=numberSTARTSWITHRIT
+
+```
 # Query params
 
 ### field(field)
 Define the field to operate
 
 **parameters**: field – field (str) to operate
```


# Comparing `tmp/bmsdna_lakeapi-0.9.6.tar.gz` & `tmp/bmsdna_lakeapi-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.9.6.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.9.7.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.9.6.tar` & `bmsdna_lakeapi-0.9.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-07-04 13:39:00.683609 bmsdna_lakeapi-0.9.6/LICENSE
--rw-r--r--   0        0        0     9235 2023-07-04 13:39:00.683609 bmsdna_lakeapi-0.9.6/README.md
--rw-r--r--   0        0        0      380 2023-07-04 13:39:00.683609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 13:39:00.683609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1138 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      625 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     7186 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10721 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6256 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11332 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12623 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/datasource.py
--rw-r--r--   0        0        0     6889 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/detail_endpoint.py
--rw-r--r--   0        0        0    10169 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6891 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6813 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4553 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3813 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3040 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2409 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1084 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     2017 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    10434 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-06 09:51:56.851343 bmsdna_lakeapi-0.9.7/LICENSE
+-rw-r--r--   0        0        0     9235 2023-07-06 09:51:56.851343 bmsdna_lakeapi-0.9.7/README.md
+-rw-r--r--   0        0        0      380 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1138 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      625 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     7186 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10721 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6256 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11414 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12623 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/datasource.py
+-rw-r--r--   0        0        0     6889 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/detail_endpoint.py
+-rw-r--r--   0        0        0    10169 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6891 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6813 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4553 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3813 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3040 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2409 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1084 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-07-06 09:51:56.855343 bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     2017 2023-07-06 09:51:56.859343 bmsdna_lakeapi-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0    10434 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.7/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.9.6/LICENSE` & `bmsdna_lakeapi-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/README.md` & `bmsdna_lakeapi-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Tuple,
     TypedDict,
     Union,
     cast,
     TYPE_CHECKING,
 )
 from typing_extensions import TypedDict, NotRequired, Required
-
+import copy
 import yaml
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.partition_utils import _with_implicit_parameters
 from bmsdna.lakeapi.core.types import FileTypes, OperatorType, Param, PolaryTypeFunction, Engines, SearchConfig
 
@@ -227,15 +227,15 @@
             root_folder = os.path.join(basic_config.data_path, folder)
             if not os.path.exists(root_folder):
                 logger.warning("Path not existing: " + root_folder)
                 return []
             else:
                 ls = []
                 for it in os.scandir(root_folder):
-                    config_sub = config.copy()
+                    config_sub = copy.deepcopy(config)  # important! deepcopy required for subobjects like datasource
                     config_sub["name"] = it.name
                     config_sub["datasource"]["uri"] = config["datasource"]["uri"].replace("/*", "/" + it.name)
                     tbl_name = (config_sub.get("version", 1), config_sub["tag"], config_sub["name"])
                     file_type = config_sub["datasource"].get("file_type", "delta")
                     res_name = config_sub
                     if tbl_name not in table_names and (
                         (it.is_dir() and file_type == "delta") or (it.is_file() and file_type != "delta")
```

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/datasource.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/datasource.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/detail_endpoint.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/detail_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.9.7/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.6/pyproject.toml` & `bmsdna_lakeapi-0.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.9.6"
+version = "0.9.7"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.9.6/PKG-INFO` & `bmsdna_lakeapi-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.9.6
+Version: 0.9.7
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


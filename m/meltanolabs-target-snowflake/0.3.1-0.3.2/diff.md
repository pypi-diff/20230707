# Comparing `tmp/meltanolabs_target_snowflake-0.3.1.tar.gz` & `tmp/meltanolabs_target_snowflake-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.3.1.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.3.2.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.3.1.tar` & `meltanolabs_target_snowflake-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3860 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/LICENSE
--rw-r--r--   0        0        0     3924 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/README.md
--rw-r--r--   0        0        0     1282 2023-07-06 18:26:35.312003 meltanolabs_target_snowflake-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       89 2023-07-06 18:26:35.316004 meltanolabs_target_snowflake-0.3.1/target_snowflake/__init__.py
--rw-r--r--   0        0        0    18756 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/target_snowflake/connector.py
--rw-r--r--   0        0        0     7872 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/target_snowflake/sinks.py
--rw-r--r--   0        0        0      724 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/target_snowflake/snowflake_types.py
--rw-r--r--   0        0        0     4057 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/target_snowflake/target.py
--rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-07-07 21:27:05.276414 meltanolabs_target_snowflake-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3924 2023-07-07 21:27:05.276414 meltanolabs_target_snowflake-0.3.2/README.md
+-rw-r--r--   0        0        0     1307 2023-07-07 21:27:28.452564 meltanolabs_target_snowflake-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-07-07 21:27:28.452564 meltanolabs_target_snowflake-0.3.2/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    17854 2023-07-07 21:27:05.280414 meltanolabs_target_snowflake-0.3.2/target_snowflake/connector.py
+-rw-r--r--   0        0        0     8248 2023-07-07 21:27:05.280414 meltanolabs_target_snowflake-0.3.2/target_snowflake/sinks.py
+-rw-r--r--   0        0        0      724 2023-07-07 21:27:05.280414 meltanolabs_target_snowflake-0.3.2/target_snowflake/snowflake_types.py
+-rw-r--r--   0        0        0     2188 2023-07-07 21:27:05.280414 meltanolabs_target_snowflake-0.3.2/target_snowflake/target.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.3.2/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.3.1/LICENSE` & `meltanolabs_target_snowflake-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.1/README.md` & `meltanolabs_target_snowflake-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.1/pyproject.toml` & `meltanolabs_target_snowflake-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.3.1"
+version = "0.3.2"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
@@ -12,20 +12,21 @@
 packages = [
     { include = "target_snowflake" }
 ]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
 requests = "^2.31.0"
-snowflake-sqlalchemy = "^1.4.1"
-singer-sdk = "0.28.0"
+snowflake-sqlalchemy = "^1.4.7"
+singer-sdk = "0.29.0"
+cryptography = "^40.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
-singer-sdk = { version="0.28.0", extras = ["testing"] }
+singer-sdk = { version="0.29.0", extras = ["testing"] }
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.7"
 
 [tool.ruff]
 ignore = [
     "ANN101",  # missing-type-self
```

### Comparing `meltanolabs_target_snowflake-0.3.1/target_snowflake/connector.py` & `meltanolabs_target_snowflake-0.3.2/target_snowflake/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,42 +34,14 @@
 def evaluate_typemaps(type_maps, compare_value, unmatched_value):
     for type_map in type_maps:
         if type_map.match(compare_value):
             return type_map.map_value
     return unmatched_value
 
 
-def _jsonschema_type_check(jsonschema_type: dict, type_check: Tuple[str]) -> bool:
-    """Return True if the jsonschema_type supports the provided type.
-
-    Args:
-        jsonschema_type: The type dict.
-        type_check: A tuple of type strings to look for.
-
-    Returns:
-        True if the schema suports the type.
-    """
-    if "type" in jsonschema_type:
-        if isinstance(jsonschema_type["type"], (list, tuple)):
-            for schema_type in jsonschema_type["type"]:
-                if schema_type in type_check:
-                    return True
-        else:
-            if jsonschema_type.get("type") in type_check:  # noqa: PLR5501
-                return True
-
-    # TODO: remove following release of https://github.com/meltano/sdk/issues/1774
-    if any(
-        _jsonschema_type_check(t, type_check)
-        for t in jsonschema_type.get("anyOf", ())
-    ):
-        return True
-
-    return False
-
 class SnowflakeConnector(SQLConnector):
     """Snowflake Target Connector.
 
     This class handles all DDL and type conversions.
     """
 
     allow_column_add: bool = True  # Whether ADD COLUMN is supported.
@@ -263,20 +235,20 @@
         string_submaps = [
             TypeMap(eq, TIMESTAMP_NTZ(), "date-time"),
             TypeMap(contains, sqlalchemy.types.TIME(), "time"),
             TypeMap(eq, sqlalchemy.types.DATE(), "date"),
             TypeMap(eq, sqlalchemy.types.VARCHAR(maxlength), None),
         ]
         type_maps = [
-            TypeMap(_jsonschema_type_check, NUMBER(), ("integer",)),
-            TypeMap(_jsonschema_type_check, VARIANT(), ("object",)),
-            TypeMap(_jsonschema_type_check, VARIANT(), ("array",)),
+            TypeMap(th._jsonschema_type_check, NUMBER(), ("integer",)),
+            TypeMap(th._jsonschema_type_check, VARIANT(), ("object",)),
+            TypeMap(th._jsonschema_type_check, VARIANT(), ("array",)),
         ]
         # apply type maps
-        if _jsonschema_type_check(jsonschema_type, ("string",)):
+        if th._jsonschema_type_check(jsonschema_type, ("string",)):
             datelike_type = th.get_datelike_property_type(jsonschema_type)
             target_type = evaluate_typemaps(string_submaps, datelike_type, target_type)
         else:
             target_type = evaluate_typemaps(type_maps, jsonschema_type, target_type)
 
         return cast(sqlalchemy.types.TypeEngine, target_type)
```

### Comparing `meltanolabs_target_snowflake-0.3.1/target_snowflake/sinks.py` & `meltanolabs_target_snowflake-0.3.2/target_snowflake/sinks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Snowflake target sink class, which handles writing streams."""
 from __future__ import annotations
 
-import gzip
-import json
 import os
 import typing as t
 from urllib.parse import urlparse
 from uuid import uuid4
 
 from singer_sdk import PluginBase, SQLConnector
 from singer_sdk.batch import JSONLinesBatcher
 from singer_sdk.helpers._batch import (
     BaseBatchFileEncoding,
     BatchConfig,
     BatchFileFormat,
-    StorageTarget,
 )
 from singer_sdk.helpers._typing import conform_record_data_types
 from singer_sdk.sinks import SQLSink
 from snowflake.sqlalchemy.base import SnowflakeIdentifierPreparer
 from snowflake.sqlalchemy.snowdialect import SnowflakeDialect
 
 from target_snowflake.connector import SnowflakeConnector
@@ -231,7 +228,19 @@
                 full_table_name=self.full_table_name,
                 files=files,
             )
         else:
             raise NotImplementedError(
                 f"Unsupported batch file encoding: {encoding.format}"
             )
+
+    # TODO: remove after https://github.com/meltano/sdk/issues/1819 is fixed
+    def _singer_validate_message(self, record: dict) -> None:
+        """Ensure record conforms to Singer Spec.
+
+        Args:
+            record: Record (after parsing, schema validations and transformations).
+
+        Raises:
+            MissingKeyPropertiesError: If record is missing one or more key properties.
+        """
+        pass
```

### Comparing `meltanolabs_target_snowflake-0.3.1/target_snowflake/snowflake_types.py` & `meltanolabs_target_snowflake-0.3.2/target_snowflake/snowflake_types.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.1/PKG-INFO` & `meltanolabs_target_snowflake-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: meltanolabs-target-snowflake
-Version: 0.3.1
+Version: 0.3.2
 Summary: `target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,Snowflake
 Author: Ken Payne
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography (>=40.0.2,<41.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: singer-sdk (==0.28.0)
-Requires-Dist: snowflake-sqlalchemy (>=1.4.1,<2.0.0)
+Requires-Dist: singer-sdk (==0.29.0)
+Requires-Dist: snowflake-sqlalchemy (>=1.4.7,<2.0.0)
 Description-Content-Type: text/markdown
 
 # `target-snowflake`
 
 Target for Snowflake.
 
 Built with the [Meltano Singer SDK](https://sdk.meltano.com).
```


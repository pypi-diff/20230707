# Comparing `tmp/nhs_aws_helpers-0.1.3.tar.gz` & `tmp/nhs_aws_helpers-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_aws_helpers-0.1.3.tar", max compression
+gzip compressed data, was "nhs_aws_helpers-0.1.4.tar", max compression
```

## Comparing `nhs_aws_helpers-0.1.3.tar` & `nhs_aws_helpers-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1078 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/LICENSE.md
--rw-r--r--   0        0        0      666 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/README.md
--rw-r--r--   0        0        0    39862 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/__init__.py
--rw-r--r--   0        0        0     7980 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/async_s3_object_reader.py
--rw-r--r--   0        0        0     6673 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/async_s3_object_writer.py
--rw-r--r--   0        0        0      674 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/common.py
--rw-r--r--   0        0        0     4508 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/fixtures.py
--rw-r--r--   0        0        0        0 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/py.typed
--rw-r--r--   0        0        0     7916 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/s3_object_reader.py
--rw-r--r--   0        0        0     6681 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/s3_object_writer.py
--rw-r--r--   0        0        0     3058 2023-07-06 21:25:40.192826 nhs_aws_helpers-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0    10996 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/async_s3_object_buffer_tests.py
--rw-r--r--   0        0        0     7558 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/aws_tests.py
--rw-r--r--   0        0        0      280 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0     2272 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/ddb_tests.py
--rw-r--r--   0        0        0    10316 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/s3_object_buffer_tests.py
--rw-r--r--   0        0        0      518 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/utils.py
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      666 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/README.md
+-rw-r--r--   0        0        0    39862 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/__init__.py
+-rw-r--r--   0        0        0     7980 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/async_s3_object_reader.py
+-rw-r--r--   0        0        0     6673 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/async_s3_object_writer.py
+-rw-r--r--   0        0        0      674 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/common.py
+-rw-r--r--   0        0        0     4618 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/fixtures.py
+-rw-r--r--   0        0        0        0 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/py.typed
+-rw-r--r--   0        0        0     7916 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/s3_object_reader.py
+-rw-r--r--   0        0        0     6681 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/s3_object_writer.py
+-rw-r--r--   0        0        0     3058 2023-07-06 22:07:09.457001 nhs_aws_helpers-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0    10996 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/async_s3_object_buffer_tests.py
+-rw-r--r--   0        0        0     7558 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/aws_tests.py
+-rw-r--r--   0        0        0      280 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0     2272 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/ddb_tests.py
+-rw-r--r--   0        0        0    10316 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/s3_object_buffer_tests.py
+-rw-r--r--   0        0        0      518 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/utils.py
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.1.4/PKG-INFO
```

### Comparing `nhs_aws_helpers-0.1.3/LICENSE.md` & `nhs_aws_helpers-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/README.md` & `nhs_aws_helpers-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/nhs_aws_helpers/__init__.py` & `nhs_aws_helpers-0.1.4/nhs_aws_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/nhs_aws_helpers/async_s3_object_reader.py` & `nhs_aws_helpers-0.1.4/nhs_aws_helpers/async_s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/nhs_aws_helpers/async_s3_object_writer.py` & `nhs_aws_helpers-0.1.4/nhs_aws_helpers/async_s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/nhs_aws_helpers/common.py` & `nhs_aws_helpers-0.1.4/nhs_aws_helpers/common.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/nhs_aws_helpers/fixtures.py` & `nhs_aws_helpers-0.1.4/nhs_aws_helpers/fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,33 +95,35 @@
     queue = sqs.create_queue(QueueName=queue_name, Attributes=dict(FifoQueue="true", VisibilityTimeout="2"))
 
     yield queue
 
     queue.delete()
 
 
-def clone_schema(table, on_demand_billing_mode: bool = True, provisioned_capacity: int = 500):
+def clone_schema(table, on_demand_billing_mode: bool = True, provisioned_capacity: int = 250):
     key_schema = table.key_schema
 
     attributes = table.attribute_definitions
 
     indexes = table.global_secondary_indexes
 
     if indexes:
         for index in indexes:
             del index["IndexStatus"]
             del index["IndexSizeBytes"]
             del index["ItemCount"]
             del index["IndexArn"]
+            del index["ProvisionedThroughput"]
 
     clone = {
         "KeySchema": key_schema,
         "AttributeDefinitions": attributes,
     }
-
+    if on_demand_billing_mode:
+        provisioned_capacity = 0
     billing: Dict[str, Any] = (
         {
             "BillingMode": "PAY_PER_REQUEST",
         }
         if on_demand_billing_mode
         else {
             "ProvisionedThroughput": {
```

### Comparing `nhs_aws_helpers-0.1.3/nhs_aws_helpers/s3_object_reader.py` & `nhs_aws_helpers-0.1.4/nhs_aws_helpers/s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/nhs_aws_helpers/s3_object_writer.py` & `nhs_aws_helpers-0.1.4/nhs_aws_helpers/s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/pyproject.toml` & `nhs_aws_helpers-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhs_aws_helpers"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "nhs_aws_helpers" },
     { include = "tests", format = "sdist" },
 ]
```

### Comparing `nhs_aws_helpers-0.1.3/tests/async_s3_object_buffer_tests.py` & `nhs_aws_helpers-0.1.4/tests/async_s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/tests/aws_tests.py` & `nhs_aws_helpers-0.1.4/tests/aws_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/tests/ddb_tests.py` & `nhs_aws_helpers-0.1.4/tests/ddb_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/tests/s3_object_buffer_tests.py` & `nhs_aws_helpers-0.1.4/tests/s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/tests/utils.py` & `nhs_aws_helpers-0.1.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.3/PKG-INFO` & `nhs_aws_helpers-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-aws-helpers
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: spinecore
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


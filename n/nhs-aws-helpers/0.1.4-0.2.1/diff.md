# Comparing `tmp/nhs_aws_helpers-0.1.4.tar.gz` & `tmp/nhs_aws_helpers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_aws_helpers-0.1.4.tar", max compression
+gzip compressed data, was "nhs_aws_helpers-0.2.1.tar", max compression
```

## Comparing `nhs_aws_helpers-0.1.4.tar` & `nhs_aws_helpers-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0     1078 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/LICENSE.md
--rw-r--r--   0        0        0      666 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/README.md
--rw-r--r--   0        0        0    39862 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/__init__.py
--rw-r--r--   0        0        0     7980 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/async_s3_object_reader.py
--rw-r--r--   0        0        0     6673 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/async_s3_object_writer.py
--rw-r--r--   0        0        0      674 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/common.py
--rw-r--r--   0        0        0     4618 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/fixtures.py
--rw-r--r--   0        0        0        0 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/py.typed
--rw-r--r--   0        0        0     7916 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/s3_object_reader.py
--rw-r--r--   0        0        0     6681 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/nhs_aws_helpers/s3_object_writer.py
--rw-r--r--   0        0        0     3058 2023-07-06 22:07:09.457001 nhs_aws_helpers-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0    10996 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/async_s3_object_buffer_tests.py
--rw-r--r--   0        0        0     7558 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/aws_tests.py
--rw-r--r--   0        0        0      280 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     2272 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/ddb_tests.py
--rw-r--r--   0        0        0    10316 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/s3_object_buffer_tests.py
--rw-r--r--   0        0        0      518 2023-07-06 22:06:50.605317 nhs_aws_helpers-0.1.4/tests/utils.py
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0      666 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/README.md
+-rw-r--r--   0        0        0    39862 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/__init__.py
+-rw-r--r--   0        0        0     7980 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/async_s3_object_reader.py
+-rw-r--r--   0        0        0     6673 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/async_s3_object_writer.py
+-rw-r--r--   0        0        0     1331 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/common.py
+-rw-r--r--   0        0        0        0 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/dynamodb_model_store/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-07 19:42:02.816047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/dynamodb_model_store/base_model.py
+-rw-r--r--   0        0        0    26465 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/dynamodb_model_store/base_model_store.py
+-rw-r--r--   0        0        0     4618 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/fixtures.py
+-rw-r--r--   0        0        0        0 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/py.typed
+-rw-r--r--   0        0        0     7916 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/s3_object_reader.py
+-rw-r--r--   0        0        0     6681 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/nhs_aws_helpers/s3_object_writer.py
+-rw-r--r--   0        0        0     3056 2023-07-07 19:42:25.635909 nhs_aws_helpers-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0    10996 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/async_s3_object_buffer_tests.py
+-rw-r--r--   0        0        0     7558 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/aws_tests.py
+-rw-r--r--   0        0        0    21983 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/base_model_store_tests.py
+-rw-r--r--   0        0        0      280 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     2272 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/ddb_tests.py
+-rw-r--r--   0        0        0    10316 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/s3_object_buffer_tests.py
+-rw-r--r--   0        0        0      518 2023-07-07 19:42:02.820047 nhs_aws_helpers-0.2.1/tests/utils.py
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.2.1/PKG-INFO
```

### Comparing `nhs_aws_helpers-0.1.4/LICENSE.md` & `nhs_aws_helpers-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/README.md` & `nhs_aws_helpers-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/nhs_aws_helpers/__init__.py` & `nhs_aws_helpers-0.2.1/nhs_aws_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/nhs_aws_helpers/async_s3_object_reader.py` & `nhs_aws_helpers-0.2.1/nhs_aws_helpers/async_s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/nhs_aws_helpers/async_s3_object_writer.py` & `nhs_aws_helpers-0.2.1/nhs_aws_helpers/async_s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/nhs_aws_helpers/fixtures.py` & `nhs_aws_helpers-0.2.1/nhs_aws_helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/nhs_aws_helpers/s3_object_reader.py` & `nhs_aws_helpers-0.2.1/nhs_aws_helpers/s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/nhs_aws_helpers/s3_object_writer.py` & `nhs_aws_helpers-0.2.1/nhs_aws_helpers/s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/pyproject.toml` & `nhs_aws_helpers-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 [tool.poetry]
 name = "nhs_aws_helpers"
-version = "0.1.4"
+version = "0.2.1"
 description = ""
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "nhs_aws_helpers" },
     { include = "tests", format = "sdist" },
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 # core dependencies
 python = ">=3.8.1,<4.0"
-
-
 boto3 = "^1.26.159"
 boto3-stubs = {extras = ["s3", "ssm", "secretsmanager", "dynamodb", "stepfunctions", "sqs", "lambda", "logs", "sns", "events", "kms", "firehose", "athena"], version = "^1.26.159"}
 botocore-stubs = "^1.29.159"
 
 
 [tool.setuptools.package-data]
 "nhs_aws_helpers" = ["py.typed"]
 
 [tool.poetry.group.dev.dependencies]
 # ci / testing dependencies
 petname = "^2.6"
 black = "^22.12.0"
 isort = "^5.12.0"
-mypy = "^1.3.0"
+mypy = "^1.4.0"
 coverage = "^7.2.7"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 flake8 = "^6.0.0"
 flake8-pyproject = "^1.2.3"
 flake8-black = "^0.3.6"
 tox = "^4.6.3"
@@ -93,15 +91,15 @@
 ]
 omit = [
     "tests/*",
 ]
 sort = "-cover"
 ignore_errors = true
 precision = 2
-fail_under = 54
+fail_under = 65
 show_missing = true
 
 [tool.coverage.xml]
 output = "reports/coverage.xml"
```

### Comparing `nhs_aws_helpers-0.1.4/tests/async_s3_object_buffer_tests.py` & `nhs_aws_helpers-0.2.1/tests/async_s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/tests/aws_tests.py` & `nhs_aws_helpers-0.2.1/tests/aws_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/tests/ddb_tests.py` & `nhs_aws_helpers-0.2.1/tests/ddb_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/tests/s3_object_buffer_tests.py` & `nhs_aws_helpers-0.2.1/tests/s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/tests/utils.py` & `nhs_aws_helpers-0.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.4/PKG-INFO` & `nhs_aws_helpers-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-aws-helpers
-Version: 0.1.4
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: spinecore
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


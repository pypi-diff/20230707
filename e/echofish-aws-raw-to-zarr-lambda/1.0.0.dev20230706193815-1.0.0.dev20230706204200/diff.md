# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815.tar", last modified: Thu Jul  6 19:39:16 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200.tar", last modified: Thu Jul  6 20:42:59 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:39:16.854461 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 19:38:10.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 19:39:16.850461 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-06 19:38:10.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 19:39:16.854461 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-06 19:39:12.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:39:16.850461 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:39:16.850461 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 19:38:10.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-06 19:38:10.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15156 2023-07-06 19:38:10.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-06 19:38:10.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3812 2023-07-06 19:38:10.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:39:16.850461 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 19:39:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-06 19:39:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 19:39:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-06 19:39:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-06 19:39:16.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 20:42:59.855166 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 20:41:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 20:42:59.855166 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-06 20:41:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 20:42:59.855166 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-06 20:42:55.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 20:42:59.851166 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 20:42:59.855166 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 20:41:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-06 20:41:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15153 2023-07-06 20:41:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-06 20:41:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-07-06 20:41:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 20:42:59.855166 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 20:42:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-06 20:42:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 20:42:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-06 20:42:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-06 20:42:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230706193815
+Version: 1.0.0.dev20230706204200
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230706193815",
+  version="1.0.0.dev20230706204200",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.__input_bucket = input_bucket
         self.__output_bucket = output_bucket
         self.__table_name = table_name
         self.__output_bucket_access_key = output_bucket_access_key
         self.__output_bucket_secret_access_key = output_bucket_secret_access_key
 
     ############################################################################
-    def __delete_all_local_raw_and_zarr_files(self):
+    def __delete_all_local_raw_and_zarr_files(self):  # good
         """Used to clean up any residual files from warm lambdas
         to keep the storage footprint below the 512 MB allocation.
 
         Returns
         -------
         None : None
             No return value.
@@ -52,15 +52,14 @@
                 if os.path.isdir(j):
                     shutil.rmtree(j, ignore_errors=True)
                 elif os.path.isfile(j):
                     os.remove(j)
 
     ############################################################################
     def __set_processing_status(
-        # TODO: need to pass in the table name
         self,
         ship_name: str,
         cruise_name: str,
         sensor_name: str,
         file_name: str,
         new_status: str
     ):
@@ -335,15 +334,14 @@
     ############################################################################
     def execute(self, message):
         ship_name = message['ship_name']
         cruise_name = message['cruise_name']
         sensor_name = message['sensor_name']
         input_file_name = message['input_file_name']
         #
-        #
         store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
         output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{store_name}/"
         bucket_key = f"data/raw/{ship_name}/{cruise_name}/{sensor_name}/{input_file_name}"
         print(bucket_key)
         #
         # TODO: get processing status here and handle for idempotency
         # print(f"Processing: {input_file_name} for {cruise_name}")
@@ -356,15 +354,19 @@
             ship_name=ship_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             file_name=input_file_name,
             new_status="PROCESSING"
         )
         self.__delete_all_local_raw_and_zarr_files()  # good
-        self.__s3.download_file(bucket_name=self.__input_bucket, key=bucket_key, file_name=input_file_name)
+        self.__s3.download_file(
+            bucket_name=self.__input_bucket,
+            key=bucket_key,
+            file_name=input_file_name
+        )
         print('s3 download file done')
         self.__create_local_zarr_store(
             raw_file_name=input_file_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             output_zarr_prefix=output_zarr_prefix,
             store_name=store_name
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import boto3
 from collections.abc import Generator
 
 class S3Operations:
-
+    #####################################################################
     def __get_client(self, access_key_id=None, secret_access_key=None):
         client = None
         if access_key_id:
             client = boto3.Session().client(
                 service_name='s3',
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=secret_access_key
             )
         else:
             client = boto3.Session().client('s3')
         return client
 
+    #####################################################################
     def list_objects(  # analog to find_children_objects
         self,
         bucket_name,
         prefix,
         access_key_id=None,
         secret_access_key=None
     ):
@@ -45,29 +46,35 @@
             contents = page["Contents"]
             # for obj in contents:
             #     keys.append(obj["Key"])
             if 'Contents' in page.keys():
                 keys.extend(page['Contents'])
         return keys
 
+    #####################################################################
     def get_s3_files(self):
         # gets a set of files
         pass
 
+    #####################################################################
     def download_file(
         self,
         bucket_name,
         key,
         file_name,
-        access_key_id=None,
+        access_key_id=None,  # This should always be a bucket we have aws credentials for
         secret_access_key=None
     ):
-        self.__get_client(access_key_id, secret_access_key).download_file(bucket_name, key, file_name)
+        self.__get_client(
+            access_key_id,
+            secret_access_key
+        ).download_file(Bucket=bucket_name, Key=key, Filename=file_name)
 
-    def chunked(
+    #####################################################################
+    def __chunked(
             ll: list,
             n: int
     ) -> Generator:
         """Yields successively n-sized chunks from ll.
 
         Parameters
         ----------
@@ -80,52 +87,50 @@
         -------
         Batches : Generator
             Breaks the data into smaller chunks for processing
         """
         for i in range(0, len(ll), n):
             yield ll[i:i + n]
 
+    #####################################################################
     def delete(
         self,
         bucket_name,
         key,
         access_key_id=None,
         secret_access_key=None
     ):
         self.__get_client(access_key_id, secret_access_key).delete_object(
             Bucket=bucket_name,
             Key=key,
         )
 
-
-    def delete_children_files(
-            self,
-            bucket_name,
-            key,
-            access_key_id=None,
-            secret_access_key=None
+    #####################################################################
+    def delete_children_files(  # was "delete_remote_objects"
+        self,
+        raw_zarr_files: list,
+        output_bucket: str,
+        access_key_id: str = None,
+        secret_access_key: str = None,
     ):
-        # self.__get_client(access_key_id, secret_access_key).delete_object(
-        #     Bucket=bucket_name,
-        #     Key=key,
-        # )
+        # deletes all given keys in s3 bucket
         objects_to_delete = []
         for raw_zarr_file in raw_zarr_files:
             objects_to_delete.append({'Key': raw_zarr_file['Key']})
-        # Delete in groups of 100 -- Boto3 constraint.
-        for batch in chunked(objects_to_delete, 100):
-            # print(f"0: {batch[0]}, -1: {batch[-1]}")
-            deleted = s3.delete_objects(
+        # Delete in groups of 100 — Boto3 constraint
+        for batch in self.__chunked(objects_to_delete, 100):
+            deleted = self.__get_client(access_key_id, secret_access_key).delete_objects(
                 Bucket=output_bucket,
                 Delete={
                     "Objects": batch
                 }
             )
             print(f"Deleted {len(deleted['Deleted'])} files")
 
+    #####################################################################
     def upload_file(
         self,
         file_name,
         bucket_name,
         key,
         access_key_id=None,
         secret_access_key=None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230706193815
+Version: 1.0.0.dev20230706204200
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706193815/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706204200/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*


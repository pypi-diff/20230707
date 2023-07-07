# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354.tar", last modified: Thu Jul  6 23:04:57 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722.tar", last modified: Fri Jul  7 18:48:24 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-06 23:04:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:04:57.898265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15206 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3875 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-07 18:48:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:48:24.363593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15457 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-07-07 18:47:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 18:48:24.367593 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-07 18:48:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230706230354
+Version: 1.0.0.dev20230707184722
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230706230354",
+  version="1.0.0.dev20230707184722",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,20 +297,22 @@
             start_time=start_time,
             end_time=end_time,
             frequencies=frequencies,
             channels=channels
         )
 
     ############################################################################
-    # TODO: I am thinking that that this won't delete everything? Needs batches -rk
+    # TODO: I am thinking that that this won't delete everything?
+    #  Needs batches -rk
+    #  Needs passed in list of files by prefix
     def __remove_existing_s3_objects(
         self,
         output_zarr_prefix
     ):
-        for key in self.__s3.list_objects(
+        for key in self.__s3.list_objects(  # problem here
                 bucket_name=self.__output_bucket,
                 prefix=output_zarr_prefix,
                 access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
         ):
             self.__s3.delete(
                 bucket_name=self.__output_bucket,
@@ -326,18 +328,25 @@
         object_prefix
     ):
         for subdir, dirs, files in os.walk(local_directory):
             for file in files:
                 local_path = os.path.join(subdir, file)
                 print(local_path)
                 s3_key = os.path.join(object_prefix, local_path)
-                self.__s3.upload_file(local_path, self.__output_bucket, s3_key, access_key=self.__output_bucket_access_key, secret_access_key=self.__output_bucket_secret_access_key)
+                self.__s3.upload_file(
+                    file_name=local_path,
+                    bucket_name=self.__output_bucket,
+                    key=s3_key,
+                    access_key_id=self.__output_bucket_access_key,
+                    secret_access_key=self.__output_bucket_secret_access_key
+                )
 
     ############################################################################
     def execute(self, message):
+        # SNS Variables passed in
         ship_name = message['ship_name']
         cruise_name = message['cruise_name']
         sensor_name = message['sensor_name']
         input_file_name = message['input_file_name']
         #
         store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
         output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{store_name}/"
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,27 @@
                 aws_secret_access_key=secret_access_key
             )
         else:
             client = boto3.Session().client('s3')
         return client
 
     #####################################################################
-    def list_objects(  # analog to find_children_objects
+    def list_objects(  # analog to "find_children_objects"
         self,
         bucket_name,
         prefix,
-        access_key_id=None,
-        secret_access_key=None
+        access_key_id,
+        secret_access_key
     ):
         keys = []
-        for page in self.__get_client(access_key_id, secret_access_key).get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
+        for page in self.__get_client(
+                access_key_id,
+                secret_access_key
+        ).get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
+            # problem here
             contents = page["Contents"]
             if 'Contents' in page.keys():
                 keys.extend(page['Contents'])
         return keys
 
     #####################################################################
     def get_s3_files(self):
@@ -47,14 +51,15 @@
         self.__get_client(
             access_key_id,
             secret_access_key
         ).download_file(Bucket=bucket_name, Key=key, Filename=file_name)
 
     #####################################################################
     def __chunked(
+            self,
             ll: list,
             n: int
     ) -> Generator:
         """Yields successively n-sized chunks from ll.
 
         Parameters
         ----------
@@ -93,15 +98,15 @@
         secret_access_key: str = None,
     ):
         # deletes all given keys in s3 bucket
         objects_to_delete = []
         for raw_zarr_file in raw_zarr_files:
             objects_to_delete.append({'Key': raw_zarr_file['Key']})
         # Delete in groups of 100 — Boto3 constraint
-        for batch in self.__chunked(objects_to_delete, 100):
+        for batch in self.__chunked(ll=objects_to_delete, n=100):
             deleted = self.__get_client(access_key_id, secret_access_key).delete_objects(
                 Bucket=output_bucket,
                 Delete={
                     "Objects": batch
                 }
             )
             print(f"Deleted {len(deleted['Deleted'])} files")
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230706230354
+Version: 1.0.0.dev20230707184722
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230707184722/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*


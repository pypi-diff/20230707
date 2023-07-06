# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255.tar", last modified: Thu Jul  6 22:13:52 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354.tar", last modified: Thu Jul  6 23:04:57 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:13:52.536342 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 22:12:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 22:13:52.536342 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-06 22:12:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 22:13:52.536342 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-06 22:13:48.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:13:52.532343 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:13:52.536342 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:12:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-06 22:12:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15217 2023-07-06 22:12:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-06 22:12:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     4471 2023-07-06 22:12:50.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:13:52.536342 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 22:13:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-06 22:13:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 22:13:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-06 22:13:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-06 22:13:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-06 23:04:53.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:04:57.898265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15206 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-07-06 23:03:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:04:57.902265 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-06 23:04:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230706221255
+Version: 1.0.0.dev20230706230354
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230706221255",
+  version="1.0.0.dev20230706230354",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import os
 import glob
 import shutil
 import echopype as ep
-import boto3
-import botocore
 import numpy as np
 import pandas as pd
 import geopandas
 from datetime import datetime
-from botocore.config import Config
-from botocore.exceptions import ClientError
 
 TEMPDIR = "/tmp"
 
 
 class LambdaExecutor:
 
     ############################################################################
@@ -270,32 +266,29 @@
         print('Compute volume backscattering strength (Sv) from raw data.')
         ds_sv = ep.calibrate.compute_Sv(echodata)
         frequencies = echodata.environment.frequency_nominal.values
         #################################################################
         # Get GPS coordinates
         gps_data, lat, lon = self.__get_gps_data(echodata=echodata)
         #################################################################
+        # Technically the min_echo_range would be 0 m.
         min_echo_range = np.min(np.diff(ds_sv.echo_range.values))  # TODO: change to min_depth_diff
         max_echo_range = float(np.nanmax(ds_sv.echo_range))
         #
         num_ping_time_dropna = lat[~np.isnan(lat)].shape[0]  # symmetric to lon
         #
         start_time = np.datetime_as_string(ds_sv.ping_time.values[0], unit='ms') + "Z"
         end_time = np.datetime_as_string(ds_sv.ping_time.values[-1], unit='ms') + "Z"
         channels = list(ds_sv.channel.values)
         #
         #################################################################
         # Create the zarr store
         ds_sv.to_zarr(store=store_name)
         #################################################################
         print('Note: Adding GeoJSON inside Zarr store')
-        print(f"store_name: {store_name}")
-        print(type(store_name))
-        print(type(gps_data))
-        print(gps_data)
         self.__write_geojson_to_file(store_name=store_name, data=gps_data)
         #################################################################
         self.__zarr_info_to_table(
             cruise_name=cruise_name,
             file_name=raw_file_name,
             zarr_path=output_zarr_prefix,
             min_echo_range=min_echo_range,
@@ -310,21 +303,25 @@
     ############################################################################
     # TODO: I am thinking that that this won't delete everything? Needs batches -rk
     def __remove_existing_s3_objects(
         self,
         output_zarr_prefix
     ):
         for key in self.__s3.list_objects(
-                self,
-                self.__output_bucket,
-                output_zarr_prefix,
-                access_key=self.__output_bucket_access_key,
+                bucket_name=self.__output_bucket,
+                prefix=output_zarr_prefix,
+                access_key_id=self.__output_bucket_access_key,
                 secret_access_key=self.__output_bucket_secret_access_key
         ):
-            self.__s3.delete(self.__output_bucket, key, access_key=None, secret_access_key=None)
+            self.__s3.delete(
+                bucket_name=self.__output_bucket,
+                key=key,
+                access_key_id=self.__output_bucket_access_key,
+                secret_access_key=self.__output_bucket_secret_access_key
+            )
 
     ############################################################################
     def __upload_files(
         self,
         local_directory,
         object_prefix
     ):
@@ -347,25 +344,27 @@
         bucket_key = f"data/raw/{ship_name}/{cruise_name}/{sensor_name}/{input_file_name}"
         print(bucket_key)
         #
         # TODO: get processing status here and handle for idempotency
         # print(f"Processing: {input_file_name} for {cruise_name}")
         # processing_status = self.__get_processing_status(input_file_name, cruise_name)
         #
-        os.chdir(TEMPDIR)  # TODO: PUT BACK
+        os.chdir(TEMPDIR)
         print(os.getcwd())
         #
         self.__set_processing_status(
             ship_name=ship_name,
             cruise_name=cruise_name,
             sensor_name=sensor_name,
             file_name=input_file_name,
             new_status="PROCESSING"
         )
-        self.__delete_all_local_raw_and_zarr_files()  # good
+        #
+        self.__delete_all_local_raw_and_zarr_files()
+        #
         self.__s3.download_file(
             bucket_name=self.__input_bucket,
             key=bucket_key,
             file_name=input_file_name
         )
         print('s3 download file done')
         self.__create_local_zarr_store(
@@ -376,15 +375,15 @@
             store_name=store_name
         )
         print('create local zarr store done')
         # self.__create_local_zarr_store(file_name, cruise_name, sensor_name, output_zarr_prefix, store_name)
         # TODO: needs to (1) find all objects in s3 bucket and then (2) delete those files in batches
         # TODO: (1) needs to search by prefix for all files
         # TODO: (2) needs to search
-        self.__remove_existing_s3_objects(output_zarr_prefix)
+        self.__remove_existing_s3_objects(output_zarr_prefix=output_zarr_prefix)
         print('remove existing s3 objects done')
         self.__upload_files(store_name, output_zarr_prefix)
         print('upload files done')
         self.__update_processing_status(
             cruise_name=cruise_name,
             file_name=input_file_name,
             new_status='SUCCESS'
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,37 +19,17 @@
     def list_objects(  # analog to find_children_objects
         self,
         bucket_name,
         prefix,
         access_key_id=None,
         secret_access_key=None
     ):
-        """Finds all child objects for a given prefix in a s3 bucket.
-
-        Parameters
-        ----------
-        bucket_name : str
-            Name of bucket to read from.
-        prefix : str
-            Prefix path to folder containing children objects.
-        access_key_id : str
-            AWS access key id. Optional.
-        secret_access_key : str
-            AWS access key secret. Optional.
-
-        Returns
-        -------
-        objects : list
-            List of object names as strings.
-        """
         keys = []
         for page in self.__get_client(access_key_id, secret_access_key).get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
             contents = page["Contents"]
-            # for obj in contents:
-            #     keys.append(obj["Key"])
             if 'Contents' in page.keys():
                 keys.extend(page['Contents'])
         return keys
 
     #####################################################################
     def get_s3_files(self):
         # gets a set of files
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230706221255
+Version: 1.0.0.dev20230706230354
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706221255/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706230354/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*


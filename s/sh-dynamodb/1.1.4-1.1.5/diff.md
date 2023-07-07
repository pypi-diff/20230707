# Comparing `tmp/sh-dynamodb-1.1.4.tar.gz` & `tmp/sh-dynamodb-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.1.4.tar", last modified: Thu Jul  6 12:53:24 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.1.5.tar", last modified: Fri Jul  7 06:33:48 2023, max compression
```

## Comparing `sh-dynamodb-1.1.4.tar` & `sh-dynamodb-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:53:24.627689 sh-dynamodb-1.1.4/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.4/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 12:53:24.627350 sh-dynamodb-1.1.4/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.1.4/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 12:53:24.627806 sh-dynamodb-1.1.4/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 12:53:20.000000 sh-dynamodb-1.1.4/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:53:24.622999 sh-dynamodb-1.1.4/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.1.4/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.4/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.4/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5825 2023-07-06 12:52:58.000000 sh-dynamodb-1.1.4/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.4/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:53:24.626586 sh-dynamodb-1.1.4/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.4/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.4/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.4/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:53:24.625506 sh-dynamodb-1.1.4/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 12:53:24.000000 sh-dynamodb-1.1.4/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 12:53:24.000000 sh-dynamodb-1.1.4/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 12:53:24.000000 sh-dynamodb-1.1.4/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 12:53:24.000000 sh-dynamodb-1.1.4/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 12:53:24.000000 sh-dynamodb-1.1.4/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 12:53:24.000000 sh-dynamodb-1.1.4/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:33:48.199836 sh-dynamodb-1.1.5/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.5/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 06:33:48.199357 sh-dynamodb-1.1.5/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.1.5/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 06:33:48.200049 sh-dynamodb-1.1.5/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 06:33:37.000000 sh-dynamodb-1.1.5/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:33:48.192825 sh-dynamodb-1.1.5/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.1.5/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.5/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.5/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5824 2023-07-07 06:33:07.000000 sh-dynamodb-1.1.5/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.5/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:33:48.198277 sh-dynamodb-1.1.5/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.5/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.5/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.5/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:33:48.196497 sh-dynamodb-1.1.5/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 06:33:48.000000 sh-dynamodb-1.1.5/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 06:33:48.000000 sh-dynamodb-1.1.5/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 06:33:48.000000 sh-dynamodb-1.1.5/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 06:33:48.000000 sh-dynamodb-1.1.5/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 06:33:48.000000 sh-dynamodb-1.1.5/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 06:33:48.000000 sh-dynamodb-1.1.5/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.1.4/LICENSE` & `sh-dynamodb-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.4/README.md` & `sh-dynamodb-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.4/setup.py` & `sh-dynamodb-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.1.4",
+    version="1.1.5",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.1.4/sh_dynamodb/__init__.py` & `sh-dynamodb-1.1.5/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.4/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.1.5/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.4/sh_dynamodb/discover.py` & `sh-dynamodb-1.1.5/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.4/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.1.5/sh_dynamodb/dynamodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,27 +49,29 @@
 
 @retry_pattern()
 def setup_aws_client(config):
     """
     Setup the aws session for making the API calls
     """
 
-    # aws_access_key = config['access_key']
-    # aws_secret_access_key = config['access_secret_key']
-    # aws_region_name = config['region_name']
-
-    # session = boto3.Session(
-    #     aws_access_key_id=aws_access_key,
-    #     aws_secret_access_key=aws_secret_access_key,
-    #     region_name=aws_region_name
-    # )
+    aws_access_key = config['access_key']
+    aws_secret_access_key = config['access_secret_key']
+    aws_region_name = config['region_name']
+
+    new_session = boto3.Session(
+        aws_access_key_id=aws_access_key,
+        aws_secret_access_key=aws_secret_access_key,
+        region_name=aws_region_name
+    )
 
     # LOGGER.info("Attempting to access AWS Account")
-    # print("the session is : ", session)
-    # boto3.setup_default_session(botocore_session=session)
+    print("the session is : ", new_session)
+
+    # sesion = Session()
+    # boto3.setup_default_session(session)
 
     if 'role_name' in config:
         role_arn = "arn:aws:iam::{}:role/{}".format(config['account_id'].replace('-', ''),
                                                     config['role_name'])
 
         session = Session()
```

### Comparing `sh-dynamodb-1.1.4/sh_dynamodb/sync.py` & `sh-dynamodb-1.1.5/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.4/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.1.5/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.4/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.1.5/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*


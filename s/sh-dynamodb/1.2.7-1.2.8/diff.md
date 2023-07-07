# Comparing `tmp/sh-dynamodb-1.2.7.tar.gz` & `tmp/sh-dynamodb-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.2.7.tar", last modified: Fri Jul  7 07:32:49 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.2.8.tar", last modified: Fri Jul  7 07:34:23 2023, max compression
```

## Comparing `sh-dynamodb-1.2.7.tar` & `sh-dynamodb-1.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:32:49.896909 sh-dynamodb-1.2.7/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.7/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:32:49.896558 sh-dynamodb-1.2.7/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.2.7/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 07:32:49.897060 sh-dynamodb-1.2.7/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 07:32:40.000000 sh-dynamodb-1.2.7/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:32:49.890833 sh-dynamodb-1.2.7/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.2.7/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.7/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.7/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5962 2023-07-07 07:32:31.000000 sh-dynamodb-1.2.7/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.7/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:32:49.895953 sh-dynamodb-1.2.7/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.7/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.7/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.7/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:32:49.894721 sh-dynamodb-1.2.7/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:32:49.000000 sh-dynamodb-1.2.7/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 07:32:49.000000 sh-dynamodb-1.2.7/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 07:32:49.000000 sh-dynamodb-1.2.7/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 07:32:49.000000 sh-dynamodb-1.2.7/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 07:32:49.000000 sh-dynamodb-1.2.7/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 07:32:49.000000 sh-dynamodb-1.2.7/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:34:23.189812 sh-dynamodb-1.2.8/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.8/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:34:23.189411 sh-dynamodb-1.2.8/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.2.8/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 07:34:23.189987 sh-dynamodb-1.2.8/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 07:34:16.000000 sh-dynamodb-1.2.8/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:34:23.185856 sh-dynamodb-1.2.8/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.2.8/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.8/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.8/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     6060 2023-07-07 07:33:58.000000 sh-dynamodb-1.2.8/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.8/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:34:23.188672 sh-dynamodb-1.2.8/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.8/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.8/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.8/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:34:23.187614 sh-dynamodb-1.2.8/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:34:23.000000 sh-dynamodb-1.2.8/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 07:34:23.000000 sh-dynamodb-1.2.8/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 07:34:23.000000 sh-dynamodb-1.2.8/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 07:34:23.000000 sh-dynamodb-1.2.8/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 07:34:23.000000 sh-dynamodb-1.2.8/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 07:34:23.000000 sh-dynamodb-1.2.8/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.2.7/LICENSE` & `sh-dynamodb-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.7/README.md` & `sh-dynamodb-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.7/setup.py` & `sh-dynamodb-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.2.7",
+    version="1.2.8",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.2.7/sh_dynamodb/__init__.py` & `sh-dynamodb-1.2.8/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.7/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.2.8/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.7/sh_dynamodb/discover.py` & `sh-dynamodb-1.2.8/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.7/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.2.8/sh_dynamodb/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,18 @@
 
 @retry_pattern()
 def setup_aws_client(config):
     """
     Setup the aws session for making the API calls
     """
 
-    if 'role_name' in config:
+    if 'access_key' in config:
+        setup_aws_client_with_access_secret_key(config)
+        
+    elif 'role_name' in config:
         role_arn = "arn:aws:iam::{}:role/{}".format(config['account_id'].replace('-', ''),
                                                     config['role_name'])
 
         session = Session()
 
         print("The session credentials are : " , session.get_credentials() , end="\n")
         print("The access key is : " , session.get_credentials().access_key , end="\n")
```

### Comparing `sh-dynamodb-1.2.7/sh_dynamodb/sync.py` & `sh-dynamodb-1.2.8/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.7/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.2.8/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.7/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.2.8/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*


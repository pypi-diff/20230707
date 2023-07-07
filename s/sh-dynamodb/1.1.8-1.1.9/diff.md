# Comparing `tmp/sh-dynamodb-1.1.8.tar.gz` & `tmp/sh-dynamodb-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.1.8.tar", last modified: Fri Jul  7 06:44:07 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.1.9.tar", last modified: Fri Jul  7 06:46:04 2023, max compression
```

## Comparing `sh-dynamodb-1.1.8.tar` & `sh-dynamodb-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:44:07.368480 sh-dynamodb-1.1.8/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.8/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 06:44:07.368168 sh-dynamodb-1.1.8/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.1.8/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 06:44:07.368607 sh-dynamodb-1.1.8/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 06:43:58.000000 sh-dynamodb-1.1.8/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:44:07.362055 sh-dynamodb-1.1.8/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.1.8/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.8/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.8/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     6105 2023-07-07 06:43:17.000000 sh-dynamodb-1.1.8/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.8/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:44:07.367236 sh-dynamodb-1.1.8/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.8/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.8/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.8/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:44:07.365342 sh-dynamodb-1.1.8/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 06:44:07.000000 sh-dynamodb-1.1.8/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 06:44:07.000000 sh-dynamodb-1.1.8/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 06:44:07.000000 sh-dynamodb-1.1.8/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 06:44:07.000000 sh-dynamodb-1.1.8/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 06:44:07.000000 sh-dynamodb-1.1.8/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 06:44:07.000000 sh-dynamodb-1.1.8/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:46:04.589420 sh-dynamodb-1.1.9/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.9/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 06:46:04.589047 sh-dynamodb-1.1.9/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.1.9/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 06:46:04.589578 sh-dynamodb-1.1.9/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 06:45:55.000000 sh-dynamodb-1.1.9/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:46:04.583522 sh-dynamodb-1.1.9/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.1.9/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.9/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.9/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     6120 2023-07-07 06:45:45.000000 sh-dynamodb-1.1.9/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.9/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:46:04.587971 sh-dynamodb-1.1.9/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.9/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.9/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.9/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 06:46:04.586258 sh-dynamodb-1.1.9/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 06:46:04.000000 sh-dynamodb-1.1.9/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 06:46:04.000000 sh-dynamodb-1.1.9/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 06:46:04.000000 sh-dynamodb-1.1.9/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 06:46:04.000000 sh-dynamodb-1.1.9/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 06:46:04.000000 sh-dynamodb-1.1.9/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 06:46:04.000000 sh-dynamodb-1.1.9/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.1.8/LICENSE` & `sh-dynamodb-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.8/README.md` & `sh-dynamodb-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.8/setup.py` & `sh-dynamodb-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.1.8",
+    version="1.1.9",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.1.8/sh_dynamodb/__init__.py` & `sh-dynamodb-1.1.9/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.8/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.1.9/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.8/sh_dynamodb/discover.py` & `sh-dynamodb-1.1.9/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.8/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.1.9/sh_dynamodb/dynamodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,19 +53,19 @@
     Setup the aws session for making the API calls
     """
 
     aws_access_key = config['access_key']
     aws_secret_access_key = config['access_secret_key']
     aws_region_name = config['region_name']
 
-    new_session = Session(
+    new_session = Session(session_vars={
         aws_access_key_id=aws_access_key,
         aws_secret_access_key=aws_secret_access_key,
         region_name=aws_region_name
-    )
+    })
 
     # LOGGER.info("Attempting to access AWS Account")
     # print("the session is : ", new_session , end="\n")
     # print("access key is : ", new_session.get_credentials().access_key , end="\n")
     # print("the session is : ", new_session.get_credentials().secret_key , end="\n")
     LOGGER.info("Attempting to access aws resources")
     boto3.setup_default_session(botocore_session=new_session)
```

### Comparing `sh-dynamodb-1.1.8/sh_dynamodb/sync.py` & `sh-dynamodb-1.1.9/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.8/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.1.9/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.8/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.1.9/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*


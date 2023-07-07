# Comparing `tmp/sh-dynamodb-1.2.9.tar.gz` & `tmp/sh-dynamodb-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.2.9.tar", last modified: Fri Jul  7 07:38:45 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.3.0.tar", last modified: Fri Jul  7 07:39:55 2023, max compression
```

## Comparing `sh-dynamodb-1.2.9.tar` & `sh-dynamodb-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:38:45.951420 sh-dynamodb-1.2.9/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.9/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:38:45.951083 sh-dynamodb-1.2.9/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.2.9/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 07:38:45.951529 sh-dynamodb-1.2.9/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 07:38:36.000000 sh-dynamodb-1.2.9/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:38:45.946230 sh-dynamodb-1.2.9/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.2.9/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.9/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.9/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     6086 2023-07-07 07:37:34.000000 sh-dynamodb-1.2.9/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.9/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:38:45.950347 sh-dynamodb-1.2.9/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.9/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.9/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.9/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:38:45.948786 sh-dynamodb-1.2.9/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:38:45.000000 sh-dynamodb-1.2.9/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 07:38:45.000000 sh-dynamodb-1.2.9/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 07:38:45.000000 sh-dynamodb-1.2.9/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 07:38:45.000000 sh-dynamodb-1.2.9/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 07:38:45.000000 sh-dynamodb-1.2.9/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 07:38:45.000000 sh-dynamodb-1.2.9/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:39:55.281536 sh-dynamodb-1.3.0/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.0/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:39:55.281217 sh-dynamodb-1.3.0/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.3.0/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 07:39:55.281672 sh-dynamodb-1.3.0/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 07:39:50.000000 sh-dynamodb-1.3.0/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:39:55.276808 sh-dynamodb-1.3.0/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.3.0/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.0/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.0/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     6086 2023-07-07 07:39:36.000000 sh-dynamodb-1.3.0/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.0/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:39:55.280364 sh-dynamodb-1.3.0/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.0/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.0/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.0/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:39:55.279008 sh-dynamodb-1.3.0/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:39:55.000000 sh-dynamodb-1.3.0/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 07:39:55.000000 sh-dynamodb-1.3.0/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 07:39:55.000000 sh-dynamodb-1.3.0/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 07:39:55.000000 sh-dynamodb-1.3.0/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 07:39:55.000000 sh-dynamodb-1.3.0/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 07:39:55.000000 sh-dynamodb-1.3.0/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.2.9/LICENSE` & `sh-dynamodb-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.9/README.md` & `sh-dynamodb-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.9/setup.py` & `sh-dynamodb-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.2.9",
+    version="1.3.0",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.2.9/sh_dynamodb/__init__.py` & `sh-dynamodb-1.3.0/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.9/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.3.0/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.9/sh_dynamodb/discover.py` & `sh-dynamodb-1.3.0/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.9/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.3.0/sh_dynamodb/dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 def setup_aws_client_with_access_secret_key(config):
     """
     Args : config containing aws access key , access secret key and region name 
     """
 
     aws_access_key = config['access_key']
-    aws_access_secret_key = config['access_secret_key']
+    aws_access_secret_key = config['secret_access_key']
     aws_region_name = config['region_name']
 
     session = boto3.Session(
         aws_access_key_id=aws_access_key,
         aws_secret_access_key=aws_access_secret_key,
         region_name=aws_region_name
     )
```

### Comparing `sh-dynamodb-1.2.9/sh_dynamodb/sync.py` & `sh-dynamodb-1.3.0/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.9/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.3.0/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.9/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.3.0/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*


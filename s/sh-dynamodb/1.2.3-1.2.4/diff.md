# Comparing `tmp/sh-dynamodb-1.2.3.tar.gz` & `tmp/sh-dynamodb-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.2.3.tar", last modified: Fri Jul  7 07:08:32 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.2.4.tar", last modified: Fri Jul  7 07:10:01 2023, max compression
```

## Comparing `sh-dynamodb-1.2.3.tar` & `sh-dynamodb-1.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:08:32.313573 sh-dynamodb-1.2.3/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.3/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:08:32.313248 sh-dynamodb-1.2.3/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.2.3/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 07:08:32.313707 sh-dynamodb-1.2.3/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 07:08:24.000000 sh-dynamodb-1.2.3/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:08:32.307424 sh-dynamodb-1.2.3/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.2.3/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.3/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.3/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5894 2023-07-07 07:05:22.000000 sh-dynamodb-1.2.3/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.3/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:08:32.312274 sh-dynamodb-1.2.3/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.3/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.3/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.3/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:08:32.310362 sh-dynamodb-1.2.3/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:08:32.000000 sh-dynamodb-1.2.3/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 07:08:32.000000 sh-dynamodb-1.2.3/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 07:08:32.000000 sh-dynamodb-1.2.3/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 07:08:32.000000 sh-dynamodb-1.2.3/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 07:08:32.000000 sh-dynamodb-1.2.3/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 07:08:32.000000 sh-dynamodb-1.2.3/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:10:01.369161 sh-dynamodb-1.2.4/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.4/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:10:01.368884 sh-dynamodb-1.2.4/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.2.4/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 07:10:01.369276 sh-dynamodb-1.2.4/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 07:09:53.000000 sh-dynamodb-1.2.4/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:10:01.363097 sh-dynamodb-1.2.4/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.2.4/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.4/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.4/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5868 2023-07-07 07:09:24.000000 sh-dynamodb-1.2.4/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.4/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:10:01.368106 sh-dynamodb-1.2.4/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.2.4/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.4/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.2.4/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 07:10:01.366956 sh-dynamodb-1.2.4/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 07:10:01.000000 sh-dynamodb-1.2.4/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 07:10:01.000000 sh-dynamodb-1.2.4/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 07:10:01.000000 sh-dynamodb-1.2.4/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 07:10:01.000000 sh-dynamodb-1.2.4/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 07:10:01.000000 sh-dynamodb-1.2.4/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 07:10:01.000000 sh-dynamodb-1.2.4/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.2.3/LICENSE` & `sh-dynamodb-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.3/README.md` & `sh-dynamodb-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.3/setup.py` & `sh-dynamodb-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.2.3",
+    version="1.2.4",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.2.3/sh_dynamodb/__init__.py` & `sh-dynamodb-1.2.4/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.3/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.2.4/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.3/sh_dynamodb/discover.py` & `sh-dynamodb-1.2.4/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.3/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.2.4/sh_dynamodb/dynamodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     session = boto3.Session(
         aws_access_key_id=aws_access_key,
         aws_secret_access_key=aws_access_secret_key,
         region_name=aws_region_name
     )
 
-    botocore_session = Session(botocore_session=session._session)
+    botocore_session = session._session
     
     print("Attempting to access aws resource")
     boto3.setup_default_session(botocore_session=botocore_session)
 
     # if 'role_name' in config:
     #     role_arn = "arn:aws:iam::{}:role/{}".format(config['account_id'].replace('-', ''),
     #                                                 config['role_name'])
```

### Comparing `sh-dynamodb-1.2.3/sh_dynamodb/sync.py` & `sh-dynamodb-1.2.4/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.3/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.2.4/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.2.3/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.2.4/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*


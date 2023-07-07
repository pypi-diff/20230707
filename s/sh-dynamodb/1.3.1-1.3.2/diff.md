# Comparing `tmp/sh-dynamodb-1.3.1.tar.gz` & `tmp/sh-dynamodb-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.3.1.tar", last modified: Fri Jul  7 08:30:21 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.3.2.tar", last modified: Fri Jul  7 08:33:12 2023, max compression
```

## Comparing `sh-dynamodb-1.3.1.tar` & `sh-dynamodb-1.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:30:21.707034 sh-dynamodb-1.3.1/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.1/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 08:30:21.706701 sh-dynamodb-1.3.1/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.3.1/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 08:30:21.707175 sh-dynamodb-1.3.1/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 08:30:15.000000 sh-dynamodb-1.3.1/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:30:21.700885 sh-dynamodb-1.3.1/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.3.1/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.1/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.1/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5985 2023-07-07 08:29:04.000000 sh-dynamodb-1.3.1/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.1/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:30:21.705582 sh-dynamodb-1.3.1/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.1/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.1/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.1/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:30:21.703617 sh-dynamodb-1.3.1/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 08:30:21.000000 sh-dynamodb-1.3.1/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 08:30:21.000000 sh-dynamodb-1.3.1/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 08:30:21.000000 sh-dynamodb-1.3.1/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 08:30:21.000000 sh-dynamodb-1.3.1/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 08:30:21.000000 sh-dynamodb-1.3.1/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 08:30:21.000000 sh-dynamodb-1.3.1/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:33:12.374046 sh-dynamodb-1.3.2/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.2/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 08:33:12.373622 sh-dynamodb-1.3.2/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.3.2/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 08:33:12.374194 sh-dynamodb-1.3.2/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 08:33:02.000000 sh-dynamodb-1.3.2/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:33:12.367747 sh-dynamodb-1.3.2/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.3.2/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5444 2023-07-07 08:32:55.000000 sh-dynamodb-1.3.2/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:33:12.372417 sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:33:12.370685 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.3.1/LICENSE` & `sh-dynamodb-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.1/README.md` & `sh-dynamodb-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.1/setup.py` & `sh-dynamodb-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.3.1",
+    version="1.3.2",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.3.1/sh_dynamodb/__init__.py` & `sh-dynamodb-1.3.2/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.1/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.3.2/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.1/sh_dynamodb/discover.py` & `sh-dynamodb-1.3.2/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.1/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.3.2/sh_dynamodb/dynamodb.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def load(self):
         return DeferredRefreshableCredentials(
             self._fetcher.fetch_credentials,
             self.METHOD
         )
 
-def setup_aws_client_with_access_secret_key(config):
+def setup_aws_client_with_access_and_secret_key(config):
     """
     Args : config
     """
 
     aws_access_key = config['access_key']
     aws_access_secret_key = config['secret_access_key']
     aws_region_name = config['region_name']
@@ -67,25 +67,21 @@
 @retry_pattern()
 def setup_aws_client(config):
     """
     Setup the aws session for making the API calls
     """
 
     if 'access_key' in config and 'secret_access_key' in config:
-        setup_aws_client_with_access_secret_key(config)
-
+        setup_aws_client_with_access_and_secret_key(config)
     elif 'role_name' in config:
         role_arn = "arn:aws:iam::{}:role/{}".format(config['account_id'].replace('-', ''),
                                                     config['role_name'])
 
         session = Session()
 
-        print("The session credentials are : " , session.get_credentials() , end="\n")
-        print("The access key is : " , session.get_credentials().access_key , end="\n")
-        print("The secret key is : " , session.get_credentials().secret_key , end="\n")
         fetcher = AssumeRoleCredentialFetcher(
             session.create_client,
             session.get_credentials(),
             role_arn,
             extra_args={
                 'DurationSeconds': 3600,
                 'RoleSessionName': 'TapDynamodDB',
@@ -96,17 +92,14 @@
 
         refreshable_session = Session()
         refreshable_session.register_component(
             'credential_provider',
             CredentialResolver([AssumeRoleProvider(fetcher)])
         )
 
-        print("Credentials are : ", refreshable_session.get_credentials(), end="\n")
-        print("The access key is : " , refreshable_session.get_credentials().access_key , end="\n")
-        print("The secret key is : " , refreshable_session.get_credentials().secret_key , end="\n")
         LOGGER.info("Attempting to assume_role on RoleArn: %s", role_arn)
         boto3.setup_default_session(botocore_session=refreshable_session)
 
 def get_request_timeout(config):
     # if request_timeout is other than 0,"0" or "" then use request_timeout
     request_timeout = config.get('request_timeout')
     if request_timeout and float(request_timeout):
```

### Comparing `sh-dynamodb-1.3.1/sh_dynamodb/sync.py` & `sh-dynamodb-1.3.2/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.1/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.1/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*


# Comparing `tmp/sh-dynamodb-1.3.2.tar.gz` & `tmp/sh-dynamodb-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.3.2.tar", last modified: Fri Jul  7 08:33:12 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.3.3.tar", last modified: Fri Jul  7 09:00:24 2023, max compression
```

## Comparing `sh-dynamodb-1.3.2.tar` & `sh-dynamodb-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:33:12.374046 sh-dynamodb-1.3.2/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.2/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 08:33:12.373622 sh-dynamodb-1.3.2/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.3.2/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 08:33:12.374194 sh-dynamodb-1.3.2/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 08:33:02.000000 sh-dynamodb-1.3.2/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:33:12.367747 sh-dynamodb-1.3.2/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.3.2/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5444 2023-07-07 08:32:55.000000 sh-dynamodb-1.3.2/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:33:12.372417 sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 08:33:12.370685 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 08:33:12.000000 sh-dynamodb-1.3.2/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 09:00:24.410313 sh-dynamodb-1.3.3/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.3/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 09:00:24.410019 sh-dynamodb-1.3.3/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.3.3/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-07 09:00:24.410449 sh-dynamodb-1.3.3/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-07 08:59:30.000000 sh-dynamodb-1.3.3/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 09:00:24.405831 sh-dynamodb-1.3.3/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-07 08:59:17.000000 sh-dynamodb-1.3.3/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.3/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.3/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5444 2023-07-07 08:32:55.000000 sh-dynamodb-1.3.3/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.3/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 09:00:24.409491 sh-dynamodb-1.3.3/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.3.3/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4837 2023-07-07 08:58:54.000000 sh-dynamodb-1.3.3/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.3.3/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-07 09:00:24.408365 sh-dynamodb-1.3.3/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-07 09:00:24.000000 sh-dynamodb-1.3.3/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-07 09:00:24.000000 sh-dynamodb-1.3.3/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-07 09:00:24.000000 sh-dynamodb-1.3.3/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-07 09:00:24.000000 sh-dynamodb-1.3.3/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-07 09:00:24.000000 sh-dynamodb-1.3.3/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-07 09:00:24.000000 sh-dynamodb-1.3.3/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.3.2/LICENSE` & `sh-dynamodb-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.2/README.md` & `sh-dynamodb-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.2/setup.py` & `sh-dynamodb-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.3.2",
+    version="1.3.3",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.3.2/sh_dynamodb/__init__.py` & `sh-dynamodb-1.3.3/sh_dynamodb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,16 +91,14 @@
 
 
 @singer.utils.handle_top_exception(LOGGER)
 def main():
     args = singer.utils.parse_args(REQUIRED_CONFIG_KEYS)
     config = args.config
 
-    print("The config used for authenticating to AWS is : ", config)
-
     # TODO Is this the right way to do this? It seems bad
     if not config.get('use_local_dynamo'):
         setup_aws_client(config)
 
     if args.discover:
         do_discover(args.config)
     elif args.catalog:
```

### Comparing `sh-dynamodb-1.3.2/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.3.3/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.2/sh_dynamodb/discover.py` & `sh-dynamodb-1.3.3/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.2/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.3.3/sh_dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.2/sh_dynamodb/sync.py` & `sh-dynamodb-1.3.3/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.3.3/sh_dynamodb/sync_strategies/full_table.py`

 * *Files 14% similar despite different names*

```diff
@@ -78,21 +78,19 @@
 
     last_evaluated_key = singer.get_bookmark(state,
                                              table_name,
                                              'last_evaluated_key')
 
     md_map = metadata.to_map(stream['metadata'])
     projection = metadata.get(md_map, (), 'tap-mongodb.projection')
-    print(f"printing projection : {projection}")
 
     # An expression attribute name is a placeholder that one uses in an Amazon DynamoDB expression as an alternative to an actual attribute name.
     # Sometimes it might need to write an expression containing an attribute name that conflicts with a DynamoDB reserved word.
     # For example, table `A` contains the field `Comment` but `Comment` is a reserved word. So, it fails during fetch.
     expression = metadata.get(md_map, (), 'sh-dynamodb.expression-attributes')
-    print(f"printing expression : {expression}")
 
     rows_saved = 0
 
     deserializer = Deserializer()
     for result in scan_table(table_name, projection, expression, last_evaluated_key, config):
         for item in result.get('Items', []):
             rows_saved += 1
```

### Comparing `sh-dynamodb-1.3.2/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.3.3/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*


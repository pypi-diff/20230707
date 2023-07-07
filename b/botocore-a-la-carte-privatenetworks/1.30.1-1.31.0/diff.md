# Comparing `tmp/botocore-a-la-carte-privatenetworks-1.30.1.tar.gz` & `tmp/botocore-a-la-carte-privatenetworks-1.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-privatenetworks-1.30.1.tar", last modified: Thu Jul  6 01:45:21 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-privatenetworks-1.31.0.tar", last modified: Fri Jul  7 01:44:13 2023, max compression
```

## Comparing `botocore-a-la-carte-privatenetworks-1.30.1.tar` & `botocore-a-la-carte-privatenetworks-1.31.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:21.191057 botocore-a-la-carte-privatenetworks-1.30.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:45:20.000000 botocore-a-la-carte-privatenetworks-1.30.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 01:45:21.187057 botocore-a-la-carte-privatenetworks-1.30.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:21.187057 botocore-a-la-carte-privatenetworks-1.30.1/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:21.187057 botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:21.187057 botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/privatenetworks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:21.187057 botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/privatenetworks/2021-12-03/
--rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-06 01:44:40.000000 botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/privatenetworks/2021-12-03/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-06 01:44:40.000000 botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/privatenetworks/2021-12-03/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    76726 2023-07-06 01:44:40.000000 botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/privatenetworks/2021-12-03/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:21.187057 botocore-a-la-carte-privatenetworks-1.30.1/botocore_a_la_carte_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 01:45:21.000000 botocore-a-la-carte-privatenetworks-1.30.1/botocore_a_la_carte_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 01:45:21.000000 botocore-a-la-carte-privatenetworks-1.30.1/botocore_a_la_carte_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:45:21.000000 botocore-a-la-carte-privatenetworks-1.30.1/botocore_a_la_carte_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:45:21.000000 botocore-a-la-carte-privatenetworks-1.30.1/botocore_a_la_carte_privatenetworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:45:21.191057 botocore-a-la-carte-privatenetworks-1.30.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-06 01:45:20.000000 botocore-a-la-carte-privatenetworks-1.30.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:13.379580 botocore-a-la-carte-privatenetworks-1.31.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-07 01:44:13.000000 botocore-a-la-carte-privatenetworks-1.31.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-07 01:44:13.379580 botocore-a-la-carte-privatenetworks-1.31.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:13.379580 botocore-a-la-carte-privatenetworks-1.31.0/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:13.379580 botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:13.379580 botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/privatenetworks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:13.379580 botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/privatenetworks/2021-12-03/
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-07 01:43:28.000000 botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/privatenetworks/2021-12-03/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-07 01:43:28.000000 botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/privatenetworks/2021-12-03/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    76726 2023-07-07 01:43:28.000000 botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/privatenetworks/2021-12-03/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:44:13.379580 botocore-a-la-carte-privatenetworks-1.31.0/botocore_a_la_carte_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-07 01:44:13.000000 botocore-a-la-carte-privatenetworks-1.31.0/botocore_a_la_carte_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-07 01:44:13.000000 botocore-a-la-carte-privatenetworks-1.31.0/botocore_a_la_carte_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:44:13.000000 botocore-a-la-carte-privatenetworks-1.31.0/botocore_a_la_carte_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 01:44:13.000000 botocore-a-la-carte-privatenetworks-1.31.0/botocore_a_la_carte_privatenetworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:44:13.379580 botocore-a-la-carte-privatenetworks-1.31.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-07 01:44:13.000000 botocore-a-la-carte-privatenetworks-1.31.0/setup.py
```

### Comparing `botocore-a-la-carte-privatenetworks-1.30.1/LICENSE.txt` & `botocore-a-la-carte-privatenetworks-1.31.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-privatenetworks-1.30.1/PKG-INFO` & `botocore-a-la-carte-privatenetworks-1.31.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-privatenetworks
-Version: 1.30.1
+Version: 1.31.0
 Summary: privatenetworks data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/privatenetworks/2021-12-03/endpoint-rule-set-1.json` & `botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/privatenetworks/2021-12-03/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/privatenetworks/2021-12-03/paginators-1.json` & `botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/privatenetworks/2021-12-03/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-privatenetworks-1.30.1/botocore/data/privatenetworks/2021-12-03/service-2.json` & `botocore-a-la-carte-privatenetworks-1.31.0/botocore/data/privatenetworks/2021-12-03/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-privatenetworks-1.30.1/botocore_a_la_carte_privatenetworks.egg-info/PKG-INFO` & `botocore-a-la-carte-privatenetworks-1.31.0/botocore_a_la_carte_privatenetworks.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-privatenetworks
-Version: 1.30.1
+Version: 1.31.0
 Summary: privatenetworks data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-privatenetworks-1.30.1/setup.py` & `botocore-a-la-carte-privatenetworks-1.31.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-privatenetworks',
-    version="1.30.1",
+    version="1.31.0",
     description='privatenetworks data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/privatenetworks/*/*.json'],
```


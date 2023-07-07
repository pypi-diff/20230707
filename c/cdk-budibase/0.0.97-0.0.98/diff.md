# Comparing `tmp/cdk-budibase-0.0.97.tar.gz` & `tmp/cdk-budibase-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-budibase-0.0.97.tar", last modified: Thu Jul  6 00:21:15 2023, max compression
+gzip compressed data, was "cdk-budibase-0.0.98.tar", last modified: Fri Jul  7 00:22:04 2023, max compression
```

## Comparing `cdk-budibase-0.0.97.tar` & `cdk-budibase-0.0.98.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:21:15.241569 cdk-budibase-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-06 00:21:15.241569 cdk-budibase-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 00:21:15.241569 cdk-budibase-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:21:15.237569 cdk-budibase-0.0.97/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:21:15.237569 cdk-budibase-0.0.97/src/cdk_budibase/
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/src/cdk_budibase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:21:15.241569 cdk-budibase-0.0.97/src/cdk_budibase/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/src/cdk_budibase/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   486674 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/src/cdk_budibase/_jsii/cdk-budibase@0.0.97.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:21:02.000000 cdk-budibase-0.0.97/src/cdk_budibase/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:21:15.241569 cdk-budibase-0.0.97/src/cdk_budibase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-06 00:21:15.000000 cdk-budibase-0.0.97/src/cdk_budibase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-06 00:21:15.000000 cdk-budibase-0.0.97/src/cdk_budibase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:21:15.000000 cdk-budibase-0.0.97/src/cdk_budibase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 00:21:15.000000 cdk-budibase-0.0.97/src/cdk_budibase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 00:21:15.000000 cdk-budibase-0.0.97/src/cdk_budibase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:22:04.105898 cdk-budibase-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-07 00:22:04.105898 cdk-budibase-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 00:22:04.105898 cdk-budibase-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:22:04.105898 cdk-budibase-0.0.98/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:22:04.105898 cdk-budibase-0.0.98/src/cdk_budibase/
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/src/cdk_budibase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:22:04.105898 cdk-budibase-0.0.98/src/cdk_budibase/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/src/cdk_budibase/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   486675 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/src/cdk_budibase/_jsii/cdk-budibase@0.0.98.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:21:51.000000 cdk-budibase-0.0.98/src/cdk_budibase/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 00:22:04.105898 cdk-budibase-0.0.98/src/cdk_budibase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-07 00:22:04.000000 cdk-budibase-0.0.98/src/cdk_budibase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-07 00:22:04.000000 cdk-budibase-0.0.98/src/cdk_budibase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 00:22:04.000000 cdk-budibase-0.0.98/src/cdk_budibase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 00:22:04.000000 cdk-budibase-0.0.98/src/cdk_budibase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 00:22:04.000000 cdk-budibase-0.0.98/src/cdk_budibase.egg-info/top_level.txt
```

### Comparing `cdk-budibase-0.0.97/LICENSE` & `cdk-budibase-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-budibase-0.0.97/PKG-INFO` & `cdk-budibase-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-budibase
-Version: 0.0.97
+Version: 0.0.98
 Summary: Use AWS CDK to create budibase server
 Home-page: https://github.com/neilkuan/cdk-budibase.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-budibase.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-budibase-0.0.97/README.md` & `cdk-budibase-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `cdk-budibase-0.0.97/setup.py` & `cdk-budibase-0.0.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-budibase",
-    "version": "0.0.97",
+    "version": "0.0.98",
     "description": "Use AWS CDK to create budibase server",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-budibase.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_budibase",
         "cdk_budibase._jsii"
     ],
     "package_data": {
         "cdk_budibase._jsii": [
-            "cdk-budibase@0.0.97.jsii.tgz"
+            "cdk-budibase@0.0.98.jsii.tgz"
         ],
         "cdk_budibase": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-budibase-0.0.97/src/cdk_budibase/__init__.py` & `cdk-budibase-0.0.98/src/cdk_budibase/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-budibase-0.0.97/src/cdk_budibase.egg-info/PKG-INFO` & `cdk-budibase-0.0.98/src/cdk_budibase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-budibase
-Version: 0.0.97
+Version: 0.0.98
 Summary: Use AWS CDK to create budibase server
 Home-page: https://github.com/neilkuan/cdk-budibase.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-budibase.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


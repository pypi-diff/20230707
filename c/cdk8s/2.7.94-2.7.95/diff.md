# Comparing `tmp/cdk8s-2.7.94.tar.gz` & `tmp/cdk8s-2.7.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-2.7.94.tar", last modified: Wed Jul  5 00:25:09 2023, max compression
+gzip compressed data, was "cdk8s-2.7.95.tar", last modified: Thu Jul  6 00:23:39 2023, max compression
```

## Comparing `cdk8s-2.7.94.tar` & `cdk8s-2.7.95.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:09.480872 cdk8s-2.7.94/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-05 00:24:57.000000 cdk8s-2.7.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 00:24:57.000000 cdk8s-2.7.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 00:24:57.000000 cdk8s-2.7.94/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-05 00:25:09.480872 cdk8s-2.7.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-05 00:24:57.000000 cdk8s-2.7.94/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 00:24:57.000000 cdk8s-2.7.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:25:09.480872 cdk8s-2.7.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-05 00:24:57.000000 cdk8s-2.7.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:09.476872 cdk8s-2.7.94/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:09.476872 cdk8s-2.7.94/src/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   138472 2023-07-05 00:24:57.000000 cdk8s-2.7.94/src/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:09.476872 cdk8s-2.7.94/src/cdk8s/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-05 00:24:57.000000 cdk8s-2.7.94/src/cdk8s/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   298138 2023-07-05 00:24:57.000000 cdk8s-2.7.94/src/cdk8s/_jsii/cdk8s@2.7.94.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:24:57.000000 cdk8s-2.7.94/src/cdk8s/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:09.476872 cdk8s-2.7.94/src/cdk8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-05 00:25:09.000000 cdk8s-2.7.94/src/cdk8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-05 00:25:09.000000 cdk8s-2.7.94/src/cdk8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:25:09.000000 cdk8s-2.7.94/src/cdk8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 00:25:09.000000 cdk8s-2.7.94/src/cdk8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 00:25:09.000000 cdk8s-2.7.94/src/cdk8s.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:23:39.738067 cdk8s-2.7.95/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 00:23:27.000000 cdk8s-2.7.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 00:23:27.000000 cdk8s-2.7.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 00:23:27.000000 cdk8s-2.7.95/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-06 00:23:39.738067 cdk8s-2.7.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-06 00:23:27.000000 cdk8s-2.7.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 00:23:27.000000 cdk8s-2.7.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 00:23:39.738067 cdk8s-2.7.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-06 00:23:27.000000 cdk8s-2.7.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:23:39.734067 cdk8s-2.7.95/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:23:39.734067 cdk8s-2.7.95/src/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   138472 2023-07-06 00:23:27.000000 cdk8s-2.7.95/src/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:23:39.738067 cdk8s-2.7.95/src/cdk8s/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-06 00:23:27.000000 cdk8s-2.7.95/src/cdk8s/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   298141 2023-07-06 00:23:27.000000 cdk8s-2.7.95/src/cdk8s/_jsii/cdk8s@2.7.95.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:23:27.000000 cdk8s-2.7.95/src/cdk8s/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 00:23:39.738067 cdk8s-2.7.95/src/cdk8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-06 00:23:39.000000 cdk8s-2.7.95/src/cdk8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-06 00:23:39.000000 cdk8s-2.7.95/src/cdk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 00:23:39.000000 cdk8s-2.7.95/src/cdk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 00:23:39.000000 cdk8s-2.7.95/src/cdk8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 00:23:39.000000 cdk8s-2.7.95/src/cdk8s.egg-info/top_level.txt
```

### Comparing `cdk8s-2.7.94/LICENSE` & `cdk8s-2.7.95/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.94/PKG-INFO` & `cdk8s-2.7.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s
-Version: 2.7.94
+Version: 2.7.95
 Summary: This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.
 Home-page: https://github.com/cdk8s-team/cdk8s-core.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-core.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-2.7.94/README.md` & `cdk8s-2.7.95/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.94/setup.py` & `cdk8s-2.7.95/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s",
-    "version": "2.7.94",
+    "version": "2.7.95",
     "description": "This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-core.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s",
         "cdk8s._jsii"
     ],
     "package_data": {
         "cdk8s._jsii": [
-            "cdk8s@2.7.94.jsii.tgz"
+            "cdk8s@2.7.95.jsii.tgz"
         ],
         "cdk8s": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-2.7.94/src/cdk8s/__init__.py` & `cdk8s-2.7.95/src/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-2.7.94/src/cdk8s.egg-info/PKG-INFO` & `cdk8s-2.7.95/src/cdk8s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s
-Version: 2.7.94
+Version: 2.7.95
 Summary: This is the core library of Cloud Development Kit (CDK) for Kubernetes (cdk8s). cdk8s apps synthesize into standard Kubernetes manifests which can be applied to any Kubernetes cluster.
 Home-page: https://github.com/cdk8s-team/cdk8s-core.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-core.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


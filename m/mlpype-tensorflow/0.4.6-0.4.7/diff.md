# Comparing `tmp/mlpype-tensorflow-0.4.6.tar.gz` & `tmp/mlpype-tensorflow-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-tensorflow-0.4.6.tar", last modified: Fri Jun 30 14:22:47 2023, max compression
+gzip compressed data, was "mlpype-tensorflow-0.4.7.tar", last modified: Fri Jul  7 12:44:39 2023, max compression
```

## Comparing `mlpype-tensorflow-0.4.6.tar` & `mlpype-tensorflow-0.4.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:47.783506 mlpype-tensorflow-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 14:22:47.779506 mlpype-tensorflow-0.4.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:47.779506 mlpype-tensorflow-0.4.6/mlpype_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 14:22:47.000000 mlpype-tensorflow-0.4.6/mlpype_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-30 14:22:47.000000 mlpype-tensorflow-0.4.6/mlpype_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:47.000000 mlpype-tensorflow-0.4.6/mlpype_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-30 14:22:47.000000 mlpype-tensorflow-0.4.6/mlpype_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:47.000000 mlpype-tensorflow-0.4.6/mlpype_tensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:22:47.783506 mlpype-tensorflow-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-30 14:18:44.000000 mlpype-tensorflow-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:39.717796 mlpype-tensorflow-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 12:44:39.717796 mlpype-tensorflow-0.4.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:39.717796 mlpype-tensorflow-0.4.7/mlpype_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 12:44:39.000000 mlpype-tensorflow-0.4.7/mlpype_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-07 12:44:39.000000 mlpype-tensorflow-0.4.7/mlpype_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:39.000000 mlpype-tensorflow-0.4.7/mlpype_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-07 12:44:39.000000 mlpype-tensorflow-0.4.7/mlpype_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:39.000000 mlpype-tensorflow-0.4.7/mlpype_tensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:44:39.717796 mlpype-tensorflow-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 12:39:43.000000 mlpype-tensorflow-0.4.7/setup.py
```

### Comparing `mlpype-tensorflow-0.4.6/setup.py` & `mlpype-tensorflow-0.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.6"
+    version = "0.4.7"
 
     deps = [
         f"mlpype-base=={version}",
         # on mac, it is recommended to use conda/mamba or source to install tensorflow
         "tensorflow>=2.12",
         "numpy>=1.23.0",
         "protobuf>=3.20.3",
```


# Comparing `tmp/mlpype-mlflow-0.4.6.tar.gz` & `tmp/mlpype-mlflow-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-mlflow-0.4.6.tar", last modified: Fri Jun 30 14:22:24 2023, max compression
+gzip compressed data, was "mlpype-mlflow-0.4.7.tar", last modified: Fri Jul  7 12:44:14 2023, max compression
```

## Comparing `mlpype-mlflow-0.4.6.tar` & `mlpype-mlflow-0.4.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:24.147387 mlpype-mlflow-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 14:22:24.147387 mlpype-mlflow-0.4.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:22:24.147387 mlpype-mlflow-0.4.6/mlpype_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 14:22:24.000000 mlpype-mlflow-0.4.6/mlpype_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-30 14:22:24.000000 mlpype-mlflow-0.4.6/mlpype_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:24.000000 mlpype-mlflow-0.4.6/mlpype_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-30 14:22:24.000000 mlpype-mlflow-0.4.6/mlpype_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:22:24.000000 mlpype-mlflow-0.4.6/mlpype_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:22:24.147387 mlpype-mlflow-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-30 14:18:44.000000 mlpype-mlflow-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:14.172973 mlpype-mlflow-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 12:44:14.172973 mlpype-mlflow-0.4.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:14.172973 mlpype-mlflow-0.4.7/mlpype_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 12:44:14.000000 mlpype-mlflow-0.4.7/mlpype_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-07 12:44:14.000000 mlpype-mlflow-0.4.7/mlpype_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:14.000000 mlpype-mlflow-0.4.7/mlpype_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 12:44:14.000000 mlpype-mlflow-0.4.7/mlpype_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:14.000000 mlpype-mlflow-0.4.7/mlpype_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:44:14.172973 mlpype-mlflow-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-07 12:39:43.000000 mlpype-mlflow-0.4.7/setup.py
```

### Comparing `mlpype-mlflow-0.4.6/setup.py` & `mlpype-mlflow-0.4.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.6"
+    version = "0.4.7"
 
     deps = [
         f"mlpype-base=={version}",
         "mlflow>=1.28.0, <2.0",
         "GitPython>=3.1.27",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
```


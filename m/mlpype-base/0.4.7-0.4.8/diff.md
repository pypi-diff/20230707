# Comparing `tmp/mlpype-base-0.4.7.tar.gz` & `tmp/mlpype-base-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-base-0.4.7.tar", last modified: Fri Jul  7 12:43:48 2023, max compression
+gzip compressed data, was "mlpype-base-0.4.8.tar", last modified: Fri Jul  7 14:00:31 2023, max compression
```

## Comparing `mlpype-base-0.4.7.tar` & `mlpype-base-0.4.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:48.324133 mlpype-base-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 12:43:48.324133 mlpype-base-0.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:48.324133 mlpype-base-0.4.7/mlpype_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 12:43:48.000000 mlpype-base-0.4.7/mlpype_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-07 12:43:48.000000 mlpype-base-0.4.7/mlpype_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:43:48.000000 mlpype-base-0.4.7/mlpype_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-07 12:43:48.000000 mlpype-base-0.4.7/mlpype_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:43:48.000000 mlpype-base-0.4.7/mlpype_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:43:48.324133 mlpype-base-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 12:39:43.000000 mlpype-base-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:31.765473 mlpype-base-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 14:00:31.765473 mlpype-base-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:31.765473 mlpype-base-0.4.8/mlpype_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 14:00:31.000000 mlpype-base-0.4.8/mlpype_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-07 14:00:31.000000 mlpype-base-0.4.8/mlpype_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:00:31.000000 mlpype-base-0.4.8/mlpype_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-07 14:00:31.000000 mlpype-base-0.4.8/mlpype_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:00:31.000000 mlpype-base-0.4.8/mlpype_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:00:31.765473 mlpype-base-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 13:57:33.000000 mlpype-base-0.4.8/setup.py
```

### Comparing `mlpype-base-0.4.7/setup.py` & `mlpype-base-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
     deps = [
         f"mlpype=={version}",
         "docstring_parser>=0.14.1",
         "pydantic>=1.9.1",
```


# Comparing `tmp/mlpype-spark-0.4.7.tar.gz` & `tmp/mlpype-spark-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-spark-0.4.7.tar", last modified: Fri Jul  7 12:44:31 2023, max compression
+gzip compressed data, was "mlpype-spark-0.4.8.tar", last modified: Fri Jul  7 14:01:06 2023, max compression
```

## Comparing `mlpype-spark-0.4.7.tar` & `mlpype-spark-0.4.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:31.113518 mlpype-spark-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 12:44:31.113518 mlpype-spark-0.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:31.113518 mlpype-spark-0.4.7/mlpype_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 12:44:31.000000 mlpype-spark-0.4.7/mlpype_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-07 12:44:31.000000 mlpype-spark-0.4.7/mlpype_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:31.000000 mlpype-spark-0.4.7/mlpype_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-07 12:44:31.000000 mlpype-spark-0.4.7/mlpype_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:31.000000 mlpype-spark-0.4.7/mlpype_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:44:31.113518 mlpype-spark-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 12:39:43.000000 mlpype-spark-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:01:06.581717 mlpype-spark-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 14:01:06.577717 mlpype-spark-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:01:06.577717 mlpype-spark-0.4.8/mlpype_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 14:01:06.000000 mlpype-spark-0.4.8/mlpype_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-07 14:01:06.000000 mlpype-spark-0.4.8/mlpype_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:01:06.000000 mlpype-spark-0.4.8/mlpype_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-07 14:01:06.000000 mlpype-spark-0.4.8/mlpype_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:01:06.000000 mlpype-spark-0.4.8/mlpype_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:01:06.581717 mlpype-spark-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 13:57:33.000000 mlpype-spark-0.4.8/setup.py
```

### Comparing `mlpype-spark-0.4.7/setup.py` & `mlpype-spark-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
 
     deps = [
         f"mlpype-base=={version}",
         # We will provide absolute no guarantees that our integration will work with
         # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
         "pyspark>=3.2.1",
     ]
```


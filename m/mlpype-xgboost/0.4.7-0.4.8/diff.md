# Comparing `tmp/mlpype-xgboost-0.4.7.tar.gz` & `tmp/mlpype-xgboost-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-xgboost-0.4.7.tar", last modified: Fri Jul  7 12:44:48 2023, max compression
+gzip compressed data, was "mlpype-xgboost-0.4.8.tar", last modified: Fri Jul  7 14:01:20 2023, max compression
```

## Comparing `mlpype-xgboost-0.4.7.tar` & `mlpype-xgboost-0.4.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:48.294062 mlpype-xgboost-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 12:44:48.294062 mlpype-xgboost-0.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:48.294062 mlpype-xgboost-0.4.7/mlpype_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 12:44:48.000000 mlpype-xgboost-0.4.7/mlpype_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 12:44:48.000000 mlpype-xgboost-0.4.7/mlpype_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:48.000000 mlpype-xgboost-0.4.7/mlpype_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 12:44:48.000000 mlpype-xgboost-0.4.7/mlpype_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:48.000000 mlpype-xgboost-0.4.7/mlpype_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:44:48.294062 mlpype-xgboost-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-07 12:39:43.000000 mlpype-xgboost-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:01:20.273813 mlpype-xgboost-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 14:01:20.273813 mlpype-xgboost-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:01:20.273813 mlpype-xgboost-0.4.8/mlpype_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 14:01:20.000000 mlpype-xgboost-0.4.8/mlpype_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 14:01:20.000000 mlpype-xgboost-0.4.8/mlpype_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:01:20.000000 mlpype-xgboost-0.4.8/mlpype_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 14:01:20.000000 mlpype-xgboost-0.4.8/mlpype_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:01:20.000000 mlpype-xgboost-0.4.8/mlpype_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:01:20.273813 mlpype-xgboost-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-07 13:57:33.000000 mlpype-xgboost-0.4.8/setup.py
```


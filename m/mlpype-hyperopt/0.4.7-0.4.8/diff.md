# Comparing `tmp/mlpype-hyperopt-0.4.7.tar.gz` & `tmp/mlpype-hyperopt-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-hyperopt-0.4.7.tar", last modified: Fri Jul  7 12:44:05 2023, max compression
+gzip compressed data, was "mlpype-hyperopt-0.4.8.tar", last modified: Fri Jul  7 14:00:45 2023, max compression
```

## Comparing `mlpype-hyperopt-0.4.7.tar` & `mlpype-hyperopt-0.4.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:05.692698 mlpype-hyperopt-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 12:44:05.692698 mlpype-hyperopt-0.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:44:05.692698 mlpype-hyperopt-0.4.7/mlpype_hyperopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 12:44:05.000000 mlpype-hyperopt-0.4.7/mlpype_hyperopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 12:44:05.000000 mlpype-hyperopt-0.4.7/mlpype_hyperopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:05.000000 mlpype-hyperopt-0.4.7/mlpype_hyperopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-07 12:44:05.000000 mlpype-hyperopt-0.4.7/mlpype_hyperopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:44:05.000000 mlpype-hyperopt-0.4.7/mlpype_hyperopt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:44:05.692698 mlpype-hyperopt-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-07 12:39:43.000000 mlpype-hyperopt-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:45.385568 mlpype-hyperopt-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 14:00:45.385568 mlpype-hyperopt-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:45.381569 mlpype-hyperopt-0.4.8/mlpype_hyperopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 14:00:45.000000 mlpype-hyperopt-0.4.8/mlpype_hyperopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 14:00:45.000000 mlpype-hyperopt-0.4.8/mlpype_hyperopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:00:45.000000 mlpype-hyperopt-0.4.8/mlpype_hyperopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-07 14:00:45.000000 mlpype-hyperopt-0.4.8/mlpype_hyperopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:00:45.000000 mlpype-hyperopt-0.4.8/mlpype_hyperopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:00:45.385568 mlpype-hyperopt-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-07 13:57:33.000000 mlpype-hyperopt-0.4.8/setup.py
```


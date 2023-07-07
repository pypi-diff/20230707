# Comparing `tmp/mlpype-fastapi-0.4.7.tar.gz` & `tmp/mlpype-fastapi-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-fastapi-0.4.7.tar", last modified: Fri Jul  7 12:43:56 2023, max compression
+gzip compressed data, was "mlpype-fastapi-0.4.8.tar", last modified: Fri Jul  7 14:00:38 2023, max compression
```

## Comparing `mlpype-fastapi-0.4.7.tar` & `mlpype-fastapi-0.4.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:56.844411 mlpype-fastapi-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 12:43:56.844411 mlpype-fastapi-0.4.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:56.840411 mlpype-fastapi-0.4.7/mlpype_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 12:43:56.000000 mlpype-fastapi-0.4.7/mlpype_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 12:43:56.000000 mlpype-fastapi-0.4.7/mlpype_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:43:56.000000 mlpype-fastapi-0.4.7/mlpype_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 12:43:56.000000 mlpype-fastapi-0.4.7/mlpype_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:43:56.000000 mlpype-fastapi-0.4.7/mlpype_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:43:56.844411 mlpype-fastapi-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-07 12:39:43.000000 mlpype-fastapi-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:38.589521 mlpype-fastapi-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 14:00:38.589521 mlpype-fastapi-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:38.589521 mlpype-fastapi-0.4.8/mlpype_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 14:00:38.000000 mlpype-fastapi-0.4.8/mlpype_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 14:00:38.000000 mlpype-fastapi-0.4.8/mlpype_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:00:38.000000 mlpype-fastapi-0.4.8/mlpype_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 14:00:38.000000 mlpype-fastapi-0.4.8/mlpype_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:00:38.000000 mlpype-fastapi-0.4.8/mlpype_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:00:38.589521 mlpype-fastapi-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-07 13:57:33.000000 mlpype-fastapi-0.4.8/setup.py
```

### Comparing `mlpype-fastapi-0.4.7/setup.py` & `mlpype-fastapi-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```


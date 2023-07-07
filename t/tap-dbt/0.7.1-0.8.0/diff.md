# Comparing `tmp/tap_dbt-0.7.1.tar.gz` & `tmp/tap_dbt-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_dbt-0.7.1.tar", max compression
+gzip compressed data, was "tap_dbt-0.8.0.tar", max compression
```

## Comparing `tap_dbt-0.7.1.tar` & `tap_dbt-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/LICENSE
--rw-r--r--   0        0        0     7180 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/README.md
--rw-r--r--   0        0        0     1764 2023-06-19 21:26:20.593377 tap_dbt-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/tap_dbt/__init__.py
--rw-r--r--   0        0        0     2371 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/tap_dbt/client.py
--rw-r--r--   0        0        0     1780 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/tap_dbt/schemas/accounts.json
--rw-r--r--   0        0        0     2264 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/tap_dbt/schemas/jobs.json
--rw-r--r--   0        0        0     1821 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/tap_dbt/schemas/projects.json
--rw-r--r--   0        0        0     3368 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/tap_dbt/schemas/runs.json
--rw-r--r--   0        0        0     6900 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/tap_dbt/streams.py
--rw-r--r--   0        0        0     2230 2023-06-19 21:25:55.309393 tap_dbt-0.7.1/tap_dbt/tap.py
--rw-r--r--   0        0        0     8074 1970-01-01 00:00:00.000000 tap_dbt-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7180 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/README.md
+-rw-r--r--   0        0        0     1764 2023-07-07 16:39:19.493236 tap_dbt-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/tap_dbt/__init__.py
+-rw-r--r--   0        0        0     2371 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/tap_dbt/client.py
+-rw-r--r--   0        0        0     1780 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/tap_dbt/schemas/accounts.json
+-rw-r--r--   0        0        0     2264 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/tap_dbt/schemas/jobs.json
+-rw-r--r--   0        0        0     1821 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/tap_dbt/schemas/projects.json
+-rw-r--r--   0        0        0     3368 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/tap_dbt/schemas/runs.json
+-rw-r--r--   0        0        0     6900 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/tap_dbt/streams.py
+-rw-r--r--   0        0        0     2230 2023-07-07 16:38:58.320679 tap_dbt-0.8.0/tap_dbt/tap.py
+-rw-r--r--   0        0        0     8074 1970-01-01 00:00:00.000000 tap_dbt-0.8.0/PKG-INFO
```

### Comparing `tap_dbt-0.7.1/LICENSE` & `tap_dbt-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/README.md` & `tap_dbt-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/pyproject.toml` & `tap_dbt-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 requires = [
   "poetry-core==1.6",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-dbt"
-version = "0.7.1"
+version = "0.8.0"
 description = "Singer tap for dbt, built with the Singer SDK."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 maintainers = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 readme = "README.md"
 repository = "https://github.com/edgarrmondragon/tap-dbt"
 keywords = ["singer.io", "elt", "dbt", "singer-sdk"]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
 pyyaml = "^6.0"
-singer-sdk = "==0.28.0"
+singer-sdk = "==0.29.0"
 
 [tool.poetry.group.dev.dependencies]
 faker = ">=17.6,<19.0"
 pytest = "^7.2.2"
 responses = "^0.23.1"
 
 [tool.poetry.scripts]
```

### Comparing `tap_dbt-0.7.1/tap_dbt/client.py` & `tap_dbt-0.8.0/tap_dbt/client.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/tap_dbt/schemas/accounts.json` & `tap_dbt-0.8.0/tap_dbt/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/tap_dbt/schemas/jobs.json` & `tap_dbt-0.8.0/tap_dbt/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/tap_dbt/schemas/projects.json` & `tap_dbt-0.8.0/tap_dbt/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/tap_dbt/schemas/runs.json` & `tap_dbt-0.8.0/tap_dbt/schemas/runs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/tap_dbt/streams.py` & `tap_dbt-0.8.0/tap_dbt/streams.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/tap_dbt/tap.py` & `tap_dbt-0.8.0/tap_dbt/tap.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.7.1/PKG-INFO` & `tap_dbt-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-dbt
-Version: 0.7.1
+Version: 0.8.0
 Summary: Singer tap for dbt, built with the Singer SDK.
 Home-page: https://github.com/edgarrmondragon/tap-dbt
 License: Apache-2.0
 Keywords: singer.io,elt,dbt,singer-sdk
 Author: Edgar Ramírez Mondragón
 Author-email: edgarrm358@sample.com
 Maintainer: Edgar Ramírez Mondragón
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: singer-sdk (==0.28.0)
+Requires-Dist: singer-sdk (==0.29.0)
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-dbt
 Description-Content-Type: text/markdown
 
 # tap-dbt
 
 [![PyPI](https://img.shields.io/pypi/v/tap-dbt.svg?color=blue)](https://pypi.org/project/tap-dbt/)
 [![Python versions](https://img.shields.io/pypi/pyversions/tap-dbt.svg)](https://pypi.org/project/tap-dbt/)
```


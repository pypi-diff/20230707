# Comparing `tmp/tap_dbf-0.0.1.tar.gz` & `tmp/tap_dbf-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_dbf-0.0.1.tar", max compression
+gzip compressed data, was "tap_dbf-0.0.1a2.tar", max compression
```

## Comparing `tap_dbf-0.0.1.tar` & `tap_dbf-0.0.1a2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-07 17:15:36.268963 tap_dbf-0.0.1/LICENSE
--rw-r--r--   0        0        0     1423 2023-07-07 17:15:36.268963 tap_dbf-0.0.1/README.md
--rw-r--r--   0        0        0     2291 2023-07-07 17:16:01.810709 tap_dbf-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       33 2023-07-07 17:15:36.272963 tap_dbf-0.0.1/tap_dbf/__init__.py
--rw-r--r--   0        0        0     6981 2023-07-07 17:15:36.272963 tap_dbf-0.0.1/tap_dbf/tap.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 tap_dbf-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 17:07:09.806123 tap_dbf-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     1423 2023-07-07 17:07:09.806123 tap_dbf-0.0.1a2/README.md
+-rw-r--r--   0        0        0     2293 2023-07-07 17:07:28.110250 tap_dbf-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-07-07 17:07:09.810123 tap_dbf-0.0.1a2/tap_dbf/__init__.py
+-rw-r--r--   0        0        0     6981 2023-07-07 17:07:09.810123 tap_dbf-0.0.1a2/tap_dbf/tap.py
+-rw-r--r--   0        0        0     2591 1970-01-01 00:00:00.000000 tap_dbf-0.0.1a2/PKG-INFO
```

### Comparing `tap_dbf-0.0.1/LICENSE` & `tap_dbf-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.0.1/README.md` & `tap_dbf-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.0.1/pyproject.toml` & `tap_dbf-0.0.1a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core==1.6",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-dbf"
-version = "0.0.1"
+version = "0.0.1a2"
 description = "Singer tap for .DBF files"
 authors = ["Edgar R. Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "dbf",
   "dBase",
```

### Comparing `tap_dbf-0.0.1/tap_dbf/tap.py` & `tap_dbf-0.0.1a2/tap_dbf/tap.py`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.0.1/PKG-INFO` & `tap_dbf-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-dbf
-Version: 0.0.1
+Version: 0.0.1a2
 Summary: Singer tap for .DBF files
 Home-page: https://github.com/edgarrmondragon/tap-pulumi-cloud
 License: Apache-2.0
 Keywords: ELT,singer.io,dbf,dBase
 Author: Edgar R. Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
```


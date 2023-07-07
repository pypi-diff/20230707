# Comparing `tmp/xdynamo-0.3.0.tar.gz` & `tmp/xdynamo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdynamo-0.3.0.tar", max compression
+gzip compressed data, was "xdynamo-0.4.0.tar", max compression
```

## Comparing `xdynamo-0.3.0.tar` & `xdynamo-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      692 2023-05-02 21:03:20.566472 xdynamo-0.3.0/README.md
--rw-r--r--   0        0        0     1683 2023-05-02 21:03:20.570472 xdynamo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    22321 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/__init__.py
--rw-r--r--   0        0        0     5401 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/api.py
--rw-r--r--   0        0        0    32959 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/client.py
--rw-r--r--   0        0        0    14349 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/common_types.py
--rw-r--r--   0        0        0     6464 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/db.py
--rw-r--r--   0        0        0       45 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/errors.py
--rw-r--r--   0        0        0     3501 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/fields.py
--rw-r--r--   0        0        0       25 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/meta.json
--rw-r--r--   0        0        0     2085 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/model.py
--rw-r--r--   0        0        0     5522 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/resources.py
--rw-r--r--   0        0        0    10193 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/structure.py
--rw-r--r--   0        0        0      161 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/utils.py
--rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 xdynamo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      692 2023-07-07 21:50:36.557684 xdynamo-0.4.0/README.md
+-rw-r--r--   0        0        0     1679 2023-07-07 21:50:36.561684 xdynamo-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    22321 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/__init__.py
+-rw-r--r--   0        0        0     5401 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/api.py
+-rw-r--r--   0        0        0    32959 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/client.py
+-rw-r--r--   0        0        0    14349 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/common_types.py
+-rw-r--r--   0        0        0     6464 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/db.py
+-rw-r--r--   0        0        0       45 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/errors.py
+-rw-r--r--   0        0        0     3501 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/fields.py
+-rw-r--r--   0        0        0       25 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/meta.json
+-rw-r--r--   0        0        0     2085 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/model.py
+-rw-r--r--   0        0        0     5522 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/resources.py
+-rw-r--r--   0        0        0    10193 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/structure.py
+-rw-r--r--   0        0        0      161 2023-07-07 21:50:36.561684 xdynamo-0.4.0/xdynamo/utils.py
+-rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 xdynamo-0.4.0/PKG-INFO
```

### Comparing `xdynamo-0.3.0/README.md` & `xdynamo-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/pyproject.toml` & `xdynamo-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "xdynamo"
-version = "0.3.0"
+version = "0.4.0"
 description = "Use dynamo with xmodel objects."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xdynamo"}]
 readme = "README.md"
 repository = "https://github.com/xyngular/py-xdynamo"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.17.54"
 
-xmodel = "^0.4.0"
+xmodel = "^0"
 xinject = "^1.4.0"
 xloop = "^1.0.1"
 xsentinels = "^1.2.1"
 xurls = "^0.2.1"
 ciso8601 = "^2.3.0"
 xsettings = "^1.3.0"
 xboto = "^1.0.2"
```

### Comparing `xdynamo-0.3.0/xdynamo/__init__.py` & `xdynamo-0.4.0/xdynamo/__init__.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/xdynamo/api.py` & `xdynamo-0.4.0/xdynamo/api.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/xdynamo/client.py` & `xdynamo-0.4.0/xdynamo/client.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/xdynamo/common_types.py` & `xdynamo-0.4.0/xdynamo/common_types.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/xdynamo/db.py` & `xdynamo-0.4.0/xdynamo/db.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/xdynamo/fields.py` & `xdynamo-0.4.0/xdynamo/fields.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/xdynamo/model.py` & `xdynamo-0.4.0/xdynamo/model.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/xdynamo/resources.py` & `xdynamo-0.4.0/xdynamo/resources.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/xdynamo/structure.py` & `xdynamo-0.4.0/xdynamo/structure.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.3.0/PKG-INFO` & `xdynamo-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdynamo
-Version: 0.3.0
+Version: 0.4.0
 Summary: Use dynamo with xmodel objects.
 Home-page: https://github.com/xyngular/py-xdynamo
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: boto3 (>=1.17.54,<2.0.0)
 Requires-Dist: ciso8601 (>=2.3.0,<3.0.0)
 Requires-Dist: xboto (>=1.0.2,<2.0.0)
 Requires-Dist: xinject (>=1.4.0,<2.0.0)
 Requires-Dist: xloop (>=1.0.1,<2.0.0)
-Requires-Dist: xmodel (>=0.4.0,<0.5.0)
+Requires-Dist: xmodel (>=0,<1)
 Requires-Dist: xsentinels (>=1.2.1,<2.0.0)
 Requires-Dist: xsettings (>=1.3.0,<2.0.0)
 Requires-Dist: xurls (>=0.2.1,<0.3.0)
 Project-URL: Repository, https://github.com/xyngular/py-xdynamo
 Description-Content-Type: text/markdown
 
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8|%203.9|%203.10|%203.11&color=blue?style=flat-square&logo=python)
```


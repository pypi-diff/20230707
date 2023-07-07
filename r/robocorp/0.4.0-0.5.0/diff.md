# Comparing `tmp/robocorp-0.4.0.tar.gz` & `tmp/robocorp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp-0.4.0.tar", max compression
+gzip compressed data, was "robocorp-0.5.0.tar", max compression
```

## Comparing `robocorp-0.4.0.tar` & `robocorp-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      599 2023-06-30 14:01:52.199913 robocorp-0.4.0/README.md
--rw-r--r--   0        0        0      776 2023-06-30 14:01:52.199913 robocorp-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-06-30 14:01:52.199913 robocorp-0.4.0/src/robocorp/_meta/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 14:01:52.199913 robocorp-0.4.0/src/robocorp/_meta/py.typed
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 robocorp-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-07-07 11:20:40.108453 robocorp-0.5.0/README.md
+-rw-r--r--   0        0        0      776 2023-07-07 11:20:40.108453 robocorp-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-07 11:20:40.108453 robocorp-0.5.0/src/robocorp/_meta/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 11:20:40.108453 robocorp-0.5.0/src/robocorp/_meta/py.typed
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 robocorp-0.5.0/PKG-INFO
```

### Comparing `robocorp-0.4.0/README.md` & `robocorp-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp-0.4.0/pyproject.toml` & `robocorp-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "robocorp"
-version = "0.4.0"
+version = "0.5.0"
 description = "Robocorp core libraries for Python automation"
 authors = [
 	"Ossi Rajuvaara <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
 license = "Apache-2.0"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-tasks = "2.0.0"
-robocorp-log = "2.1.0"
+robocorp-tasks = "2.1.1"
+robocorp-log = "2.2.0"
 robocorp-workitems = "1.2.1"
-robocorp-vault = "0.4.0"
+robocorp-vault = "1.0.0"
 robocorp-storage = "0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.black]
 skip-string-normalization = false
```

### Comparing `robocorp-0.4.0/PKG-INFO` & `robocorp-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: robocorp
-Version: 0.4.0
+Version: 0.5.0
 Summary: Robocorp core libraries for Python automation
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Ossi Rajuvaara
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: robocorp-log (==2.1.0)
+Requires-Dist: robocorp-log (==2.2.0)
 Requires-Dist: robocorp-storage (==0.2.0)
-Requires-Dist: robocorp-tasks (==2.0.0)
-Requires-Dist: robocorp-vault (==0.4.0)
+Requires-Dist: robocorp-tasks (==2.1.1)
+Requires-Dist: robocorp-vault (==1.0.0)
 Requires-Dist: robocorp-workitems (==1.2.1)
 Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
 # robocorp (metapackage)
 
 This is a metapackage for installing the core libraries of [Robocorp](https://robocorp.com/)'s Python automation framework.
```


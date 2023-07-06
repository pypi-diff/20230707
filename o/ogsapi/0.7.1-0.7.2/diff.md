# Comparing `tmp/ogsapi-0.7.1.tar.gz` & `tmp/ogsapi-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.7.1.tar", last modified: Thu Jul  6 23:23:24 2023, max compression
+gzip compressed data, was "ogsapi-0.7.2.tar", last modified: Thu Jul  6 23:44:44 2023, max compression
```

## Comparing `ogsapi-0.7.1.tar` & `ogsapi-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:23:24.646418 ogsapi-0.7.1/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-07-06 23:23:12.000000 ogsapi-0.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5557 2023-07-06 23:23:24.646418 ogsapi-0.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5123 2023-07-06 23:23:12.000000 ogsapi-0.7.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-06 23:23:12.000000 ogsapi-0.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 23:23:24.646418 ogsapi-0.7.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:23:24.643418 ogsapi-0.7.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:23:24.645419 ogsapi-0.7.1/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 23:23:12.000000 ogsapi-0.7.1/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22383 2023-07-06 23:23:12.000000 ogsapi-0.7.1/src/ogsapi/client.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-06 23:23:12.000000 ogsapi-0.7.1/src/ogsapi/ogs_api_exception.py
--rw-rw-rw-   0 root         (0) root         (0)    14931 2023-07-06 23:23:12.000000 ogsapi-0.7.1/src/ogsapi/ogsgame.py
--rw-rw-rw-   0 root         (0) root         (0)     6726 2023-07-06 23:23:12.000000 ogsapi-0.7.1/src/ogsapi/ogssocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:23:24.646418 ogsapi-0.7.1/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5557 2023-07-06 23:23:24.000000 ogsapi-0.7.1/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-06 23:23:24.000000 ogsapi-0.7.1/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 23:23:24.000000 ogsapi-0.7.1/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 23:23:24.000000 ogsapi-0.7.1/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 23:23:24.000000 ogsapi-0.7.1/src/ogsapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:23:24.646418 ogsapi-0.7.1/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)      879 2023-07-06 23:23:12.000000 ogsapi-0.7.1/src/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.831642 ogsapi-0.7.2/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-07-06 23:44:33.000000 ogsapi-0.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-07-06 23:44:44.831642 ogsapi-0.7.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-07-06 23:44:33.000000 ogsapi-0.7.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-06 23:44:33.000000 ogsapi-0.7.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 23:44:44.831642 ogsapi-0.7.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.828642 ogsapi-0.7.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.830642 ogsapi-0.7.2/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22383 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/ogs_api_exception.py
+-rw-rw-rw-   0 root         (0) root         (0)    14931 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/ogsgame.py
+-rw-rw-rw-   0 root         (0) root         (0)     6726 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/ogsapi/ogssocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.831642 ogsapi-0.7.2/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 23:44:44.000000 ogsapi-0.7.2/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 23:44:44.831642 ogsapi-0.7.2/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      879 2023-07-06 23:44:33.000000 ogsapi-0.7.2/src/tests/test.py
```

### Comparing `ogsapi-0.7.1/LICENSE` & `ogsapi-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.1/PKG-INFO` & `ogsapi-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.7.1
+Version: 0.7.2
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.7.1/README.md` & `ogsapi-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.1/pyproject.toml` & `ogsapi-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ogsapi-0.7.1/src/ogsapi/client.py` & `ogsapi-0.7.2/src/ogsapi/client.py`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.1/src/ogsapi/ogsgame.py` & `ogsapi-0.7.2/src/ogsapi/ogsgame.py`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.1/src/ogsapi/ogssocket.py` & `ogsapi-0.7.2/src/ogsapi/ogssocket.py`

 * *Files identical despite different names*

### Comparing `ogsapi-0.7.1/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.7.2/src/ogsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.7.1
+Version: 0.7.2
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ogsapi-0.7.1/src/tests/test.py` & `ogsapi-0.7.2/src/tests/test.py`

 * *Files identical despite different names*


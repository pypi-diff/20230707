# Comparing `tmp/predibase-api-2023.7.4.tar.gz` & `tmp/predibase-api-2023.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2023.7.4.tar", last modified: Fri Jul  7 17:41:59 2023, max compression
+gzip compressed data, was "predibase-api-2023.7.5.tar", last modified: Fri Jul  7 18:11:13 2023, max compression
```

## Comparing `predibase-api-2023.7.4.tar` & `predibase-api-2023.7.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 17:41:59.000000 predibase-api-2023.7.4/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-07 17:41:59.000000 predibase-api-2023.7.4/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:41:59.000000 predibase-api-2023.7.4/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:41:33.000000 predibase-api-2023.7.4/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 17:41:59.000000 predibase-api-2023.7.4/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 17:41:59.000000 predibase-api-2023.7.4/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:41:59.953392 predibase-api-2023.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-07 17:41:02.000000 predibase-api-2023.7.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 17:41:52.000000 predibase-api-2023.7.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.159721 predibase-api-2023.7.5/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 18:11:13.000000 predibase-api-2023.7.5/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-07 18:11:13.000000 predibase-api-2023.7.5/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:11:13.000000 predibase-api-2023.7.5/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:10:44.000000 predibase-api-2023.7.5/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 18:11:13.000000 predibase-api-2023.7.5/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 18:11:13.000000 predibase-api-2023.7.5/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:11:13.163720 predibase-api-2023.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-07 18:10:17.000000 predibase-api-2023.7.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 18:11:01.000000 predibase-api-2023.7.5/version.txt
```

### Comparing `predibase-api-2023.7.4/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2023.7.5/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.4/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2023.7.5/predibase_api/foobar/v1/bar_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.4/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2023.7.5/predibase_api/foobar/v1/foo_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.4/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2023.7.5/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.4/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2023.7.5/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.4/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2023.7.5/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.4/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2023.7.5/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2023.7.4/setup.py` & `predibase-api-2023.7.5/setup.py`

 * *Files identical despite different names*


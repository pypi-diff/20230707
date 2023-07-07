# Comparing `tmp/adam_credmanager-0.1.2.tar.gz` & `tmp/adam_credmanager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_credmanager-0.1.2.tar", max compression
+gzip compressed data, was "adam_credmanager-0.1.3.tar", max compression
```

## Comparing `adam_credmanager-0.1.2.tar` & `adam_credmanager-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       48 2023-07-07 19:12:42.878599 adam_credmanager-0.1.2/README.md
--rw-r--r--   0        0        0      110 2023-07-07 19:46:24.460717 adam_credmanager-0.1.2/adam_credmanager/__init__.py
--rw-r--r--   0        0        0     1846 2023-07-07 19:43:15.577896 adam_credmanager-0.1.2/adam_credmanager/adam_credmanager.py
--rw-r--r--   0        0        0      391 2023-07-07 19:46:29.307370 adam_credmanager-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 adam_credmanager-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-07-07 19:12:42.878599 adam_credmanager-0.1.3/README.md
+-rw-r--r--   0        0        0       79 2023-07-07 19:50:12.350112 adam_credmanager-0.1.3/adam_credmanager/__init__.py
+-rw-r--r--   0        0        0     1846 2023-07-07 19:47:50.143819 adam_credmanager-0.1.3/adam_credmanager/adam_credmanager.py
+-rw-r--r--   0        0        0      391 2023-07-07 19:50:19.026762 adam_credmanager-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 adam_credmanager-0.1.3/PKG-INFO
```

### Comparing `adam_credmanager-0.1.2/adam_credmanager/adam_credmanager.py` & `adam_credmanager-0.1.3/adam_credmanager/adam_credmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #GCP
 #Secret Manager
 from google.cloud import secretmanager
 #Resource Manager (para obtener project number)
 from google.cloud import resourcemanager_v3
 
-class Adam_credmanager():
+class adam_credmanager():
     def __init__(self, project_id) -> None:
         self.project_id=project_id
         self.client= secretmanager.SecretManagerServiceClient()
 
     def list_secret_versions(self, secret_id: str) -> None:
         """
         List all secret versions in the given secret and their metadata.
```

### Comparing `adam_credmanager-0.1.2/PKG-INFO` & `adam_credmanager-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-credmanager
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Eduardo Pagnone
 Author-email: eduardopagnone@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```


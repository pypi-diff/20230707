# Comparing `tmp/adam_credmanager-0.1.1.tar.gz` & `tmp/adam_credmanager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_credmanager-0.1.1.tar", max compression
+gzip compressed data, was "adam_credmanager-0.1.2.tar", max compression
```

## Comparing `adam_credmanager-0.1.1.tar` & `adam_credmanager-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       48 2023-07-07 19:12:42.878599 adam_credmanager-0.1.1/README.md
--rw-r--r--   0        0        0      108 2023-07-07 19:31:52.676114 adam_credmanager-0.1.1/adam_credmanager/__init__.py
--rw-r--r--   0        0        0     1846 2023-07-07 19:43:15.577896 adam_credmanager-0.1.1/adam_credmanager/adam_credmanager.py
--rw-r--r--   0        0        0      391 2023-07-07 19:43:39.337842 adam_credmanager-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 adam_credmanager-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-07-07 19:12:42.878599 adam_credmanager-0.1.2/README.md
+-rw-r--r--   0        0        0      110 2023-07-07 19:46:24.460717 adam_credmanager-0.1.2/adam_credmanager/__init__.py
+-rw-r--r--   0        0        0     1846 2023-07-07 19:43:15.577896 adam_credmanager-0.1.2/adam_credmanager/adam_credmanager.py
+-rw-r--r--   0        0        0      391 2023-07-07 19:46:29.307370 adam_credmanager-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 adam_credmanager-0.1.2/PKG-INFO
```

### Comparing `adam_credmanager-0.1.1/adam_credmanager/adam_credmanager.py` & `adam_credmanager-0.1.2/adam_credmanager/adam_credmanager.py`

 * *Files identical despite different names*

### Comparing `adam_credmanager-0.1.1/PKG-INFO` & `adam_credmanager-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-credmanager
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Eduardo Pagnone
 Author-email: eduardopagnone@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```


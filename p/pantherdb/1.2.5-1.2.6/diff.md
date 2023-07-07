# Comparing `tmp/pantherdb-1.2.5.tar.gz` & `tmp/pantherdb-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantherdb-1.2.5.tar", last modified: Fri Jul  7 09:13:30 2023, max compression
+gzip compressed data, was "pantherdb-1.2.6.tar", last modified: Fri Jul  7 10:19:02 2023, max compression
```

## Comparing `pantherdb-1.2.5.tar` & `pantherdb-1.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:13:30.249374 pantherdb-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 09:13:30.249374 pantherdb-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-07 09:13:15.000000 pantherdb-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:13:30.245374 pantherdb-1.2.5/pantherdb/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 09:13:15.000000 pantherdb-1.2.5/pantherdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-07-07 09:13:15.000000 pantherdb-1.2.5/pantherdb/pantherdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:13:30.249374 pantherdb-1.2.5/pantherdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 09:13:30.000000 pantherdb-1.2.5/pantherdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-07 09:13:30.000000 pantherdb-1.2.5/pantherdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:13:30.000000 pantherdb-1.2.5/pantherdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 09:13:30.000000 pantherdb-1.2.5/pantherdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 09:13:30.000000 pantherdb-1.2.5/pantherdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:13:30.249374 pantherdb-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 09:13:15.000000 pantherdb-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:13:30.249374 pantherdb-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-07-07 09:13:15.000000 pantherdb-1.2.5/tests/test_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:19:02.541128 pantherdb-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-07 10:19:02.541128 pantherdb-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-07 10:18:46.000000 pantherdb-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:19:02.541128 pantherdb-1.2.6/pantherdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 10:18:46.000000 pantherdb-1.2.6/pantherdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-07-07 10:18:46.000000 pantherdb-1.2.6/pantherdb/pantherdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:19:02.541128 pantherdb-1.2.6/pantherdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 10:19:02.000000 pantherdb-1.2.6/pantherdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:19:02.541128 pantherdb-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-07 10:18:46.000000 pantherdb-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:19:02.541128 pantherdb-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-07-07 10:18:46.000000 pantherdb-1.2.6/tests/test_normal.py
```

### Comparing `pantherdb-1.2.5/PKG-INFO` & `pantherdb-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantherdb
-Version: 1.2.5
+Version: 1.2.6
 Summary: is a Simple, FileBase and Document Oriented database
 Home-page: https://github.com/alirn76/pantherdb
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Introduction
 
 PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
 - Document Oriented
 - Easy to use
-- Written in pure Python +3.11 based on standard type hints
+- Written in pure Python +3.8 based on standard type hints
 - Handle Database Encryption
 
 
 ## Usage
 
 ### Database:
 - #### Create a database:
```

### Comparing `pantherdb-1.2.5/README.md` & `pantherdb-1.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## Introduction
 
 PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
 - Document Oriented
 - Easy to use
-- Written in pure Python +3.11 based on standard type hints
+- Written in pure Python +3.8 based on standard type hints
 - Handle Database Encryption
 
 
 ## Usage
 
 ### Database:
 - #### Create a database:
```

### Comparing `pantherdb-1.2.5/pantherdb/pantherdb.py` & `pantherdb-1.2.6/pantherdb/pantherdb.py`

 * *Files identical despite different names*

### Comparing `pantherdb-1.2.5/pantherdb.egg-info/PKG-INFO` & `pantherdb-1.2.6/pantherdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantherdb
-Version: 1.2.5
+Version: 1.2.6
 Summary: is a Simple, FileBase and Document Oriented database
 Home-page: https://github.com/alirn76/pantherdb
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Introduction
 
 PantherDB is a <b>Simple</b>, <b>FileBase</b> and <b>Document Oriented</b> database that you can use in your projects.
 
 ### Features:
 - Document Oriented
 - Easy to use
-- Written in pure Python +3.11 based on standard type hints
+- Written in pure Python +3.8 based on standard type hints
 - Handle Database Encryption
 
 
 ## Usage
 
 ### Database:
 - #### Create a database:
```

### Comparing `pantherdb-1.2.5/setup.py` & `pantherdb-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `pantherdb-1.2.5/tests/test_normal.py` & `pantherdb-1.2.6/tests/test_normal.py`

 * *Files identical despite different names*


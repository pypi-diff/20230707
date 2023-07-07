# Comparing `tmp/ipams-1.3.2.tar.gz` & `tmp/ipams-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipams-1.3.2.tar", last modified: Sat Mar 11 12:53:14 2023, max compression
+gzip compressed data, was "ipams-1.3.3.tar", last modified: Fri Jul  7 10:26:16 2023, max compression
```

## Comparing `ipams-1.3.2.tar` & `ipams-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:53:14.672822 ipams-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-11 12:53:09.000000 ipams-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-03-11 12:53:14.672822 ipams-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-03-11 12:53:09.000000 ipams-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:53:14.668822 ipams-1.3.2/ipams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/netbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/phpipam.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-11 12:53:09.000000 ipams-1.3.2/ipams/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:53:14.672822 ipams-1.3.2/ipams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-03-11 12:53:14.000000 ipams-1.3.2/ipams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-11 12:53:14.000000 ipams-1.3.2/ipams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 12:53:14.000000 ipams-1.3.2/ipams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-11 12:53:14.000000 ipams-1.3.2/ipams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-11 12:53:14.000000 ipams-1.3.2/ipams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-11 12:53:14.000000 ipams-1.3.2/ipams.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 12:53:14.672822 ipams-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-11 12:53:09.000000 ipams-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:16.191565 ipams-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-07 10:26:11.000000 ipams-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-07 10:26:16.191565 ipams-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-07 10:26:11.000000 ipams-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:16.191565 ipams-1.3.3/ipams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/netbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/phpipam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 10:26:11.000000 ipams-1.3.3/ipams/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:26:16.191565 ipams-1.3.3/ipams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-07 10:26:16.000000 ipams-1.3.3/ipams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-07 10:26:16.000000 ipams-1.3.3/ipams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:26:16.000000 ipams-1.3.3/ipams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 10:26:16.000000 ipams-1.3.3/ipams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 10:26:16.000000 ipams-1.3.3/ipams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 10:26:16.000000 ipams-1.3.3/ipams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:26:16.191565 ipams-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-07 10:26:11.000000 ipams-1.3.3/setup.py
```

### Comparing `ipams-1.3.2/LICENSE` & `ipams-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipams-1.3.2/PKG-INFO` & `ipams-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipams
-Version: 1.3.2
+Version: 1.3.3
 Summary: Tool to query multiple IPAMs.
 Home-page: https://github.com/rwxd/ipams
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ipams-1.3.2/README.md` & `ipams-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ipams-1.3.2/ipams/cli.py` & `ipams-1.3.3/ipams/cli.py`

 * *Files identical despite different names*

### Comparing `ipams-1.3.2/ipams/config.py` & `ipams-1.3.3/ipams/config.py`

 * *Files identical despite different names*

### Comparing `ipams-1.3.2/ipams/logging.py` & `ipams-1.3.3/ipams/logging.py`

 * *Files identical despite different names*

### Comparing `ipams-1.3.2/ipams/netbox.py` & `ipams-1.3.3/ipams/netbox.py`

 * *Files identical despite different names*

### Comparing `ipams-1.3.2/ipams/output.py` & `ipams-1.3.3/ipams/output.py`

 * *Files identical despite different names*

### Comparing `ipams-1.3.2/ipams/phpipam.py` & `ipams-1.3.3/ipams/phpipam.py`

 * *Files identical despite different names*

### Comparing `ipams-1.3.2/ipams.egg-info/PKG-INFO` & `ipams-1.3.3/ipams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipams
-Version: 1.3.2
+Version: 1.3.3
 Summary: Tool to query multiple IPAMs.
 Home-page: https://github.com/rwxd/ipams
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ipams-1.3.2/setup.py` & `ipams-1.3.3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/bSuite-python-1.1.2.tar.gz` & `tmp/bSuite-python-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bSuite-python-1.1.2.tar", last modified: Fri Jul  7 20:54:24 2023, max compression
+gzip compressed data, was "bSuite-python-1.1.3.tar", last modified: Fri Jul  7 21:12:42 2023, max compression
```

## Comparing `bSuite-python-1.1.2.tar` & `bSuite-python-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.519953 bSuite-python-1.1.2/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.2/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-07 20:54:24.519763 bSuite-python-1.1.2/PKG-INFO
--rw-r--r--   0 birdwell   (501) staff       (20)       16 2023-07-05 15:45:08.000000 bSuite-python-1.1.2/README.md
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.512819 bSuite-python-1.1.2/bSuite_configure/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.2/bSuite_configure/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)      372 2023-07-05 02:23:50.000000 bSuite-python-1.1.2/bSuite_configure/pyproject.toml
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.511242 bSuite-python-1.1.2/bSuite_configure/src/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.511287 bSuite-python-1.1.2/bSuite_configure/src/bSuite/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.513509 bSuite-python-1.1.2/bSuite_configure/src/bSuite/configure/
--rw-r--r--   0 birdwell   (501) staff       (20)       52 2023-07-05 01:59:36.000000 bSuite-python-1.1.2/bSuite_configure/src/bSuite/configure/__init__.py
--rw-r--r--   0 birdwell   (501) staff       (20)     1233 2023-07-05 01:05:11.000000 bSuite-python-1.1.2/bSuite_configure/src/bSuite/configure/configure.py
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.513988 bSuite-python-1.1.2/bSuite_database/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.2/bSuite_database/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)      490 2023-07-05 02:26:14.000000 bSuite-python-1.1.2/bSuite_database/pyproject.toml
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.511452 bSuite-python-1.1.2/bSuite_database/src/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.511493 bSuite-python-1.1.2/bSuite_database/src/bSuite/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.515222 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/
--rw-r--r--   0 birdwell   (501) staff       (20)      112 2023-07-04 23:38:47.000000 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/__init__.py
--rw-r--r--   0 birdwell   (501) staff       (20)     8187 2023-07-07 20:47:35.000000 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/base.py
--rw-r--r--   0 birdwell   (501) staff       (20)     2851 2023-07-06 00:12:17.000000 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/crypto.py
--rw-r--r--   0 birdwell   (501) staff       (20)     2629 2023-07-07 20:26:55.000000 bSuite-python-1.1.2/bSuite_database/src/bSuite/database/mapped.py
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 20:54:24.519412 bSuite-python-1.1.2/bSuite_python.egg-info/
--rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/PKG-INFO
--rw-r--r--   0 birdwell   (501) staff       (20)      622 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/SOURCES.txt
--rw-r--r--   0 birdwell   (501) staff       (20)        1 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/dependency_links.txt
--rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/requires.txt
--rw-r--r--   0 birdwell   (501) staff       (20)        7 2023-07-07 20:54:24.000000 bSuite-python-1.1.2/bSuite_python.egg-info/top_level.txt
--rw-r--r--   0 birdwell   (501) staff       (20)      788 2023-07-07 20:53:35.000000 bSuite-python-1.1.2/pyproject.toml
--rw-r--r--   0 birdwell   (501) staff       (20)       38 2023-07-07 20:54:24.519993 bSuite-python-1.1.2/setup.cfg
--rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-05 00:44:00.000000 bSuite-python-1.1.2/setup.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.783470 bSuite-python-1.1.3/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.3/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-07 21:12:42.783277 bSuite-python-1.1.3/PKG-INFO
+-rw-r--r--   0 birdwell   (501) staff       (20)       16 2023-07-05 15:45:08.000000 bSuite-python-1.1.3/README.md
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.775058 bSuite-python-1.1.3/bSuite_configure/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.3/bSuite_configure/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)      372 2023-07-05 02:23:50.000000 bSuite-python-1.1.3/bSuite_configure/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.773492 bSuite-python-1.1.3/bSuite_configure/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.773534 bSuite-python-1.1.3/bSuite_configure/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.775768 bSuite-python-1.1.3/bSuite_configure/src/bSuite/configure/
+-rw-r--r--   0 birdwell   (501) staff       (20)       52 2023-07-05 01:59:36.000000 bSuite-python-1.1.3/bSuite_configure/src/bSuite/configure/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     1233 2023-07-05 01:05:11.000000 bSuite-python-1.1.3/bSuite_configure/src/bSuite/configure/configure.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.776261 bSuite-python-1.1.3/bSuite_database/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-python-1.1.3/bSuite_database/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)      490 2023-07-05 02:26:14.000000 bSuite-python-1.1.3/bSuite_database/pyproject.toml
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.773698 bSuite-python-1.1.3/bSuite_database/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.773740 bSuite-python-1.1.3/bSuite_database/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.777390 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/
+-rw-r--r--   0 birdwell   (501) staff       (20)      112 2023-07-04 23:38:47.000000 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     8010 2023-07-07 21:11:43.000000 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/base.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     2851 2023-07-06 00:12:17.000000 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/crypto.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     2629 2023-07-07 20:26:55.000000 bSuite-python-1.1.3/bSuite_database/src/bSuite/database/mapped.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-07 21:12:42.782967 bSuite-python-1.1.3/bSuite_python.egg-info/
+-rw-r--r--   0 birdwell   (501) staff       (20)    40984 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/PKG-INFO
+-rw-r--r--   0 birdwell   (501) staff       (20)      622 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)        1 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/requires.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)        7 2023-07-07 21:12:42.000000 bSuite-python-1.1.3/bSuite_python.egg-info/top_level.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)      788 2023-07-07 21:12:34.000000 bSuite-python-1.1.3/pyproject.toml
+-rw-r--r--   0 birdwell   (501) staff       (20)       38 2023-07-07 21:12:42.783510 bSuite-python-1.1.3/setup.cfg
+-rw-r--r--   0 birdwell   (501) staff       (20)       39 2023-07-05 00:44:00.000000 bSuite-python-1.1.3/setup.py
```

### Comparing `bSuite-python-1.1.2/LICENSE` & `bSuite-python-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.2/PKG-INFO` & `bSuite-python-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bSuite-python
-Version: 1.1.2
+Version: 1.1.3
 Summary: advanced helper modules. python edition
 Author-email: John Birdwell <j.c.birdwell@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bSuite-python-1.1.2/bSuite_configure/LICENSE` & `bSuite-python-1.1.3/bSuite_configure/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.2/bSuite_configure/src/bSuite/configure/configure.py` & `bSuite-python-1.1.3/bSuite_configure/src/bSuite/configure/configure.py`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.2/bSuite_database/LICENSE` & `bSuite-python-1.1.3/bSuite_database/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.2/bSuite_database/src/bSuite/database/base.py` & `bSuite-python-1.1.3/bSuite_database/src/bSuite/database/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,14 @@
             csr.execute(query, vals)
             if not no_resp:
                 # grab columns for record formation
                 if not as_tuple:
                     cols = tuple(x[0] for x in csr.description)
                 # retrieve values
                 fetched = csr.fetchall()
-            elif 'select' in query:
-                # Save some sanity when debugging
-                print("Warning: You passed a select query but didn't request a response!")
 
         # cursor returned to pool before parsing, if required.
         if fetched:
             if cols:
                 return [{k: v for k, v in zip(cols, row)} for row in fetched]
             elif as_tuple:
                 return [x for x in fetched]
```

### Comparing `bSuite-python-1.1.2/bSuite_database/src/bSuite/database/crypto.py` & `bSuite-python-1.1.3/bSuite_database/src/bSuite/database/crypto.py`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.2/bSuite_database/src/bSuite/database/mapped.py` & `bSuite-python-1.1.3/bSuite_database/src/bSuite/database/mapped.py`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.2/bSuite_python.egg-info/PKG-INFO` & `bSuite-python-1.1.3/bSuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bSuite-python
-Version: 1.1.2
+Version: 1.1.3
 Summary: advanced helper modules. python edition
 Author-email: John Birdwell <j.c.birdwell@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bSuite-python-1.1.2/bSuite_python.egg-info/SOURCES.txt` & `bSuite-python-1.1.3/bSuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bSuite-python-1.1.2/pyproject.toml` & `bSuite-python-1.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name='bSuite-python'
-version='1.1.2'
+version='1.1.3'
 description='advanced helper modules. python edition'
 authors = [{name = "John Birdwell", email = "j.c.birdwell@gmail.com"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
 keywords = ["helpers", "utilities", "database", "postgres", ".ini"]
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
```


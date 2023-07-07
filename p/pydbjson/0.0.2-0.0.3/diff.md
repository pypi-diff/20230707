# Comparing `tmp/pydbjson-0.0.2.tar.gz` & `tmp/pydbjson-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbjson-0.0.2.tar", last modified: Fri Jul  7 15:38:35 2023, max compression
+gzip compressed data, was "pydbjson-0.0.3.tar", last modified: Fri Jul  7 15:40:28 2023, max compression
```

## Comparing `pydbjson-0.0.2.tar` & `pydbjson-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:38:35.668668 pydbjson-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-07 14:29:42.000000 pydbjson-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1916 2023-07-07 15:38:35.667671 pydbjson-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1348 2023-07-07 15:34:37.000000 pydbjson-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 15:38:35.657702 pydbjson-0.0.2/pydbjson/
--rw-rw-rw-   0        0        0       29 2023-07-07 15:37:09.000000 pydbjson-0.0.2/pydbjson/__init__.py
--rw-rw-rw-   0        0        0     1462 2023-07-07 15:31:33.000000 pydbjson-0.0.2/pydbjson/pyjsondb.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:38:35.666672 pydbjson-0.0.2/pydbjson.egg-info/
--rw-rw-rw-   0        0        0     1916 2023-07-07 15:38:35.000000 pydbjson-0.0.2/pydbjson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-07-07 15:38:35.000000 pydbjson-0.0.2/pydbjson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:38:35.000000 pydbjson-0.0.2/pydbjson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 15:38:35.000000 pydbjson-0.0.2/pydbjson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-07-07 13:30:09.000000 pydbjson-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 15:38:35.669664 pydbjson-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-07-07 15:38:20.000000 pydbjson-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:40:28.854394 pydbjson-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-07 14:29:42.000000 pydbjson-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1925 2023-07-07 15:40:28.853414 pydbjson-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-07-07 15:39:18.000000 pydbjson-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 15:40:28.842245 pydbjson-0.0.3/pydbjson/
+-rw-rw-rw-   0        0        0       29 2023-07-07 15:37:09.000000 pydbjson-0.0.3/pydbjson/__init__.py
+-rw-rw-rw-   0        0        0     1462 2023-07-07 15:31:33.000000 pydbjson-0.0.3/pydbjson/pyjsondb.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:40:28.850067 pydbjson-0.0.3/pydbjson.egg-info/
+-rw-rw-rw-   0        0        0     1925 2023-07-07 15:40:28.000000 pydbjson-0.0.3/pydbjson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-07-07 15:40:28.000000 pydbjson-0.0.3/pydbjson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:40:28.000000 pydbjson-0.0.3/pydbjson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 15:40:28.000000 pydbjson-0.0.3/pydbjson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-07-07 13:30:09.000000 pydbjson-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-07 15:40:28.854394 pydbjson-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-07-07 15:40:06.000000 pydbjson-0.0.3/setup.py
```

### Comparing `pydbjson-0.0.2/LICENSE` & `pydbjson-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydbjson-0.0.2/PKG-INFO` & `pydbjson-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbjson
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small database using json
 Author: Sampath
 Author-email: gujarathisampath@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -37,15 +37,15 @@
 `pydbjson` provides a convenient way to interact with JSON-based databases in Python. It allows you to load data from a JSON file, insert, retrieve, delete, and find documents, and save the data back to the file.
 
 ## Usage
 
 ### Importing the library
 
 ```python
-from pydbjson import pydbjson
+from pydbjson.pydbjson import pydbjson
 ```
 
 ### Creating an instance of pydbjson
 
 ```python
 db = pydbjson("database.json")
 ```
```

### Comparing `pydbjson-0.0.2/README.md` & `pydbjson-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 `pydbjson` provides a convenient way to interact with JSON-based databases in Python. It allows you to load data from a JSON file, insert, retrieve, delete, and find documents, and save the data back to the file.
 
 ## Usage
 
 ### Importing the library
 
 ```python
-from pydbjson import pydbjson
+from pydbjson.pydbjson import pydbjson
 ```
 
 ### Creating an instance of pydbjson
 
 ```python
 db = pydbjson("database.json")
 ```
```

### Comparing `pydbjson-0.0.2/pydbjson/pyjsondb.py` & `pydbjson-0.0.3/pydbjson/pyjsondb.py`

 * *Files identical despite different names*

### Comparing `pydbjson-0.0.2/pydbjson.egg-info/PKG-INFO` & `pydbjson-0.0.3/pydbjson.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbjson
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small database using json
 Author: Sampath
 Author-email: gujarathisampath@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -37,15 +37,15 @@
 `pydbjson` provides a convenient way to interact with JSON-based databases in Python. It allows you to load data from a JSON file, insert, retrieve, delete, and find documents, and save the data back to the file.
 
 ## Usage
 
 ### Importing the library
 
 ```python
-from pydbjson import pydbjson
+from pydbjson.pydbjson import pydbjson
 ```
 
 ### Creating an instance of pydbjson
 
 ```python
 db = pydbjson("database.json")
 ```
```

### Comparing `pydbjson-0.0.2/setup.py` & `pydbjson-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A small database using json'
 
 # Setting up
 setup(
     name="pydbjson",
     version=VERSION,
     author="Sampath",
```


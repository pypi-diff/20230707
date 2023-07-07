# Comparing `tmp/DefyDatabase-10.0.0a4.dev202307061815.tar.gz` & `tmp/DefyDatabase-10.0.0a4.dev202307071900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DefyDatabase-10.0.0a4.dev202307061815.tar", last modified: Thu Jul  6 10:12:44 2023, max compression
+gzip compressed data, was "DefyDatabase-10.0.0a4.dev202307071900.tar", last modified: Fri Jul  7 10:55:25 2023, max compression
```

## Comparing `DefyDatabase-10.0.0a4.dev202307061815.tar` & `DefyDatabase-10.0.0a4.dev202307071900.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 10:12:44.797074 DefyDatabase-10.0.0a4.dev202307061815/
-drwxrwxrwx   0        0        0        0 2023-07-06 10:12:44.791025 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/
--rw-rw-rw-   0        0        0      567 2023-07-06 10:12:44.000000 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-06 10:12:44.000000 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:12:44.000000 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-06 10:12:44.000000 DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-07-06 10:12:44.796040 DefyDatabase-10.0.0a4.dev202307061815/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202307061815/README.md
--rw-rw-rw-   0        0        0     2578 2023-07-06 10:12:01.000000 DefyDatabase-10.0.0a4.dev202307061815/defy.py
--rw-rw-rw-   0        0        0       42 2023-07-06 10:12:44.797074 DefyDatabase-10.0.0a4.dev202307061815/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202307061815/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:55:25.921162 DefyDatabase-10.0.0a4.dev202307071900/
+drwxrwxrwx   0        0        0        0 2023-07-07 10:55:25.919170 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-07-07 10:55:25.000000 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-07-07 10:55:25.000000 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:55:25.000000 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 10:55:25.000000 DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-07-07 10:55:25.919677 DefyDatabase-10.0.0a4.dev202307071900/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202307071900/README.md
+-rw-rw-rw-   0        0        0     2578 2023-07-07 10:54:48.000000 DefyDatabase-10.0.0a4.dev202307071900/defydb.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:55:25.921162 DefyDatabase-10.0.0a4.dev202307071900/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-07-07 10:54:16.000000 DefyDatabase-10.0.0a4.dev202307071900/setup.py
```

### Comparing `DefyDatabase-10.0.0a4.dev202307061815/DefyDatabase.egg-info/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202307071900/DefyDatabase.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202307061815
+Version: 10.0.0a4.dev202307071900
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202307061815/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202307071900/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202307061815
+Version: 10.0.0a4.dev202307071900
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202307061815/defy.py` & `DefyDatabase-10.0.0a4.dev202307071900/defydb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #Rules are meant to break by proudest ones.
 '''
 这是亮天计划的数据库官方API。
 '''
 import sqlite3,sys,os,datetime,io
 
 tor='DefyDatabase'
-version='10.0.0a4.dev202307061815'
+version='10.0.0a4.dev202307071900'
 
 
 
 commands={
     'COUNT_MAIN':'SELECT COUNT(*) FROM LIGHTSKY1',
     'CHECK_BIND':'SELECT UID,BIND FROM BIND1 WHERE UID = "{}"',
     'QUERYUID':'SELECT UID, GRADE, JOB FROM LIGHTSKY1 WHERE UID = "{}"',
```

### Comparing `DefyDatabase-10.0.0a4.dev202307061815/setup.py` & `DefyDatabase-10.0.0a4.dev202307071900/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import setuptools,defy
+import setuptools,defydb
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DefyDatabase",
-    version=defy.version,
+    version=defydb.version,
     author="Defymen",
     author_email="vmuonline@126.com",
     description="Database for personal data based on SQLite",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    py_modules=['defy'],
+    py_modules=['defydb'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```


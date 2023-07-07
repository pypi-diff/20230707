# Comparing `tmp/gsheet-pandas-0.1.4.tar.gz` & `tmp/gsheet-pandas-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsheet-pandas-0.1.4.tar", last modified: Fri Dec 23 12:02:34 2022, max compression
+gzip compressed data, was "gsheet-pandas-0.1.5.tar", last modified: Fri Jul  7 07:39:26 2023, max compression
```

## Comparing `gsheet-pandas-0.1.4.tar` & `gsheet-pandas-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 iakov      (501) staff       (20)        0 2022-12-23 12:02:34.992115 gsheet-pandas-0.1.4/
--rw-r--r--   0 iakov      (501) staff       (20)     1069 2022-12-20 13:29:05.000000 gsheet-pandas-0.1.4/LICENSE
--rw-r--r--   0 iakov      (501) staff       (20)     3761 2022-12-23 12:02:34.991711 gsheet-pandas-0.1.4/PKG-INFO
-drwxr-xr-x   0 iakov      (501) staff       (20)        0 2022-12-23 12:02:34.988044 gsheet-pandas-0.1.4/gsheet-pandas/
--rw-r--r--   0 iakov      (501) staff       (20)       99 2022-12-22 14:05:52.000000 gsheet-pandas-0.1.4/gsheet-pandas/__init__.py
--rw-r--r--   0 iakov      (501) staff       (20)     4658 2022-12-23 11:56:26.000000 gsheet-pandas-0.1.4/gsheet-pandas/connection.py
--rw-r--r--   0 iakov      (501) staff       (20)     1720 2022-12-23 12:02:34.000000 gsheet-pandas-0.1.4/gsheet-pandas/test.py
-drwxr-xr-x   0 iakov      (501) staff       (20)        0 2022-12-23 12:02:34.991095 gsheet-pandas-0.1.4/gsheet_pandas.egg-info/
--rw-r--r--   0 iakov      (501) staff       (20)     3761 2022-12-23 12:02:34.000000 gsheet-pandas-0.1.4/gsheet_pandas.egg-info/PKG-INFO
--rw-r--r--   0 iakov      (501) staff       (20)      276 2022-12-23 12:02:34.000000 gsheet-pandas-0.1.4/gsheet_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 iakov      (501) staff       (20)        1 2022-12-23 12:02:34.000000 gsheet-pandas-0.1.4/gsheet_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 iakov      (501) staff       (20)       69 2022-12-23 12:02:34.000000 gsheet-pandas-0.1.4/gsheet_pandas.egg-info/requires.txt
--rw-r--r--   0 iakov      (501) staff       (20)       14 2022-12-23 12:02:34.000000 gsheet-pandas-0.1.4/gsheet_pandas.egg-info/top_level.txt
--rw-r--r--   0 iakov      (501) staff       (20)       38 2022-12-23 12:02:34.992243 gsheet-pandas-0.1.4/setup.cfg
--rw-r--r--   0 iakov      (501) staff       (20)      754 2022-12-23 12:02:34.000000 gsheet-pandas-0.1.4/setup.py
+drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 07:39:26.040836 gsheet-pandas-0.1.5/
+-rw-r--r--   0 iakov      (501) staff       (20)     1069 2022-12-20 13:29:05.000000 gsheet-pandas-0.1.5/LICENSE
+-rw-r--r--   0 iakov      (501) staff       (20)     3761 2023-07-07 07:39:26.040522 gsheet-pandas-0.1.5/PKG-INFO
+drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 07:39:26.037983 gsheet-pandas-0.1.5/gsheet-pandas/
+-rw-r--r--   0 iakov      (501) staff       (20)      107 2023-07-07 07:38:06.000000 gsheet-pandas-0.1.5/gsheet-pandas/__init__.py
+-rw-r--r--   0 iakov      (501) staff       (20)     1733 2023-07-07 07:35:02.000000 gsheet-pandas-0.1.5/gsheet-pandas/test.py
+drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 07:39:26.040002 gsheet-pandas-0.1.5/gsheet_pandas.egg-info/
+-rw-r--r--   0 iakov      (501) staff       (20)     3761 2023-07-07 07:39:25.000000 gsheet-pandas-0.1.5/gsheet_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 iakov      (501) staff       (20)      248 2023-07-07 07:39:25.000000 gsheet-pandas-0.1.5/gsheet_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 iakov      (501) staff       (20)        1 2023-07-07 07:39:25.000000 gsheet-pandas-0.1.5/gsheet_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 iakov      (501) staff       (20)       69 2023-07-07 07:39:25.000000 gsheet-pandas-0.1.5/gsheet_pandas.egg-info/requires.txt
+-rw-r--r--   0 iakov      (501) staff       (20)       14 2023-07-07 07:39:25.000000 gsheet-pandas-0.1.5/gsheet_pandas.egg-info/top_level.txt
+-rw-r--r--   0 iakov      (501) staff       (20)       38 2023-07-07 07:39:26.040961 gsheet-pandas-0.1.5/setup.cfg
+-rw-r--r--   0 iakov      (501) staff       (20)      754 2023-07-07 07:38:06.000000 gsheet-pandas-0.1.5/setup.py
```

### Comparing `gsheet-pandas-0.1.4/LICENSE` & `gsheet-pandas-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gsheet-pandas-0.1.4/PKG-INFO` & `gsheet-pandas-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsheet-pandas
-Version: 0.1.4
+Version: 0.1.5
 Summary: Download and upload pandas dataframes to the Google sheets
 Home-page: https://github.com/iakov-kaiumov/gsheet-pandas
 Author: Iakov Kaiumov
 Author-email: kaiumov.iag@phystech.edu
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gsheet-pandas-0.1.4/gsheet-pandas/test.py` & `gsheet-pandas-0.1.5/gsheet-pandas/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import random
 import unittest
 
 from pathlib import Path
 
 import pandas as pd
 
-import connection
+from adapter import connection
 
 
 class TestConnectionMethods(unittest.TestCase):
 
     def test_connection_class(self):
         table_name = os.environ['table_name']
         sheet_name = os.environ['sheet_name']
```

### Comparing `gsheet-pandas-0.1.4/gsheet_pandas.egg-info/PKG-INFO` & `gsheet-pandas-0.1.5/gsheet_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsheet-pandas
-Version: 0.1.4
+Version: 0.1.5
 Summary: Download and upload pandas dataframes to the Google sheets
 Home-page: https://github.com/iakov-kaiumov/gsheet-pandas
 Author: Iakov Kaiumov
 Author-email: kaiumov.iag@phystech.edu
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gsheet-pandas-0.1.4/setup.py` & `gsheet-pandas-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 BASE_DIR = Path(__file__).parent
 long_description = (BASE_DIR / "readme.md").read_text()
 
 setup(
     name='gsheet-pandas',
-    version='0.1.4',
+    version='0.1.5',
     description='Download and upload pandas dataframes to the Google sheets',
     url='https://github.com/iakov-kaiumov/gsheet-pandas',
     author='Iakov Kaiumov',
     author_email='kaiumov.iag@phystech.edu',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT License',
```


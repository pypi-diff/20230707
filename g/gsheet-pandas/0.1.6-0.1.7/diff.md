# Comparing `tmp/gsheet-pandas-0.1.6.tar.gz` & `tmp/gsheet-pandas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsheet-pandas-0.1.6.tar", last modified: Fri Jul  7 07:47:44 2023, max compression
+gzip compressed data, was "gsheet-pandas-0.1.7.tar", last modified: Fri Jul  7 08:05:01 2023, max compression
```

## Comparing `gsheet-pandas-0.1.6.tar` & `gsheet-pandas-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 07:47:44.807977 gsheet-pandas-0.1.6/
--rw-r--r--   0 iakov      (501) staff       (20)     1069 2022-12-20 13:29:05.000000 gsheet-pandas-0.1.6/LICENSE
--rw-r--r--   0 iakov      (501) staff       (20)     3761 2023-07-07 07:47:44.807663 gsheet-pandas-0.1.6/PKG-INFO
-drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 07:47:44.804262 gsheet-pandas-0.1.6/gsheet-pandas/
--rw-r--r--   0 iakov      (501) staff       (20)      107 2023-07-07 07:47:25.000000 gsheet-pandas-0.1.6/gsheet-pandas/__init__.py
-drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 07:47:44.805095 gsheet-pandas-0.1.6/gsheet-pandas/adapter/
--rw-r--r--   0 iakov      (501) staff       (20)        0 2023-07-07 07:34:37.000000 gsheet-pandas-0.1.6/gsheet-pandas/adapter/__init__.py
--rw-r--r--   0 iakov      (501) staff       (20)     4658 2022-12-23 11:56:26.000000 gsheet-pandas-0.1.6/gsheet-pandas/adapter/connection.py
--rw-r--r--   0 iakov      (501) staff       (20)     1733 2023-07-07 07:35:02.000000 gsheet-pandas-0.1.6/gsheet-pandas/test.py
-drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 07:47:44.807142 gsheet-pandas-0.1.6/gsheet_pandas.egg-info/
--rw-r--r--   0 iakov      (501) staff       (20)     3761 2023-07-07 07:47:44.000000 gsheet-pandas-0.1.6/gsheet_pandas.egg-info/PKG-INFO
--rw-r--r--   0 iakov      (501) staff       (20)      318 2023-07-07 07:47:44.000000 gsheet-pandas-0.1.6/gsheet_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 iakov      (501) staff       (20)        1 2023-07-07 07:47:44.000000 gsheet-pandas-0.1.6/gsheet_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 iakov      (501) staff       (20)       69 2023-07-07 07:47:44.000000 gsheet-pandas-0.1.6/gsheet_pandas.egg-info/requires.txt
--rw-r--r--   0 iakov      (501) staff       (20)       14 2023-07-07 07:47:44.000000 gsheet-pandas-0.1.6/gsheet_pandas.egg-info/top_level.txt
--rw-r--r--   0 iakov      (501) staff       (20)       38 2023-07-07 07:47:44.808110 gsheet-pandas-0.1.6/setup.cfg
--rw-r--r--   0 iakov      (501) staff       (20)      767 2023-07-07 07:47:25.000000 gsheet-pandas-0.1.6/setup.py
+drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 08:05:01.171960 gsheet-pandas-0.1.7/
+-rw-r--r--   0 iakov      (501) staff       (20)     1069 2022-12-20 13:29:05.000000 gsheet-pandas-0.1.7/LICENSE
+-rw-r--r--   0 iakov      (501) staff       (20)     3761 2023-07-07 08:05:01.171650 gsheet-pandas-0.1.7/PKG-INFO
+drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 08:05:01.168470 gsheet-pandas-0.1.7/gsheet_pandas/
+-rw-r--r--   0 iakov      (501) staff       (20)      107 2023-07-07 08:04:46.000000 gsheet-pandas-0.1.7/gsheet_pandas/__init__.py
+drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 08:05:01.171132 gsheet-pandas-0.1.7/gsheet_pandas/adapter/
+-rw-r--r--   0 iakov      (501) staff       (20)        0 2023-07-07 07:34:37.000000 gsheet-pandas-0.1.7/gsheet_pandas/adapter/__init__.py
+-rw-r--r--   0 iakov      (501) staff       (20)     4658 2022-12-23 11:56:26.000000 gsheet-pandas-0.1.7/gsheet_pandas/adapter/connection.py
+-rw-r--r--   0 iakov      (501) staff       (20)     1733 2023-07-07 07:35:02.000000 gsheet-pandas-0.1.7/gsheet_pandas/test.py
+drwxr-xr-x   0 iakov      (501) staff       (20)        0 2023-07-07 08:05:01.170437 gsheet-pandas-0.1.7/gsheet_pandas.egg-info/
+-rw-r--r--   0 iakov      (501) staff       (20)     3761 2023-07-07 08:05:01.000000 gsheet-pandas-0.1.7/gsheet_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 iakov      (501) staff       (20)      318 2023-07-07 08:05:01.000000 gsheet-pandas-0.1.7/gsheet_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 iakov      (501) staff       (20)        1 2023-07-07 08:05:01.000000 gsheet-pandas-0.1.7/gsheet_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 iakov      (501) staff       (20)       69 2023-07-07 08:05:01.000000 gsheet-pandas-0.1.7/gsheet_pandas.egg-info/requires.txt
+-rw-r--r--   0 iakov      (501) staff       (20)       14 2023-07-07 08:05:01.000000 gsheet-pandas-0.1.7/gsheet_pandas.egg-info/top_level.txt
+-rw-r--r--   0 iakov      (501) staff       (20)       38 2023-07-07 08:05:01.172091 gsheet-pandas-0.1.7/setup.cfg
+-rw-r--r--   0 iakov      (501) staff       (20)      767 2023-07-07 08:04:46.000000 gsheet-pandas-0.1.7/setup.py
```

### Comparing `gsheet-pandas-0.1.6/LICENSE` & `gsheet-pandas-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gsheet-pandas-0.1.6/PKG-INFO` & `gsheet-pandas-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsheet-pandas
-Version: 0.1.6
+Version: 0.1.7
 Summary: Download and upload pandas dataframes to the Google sheets
 Home-page: https://github.com/iakov-kaiumov/gsheet-pandas
 Author: Iakov Kaiumov
 Author-email: kaiumov.iag@phystech.edu
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gsheet-pandas-0.1.6/gsheet-pandas/adapter/connection.py` & `gsheet-pandas-0.1.7/gsheet_pandas/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `gsheet-pandas-0.1.6/gsheet-pandas/test.py` & `gsheet-pandas-0.1.7/gsheet_pandas/test.py`

 * *Files identical despite different names*

### Comparing `gsheet-pandas-0.1.6/gsheet_pandas.egg-info/PKG-INFO` & `gsheet-pandas-0.1.7/gsheet_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsheet-pandas
-Version: 0.1.6
+Version: 0.1.7
 Summary: Download and upload pandas dataframes to the Google sheets
 Home-page: https://github.com/iakov-kaiumov/gsheet-pandas
 Author: Iakov Kaiumov
 Author-email: kaiumov.iag@phystech.edu
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gsheet-pandas-0.1.6/setup.py` & `gsheet-pandas-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 
 BASE_DIR = Path(__file__).parent
 long_description = (BASE_DIR / "readme.md").read_text()
 
 setup(
     name='gsheet-pandas',
-    version='0.1.6',
+    version='0.1.7',
     description='Download and upload pandas dataframes to the Google sheets',
     url='https://github.com/iakov-kaiumov/gsheet-pandas',
     author='Iakov Kaiumov',
     author_email='kaiumov.iag@phystech.edu',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT License',
     packages=find_packages(),
-    package_dir={'gsheet_pandas': 'gsheet-pandas'},
+    package_dir={'gsheet-pandas': 'gsheet_pandas'},
     install_requires=[
         'google-api-python-client',
         'google-api-core',
         'google-auth-oauthlib',
         'pandas',
     ]
 )
```


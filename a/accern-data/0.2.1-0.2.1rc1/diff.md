# Comparing `tmp/accern_data-0.2.1.tar.gz` & `tmp/accern_data-0.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/accern_data-0.2.1.tar", last modified: Fri Jul  7 12:51:36 2023, max compression
+gzip compressed data, was "dist/accern_data-0.2.1rc1.tar", last modified: Thu Jun 22 12:07:36 2023, max compression
```

## Comparing `accern_data-0.2.1.tar` & `accern_data-0.2.1rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-07-07 12:51:36.597233 accern_data-0.2.1/
--rw-r--r--   0 shaunak    (501) staff       (20)     1063 2023-06-16 10:21:30.000000 accern_data-0.2.1/LICENSE
--rw-r--r--   0 shaunak    (501) staff       (20)     3420 2023-07-07 12:51:36.597394 accern_data-0.2.1/PKG-INFO
--rw-r--r--   0 shaunak    (501) staff       (20)     2692 2023-06-16 10:21:30.000000 accern_data-0.2.1/README.md
-drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-07-07 12:51:36.573041 accern_data-0.2.1/packages/
-drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-07-07 12:51:36.573530 accern_data-0.2.1/packages/python/
-drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-07-07 12:51:36.577515 accern_data-0.2.1/packages/python/accern_data/
--rw-r--r--   0 shaunak    (501) staff       (20)       60 2023-07-07 12:50:24.000000 accern_data-0.2.1/packages/python/accern_data/__init__.py
--rw-r--r--   0 shaunak    (501) staff       (20)        0 2023-06-16 10:21:30.000000 accern_data-0.2.1/packages/python/accern_data/__main__.py
--rw-r--r--   0 shaunak    (501) staff       (20)    58411 2023-06-21 12:04:37.000000 accern_data-0.2.1/packages/python/accern_data/accern_data.py
--rw-r--r--   0 shaunak    (501) staff       (20)        0 2023-06-16 10:21:30.000000 accern_data-0.2.1/packages/python/accern_data/py.typed
--rw-r--r--   0 shaunak    (501) staff       (20)    14488 2023-06-21 12:04:37.000000 accern_data-0.2.1/packages/python/accern_data/util.py
-drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-07-07 12:51:36.579314 accern_data-0.2.1/packages/python/accern_data.egg-info/
--rw-r--r--   0 shaunak    (501) staff       (20)     3420 2023-07-07 12:51:36.000000 accern_data-0.2.1/packages/python/accern_data.egg-info/PKG-INFO
--rw-r--r--   0 shaunak    (501) staff       (20)      729 2023-07-07 12:51:36.000000 accern_data-0.2.1/packages/python/accern_data.egg-info/SOURCES.txt
--rw-r--r--   0 shaunak    (501) staff       (20)        1 2023-07-07 12:51:36.000000 accern_data-0.2.1/packages/python/accern_data.egg-info/dependency_links.txt
--rw-r--r--   0 shaunak    (501) staff       (20)       91 2023-07-07 12:51:36.000000 accern_data-0.2.1/packages/python/accern_data.egg-info/requires.txt
--rw-r--r--   0 shaunak    (501) staff       (20)       12 2023-07-07 12:51:36.000000 accern_data-0.2.1/packages/python/accern_data.egg-info/top_level.txt
--rw-r--r--   0 shaunak    (501) staff       (20)     2288 2023-06-16 10:21:30.000000 accern_data-0.2.1/pyproject.toml
--rw-r--r--   0 shaunak    (501) staff       (20)     1078 2023-07-07 12:51:36.598020 accern_data-0.2.1/setup.cfg
--rw-r--r--   0 shaunak    (501) staff       (20)       38 2023-06-16 10:21:30.000000 accern_data-0.2.1/setup.py
-drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-07-07 12:51:36.583865 accern_data-0.2.1/tests/
-drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-07-07 12:51:36.588661 accern_data-0.2.1/tests/data/
--rw-r--r--   0 shaunak    (501) staff       (20)  1579738 2023-06-16 10:21:30.000000 accern_data-0.2.1/tests/data/data-2022.csv
--rw-r--r--   0 shaunak    (501) staff       (20)  4930620 2023-06-16 10:21:30.000000 accern_data-0.2.1/tests/data/data-2022.json
--rw-r--r--   0 shaunak    (501) staff       (20)     3658 2023-06-16 10:21:31.000000 accern_data-0.2.1/tests/test_by_date.py
--rw-r--r--   0 shaunak    (501) staff       (20)     3380 2023-06-16 10:21:31.000000 accern_data-0.2.1/tests/test_consistency.py
--rw-r--r--   0 shaunak    (501) staff       (20)     4961 2023-06-16 10:21:31.000000 accern_data-0.2.1/tests/test_data_iterator.py
--rw-r--r--   0 shaunak    (501) staff       (20)     4362 2023-06-16 10:21:31.000000 accern_data-0.2.1/tests/test_filters.py
--rw-r--r--   0 shaunak    (501) staff       (20)     1079 2023-06-16 10:21:31.000000 accern_data-0.2.1/tests/test_inconsistent_fields.py
--rw-r--r--   0 shaunak    (501) staff       (20)     4346 2023-06-16 10:21:31.000000 accern_data-0.2.1/tests/test_modes.py
--rw-r--r--   0 shaunak    (501) staff       (20)     4130 2023-06-16 10:21:31.000000 accern_data-0.2.1/tests/test_timestamps.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.313443 accern_data-0.2.1rc1/
+-rw-r--r--   0 shaunak    (501) staff       (20)     1063 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/LICENSE
+-rw-r--r--   0 shaunak    (501) staff       (20)     3423 2023-06-22 12:07:36.313640 accern_data-0.2.1rc1/PKG-INFO
+-rw-r--r--   0 shaunak    (501) staff       (20)     2692 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/README.md
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.281452 accern_data-0.2.1rc1/packages/
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.281907 accern_data-0.2.1rc1/packages/python/
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.287783 accern_data-0.2.1rc1/packages/python/accern_data/
+-rw-r--r--   0 shaunak    (501) staff       (20)       63 2023-06-21 12:50:44.000000 accern_data-0.2.1rc1/packages/python/accern_data/__init__.py
+-rw-r--r--   0 shaunak    (501) staff       (20)        0 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/packages/python/accern_data/__main__.py
+-rw-r--r--   0 shaunak    (501) staff       (20)    58411 2023-06-21 12:04:37.000000 accern_data-0.2.1rc1/packages/python/accern_data/accern_data.py
+-rw-r--r--   0 shaunak    (501) staff       (20)        0 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/packages/python/accern_data/py.typed
+-rw-r--r--   0 shaunak    (501) staff       (20)    14488 2023-06-21 12:04:37.000000 accern_data-0.2.1rc1/packages/python/accern_data/util.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.290165 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/
+-rw-r--r--   0 shaunak    (501) staff       (20)     3423 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/PKG-INFO
+-rw-r--r--   0 shaunak    (501) staff       (20)      729 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)        1 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)       91 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/requires.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)       12 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/top_level.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)     2288 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/pyproject.toml
+-rw-r--r--   0 shaunak    (501) staff       (20)     1078 2023-06-22 12:07:36.314359 accern_data-0.2.1rc1/setup.cfg
+-rw-r--r--   0 shaunak    (501) staff       (20)       38 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/setup.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.294163 accern_data-0.2.1rc1/tests/
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.300358 accern_data-0.2.1rc1/tests/data/
+-rw-r--r--   0 shaunak    (501) staff       (20)  1579738 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/tests/data/data-2022.csv
+-rw-r--r--   0 shaunak    (501) staff       (20)  4930620 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/tests/data/data-2022.json
+-rw-r--r--   0 shaunak    (501) staff       (20)     3658 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_by_date.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     3380 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_consistency.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     4961 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_data_iterator.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     4362 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_filters.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     1079 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_inconsistent_fields.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     4346 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_modes.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     4130 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_timestamps.py
```

### Comparing `accern_data-0.2.1/LICENSE` & `accern_data-0.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/PKG-INFO` & `accern_data-0.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accern_data
-Version: 0.2.1
+Version: 0.2.1rc1
 Summary: Client for consuming Accern data feeds.
 Home-page: https://github.com/Accern/accern-data-client
 Author: Accern Corp.
 Author-email: datascience@accern.com
 License: MIT
 Keywords: api client data feed NLP processing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `accern_data-0.2.1/README.md` & `accern_data-0.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/packages/python/accern_data/accern_data.py` & `accern_data-0.2.1rc1/packages/python/accern_data/accern_data.py`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/packages/python/accern_data/util.py` & `accern_data-0.2.1rc1/packages/python/accern_data/util.py`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/packages/python/accern_data.egg-info/PKG-INFO` & `accern_data-0.2.1rc1/packages/python/accern_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accern-data
-Version: 0.2.1
+Version: 0.2.1rc1
 Summary: Client for consuming Accern data feeds.
 Home-page: https://github.com/Accern/accern-data-client
 Author: Accern Corp.
 Author-email: datascience@accern.com
 License: MIT
 Keywords: api client data feed NLP processing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `accern_data-0.2.1/packages/python/accern_data.egg-info/SOURCES.txt` & `accern_data-0.2.1rc1/packages/python/accern_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/pyproject.toml` & `accern_data-0.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/setup.cfg` & `accern_data-0.2.1rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/data/data-2022.csv` & `accern_data-0.2.1rc1/tests/data/data-2022.csv`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/data/data-2022.json` & `accern_data-0.2.1rc1/tests/data/data-2022.json`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/test_by_date.py` & `accern_data-0.2.1rc1/tests/test_by_date.py`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/test_consistency.py` & `accern_data-0.2.1rc1/tests/test_consistency.py`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/test_data_iterator.py` & `accern_data-0.2.1rc1/tests/test_data_iterator.py`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/test_filters.py` & `accern_data-0.2.1rc1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/test_inconsistent_fields.py` & `accern_data-0.2.1rc1/tests/test_inconsistent_fields.py`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/test_modes.py` & `accern_data-0.2.1rc1/tests/test_modes.py`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.1/tests/test_timestamps.py` & `accern_data-0.2.1rc1/tests/test_timestamps.py`

 * *Files identical despite different names*


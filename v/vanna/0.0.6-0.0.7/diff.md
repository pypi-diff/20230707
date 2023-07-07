# Comparing `tmp/vanna-0.0.6.tar.gz` & `tmp/vanna-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.0.6.tar", last modified: Fri Jul  7 04:23:05 2023, max compression
+gzip compressed data, was "vanna-0.0.7.tar", last modified: Fri Jul  7 21:11:48 2023, max compression
```

## Comparing `vanna-0.0.6.tar` & `vanna-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:23:05.394998 vanna-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 04:22:55.000000 vanna-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 04:23:05.394998 vanna-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 04:22:55.000000 vanna-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 04:22:55.000000 vanna-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 04:23:05.394998 vanna-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:23:05.390998 vanna-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:23:05.390998 vanna-0.0.6/src/vanna/
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-07 04:22:55.000000 vanna-0.0.6/src/vanna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 04:22:55.000000 vanna-0.0.6/src/vanna/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:23:05.394998 vanna-0.0.6/src/vanna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 04:23:05.000000 vanna-0.0.6/src/vanna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:11:48.157350 vanna-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 21:11:34.000000 vanna-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 21:11:48.157350 vanna-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 21:11:34.000000 vanna-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-07 21:11:35.000000 vanna-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:11:48.157350 vanna-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:11:48.157350 vanna-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:11:48.157350 vanna-0.0.7/src/vanna/
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-07 21:11:35.000000 vanna-0.0.7/src/vanna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 21:11:35.000000 vanna-0.0.7/src/vanna/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:11:48.157350 vanna-0.0.7/src/vanna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 21:11:48.000000 vanna-0.0.7/src/vanna.egg-info/top_level.txt
```

### Comparing `vanna-0.0.6/LICENSE` & `vanna-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vanna-0.0.6/PKG-INFO` & `vanna-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vanna-0.0.6/pyproject.toml` & `vanna-0.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vanna"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vanna-0.0.6/src/vanna/__init__.py` & `vanna-0.0.7/src/vanna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,17 +196,19 @@
         if status.success:
             raise Exception(f"An organization with the name {org} already exists")
 
         create = input(f"Would you like to create organization '{org}'? (y/n): ")
 
         if create.lower() == 'y':
             db_type = input("What type of database would you like to use? (Snowflake, BigQuery, Postgres, etc.): ")
+            __org = 'demo-sales'
             if create_org(org=org, db_type=db_type):
                 __org = org
             else:
+                __org = None
                 raise Exception("Failed to create organization")
     else:
         __org = org
 
 def store_sql(question: str, sql: str) -> bool:
     """
     ## Example
```

### Comparing `vanna-0.0.6/src/vanna/types.py` & `vanna-0.0.7/src/vanna/types.py`

 * *Files identical despite different names*

### Comparing `vanna-0.0.6/src/vanna.egg-info/PKG-INFO` & `vanna-0.0.7/src/vanna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/rin_proj1-0.1.3.tar.gz` & `tmp/rin_proj1-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rin_proj1-0.1.3.tar", max compression
+gzip compressed data, was "rin_proj1-1.0.tar", max compression
```

## Comparing `rin_proj1-0.1.3.tar` & `rin_proj1-1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1754 2023-07-07 19:07:11.122670 rin_proj1-0.1.3/README.md
--rw-r--r--   0        0        0      346 2023-07-07 18:46:23.103932 rin_proj1-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 16:49:14.718478 rin_proj1-0.1.3/rin_proj1/__init__.py
--rw-r--r--   0        0        0     1214 2023-07-05 11:43:12.438622 rin_proj1-0.1.3/rin_proj1/db_insert.py
--rw-r--r--   0        0        0      311 2023-07-07 19:40:41.269360 rin_proj1-0.1.3/rin_proj1/get_yaml.py
--rw-r--r--   0        0        0     1817 2023-07-07 19:52:15.242093 rin_proj1-0.1.3/rin_proj1/logerror.py
--rw-r--r--   0        0        0     1965 2023-07-07 19:50:32.419534 rin_proj1-0.1.3/rin_proj1/main.py
--rw-r--r--   0        0        0     2157 1970-01-01 00:00:00.000000 rin_proj1-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1764 2023-07-07 19:54:15.068469 rin_proj1-1.0/README.md
+-rw-r--r--   0        0        0      403 2023-07-07 20:07:03.822864 rin_proj1-1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 16:49:14.718478 rin_proj1-1.0/rin_proj1/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-05 11:43:12.438622 rin_proj1-1.0/rin_proj1/db_insert.py
+-rw-r--r--   0        0        0      311 2023-07-07 19:40:41.269360 rin_proj1-1.0/rin_proj1/get_yaml.py
+-rw-r--r--   0        0        0     1817 2023-07-07 19:52:15.242093 rin_proj1-1.0/rin_proj1/logerror.py
+-rw-r--r--   0        0        0     1965 2023-07-07 19:50:32.419534 rin_proj1-1.0/rin_proj1/main.py
+-rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 rin_proj1-1.0/PKG-INFO
```

### Comparing `rin_proj1-0.1.3/README.md` & `rin_proj1-1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     development,
     testing,
     production
 
 <hr>
 
 Successful execution should print confirmation message in terminal. If there is no output, check for a `mpj1_error.log` file to determine the error.<br><br>
-Expected yaml file layout:
+Expected yaml file layout (minimum):
 
 ```yaml
 LOG_LEVEL: log_level (see below for valid options)
 
 APP_MODE:
   csv_file: path/to/data.csv
   db_file: path/to/data.db
```

### Comparing `rin_proj1-0.1.3/rin_proj1/db_insert.py` & `rin_proj1-1.0/rin_proj1/db_insert.py`

 * *Files identical despite different names*

### Comparing `rin_proj1-0.1.3/rin_proj1/logerror.py` & `rin_proj1-1.0/rin_proj1/logerror.py`

 * *Files identical despite different names*

### Comparing `rin_proj1-0.1.3/rin_proj1/main.py` & `rin_proj1-1.0/rin_proj1/main.py`

 * *Files identical despite different names*

### Comparing `rin_proj1-0.1.3/PKG-INFO` & `rin_proj1-1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: rin-proj1
-Version: 0.1.3
-Summary: 
+Version: 1.0
+Summary: CLI tool convert .csv files to .db files and vice-versa
 Author: Harine
-Author-email: you@example.com
+Author-email: haariinee@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
@@ -54,15 +54,15 @@
     development,
     testing,
     production
 
 <hr>
 
 Successful execution should print confirmation message in terminal. If there is no output, check for a `mpj1_error.log` file to determine the error.<br><br>
-Expected yaml file layout:
+Expected yaml file layout (minimum):
 
 ```yaml
 LOG_LEVEL: log_level (see below for valid options)
 
 APP_MODE:
   csv_file: path/to/data.csv
   db_file: path/to/data.db
```


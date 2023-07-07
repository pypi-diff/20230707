# Comparing `tmp/rin_proj1-0.1.0.tar.gz` & `tmp/rin_proj1-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rin_proj1-0.1.0.tar", max compression
+gzip compressed data, was "rin_proj1-0.1.2.tar", max compression
```

## Comparing `rin_proj1-0.1.0.tar` & `rin_proj1-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1303 2023-07-07 12:59:52.638007 rin_proj1-0.1.0/README.md
--rw-r--r--   0        0        0      348 2023-07-07 13:07:41.895116 rin_proj1-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 16:49:14.718478 rin_proj1-0.1.0/rin_proj1/__init__.py
--rw-r--r--   0        0        0     1214 2023-07-05 11:43:12.438622 rin_proj1-0.1.0/rin_proj1/db_insert.py
--rw-r--r--   0        0        0      153 2023-07-06 06:38:48.667749 rin_proj1-0.1.0/rin_proj1/get_yaml.py
--rw-r--r--   0        0        0     1732 2023-07-07 12:43:57.960019 rin_proj1-0.1.0/rin_proj1/logerror.py
--rw-r--r--   0        0        0     2118 2023-07-07 13:08:31.046597 rin_proj1-0.1.0/rin_proj1/main.py
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 rin_proj1-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1464 2023-07-07 18:00:49.495923 rin_proj1-0.1.2/README.md
+-rw-r--r--   0        0        0      344 2023-07-07 16:47:31.624858 rin_proj1-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 16:49:14.718478 rin_proj1-0.1.2/rin_proj1/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-05 11:43:12.438622 rin_proj1-0.1.2/rin_proj1/db_insert.py
+-rw-r--r--   0        0        0      322 2023-07-07 16:46:52.268137 rin_proj1-0.1.2/rin_proj1/get_yaml.py
+-rw-r--r--   0        0        0     1901 2023-07-07 17:55:51.379944 rin_proj1-0.1.2/rin_proj1/logerror.py
+-rw-r--r--   0        0        0     1980 2023-07-07 17:58:35.615410 rin_proj1-0.1.2/rin_proj1/main.py
+-rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 rin_proj1-0.1.2/PKG-INFO
```

### Comparing `rin_proj1-0.1.0/README.md` & `rin_proj1-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,58 @@
+Metadata-Version: 2.1
+Name: rin-proj1
+Version: 0.1.2
+Summary: 
+Author: Harine
+Author-email: you@example.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Description-Content-Type: text/markdown
+
 <h1> command usage (CLI) </h1>
 See list of commands with
 
 ```
-main --help
+rin_pj1 --help
 ```
+Error logging is only compatible with `exec-based-on-env`<br>
 <b>read_csv_and_insert_to_db :</b> Adds contents of provided csv to a .db file<br>
 <b>export_db_to_csv :</b> Adds contents of provided db to a .csv file
-<h2>get-config</h2>
+<h2>set-config</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the given config file.
 If no path is provided, tries to open config.yaml in the current directory.<br>
 
 ```commandline
-main get-config --path path/to/config.yaml
+ rin_pj1 set-config --path path/to/config.yaml
 ```
 for default/config in current directory, use ```main1```
 
 <hr>
-<h2>get-db</h2>
+<h2>set-db</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the db_name provided by user.<br>
 
-```main get-db``` saves data.db in current directory<br>
-```main get-db db_name``` saves to db_name in current directory. Will create a file if not present<br>
+```rin_pj1 set-db``` saves data.db in current directory<br>
+```rin_pj1 set-db db_name``` saves to db_name in current directory. Will create a file if not present<br>
 
 <hr>
-<h2>get-env</h2>
+<h2>exec-based-on-env</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with csv file depending on the environment type<br>
 
 ```bash
-main get-env
+rin_pj1 exec-based-on-env
 ```
 If you want to run the command in a different environment,
 ```bash
 poetry shell
 export APP_MODE="env_name"
-main get-env
+main exec-based-on-env
 ```
 
-available ```env_name``` options are development, testing and production.
+Available ```env_name``` options are development, testing and production.
 
 <hr>
 
-The above commands can be run with poetry as well. Add ```poetry run``` in front of each command)
+Successful executioni should print confirmation message in terminal. If there is no output, check for a `mpj1_errors.log` file to determine the error.
```

### Comparing `rin_proj1-0.1.0/rin_proj1/db_insert.py` & `rin_proj1-0.1.2/rin_proj1/db_insert.py`

 * *Files identical despite different names*

### Comparing `rin_proj1-0.1.0/rin_proj1/logerror.py` & `rin_proj1-0.1.2/rin_proj1/logerror.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 from typing import Callable
 import logging
 from functools import wraps
 from os import environ
+from rin_proj1.get_yaml import get_yaml
 
 log_map = {
     "critical": logging.CRITICAL,
     "error": logging.ERROR,
     "warning": logging.WARNING,
     "info": logging.INFO,
     "debug": logging.DEBUG,
     "": logging.NOTSET
 }
 
 
+def error_branch(e):
+    if isinstance(e, FileNotFoundError):
+        if "config.yaml" in e.filename:
+            logging.error("Config file can't be found in the current directory. "
+                          f"Create a config.yaml file or run command in directory "
+                          f"containing config.yaml")
+        else:
+            logging.error(f"{e.filename} can't be accessed. Check if it exists or if it has read "
+                          f"permissions enabled.")
+    elif isinstance(e, AttributeError):
+        logging.error("config.yaml can't be read. Is the config file empty?")
+    elif isinstance(e, KeyError):
+        if e.args[0] in ['production', 'development', 'testing']:
+            logging.error(f"{key_error.args[0]} doesn't exist. Check config file")
+    elif isinstance(e, TypeError):
+        logging.error("Check values in csv/db file. TypeError encountered.")
+    else:
+        logging.error(f"Encountered error. Traceback:\n{e}")
+
+
 def log_error(func) -> Callable[[...], None]:
     @wraps(func)
     def wrapper(*args, **kwargs) -> None:
         try:
-            logging.basicConfig(filename='mpj1_errors.log', filemode='w',
-                                encoding='utf-8', level=log_map[environ.get("LOG_LEVEL")],
-                                format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-            func(*args, **kwargs)
-        except FileNotFoundError as no_file:
-            if "config.yaml" in no_file.filename:
-                logging.error("Config file can't be found in the current directory. "
-                              f"Create a config.yaml file or run command in directory "
-                              f"containing config.yaml")
-                return
-            else:
-                logging.error(f"{no_file.filename} can't be accessed. Check if it exists or if it has read "
-                              f"permissions enabled.")
-                return
-        except AttributeError:
-            logging.error("config.yaml can't be read. Is the config file empty?")
-            return
-        except KeyError as key_error:
-            if key_error.args[0] in ['production', 'development', 'testing']:
-                logging.error(f"{key_error.args[0]} doesn't exist. Check config file")
-            return
+            log_lvl = get_yaml("config.yaml").get("LOG_LEVEL")
         except Exception as e:
-            logging.error(f"Encountered error. Traceback:\n{e.__traceback__}")
+            error_branch(e)
+            return
 
+        try:
+            logging.basicConfig(filename='mpj1_errors.log', format='%(asctime)s - %(message)s',
+                                encoding='utf-8', level=log_map[log_lvl],
+                                )
+            func(*args, **kwargs)
+        except Exception as e:
+            error_branch(e)
+            return
     return wrapper
```

### Comparing `rin_proj1-0.1.0/rin_proj1/main.py` & `rin_proj1-0.1.2/rin_proj1/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
 import os
-from rin_proj1.get_yaml import get_yaml
+from rin_proj1.get_yaml import get_yaml, return_appmode_dict
 from rin_proj1.db_insert import read_csv_and_insert_to_db as csv2db
 from rin_proj1.db_insert import export_db_to_csv as db2csv
 from rin_proj1.logerror import log_error
 
 app = typer.Typer()
 
 
@@ -26,14 +26,15 @@
     db2csv(db_file, tb_name, "../new_csv.csv")
 
     print(f"Finished execution and created files in {db_file} and new_csv.csv")
 
 
 # task 4
 @app.command()
+@log_error
 def set_db(path: str) -> None:
     """get custom db path
     :type path: str
     """
     config_data = get_yaml("config.yaml")
     db_file = path
 
@@ -43,20 +44,14 @@
     csv2db(csv_file, db_file, tb_name)
     db2csv(db_file, tb_name, "../new_csv.csv")
 
     print("Executed without errors")
 
 
 # task 5
-def return_appmode_dict(app_mode: str) -> dict:
-    set_mode = get_yaml("config.yaml").get(app_mode, {})
-    print(f"MODE: {set_mode['validate']}")
-    return set_mode
-
-
 @app.command()
 @log_error
 def exec_based_on_env() -> None:
     """get files based on environment and execute functions"""
     app_mode = os.environ.get("APP_MODE", "development")    # get the env, if None then defaults to dev
     config = return_appmode_dict(app_mode)
```


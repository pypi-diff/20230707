# Comparing `tmp/rin_proj1-0.1.2.tar.gz` & `tmp/rin_proj1-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rin_proj1-0.1.2.tar", max compression
+gzip compressed data, was "rin_proj1-0.1.3.tar", max compression
```

## Comparing `rin_proj1-0.1.2.tar` & `rin_proj1-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1464 2023-07-07 18:00:49.495923 rin_proj1-0.1.2/README.md
--rw-r--r--   0        0        0      344 2023-07-07 16:47:31.624858 rin_proj1-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 16:49:14.718478 rin_proj1-0.1.2/rin_proj1/__init__.py
--rw-r--r--   0        0        0     1214 2023-07-05 11:43:12.438622 rin_proj1-0.1.2/rin_proj1/db_insert.py
--rw-r--r--   0        0        0      322 2023-07-07 16:46:52.268137 rin_proj1-0.1.2/rin_proj1/get_yaml.py
--rw-r--r--   0        0        0     1901 2023-07-07 17:55:51.379944 rin_proj1-0.1.2/rin_proj1/logerror.py
--rw-r--r--   0        0        0     1980 2023-07-07 17:58:35.615410 rin_proj1-0.1.2/rin_proj1/main.py
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 rin_proj1-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1754 2023-07-07 19:07:11.122670 rin_proj1-0.1.3/README.md
+-rw-r--r--   0        0        0      346 2023-07-07 18:46:23.103932 rin_proj1-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 16:49:14.718478 rin_proj1-0.1.3/rin_proj1/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-05 11:43:12.438622 rin_proj1-0.1.3/rin_proj1/db_insert.py
+-rw-r--r--   0        0        0      311 2023-07-07 19:40:41.269360 rin_proj1-0.1.3/rin_proj1/get_yaml.py
+-rw-r--r--   0        0        0     1817 2023-07-07 19:52:15.242093 rin_proj1-0.1.3/rin_proj1/logerror.py
+-rw-r--r--   0        0        0     1965 2023-07-07 19:50:32.419534 rin_proj1-0.1.3/rin_proj1/main.py
+-rw-r--r--   0        0        0     2157 1970-01-01 00:00:00.000000 rin_proj1-0.1.3/PKG-INFO
```

### Comparing `rin_proj1-0.1.2/README.md` & `rin_proj1-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 <h1> command usage (CLI) </h1>
 See list of commands with
 
 ```
-rin_pj1 --help
+rin_proj1 --help
 ```
 Error logging is only compatible with `exec-based-on-env`<br>
 <b>read_csv_and_insert_to_db :</b> Adds contents of provided csv to a .db file<br>
 <b>export_db_to_csv :</b> Adds contents of provided db to a .csv file
 <h2>set-config</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the given config file.
 If no path is provided, tries to open config.yaml in the current directory.<br>
 
 ```commandline
- rin_pj1 set-config --path path/to/config.yaml
+ rin_proj1 set-config --path path/to/config.yaml
 ```
 for default/config in current directory, use ```main1```
 
 <hr>
 <h2>set-db</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the db_name provided by user.<br>
 
-```rin_pj1 set-db``` saves data.db in current directory<br>
-```rin_pj1 set-db db_name``` saves to db_name in current directory. Will create a file if not present<br>
+```rin_proj1 set-db``` saves data.db in current directory<br>
+```rin_proj1 set-db db_name``` saves to db_name in current directory. Will create a file if not present<br>
 
 <hr>
 <h2>exec-based-on-env</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with csv file depending on the environment type<br>
 
 ```bash
-rin_pj1 exec-based-on-env
+rin_proj1 exec-based-on-env
 ```
 If you want to run the command in a different environment,
 ```bash
 poetry shell
-export APP_MODE="env_name"
-main exec-based-on-env
+export APP_MODE=env_name
+rin_proj1 exec-based-on-env
 ```
-
-Available ```env_name``` options are development, testing and production.
+> <b>env_name options:</b>
+    development,
+    testing,
+    production
 
 <hr>
 
-Successful executioni should print confirmation message in terminal. If there is no output, check for a `mpj1_errors.log` file to determine the error.
+Successful execution should print confirmation message in terminal. If there is no output, check for a `mpj1_error.log` file to determine the error.<br><br>
+Expected yaml file layout:
+
+```yaml
+LOG_LEVEL: log_level (see below for valid options)
+
+APP_MODE:
+  csv_file: path/to/data.csv
+  db_file: path/to/data.db
+  table_file: your_table_name
+```
+> <b>log_level options:</b>
+    critical,
+    error,
+    warning,
+    info,
+    debug
```

### Comparing `rin_proj1-0.1.2/rin_proj1/db_insert.py` & `rin_proj1-0.1.3/rin_proj1/db_insert.py`

 * *Files identical despite different names*

### Comparing `rin_proj1-0.1.2/rin_proj1/logerror.py` & `rin_proj1-0.1.3/rin_proj1/logerror.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,32 @@
                           f"containing config.yaml")
         else:
             logging.error(f"{e.filename} can't be accessed. Check if it exists or if it has read "
                           f"permissions enabled.")
     elif isinstance(e, AttributeError):
         logging.error("config.yaml can't be read. Is the config file empty?")
     elif isinstance(e, KeyError):
-        if e.args[0] in ['production', 'development', 'testing']:
-            logging.error(f"{key_error.args[0]} doesn't exist. Check config file")
+        logging.error(f"KEY {e.args[0]} doesn't exist. Check config file")
     elif isinstance(e, TypeError):
         logging.error("Check values in csv/db file. TypeError encountered.")
     else:
-        logging.error(f"Encountered error. Traceback:\n{e}")
+        logging.error(f"Encountered error with message {e}")
 
 
 def log_error(func) -> Callable[[...], None]:
     @wraps(func)
     def wrapper(*args, **kwargs) -> None:
         try:
-            log_lvl = get_yaml("config.yaml").get("LOG_LEVEL")
+            log_lvl = get_yaml("config.yaml").get("LOG_LEVEL", "")
         except Exception as e:
             error_branch(e)
             return
 
         try:
-            logging.basicConfig(filename='mpj1_errors.log', format='%(asctime)s - %(message)s',
-                                encoding='utf-8', level=log_map[log_lvl],
-                                )
+            logging.basicConfig(filename='mpj1_error.log', format='%(asctime)s - %(message)s',
+                                encoding='utf-8', level=log_map[log_lvl])
             func(*args, **kwargs)
         except Exception as e:
+            print(e)
             error_branch(e)
             return
     return wrapper
```

### Comparing `rin_proj1-0.1.2/rin_proj1/main.py` & `rin_proj1-0.1.3/rin_proj1/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,16 @@
     db2csv(db_file, tb_name, "../new_csv.csv")
 
     print(f"Finished execution and created files in {db_file} and new_csv.csv")
 
 
 # task 4
 @app.command()
-@log_error
 def set_db(path: str) -> None:
     """get custom db path
-    :type path: str
     """
     config_data = get_yaml("config.yaml")
     db_file = path
 
     csv_file: str = config_data.get('csv_file', "data.csv")
     tb_name: str = config_data.get('table_file', "data")
 
@@ -47,23 +45,25 @@
     print("Executed without errors")
 
 
 # task 5
 @app.command()
 @log_error
 def exec_based_on_env() -> None:
-    """get files based on environment and execute functions"""
+    """
+    [logging supported]
+    get files based on environment and execute functions"""
     app_mode = os.environ.get("APP_MODE", "development")    # get the env, if None then defaults to dev
     config = return_appmode_dict(app_mode)
 
     csv_file: str = config.get('csv_file', 'data.csv')
     db_file: str = config.get('db_file', 'data.db')
     tb_name: str = config.get('table_file', 'data')
 
     csv2db(csv_file, db_file, tb_name)
-    db2csv(db_file, tb_name, "../new_csv.csv")
+    db2csv(db_file, tb_name, "new_csv.csv")
 
-    print(f"Created files {config['db_file']} and new_csv.csv")
+    print(f"Created files {db_file} and new_csv.csv")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `rin_proj1-0.1.2/PKG-INFO` & `rin_proj1-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rin-proj1
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Harine
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,47 +12,65 @@
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 <h1> command usage (CLI) </h1>
 See list of commands with
 
 ```
-rin_pj1 --help
+rin_proj1 --help
 ```
 Error logging is only compatible with `exec-based-on-env`<br>
 <b>read_csv_and_insert_to_db :</b> Adds contents of provided csv to a .db file<br>
 <b>export_db_to_csv :</b> Adds contents of provided db to a .csv file
 <h2>set-config</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the given config file.
 If no path is provided, tries to open config.yaml in the current directory.<br>
 
 ```commandline
- rin_pj1 set-config --path path/to/config.yaml
+ rin_proj1 set-config --path path/to/config.yaml
 ```
 for default/config in current directory, use ```main1```
 
 <hr>
 <h2>set-db</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with the db_name provided by user.<br>
 
-```rin_pj1 set-db``` saves data.db in current directory<br>
-```rin_pj1 set-db db_name``` saves to db_name in current directory. Will create a file if not present<br>
+```rin_proj1 set-db``` saves data.db in current directory<br>
+```rin_proj1 set-db db_name``` saves to db_name in current directory. Will create a file if not present<br>
 
 <hr>
 <h2>exec-based-on-env</h2>
 Executes read_csv_and_insert_to_db and export_db_to_csv functions with csv file depending on the environment type<br>
 
 ```bash
-rin_pj1 exec-based-on-env
+rin_proj1 exec-based-on-env
 ```
 If you want to run the command in a different environment,
 ```bash
 poetry shell
-export APP_MODE="env_name"
-main exec-based-on-env
+export APP_MODE=env_name
+rin_proj1 exec-based-on-env
 ```
-
-Available ```env_name``` options are development, testing and production.
+> <b>env_name options:</b>
+    development,
+    testing,
+    production
 
 <hr>
 
-Successful executioni should print confirmation message in terminal. If there is no output, check for a `mpj1_errors.log` file to determine the error.
+Successful execution should print confirmation message in terminal. If there is no output, check for a `mpj1_error.log` file to determine the error.<br><br>
+Expected yaml file layout:
+
+```yaml
+LOG_LEVEL: log_level (see below for valid options)
+
+APP_MODE:
+  csv_file: path/to/data.csv
+  db_file: path/to/data.db
+  table_file: your_table_name
+```
+> <b>log_level options:</b>
+    critical,
+    error,
+    warning,
+    info,
+    debug
```


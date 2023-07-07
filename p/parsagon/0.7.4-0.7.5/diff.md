# Comparing `tmp/parsagon-0.7.4.tar.gz` & `tmp/parsagon-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.7.4.tar", last modified: Fri Jun 30 06:02:48 2023, max compression
+gzip compressed data, was "parsagon-0.7.5.tar", last modified: Fri Jul  7 07:06:03 2023, max compression
```

## Comparing `parsagon-0.7.4.tar` & `parsagon-0.7.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.120802 parsagon-0.7.4/
--rw-r--r--   0 amsuh    (10002)    18010     1444 2023-06-30 06:02:48.120453 parsagon-0.7.4/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.4/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1026 2023-06-30 06:02:23.000000 parsagon-0.7.4/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-30 06:02:48.120917 parsagon-0.7.4/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.110165 parsagon-0.7.4/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.4/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.114695 parsagon-0.7.4/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       54 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     4355 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.4/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      819 2023-06-30 00:46:35.000000 parsagon-0.7.4/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    11215 2023-06-30 05:36:14.000000 parsagon-0.7.4/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     7003 2023-06-30 05:58:11.000000 parsagon-0.7.4/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     1570 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.119802 parsagon-0.7.4/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.4/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.117154 parsagon-0.7.4/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1444 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      606 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      250 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.930888 parsagon-0.7.5/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-07 07:06:03.930194 parsagon-0.7.5/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.7.5/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1048 2023-07-07 07:03:35.000000 parsagon-0.7.5/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-07-07 07:06:03.931098 parsagon-0.7.5/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.913092 parsagon-0.7.5/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.5/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.918980 parsagon-0.7.5/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     4632 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.5/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    11215 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     9044 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     2883 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.929247 parsagon-0.7.5/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.5/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/test_invalid_args.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.7.5/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-07-07 07:06:03.924101 parsagon-0.7.5/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      646 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      263 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-07-07 07:06:03.000000 parsagon-0.7.5/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.7.4/PKG-INFO` & `parsagon-0.7.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.4
+Version: 0.7.5
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -20,29 +20,51 @@
 
 ## Installation
 
 To get started, install the Parsagon python package:
 
 `pip install parsagon`
 
-and set your API key as an environment variable:
+Then run
 
-`export PARSAGON_API_KEY=<YOUR API KEY>`
+`parsagon setup`
 
-Please contact us to get your API key if you don't have it already.
+and copy-paste your API key when prompted.
+
+You can view your API key by logging in and going to <https://parsagon.io/settings>
 
 ## Usage
 
+From command line:
+
+```
+# Create a program
+parsagon create
+
+# Run a program
+parsagon run 'My program'
+
+# List your programs
+parsagon detail
+
+# Delete a program
+parsagon delete 'My program'
+```
+
+From Python:
 ```
 import parsagon
 
 # Create a program
-parsagon.create('Go to https://www.google.com/. Type "the meaning of life" into the search bar and hit enter. Scroll down and click the "More results" button 3 times. Scrape data in the format [{"title": "str", "link": "link"}].')
+parsagon.create('Go to https://www.google.com/. Type "the meaning of life" into the search bar and hit enter. Scroll down and click the "More results" button 3 times. Scrape data in the format [{"search result title": "str", "link": "link"}].')
 
 # Run a program
 parsagon.run("My program")
 
 # List your programs
 parsagon.detail()
+
+# Delete a program
+parsagon.delete("My program")
 ```
 
 See [the docs](https://parsagon.io/docs/pipelines/overview) for more information.
```

### Comparing `parsagon-0.7.4/README.md` & `parsagon-0.7.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -8,29 +8,51 @@
 
 ## Installation
 
 To get started, install the Parsagon python package:
 
 `pip install parsagon`
 
-and set your API key as an environment variable:
+Then run
 
-`export PARSAGON_API_KEY=<YOUR API KEY>`
+`parsagon setup`
 
-Please contact us to get your API key if you don't have it already.
+and copy-paste your API key when prompted.
+
+You can view your API key by logging in and going to <https://parsagon.io/settings>
 
 ## Usage
 
+From command line:
+
+```
+# Create a program
+parsagon create
+
+# Run a program
+parsagon run 'My program'
+
+# List your programs
+parsagon detail
+
+# Delete a program
+parsagon delete 'My program'
+```
+
+From Python:
 ```
 import parsagon
 
 # Create a program
-parsagon.create('Go to https://www.google.com/. Type "the meaning of life" into the search bar and hit enter. Scroll down and click the "More results" button 3 times. Scrape data in the format [{"title": "str", "link": "link"}].')
+parsagon.create('Go to https://www.google.com/. Type "the meaning of life" into the search bar and hit enter. Scroll down and click the "More results" button 3 times. Scrape data in the format [{"search result title": "str", "link": "link"}].')
 
 # Run a program
 parsagon.run("My program")
 
 # List your programs
 parsagon.detail()
+
+# Delete a program
+parsagon.delete("My program")
 ```
 
 See [the docs](https://parsagon.io/docs/pipelines/overview) for more information.
```

### Comparing `parsagon-0.7.4/pyproject.toml` & `parsagon-0.7.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.7.4"
+version = "0.7.5"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
@@ -22,14 +22,15 @@
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     'selenium == 4.9.1',
     'lxml == 4.9.2',
     'httpx == 0.24.1',
+    'halo == 0.0.31',
 
     # Used only in pipeline code execution
     'pandas==1.4.2',
     'PyVirtualDisplay==3.0',
     'selenium-wire==5.1.0',
     'cssselect==1.1.0',
     'undetected-chromedriver==3.1.5.post4',
```

### Comparing `parsagon-0.7.4/src/parsagon/api.py` & `parsagon-0.7.5/src/parsagon/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,18 +116,35 @@
         )
 
 
 def get_pipelines():
     return _api_call(httpx.get, f"/pipelines/")
 
 
-def get_pipeline_code(pipeline_name, variables, environment, headless):
+def get_pipeline_code(pipeline_name, variables, headless):
     with RaiseProgramNotFound(pipeline_name):
         return _api_call(
             httpx.post,
             f"/pipelines/name/{pipeline_name}/code/",
             json={
                 "variables": variables,
-                "environment": environment,
                 "headless": headless,
             },
         )
+
+
+def create_pipeline_run(pipeline_id, variables):
+    return _api_call(
+        httpx.post,
+        f"/pipelines/{pipeline_id}/runs/",
+        json={"variables": variables},
+    )
+
+
+def get_run(run_id):
+    """
+    Gets details about a run
+    """
+    return _api_call(
+        httpx.get,
+        f"/pipelines/runs/{run_id}/",
+    )
```

### Comparing `parsagon-0.7.4/src/parsagon/custom_function.py` & `parsagon-0.7.5/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.4/src/parsagon/exceptions.py` & `parsagon-0.7.5/src/parsagon/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.4/src/parsagon/executor.py` & `parsagon-0.7.5/src/parsagon/executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.4/src/parsagon/main.py` & `parsagon-0.7.5/src/parsagon/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import argparse
 import json
 import logging
 import logging.config
+import time
+
+from halo import Halo
 
-from parsagon import settings
 from parsagon.api import (
     get_program_sketches,
     create_pipeline,
     delete_pipeline,
     create_custom_function,
+    create_pipeline_run,
     get_pipeline,
     get_pipelines,
     get_pipeline_code,
+    get_run,
     APIException,
 )
 from parsagon.exceptions import ParsagonException
 from parsagon.executor import Executor, custom_functions_to_descriptions
+from parsagon.settings import get_api_key, get_settings, clear_settings, save_setting, get_logging_config
 
 logger = logging.getLogger(__name__)
 
 
 def configure_logging(verbose):
-    logging.config.dictConfig(settings.get_logging_config("DEBUG" if verbose else "INFO"))
+    logging.config.dictConfig(get_logging_config("DEBUG" if verbose else "INFO"))
 
 
 def get_args():
     parser = argparse.ArgumentParser(
         prog="parsagon", description="Scrapes and interacts with web pages based on natural language.", add_help=False
     )
     parser.add_argument("-v", "--verbose", action="store_true", help="run the task in verbose mode")
@@ -83,27 +88,43 @@
         help="a JSON object mapping variables to values",
     )
     parser_run.add_argument(
         "--headless",
         action="store_true",
         help="run the browser in headless mode",
     )
+    parser_run.add_argument(
+        "--remote",
+        action="store_true",
+        help="run the program in the cloud",
+    )
     parser_run.set_defaults(func=run)
 
     # Delete
     parser_delete = subparsers.add_parser(
         "delete",
         description="Deletes a program.",
     )
     parser_delete.add_argument(
         "program_name",
         type=str,
         help="the name of the program to run",
     )
+    parser_delete.add_argument(
+        "-y", "--yes", dest="confirm_with_user", action="store_false", help="auto-confirm option"
+    )
     parser_delete.set_defaults(func=delete)
+
+    # Setup
+    parser_setup = subparsers.add_parser(
+        "setup",
+        description="Interactively sets up Parsagon with an API key.",
+    )
+    parser_setup.set_defaults(func=setup)
+
     args = parser.parse_args()
     kwargs = vars(args)
     return kwargs, parser
 
 
 def main():
     kwargs, parser = get_args()
@@ -185,33 +206,73 @@
         data = get_pipelines()
     for pipeline in data:
         print(
             f"Program: {pipeline['name']}\nDescription: {pipeline['description']}\nVariables: {pipeline['variables']}\n"
         )
 
 
-def run(program_name, variables={}, environment="LOCAL", headless=False, verbose=False):
+def run(program_name, variables={}, headless=False, remote=False, verbose=False):
     """
     Executes pipeline code
     """
+    if headless and remote:
+        raise ParsagonException("Cannot run a program remotely in headless mode")
+
+    if remote:
+        pipeline_id = get_pipeline(program_name)["id"]
+        result = create_pipeline_run(pipeline_id, variables)
+        with Halo(text="Program running remotely...", spinner="dots"):
+            while True:
+                run = get_run(result["id"])
+                status = run["status"]
+                if status == "FINISHED":
+                    logger.info("Program finished running.")
+                    return run["output"]
+                elif status == "ERROR":
+                    raise ParsagonException(f"Program failed to run: {run['error']}")
+                elif status == "CANCELED":
+                    raise ParsagonException("Program execution was canceled")
+                time.sleep(5)
+
     logger.info("Preparing to run program %s", program_name)
-    code = get_pipeline_code(program_name, variables, environment, headless)["code"]
+    code = get_pipeline_code(program_name, variables, headless)["code"]
 
     logger.info("Running program...")
-    globals_locals = {"PARSAGON_API_KEY": settings.get_api_key()}
+    globals_locals = {"PARSAGON_API_KEY": get_api_key()}
     try:
         exec(code, globals_locals, globals_locals)
     finally:
         if "driver" in globals_locals:
             globals_locals["driver"].quit()
         if "display" in globals_locals:
             globals_locals["display"].stop()
     logger.info("Done.")
     return globals_locals["output"]
 
 
-def delete(program_name, verbose=False):
+def delete(program_name, verbose=False, confirm_with_user=False):
+    if (
+        confirm_with_user
+        and input(f"Are you sure you want to delete program with name {program_name}? (y/N) ").lower().strip() != "y"
+    ):
+        logger.error("Cancelled operation.")
+        return
     logger.info("Preparing to delete program %s", program_name)
     pipeline_id = get_pipeline(program_name)["id"]
     logger.info("Deleting program...")
     delete_pipeline(pipeline_id)
     logger.info("Done.")
+
+
+def setup(verbose=False):
+    try:
+        old_api_key = get_api_key()
+    except ParsagonException:
+        old_api_key = None
+    try:
+        save_setting("api_key", None)
+        get_api_key(interactive=True)
+    except KeyboardInterrupt:
+        save_setting("api_key", old_api_key)
+        logger.error("\nCancelled operation.")
+        return
+    logger.info("Setup complete.")
```

### Comparing `parsagon-0.7.4/src/parsagon/tests/api_mocks.py` & `parsagon-0.7.5/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.4/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.7.5/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.4/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.7.5/src/parsagon.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.4
+Version: 0.7.5
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -20,29 +20,51 @@
 
 ## Installation
 
 To get started, install the Parsagon python package:
 
 `pip install parsagon`
 
-and set your API key as an environment variable:
+Then run
 
-`export PARSAGON_API_KEY=<YOUR API KEY>`
+`parsagon setup`
 
-Please contact us to get your API key if you don't have it already.
+and copy-paste your API key when prompted.
+
+You can view your API key by logging in and going to <https://parsagon.io/settings>
 
 ## Usage
 
+From command line:
+
+```
+# Create a program
+parsagon create
+
+# Run a program
+parsagon run 'My program'
+
+# List your programs
+parsagon detail
+
+# Delete a program
+parsagon delete 'My program'
+```
+
+From Python:
 ```
 import parsagon
 
 # Create a program
-parsagon.create('Go to https://www.google.com/. Type "the meaning of life" into the search bar and hit enter. Scroll down and click the "More results" button 3 times. Scrape data in the format [{"title": "str", "link": "link"}].')
+parsagon.create('Go to https://www.google.com/. Type "the meaning of life" into the search bar and hit enter. Scroll down and click the "More results" button 3 times. Scrape data in the format [{"search result title": "str", "link": "link"}].')
 
 # Run a program
 parsagon.run("My program")
 
 # List your programs
 parsagon.detail()
+
+# Delete a program
+parsagon.delete("My program")
 ```
 
 See [the docs](https://parsagon.io/docs/pipelines/overview) for more information.
```

### Comparing `parsagon-0.7.4/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.7.5/src/parsagon.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 src/parsagon.egg-info/entry_points.txt
 src/parsagon.egg-info/requires.txt
 src/parsagon.egg-info/top_level.txt
 src/parsagon/tests/__init__.py
 src/parsagon/tests/api_mocks.py
 src/parsagon/tests/cli_mocks.py
 src/parsagon/tests/conftest.py
+src/parsagon/tests/test_invalid_args.py
 src/parsagon/tests/test_pipeline_operations.py
```


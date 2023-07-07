# Comparing `tmp/motion_python-0.1.73.tar.gz` & `tmp/motion_python-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.73.tar", max compression
+gzip compressed data, was "motion_python-0.1.74.tar", max compression
```

## Comparing `motion_python-0.1.73.tar` & `motion_python-0.1.74.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3344 2023-07-06 19:19:41.586125 motion_python-0.1.73/README.md
--rw-r--r--   0        0        0      344 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/cli.py
--rw-r--r--   0        0        0    22800 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/component.py
--rw-r--r--   0        0        0    17433 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/execute.py
--rw-r--r--   0        0        0    13869 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/instance.py
--rw-r--r--   0        0        0     4889 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-06 19:19:41.590126 motion_python-0.1.73/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1142 2023-07-06 19:19:41.590126 motion_python-0.1.73/motion/route.py
--rw-r--r--   0        0        0     5908 2023-07-06 19:19:41.590126 motion_python-0.1.73/motion/server/update_task.py
--rw-r--r--   0        0        0     9369 2023-07-06 19:19:41.590126 motion_python-0.1.73/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-06 19:20:05.642346 motion_python-0.1.73/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.73/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-06 19:49:53.121802 motion_python-0.1.74/README.md
+-rw-r--r--   0        0        0      344 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/cli.py
+-rw-r--r--   0        0        0    22799 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/component.py
+-rw-r--r--   0        0        0    17433 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/execute.py
+-rw-r--r--   0        0        0    13869 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/instance.py
+-rw-r--r--   0        0        0     4889 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1142 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/route.py
+-rw-r--r--   0        0        0     5908 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/server/update_task.py
+-rw-r--r--   0        0        0     9369 2023-07-06 19:49:53.125803 motion_python-0.1.74/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-06 19:50:12.791343 motion_python-0.1.74/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.74/PKG-INFO
```

### Comparing `motion_python-0.1.73/README.md` & `motion_python-0.1.74/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/motion/cli.py` & `motion_python-0.1.74/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/motion/component.py` & `motion_python-0.1.74/motion/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,15 +418,15 @@
             )
         if isinstance(keys, str):
             keys = [keys]
 
         def decorator(func: Callable) -> Any:
             if not validate_args(inspect.signature(func).parameters, "update"):
                 raise ValueError(
-                    f"Fit method {func.__name__} should have >= 2 arguments: "
+                    f"Update op {func.__name__} should have >= 2 arguments: "
                     + "`state` and `serve_result`."
                 )
 
             # func._input_key = key  # type: ignore
             # func._batch_size = batch_size  # type: ignore
             func._op = "update"  # type: ignore
```

### Comparing `motion_python-0.1.73/motion/execute.py` & `motion_python-0.1.74/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/motion/instance.py` & `motion_python-0.1.74/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/motion/migrate.py` & `motion_python-0.1.74/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.74/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/motion/route.py` & `motion_python-0.1.74/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/motion/server/update_task.py` & `motion_python-0.1.74/motion/server/update_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/motion/utils.py` & `motion_python-0.1.74/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.73/pyproject.toml` & `motion_python-0.1.74/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.73"
+version = "0.1.74"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.73/PKG-INFO` & `motion_python-0.1.74/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.73
+Version: 0.1.74
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


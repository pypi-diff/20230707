# Comparing `tmp/runweb-0.3.0.tar.gz` & `tmp/runweb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runweb-0.3.0.tar", last modified: Thu Jul  6 11:37:27 2023, max compression
+gzip compressed data, was "runweb-0.3.1.tar", last modified: Fri Jul  7 06:21:48 2023, max compression
```

## Comparing `runweb-0.3.0.tar` & `runweb-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11341 2023-07-06 11:37:10.609843 runweb-0.3.0/LICENSE
--rw-r--r--   0        0        0      729 2023-07-06 11:37:10.609843 runweb-0.3.0/README.md
--rw-r--r--   0        0        0     1230 2023-07-06 11:37:27.082029 runweb-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/__init__.py
--rw-r--r--   0        0        0       29 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/__main__.py
--rw-r--r--   0        0        0       22 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/__version__.py
--rw-r--r--   0        0        0     3544 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/main.py
--rw-r--r--   0        0        0     2171 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/multiprocess.py
--rw-r--r--   0        0        0     2120 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/parse.py
--rw-r--r--   0        0        0        0 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/runner/__init__.py
--rw-r--r--   0        0        0      837 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/runner/uvicorn.py
--rw-r--r--   0        0        0      814 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/runner/waitress.py
--rw-r--r--   0        0        0        0 2023-07-06 11:37:10.609843 runweb-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      930 2023-07-06 11:37:10.609843 runweb-0.3.0/tests/test_uvicorn.py
--rw-r--r--   0        0        0      934 2023-07-06 11:37:10.609843 runweb-0.3.0/tests/test_waitress.py
--rw-r--r--   0        0        0      866 2023-07-06 11:37:10.609843 runweb-0.3.0/tests/utils.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-07 06:21:31.797731 runweb-0.3.1/LICENSE
+-rw-r--r--   0        0        0      729 2023-07-07 06:21:31.797731 runweb-0.3.1/README.md
+-rw-r--r--   0        0        0     1230 2023-07-07 06:21:48.217938 runweb-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/__main__.py
+-rw-r--r--   0        0        0       22 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/__version__.py
+-rw-r--r--   0        0        0     3573 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/main.py
+-rw-r--r--   0        0        0     2171 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/multiprocess.py
+-rw-r--r--   0        0        0     1640 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/parse.py
+-rw-r--r--   0        0        0        0 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/runner/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-07 06:21:31.797731 runweb-0.3.1/runweb/runner/uvicorn.py
+-rw-r--r--   0        0        0      814 2023-07-07 06:21:31.801731 runweb-0.3.1/runweb/runner/waitress.py
+-rw-r--r--   0        0        0        0 2023-07-07 06:21:31.801731 runweb-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-07 06:21:31.801731 runweb-0.3.1/tests/test_uvicorn.py
+-rw-r--r--   0        0        0      934 2023-07-07 06:21:31.801731 runweb-0.3.1/tests/test_waitress.py
+-rw-r--r--   0        0        0      866 2023-07-07 06:21:31.801731 runweb-0.3.1/tests/utils.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.3.1/PKG-INFO
```

### Comparing `runweb-0.3.0/LICENSE` & `runweb-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runweb-0.3.0/README.md` & `runweb-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `runweb-0.3.0/pyproject.toml` & `runweb-0.3.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "click>=8.1.3",
 ]
 description = "Run web server with one command."
 dynamic = []
 name = "runweb"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 tui = [
     "trogon>=0.4.0",
```

### Comparing `runweb-0.3.0/runweb/main.py` & `runweb-0.3.1/runweb/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,17 +79,19 @@
 ) -> None:
     if ctx.invoked_subcommand is not None:
         return
 
     if application is None:
         raise click.UsageError("Missing option '--application' / '-a'.")
 
+    app_object = parse_application(application)
+
     if interface is None:
         try:
-            co = parse_application(application)(None, None, None)
+            co = app_object(None, None, None)
             interface = "asgi"
         except TypeError:
             interface = "wsgi"
         else:
             # close the coroutine, disable the warning
             co.close()
```

### Comparing `runweb-0.3.0/runweb/multiprocess.py` & `runweb-0.3.1/runweb/multiprocess.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.0/runweb/parse.py` & `runweb-0.3.1/runweb/parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,24 +47,10 @@
     module_str, _, attrs_str = value.partition(":")
     if not module_str or not attrs_str:
         message = (
             'Import string "{import_str}" must be in format "<module>:<attribute>".'
         )
         raise click.BadParameter(message.format(import_str=value))
 
-    try:
-        module = importlib.import_module(module_str)
-    except ImportError as exc:
-        if exc.name != module_str:
-            raise exc from None
-        message = 'Could not import module "{module_str}".'
-        raise click.BadParameter(message.format(module_str=module_str))
-
-    try:
-        instance = reduce(getattr, attrs_str.split("."), module)
-    except AttributeError:
-        message = 'Attribute "{attrs_str}" not found in module "{module_str}".'
-        raise click.BadParameter(
-            message.format(attrs_str=attrs_str, module_str=module_str)
-        )
-
+    module = importlib.import_module(module_str)
+    instance = reduce(getattr, attrs_str.split("."), module)
     return instance
```

### Comparing `runweb-0.3.0/runweb/runner/uvicorn.py` & `runweb-0.3.1/runweb/runner/uvicorn.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.0/runweb/runner/waitress.py` & `runweb-0.3.1/runweb/runner/waitress.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.0/tests/test_uvicorn.py` & `runweb-0.3.1/tests/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.0/tests/test_waitress.py` & `runweb-0.3.1/tests/test_waitress.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.0/tests/utils.py` & `runweb-0.3.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `runweb-0.3.0/PKG-INFO` & `runweb-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runweb
-Version: 0.3.0
+Version: 0.3.1
 Summary: Run web server with one command.
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Requires-Dist: click>=8.1.3
 Requires-Dist: trogon>=0.4.0; extra == "tui"
 Requires-Dist: waitress; extra == "waitress"
```


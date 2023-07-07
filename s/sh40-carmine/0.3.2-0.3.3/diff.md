# Comparing `tmp/sh40_carmine-0.3.2.tar.gz` & `tmp/sh40_carmine-0.3.3.tar.gz`

## Comparing `sh40_carmine-0.3.2.tar` & `sh40_carmine-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/__about__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/__init__.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/__main__.py
--rw-r--r--   0        0        0    17823 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/cli.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/README.md
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/carmine/__about__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/carmine/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/carmine/__main__.py
+-rw-r--r--   0        0        0    17819 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/carmine/cli.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/carmine/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/README.md
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sh40_carmine-0.3.3/PKG-INFO
```

### Comparing `sh40_carmine-0.3.2/carmine/__main__.py` & `sh40_carmine-0.3.3/carmine/__main__.py`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.2/carmine/cli.py` & `sh40_carmine-0.3.3/carmine/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,21 +283,21 @@
         if arg.startswith("-"):
             is_longhand = arg.startswith("--")
 
             value = None
             if "=" in arg:
                 arg, value = arg.split("=")
 
-            key = arg.lstrip("-")
+            key = arg.lstrip("-").replace("-", "_")
             opt = schema[key] if is_longhand else shorthand_lookup[key]
 
             if value is None and len(args) > i + 1 and not args[i + 1].startswith("-"):
                 value = args.pop(i + 1)
 
-            keywords[opt.key.replace("-", "_")] = _apply_factory(opt, value)
+            keywords[key] = _apply_factory(opt, value)
 
         else:
             index = len(positionals)
 
             if index >= len(schema_keys):
                 raise CLIRuntimeException(
                     f"can't map positional {arg!r} at index {index} to the schema."
```

### Comparing `sh40_carmine-0.3.2/carmine/exceptions.py` & `sh40_carmine-0.3.3/carmine/exceptions.py`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.2/LICENSE.txt` & `sh40_carmine-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.2/README.md` & `sh40_carmine-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.2/pyproject.toml` & `sh40_carmine-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.2/PKG-INFO` & `sh40_carmine-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh40-carmine
-Version: 0.3.2
+Version: 0.3.3
 Summary: The no-boilerplate CLI library powered by Python's introspection.
 Project-URL: Documentation, https://github.com/shade40/carmine#readme
 Project-URL: Issues, https://github.com/shade40/carmine/issues
 Project-URL: Source, https://github.com/shade40/carmine
 Author-email: bczsalba <bczsalba@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```


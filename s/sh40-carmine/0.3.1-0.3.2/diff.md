# Comparing `tmp/sh40_carmine-0.3.1.tar.gz` & `tmp/sh40_carmine-0.3.2.tar.gz`

## Comparing `sh40_carmine-0.3.1.tar` & `sh40_carmine-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/__about__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/__init__.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/__main__.py
--rw-r--r--   0        0        0    17719 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/cli.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/README.md
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/__about__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/__main__.py
+-rw-r--r--   0        0        0    17823 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/cli.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/carmine/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/README.md
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sh40_carmine-0.3.2/PKG-INFO
```

### Comparing `sh40_carmine-0.3.1/carmine/__main__.py` & `sh40_carmine-0.3.2/carmine/__main__.py`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.1/carmine/cli.py` & `sh40_carmine-0.3.2/carmine/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,22 @@
 
 except ImportError as exc:
     ZENITH_INSTALLED = False
 
 logging.getLogger("griffe").setLevel(logging.ERROR)
 
 EMPTY = object()
-TERMINAL_WIDTH = min(120, os.get_terminal_size()[0])
+TERMINAL_WIDTH = 120
+
+try:
+    TERMINAL_WIDTH = min(TERMINAL_WIDTH, os.get_terminal_size()[0])
+except OSError as exc:
+    if exc.errno != 25:
+        raise
+
 DATE_FORMAT = "%Y-%m-%dT%H:%M:%S"
 INDENT = " " * 2
 
 
 def _is_optional(annotation: object) -> bool:
     """Determines whether an annotation is optional.
```

### Comparing `sh40_carmine-0.3.1/carmine/exceptions.py` & `sh40_carmine-0.3.2/carmine/exceptions.py`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.1/LICENSE.txt` & `sh40_carmine-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.1/README.md` & `sh40_carmine-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.3.1/pyproject.toml` & `sh40_carmine-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
 ]
 
 [tool.hatch.envs.default.scripts]
-test = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=celadon --cov=tests && coverage html"
-lint = "pylint celadon"
-type = "mypy celadon"
+test = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=carmine --cov=tests && coverage html"
+lint = "pylint carmine"
+type = "mypy carmine"
 upload = "hatch build && twine upload dist/* && hatch clean"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `sh40_carmine-0.3.1/PKG-INFO` & `sh40_carmine-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh40-carmine
-Version: 0.3.1
+Version: 0.3.2
 Summary: The no-boilerplate CLI library powered by Python's introspection.
 Project-URL: Documentation, https://github.com/shade40/carmine#readme
 Project-URL: Issues, https://github.com/shade40/carmine/issues
 Project-URL: Source, https://github.com/shade40/carmine
 Author-email: bczsalba <bczsalba@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```


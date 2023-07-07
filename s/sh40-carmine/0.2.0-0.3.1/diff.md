# Comparing `tmp/sh40_carmine-0.2.0.tar.gz` & `tmp/sh40_carmine-0.3.1.tar.gz`

## Comparing `sh40_carmine-0.2.0.tar` & `sh40_carmine-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/carmine/__about__.py
--rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/carmine/__init__.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/carmine/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/README.md
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/__about__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/__main__.py
+-rw-r--r--   0        0        0    17719 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/cli.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/carmine/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/README.md
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sh40_carmine-0.3.1/PKG-INFO
```

### Comparing `sh40_carmine-0.2.0/LICENSE.txt` & `sh40_carmine-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.2.0/pyproject.toml` & `sh40_carmine-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sh40-carmine"
-description = "A dynamic CLI generator utilizing Python function signatures."
+description = "The no-boilerplate CLI library powered by Python's introspection."
 readme = "README.md"
 requires-python = ">=3.8"
+license = "MIT"
 keywords = []
 authors = [
   { name = "bczsalba", email = "bczsalba@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
+  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    # TODO: We will likely use `Terminal` in the future, so we have a direct
-    #       dependency. If that doesn't work out, we should remove this!
     "sh40-slate",
-
     "sh40-zenith",
     "griffe",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/shade40/carmine#readme"
@@ -49,30 +48,31 @@
 path = "carmine/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
 ]
+
 [tool.hatch.envs.default.scripts]
-test = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=carmine --cov=tests && coverage html"
-lint = "pylint carmine"
-type = "mypy carmine"
+test = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=celadon --cov=tests && coverage html"
+lint = "pylint celadon"
+type = "mypy celadon"
 upload = "hatch build && twine upload dist/* && hatch clean"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "carmine/__about__.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
-  "no-cov",
+  "no cov",
   "def __repr__",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
```


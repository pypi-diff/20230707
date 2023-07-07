# Comparing `tmp/sbmlmath-0.0.2.tar.gz` & `tmp/sbmlmath-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmlmath-0.0.2.tar", last modified: Sun Jun 25 05:08:51 2023, max compression
+gzip compressed data, was "sbmlmath-0.0.3.tar", last modified: Fri Jul  7 17:55:58 2023, max compression
```

## Comparing `sbmlmath-0.0.2.tar` & `sbmlmath-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.460614 sbmlmath-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.460614 sbmlmath-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/.github/workflows/deploy_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/sbmlmath/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/cfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/csymbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/mathml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/mathml_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/sbmlmath/species_symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/sbmlmath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 05:08:51.000000 sbmlmath-0.0.2/sbmlmath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:08:51.464614 sbmlmath-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_csymbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_mathml_parser_sbml_semantic_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-25 05:08:41.000000 sbmlmath-0.0.2/tests/test_species_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:55:58.772498 sbmlmath-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:55:58.768497 sbmlmath-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:55:58.768497 sbmlmath-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/.github/workflows/deploy_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-07 17:55:58.772498 sbmlmath-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:55:58.772498 sbmlmath-0.0.3/sbmlmath/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/sbmlmath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/sbmlmath/cfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/sbmlmath/csymbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/sbmlmath/mathml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/sbmlmath/mathml_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/sbmlmath/species_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:55:58.772498 sbmlmath-0.0.3/sbmlmath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-07 17:55:58.000000 sbmlmath-0.0.3/sbmlmath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-07 17:55:58.000000 sbmlmath-0.0.3/sbmlmath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:55:58.000000 sbmlmath-0.0.3/sbmlmath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-07 17:55:58.000000 sbmlmath-0.0.3/sbmlmath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 17:55:58.000000 sbmlmath-0.0.3/sbmlmath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:55:58.772498 sbmlmath-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:55:58.772498 sbmlmath-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/tests/test_csymbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/tests/test_mathml_parser_sbml_semantic_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/tests/test_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-07 17:55:47.000000 sbmlmath-0.0.3/tests/test_species_symbol.py
```

### Comparing `sbmlmath-0.0.2/.github/workflows/ci.yaml` & `sbmlmath-0.0.3/.github/workflows/ci.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.9", "3.11"]
 
     steps:
     - name: Check out repository
       uses: actions/checkout@v3
 
 
     - name: Set up Python ${{ matrix.python-version }}
@@ -24,30 +24,30 @@
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Cache pip
       uses: actions/cache@v3
       with:
         path: ~/.cache/pip
-        key: ${{ runner.os }}-${{ hashFiles('setup.py') }}
+        key: ${{ runner.os }}-${{ matrix.python-version }}-${{ hashFiles('setup.py') }}
         restore-keys: |
-          ${{ runner.os }}-
+          ${{ runner.os }}-${{ matrix.python-version }}-
 
     - name: Cache / restore SBML test suite
       id: cache-sbml-test-suite
       uses: actions/cache@v3
       with:
         path: sbml-test-suite
         key: ${{ runner.os }}-sbml-test-suite
 
     - name: Download SBML test suite
       if: steps.cache-sbml-test-suite.outputs.cache-hit != 'true'
       run: git clone --depth=1 https://github.com/sbmlteam/sbml-test-suite/
 
     - name: Install local packages
       run: |
-        pip install .[test]
+        pip install --upgrade pip setuptools && pip install .[test]
 
     - name: Unit tests
       env:
           SBML_TEST_SUITE_ROOT: "${{ github.workspace }}/sbml-test-suite/"
       run: pytest -vv
```

### Comparing `sbmlmath-0.0.2/.github/workflows/deploy_release.yaml` & `sbmlmath-0.0.3/.github/workflows/deploy_release.yaml`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/.pre-commit-config.yaml` & `sbmlmath-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/LICENSE` & `sbmlmath-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/PKG-INFO` & `sbmlmath-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sbmlmath
-Version: 0.0.2
+Version: 0.0.3
 Summary: SBML Math <-> SymPy
 Author-email: Daniel Weindl <sci@danielweindl.de>
 License: BSD-3-Clause
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # sbmlmath - a Python library for handling SBML MathML
 
 This is Python library for interconverting [SymPy](https://github.com/sympy/sympy/)
@@ -22,14 +22,16 @@
 * SBML MathML -> sympy
   * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))`
     won't do the job
   * retaining unit annotations and other `<ci>` attributes
 
 **NOTE: This is under development and the API is to be considered unstable**
 
+Python support policy: sbmlmath follows [NEP 29](https://numpy.org/neps/nep-0029-deprecation_policy.html).
+
 ## Usage
 
 ```python
 from sbmlmath import SBMLMathMLPrinter, SBMLMathMLParser
 import sympy as sp
 
 sympy_expr = sp.sympify("A ** B + exp(C) * D")
```

### Comparing `sbmlmath-0.0.2/README.md` & `sbmlmath-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 * SBML MathML -> sympy
   * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))`
     won't do the job
   * retaining unit annotations and other `<ci>` attributes
 
 **NOTE: This is under development and the API is to be considered unstable**
 
+Python support policy: sbmlmath follows [NEP 29](https://numpy.org/neps/nep-0029-deprecation_policy.html).
+
 ## Usage
 
 ```python
 from sbmlmath import SBMLMathMLPrinter, SBMLMathMLParser
 import sympy as sp
 
 sympy_expr = sp.sympify("A ** B + exp(C) * D")
```

### Comparing `sbmlmath-0.0.2/pyproject.toml` & `sbmlmath-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sbmlmath"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Daniel Weindl", email = "sci@danielweindl.de"},
 ]
 description = "SBML Math <-> SymPy"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 license = {text = "BSD-3-Clause"}
 dependencies = [
     "python-libsbml",
     "sympy",
     "pint",
-    "lxml",
+    "lxml>=4.6.4",
 ]
 
 [project.optional-dependencies]
-test = ["pytest", "pre-commit"]
+test = ["pytest>=7", "pre-commit>=3"]
 
 [tool.black]
 line-length = 80
```

### Comparing `sbmlmath-0.0.2/sbmlmath/__init__.py` & `sbmlmath-0.0.3/sbmlmath/__init__.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/sbmlmath/cfunction.py` & `sbmlmath-0.0.3/sbmlmath/cfunction.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/sbmlmath/csymbol.py` & `sbmlmath-0.0.3/sbmlmath/csymbol.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/sbmlmath/mathml_parser.py` & `sbmlmath-0.0.3/sbmlmath/mathml_parser.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/sbmlmath/mathml_printer.py` & `sbmlmath-0.0.3/sbmlmath/mathml_printer.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/sbmlmath/species_symbol.py` & `sbmlmath-0.0.3/sbmlmath/species_symbol.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/sbmlmath.egg-info/PKG-INFO` & `sbmlmath-0.0.3/sbmlmath.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sbmlmath
-Version: 0.0.2
+Version: 0.0.3
 Summary: SBML Math <-> SymPy
 Author-email: Daniel Weindl <sci@danielweindl.de>
 License: BSD-3-Clause
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # sbmlmath - a Python library for handling SBML MathML
 
 This is Python library for interconverting [SymPy](https://github.com/sympy/sympy/)
@@ -22,14 +22,16 @@
 * SBML MathML -> sympy
   * in particular for cases where `sympy.sympify(libsbml.formulaToL3String(...))`
     won't do the job
   * retaining unit annotations and other `<ci>` attributes
 
 **NOTE: This is under development and the API is to be considered unstable**
 
+Python support policy: sbmlmath follows [NEP 29](https://numpy.org/neps/nep-0029-deprecation_policy.html).
+
 ## Usage
 
 ```python
 from sbmlmath import SBMLMathMLPrinter, SBMLMathMLParser
 import sympy as sp
 
 sympy_expr = sp.sympify("A ** B + exp(C) * D")
```

### Comparing `sbmlmath-0.0.2/sbmlmath.egg-info/SOURCES.txt` & `sbmlmath-0.0.3/sbmlmath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/tests/test_mathml_parser_sbml_semantic_suite.py` & `sbmlmath-0.0.3/tests/test_mathml_parser_sbml_semantic_suite.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/tests/test_misc.py` & `sbmlmath-0.0.3/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/tests/test_parser.py` & `sbmlmath-0.0.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/tests/test_printer.py` & `sbmlmath-0.0.3/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `sbmlmath-0.0.2/tests/test_species_symbol.py` & `sbmlmath-0.0.3/tests/test_species_symbol.py`

 * *Files identical despite different names*


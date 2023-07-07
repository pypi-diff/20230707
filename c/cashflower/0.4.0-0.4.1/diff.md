# Comparing `tmp/cashflower-0.4.0.tar.gz` & `tmp/cashflower-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.4.0.tar", last modified: Thu Jul  6 19:18:54 2023, max compression
+gzip compressed data, was "cashflower-0.4.1.tar", last modified: Fri Jul  7 18:02:55 2023, max compression
```

## Comparing `cashflower-0.4.0.tar` & `cashflower-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.567023 cashflower-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-06 19:18:44.000000 cashflower-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 19:18:44.000000 cashflower-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-06 19:18:54.567023 cashflower-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-06 19:18:44.000000 cashflower-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.563023 cashflower-0.4.0/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.567023 cashflower-0.4.0/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/model_tpl/model.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-06 19:18:44.000000 cashflower-0.4.0/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.567023 cashflower-0.4.0/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 19:18:54.000000 cashflower-0.4.0/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:18:54.567023 cashflower-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-06 19:18:44.000000 cashflower-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:18:54.567023 cashflower-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-06 19:18:44.000000 cashflower-0.4.0/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-06 19:18:44.000000 cashflower-0.4.0/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-06 19:18:44.000000 cashflower-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-07 18:02:44.000000 cashflower-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 18:02:44.000000 cashflower-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-07 18:02:55.895984 cashflower-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-07 18:02:44.000000 cashflower-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/model_tpl/model.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-07 18:02:44.000000 cashflower-0.4.1/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 18:02:55.000000 cashflower-0.4.1/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:02:55.895984 cashflower-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 18:02:44.000000 cashflower-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:02:55.895984 cashflower-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 18:02:44.000000 cashflower-0.4.1/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-07 18:02:44.000000 cashflower-0.4.1/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-07 18:02:44.000000 cashflower-0.4.1/tests/test_utils.py
```

### Comparing `cashflower-0.4.0/LICENSE` & `cashflower-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.0/PKG-INFO` & `cashflower-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.0
+Version: 0.4.1
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.4.0/README.md` & `cashflower-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.0/cashflower/cashflow.py` & `cashflower-0.4.1/cashflower/cashflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import functools
-import matplotlib.pyplot as plt
+import itertools
 import networkx as nx
 import time
 import pandas as pd
 
 from .error import CashflowModelError
 from .utils import get_object_by_name, print_log, split_to_ranges, updt
 from .graph import get_calc_direction, get_calls, get_predecessors
@@ -52,29 +52,26 @@
         return self._settings
 
     @settings.setter
     def settings(self, new_settings):
         self._settings = new_settings
         self.result = [None for _ in range(0, self.settings["T_MAX_CALCULATION"] + 1)]
 
-    def calculate_forward(self):
-        for t in range(self.settings["T_MAX_CALCULATION"] + 1):
-            self.result[t] = self.func(t)
-
-    def calculate_backward(self):
-        for t in range(self.settings["T_MAX_CALCULATION"], -1, -1):
-            self.result[t] = self.func(t)
+    def calculate_t(self, t):
+        self.result[t] = self.func(t)
 
     def calculate(self):
         if self.calc_direction == "irrelevant":
             self.result = [*map(self.func, range(self.settings["T_MAX_CALCULATION"] + 1))]
         elif self.calc_direction == "forward":
-            self.calculate_forward()
+            for t in range(self.settings["T_MAX_CALCULATION"] + 1):
+                self.result[t] = self.func(t)
         elif self.calc_direction == "backward":
-            self.calculate_backward()
+            for t in range(self.settings["T_MAX_CALCULATION"], -1, -1):
+                self.result[t] = self.func(t)
         else:
             raise CashflowModelError(f"Incorrect calculation direction {self.calc_direction}")
 
 
 class Runplan:
     """Runplan of the cash flow model."""
     def __init__(self, data=None, version="1"):
@@ -220,14 +217,19 @@
                 for node in nodes_without_predecessors:
                     calc_order += 1
                     node.calc_order = calc_order
                 DG.remove_nodes_from(nodes_without_predecessors)
             else:  # it's a cycle
                 cycles = list(nx.simple_cycles(DG))
                 cycles_without_predecessors = [c for c in cycles if len(get_predecessors(c[0], DG)) == len(c)]
+
+                if len(cycles_without_predecessors) == 0:
+                    big_cycle = list(set(list(itertools.chain(*cycles))))
+                    cycles_without_predecessors = [big_cycle]
+
                 for cycle_without_predecessors in cycles_without_predecessors:
                     calc_order += 1
                     for node in cycle_without_predecessors:
                         node.calc_order = calc_order
                         node.cycle = True
                     DG.remove_nodes_from(cycle_without_predecessors)
 
@@ -296,29 +298,33 @@
             model_point_set.id = model_point_id
 
         # Perform calculations
         max_calc_order = self.variables[-1].calc_order
         for calc_order in range(1, max_calc_order + 1):
             # Either a single variable or a cycle
             variables = [variable for variable in self.variables if variable.calc_order == calc_order]
+            # Single
             if len(variables) == 1:
                 variable = variables[0]
                 start = time.time()
                 variable.calculate()
                 variable.runtime += time.time() - start
+            # Cycle
             else:
                 start = time.time()
                 first_variable = variables[0]
                 calc_direction = first_variable.calc_direction
                 if calc_direction in ("irrelevant", "forward"):
-                    for variable in variables:
-                        variable.calculate_forward()
+                    for t in range(self.settings["T_MAX_CALCULATION"] + 1):
+                        for variable in variables:
+                            variable.calculate_t(t)
                 else:
-                    for variable in variables:
-                        variable.calculate_backward()
+                    for t in range(self.settings["T_MAX_CALCULATION"], -1, -1):
+                        for variable in variables:
+                            variable.calculate_t(t)
                 end = time.time()
                 avg_runtime = (end-start)/len(variables)
                 for variable in variables:
                     variable.runtime += avg_runtime
 
         # Get results and trim for T_MAX_OUTPUT
         columns = [variable.name for variable in self.variables]
```

### Comparing `cashflower-0.4.0/cashflower/graph.py` & `cashflower-0.4.1/cashflower/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,40 +3,46 @@
 
 from queue import Queue
 
 from .error import CashflowModelError
 from .utils import get_object_by_name
 
 
+def get_calls(variable, variables):
+    """List variables called by the given variable"""
+    call_names = []
+    variable_names = [variable.name for variable in variables]
+
+    # print("\n", ast.dump(node, indent=2))
+    node = ast.parse(inspect.getsource(variable.func))
+    for subnode in ast.walk(node):
+        if isinstance(subnode, ast.Call):
+            if isinstance(subnode.func, ast.Name):
+                if subnode.func.id in variable_names:
+                    raise_error_if_incorrect_argument(subnode)
+                    call_names.append(subnode.func.id)
+
+    calls = [get_object_by_name(variables, call_name) for call_name in call_names if call_name != variable.name]
+    return calls
+
+
 def get_calc_direction(variables):
     """Set calculation direction to irrelevant/forward/backward"""
     # For non-cycle => single variable, for cycle => variables from the cycle
     variable_names = [variable.name for variable in variables]
 
     visitor = CalcDirectionVisitor(variable_names)
     for variable in variables:
         node = ast.parse(inspect.getsource(variable.func))
         visitor.visit(node)
         variable.calc_direction = visitor.calc_direction
 
     return None
 
 
-def get_calls(variable, variables):
-    """List variables called by the given variable"""
-    variable_names = [variable.name for variable in variables]
-    call_visitor = CallVisitor(variable_names)
-    node = ast.parse(inspect.getsource(variable.func))
-    # print("\n", ast.dump(node, indent=2))
-    call_visitor.visit(node)
-    call_names = call_visitor.calls
-    calls = [get_object_by_name(variables, call_name) for call_name in call_names if call_name != variable.name]
-    return calls
-
-
 def get_predecessors(node, DG):
     """Get predecessors and their predecessors and their..."""
     queue = Queue()
     visited = []
 
     queue.put(node)
     visited.append(node)
@@ -82,26 +88,14 @@
             raise CashflowModelError(msg)
 
     # The model variable calls something else
     if not (isinstance(arg, ast.Name) or isinstance(arg, ast.Constant) or isinstance(arg, ast.BinOp)):
         raise CashflowModelError(msg)
 
 
-class CallVisitor(ast.NodeVisitor):
-    def __init__(self, variable_names):
-        self.variable_names = variable_names
-        self.calls = []
-
-    def visit_Call(self, node):
-        if isinstance(node.func, ast.Name):
-            if node.func.id in self.variable_names:
-                raise_error_if_incorrect_argument(node)
-                self.calls.append(node.func.id)
-
-
 class CalcDirectionVisitor(ast.NodeVisitor):
     def __init__(self, variable_names):
         self.variable_names = variable_names
         self.calc_direction = "irrelevant"
 
     def visit_Call(self, node):
         if isinstance(node.func, ast.Name):
```

### Comparing `cashflower-0.4.0/cashflower/start.py` & `cashflower-0.4.1/cashflower/start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.0/cashflower/utils.py` & `cashflower-0.4.1/cashflower/utils.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.0/cashflower.egg-info/PKG-INFO` & `cashflower-0.4.1/cashflower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.0
+Version: 0.4.1
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.4.0/cashflower.egg-info/SOURCES.txt` & `cashflower-0.4.1/cashflower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.0/setup.py` & `cashflower-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.4.0",
+    version="0.4.1",
 )
```

### Comparing `cashflower-0.4.0/tests/test_cashflow.py` & `cashflower-0.4.1/tests/test_cashflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,28 +98,13 @@
 
         foo.name = "foo"
         foo.settings = load_settings()
 
         with pytest.raises(CashflowModelError):
             foo(10)
 
-        foo.calculate_forward()
+        foo.calculate_t(10)
 
         assert foo(10) == 10
 
         with pytest.raises(CashflowModelError):
             foo(-1)
-
-    def test_variable_is_calculated_backward(self):
-        @variable()
-        def foo(t):
-            if t == 720:
-                return 720
-            return foo(t+1) - 1
-
-        foo.name = "foo"
-        foo.settings = load_settings()
-        foo.calc_direction = "backward"
-        foo.calculate()
-
-        assert foo(0) == 0
-
```

### Comparing `cashflower-0.4.0/tests/test_start.py` & `cashflower-0.4.1/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.0/tests/test_utils.py` & `cashflower-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*


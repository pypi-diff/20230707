# Comparing `tmp/heavylight-1.0.2.tar.gz` & `tmp/heavylight-1.0.3.tar.gz`

## Comparing `heavylight-1.0.2.tar` & `heavylight-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 heavylight-1.0.2/Pipfile
--rw-r--r--   0        0        0   123112 2020-02-02 00:00:00.000000 heavylight-1.0.2/Pipfile.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 heavylight-1.0.2/Untitled.ipynb
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.2/server_user_id.txt
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/benchmark.ipynb
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/cvect_memo.cpp
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/cvect_memo.pyx
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/cvect_memo_vector.pyx
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/heavylight.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/make_data.ipynb
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_dict.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_hl.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_np.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_np_hl.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_try.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/setup.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/table_a.csv
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/test.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/readme.md
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/heavylight.py
--rw-r--r--   0        0        0    61719 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/heavylight_basic.ipynb
--rw-r--r--   0        0        0    61991 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/heavylight_tables.ipynb
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/sample_q_x_table.csv
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/table_maker.ipynb
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/vectors.ipynb
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/vectors.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 heavylight-1.0.2/heavylight/build_examples.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.2/heavylight/heavylight.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.2/src/heavylight/__init__.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.2/src/heavylight/heavylight.py
--rw-r--r--   0        0        0   300723 2020-02-02 00:00:00.000000 heavylight-1.0.2/tests/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 heavylight-1.0.2/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 heavylight-1.0.2/LICENSE
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 heavylight-1.0.2/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 heavylight-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 heavylight-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 heavylight-1.0.3/Pipfile
+-rw-r--r--   0        0        0   123112 2020-02-02 00:00:00.000000 heavylight-1.0.3/Pipfile.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 heavylight-1.0.3/Untitled.ipynb
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.3/server_user_id.txt
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/benchmark.ipynb
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/cvect_memo.cpp
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/cvect_memo.pyx
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/cvect_memo_vector.pyx
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/heavylight.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/make_data.ipynb
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/memo_dict.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/memo_hl.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/memo_np.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/memo_np_hl.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/memo_try.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/setup.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/table_a.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/test.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 heavylight-1.0.3/cythonz/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/basic_cashflow.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/readme.md
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/readme_example.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/notebook/heavylight.py
+-rw-r--r--   0        0        0    61719 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/notebook/heavylight_basic.ipynb
+-rw-r--r--   0        0        0    61991 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/notebook/heavylight_tables.ipynb
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/notebook/sample_q_x_table.csv
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/notebook/table_maker.ipynb
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/notebook/vectors.ipynb
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 heavylight-1.0.3/examples/notebook/vectors.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.3/src/heavylight/__init__.py
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 heavylight-1.0.3/src/heavylight/heavylight.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 heavylight-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0   300723 2020-02-02 00:00:00.000000 heavylight-1.0.3/tests/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.3/tests/server_user_id.txt
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 heavylight-1.0.3/tests/test_heavylight_basic.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 heavylight-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 heavylight-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 heavylight-1.0.3/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 heavylight-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 heavylight-1.0.3/PKG-INFO
```

### Comparing `heavylight-1.0.2/Pipfile.lock` & `heavylight-1.0.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/benchmark.ipynb` & `heavylight-1.0.3/cythonz/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/cvect_memo.pyx` & `heavylight-1.0.3/cythonz/cvect_memo.pyx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/cvect_memo_vector.pyx` & `heavylight-1.0.3/cythonz/cvect_memo_vector.pyx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/heavylight.py` & `heavylight-1.0.3/cythonz/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/make_data.ipynb` & `heavylight-1.0.3/cythonz/make_data.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/memo_dict.py` & `heavylight-1.0.3/cythonz/memo_dict.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/memo_np.py` & `heavylight-1.0.3/cythonz/memo_np.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/memo_np_hl.py` & `heavylight-1.0.3/cythonz/memo_np_hl.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/memo_try.py` & `heavylight-1.0.3/cythonz/memo_try.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/cythonz/table_a.csv` & `heavylight-1.0.3/cythonz/table_a.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/examples/notebook/heavylight.py` & `heavylight-1.0.3/examples/notebook/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/examples/notebook/heavylight_basic.ipynb` & `heavylight-1.0.3/examples/notebook/heavylight_basic.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/examples/notebook/heavylight_tables.ipynb` & `heavylight-1.0.3/examples/notebook/heavylight_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/examples/notebook/sample_q_x_table.csv` & `heavylight-1.0.3/examples/notebook/sample_q_x_table.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/examples/notebook/table_maker.ipynb` & `heavylight-1.0.3/examples/notebook/table_maker.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/examples/notebook/vectors.ipynb` & `heavylight-1.0.3/examples/notebook/vectors.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/examples/notebook/vectors.py` & `heavylight-1.0.3/examples/notebook/vectors.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/heavylight/heavylight.py` & `heavylight-1.0.3/src/heavylight/heavylight.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import types
-from typing import List
 import warnings
-from inspect import signature
+from inspect import signature, getmembers
 import pandas as pd
 
 class Table:
     """A Table has one or more keys, and a single column of values"""
 
     def __init__(self, series):
         """Initialise a table with a series - for multiple keys use a multikey index"""
@@ -23,15 +22,15 @@
     @staticmethod
     def read_csv(filename, sep=",", type_identifier = "|"):
         """Read in a table from a csv file, type encoding is via the header:
         
         <keyname1>|<type1>,<keyname2>|<type2>....<value>|<typeN>
         where type is one of "str", "int", "float"
         """
-        column_types = {"str":str, "int": int, "float": float}
+        column_types = {"str": str, "int": int, "float": float}
         with open(filename, "r") as csv_file:
             header = next(csv_file).strip("\n").split(sep)
         tid = type_identifier
         header_mapper_str = {item:item.split(tid)[1] for item in header}
         header_mapper_types = {col:column_types[val] for col, val in header_mapper_str.items()}
         df = pd.read_csv(filename, sep=sep, dtype=header_mapper_types)
         # strip `tid` from column names
@@ -44,30 +43,39 @@
 class _Cache:
     """Cache provides controllable memoization for model methods"""
 
     def __init__(self, func: types.MethodType, param_len: int):
         self.func = func
         self.param_len = param_len
         self.has_one_param = self.param_len == 1
-        self.values = dict()
+        self._store = dict()
         self.__name__ = "Cache: " + func.__name__
 
     def __call__(self, *arg:list):
-        if arg in self.values:
-            return self.values[arg]
+        if arg in self._store:
+            return self._store[arg]
         else:
             result = self.func(*arg)
-            self.values[arg] = result
+            self._store[arg] = result
             return result
 
     def __repr__(self) -> str:
-        return f"<Cache Function: {self.func.__name__} Size: {len(self.values)}>"
+        return f"<Cache Function: {self.func.__name__} Size: {len(self._store)}>"
+    
+    def sum(self):
+        """return the sum of all values in the Cache Function"""
+        return sum(self._store.values())
+    
+    @property
+    def values(self):
+        return list(self._store.values())
+
 
 class Model:
-    def __init__(self, *, do_run: bool = False, verbose=False, proj_len: int|types.NoneType = None, **kwargs,):
+    def __init__(self, *, do_run: bool = False, verbose: bool = False, proj_len: int|None = None, **kwargs,):
         """Base Class to subclass for user models.
 
         All variables/methods in user models should be lower case, using underscore as spaces.
 
         Class level methods:
           RunModel(proj_len):
             if the model has not been auto-run at initialisation, run it for projection length.
@@ -114,44 +122,44 @@
         self._cache_funcs(verbose)
 
         if do_run and proj_len > 0:
             self.RunModel(proj_len, verbose)
         if verbose: print("== Run complete == ")
 
 
-    def RunModel(self, proj_len, verbose=False):
+    def RunModel(self, proj_len: int, verbose: bool = False):
         if self._is_run:
             raise ValueError("Run has already been completed.")
 
         if verbose: print(f"== Running Projection | length: {proj_len} ==")
         
         if hasattr(self, "BeforeRun"):
             if verbose: print("    Calling BeforeRun")
             self.BeforeRun()
 
         if not self._cached:
             raise ValueError("Functions have not been cached")  # NB: this shouldn't occur as now caching in instance
         for t in range(proj_len):
-            for var in self._funcs.keys():
-                func = getattr(self, var)
+            for name, func in self._funcs.items():
+                #func = getattr(self, var)
                 if func.has_one_param:   # skip functions with more than one parameter
                     func(t)   #call each function in turn, starting from t==0
         self._is_run = True
         if hasattr(self, "AfterRun"):
             if verbose: print("    Calling AfterRun")
             return self.AfterRun()
     
-    def _cache_funcs(self, verbose : bool=False):
+    def _cache_funcs(self, verbose: bool = False):
         if self._cached:
             raise ValueError("Cache has already been set-up, please create a new instance")
 
         self._funcs = {}
 
-        for method_name in dir(self):
-            method = getattr(self, method_name)
+        for method_name, method in getmembers(self):
+            #method = getattr(self, method_name)
 
             if method_name[0] != "_" and method_name[0].islower() and isinstance(method, types.MethodType):
                 param_count = len(signature(method).parameters) # count the parameters in the function.
                 cached_method = _Cache(method, param_count)
                 setattr(self, method_name, cached_method)
                 self._funcs[method_name] = cached_method
                 if verbose: print(f"    Cached: {method_name}")
@@ -161,8 +169,12 @@
         
     def ToDataFrame(self):
         """return a pandas dataframe of all single parameter columns"""
         df = pd.DataFrame()
         for func in self._funcs:
             if self._funcs[func].has_one_param:
                 df[func] = pd.Series(self._funcs[func].values)
+
+        # if t is in the dataframe, move it to first position
+        if "t" in df.columns:
+            df.insert(0, "t", df.pop("t"))
         return df
```

### Comparing `heavylight-1.0.2/tests/protection_risk_model_generic.xlsx` & `heavylight-1.0.3/tests/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/.gitignore` & `heavylight-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/LICENSE` & `heavylight-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.2/README.md` & `heavylight-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,30 +5,38 @@
 - single script
 - installation optional: package with your models.
 - only depends on `pandas`
 
 ## Components
 
 Model:
-    - projection controller
-    - class to subclass with your proprietary models
-    - `BeforeRun` and `AfterRun` methods
+
+- projection controller
+- class to subclass with your proprietary models
+- `BeforeRun` and `AfterRun` methods
+- get all values as a list with `values` attribute
+- get the sum of all values with `sum()` method
 
 
 Table:
-    - simple long format table object
-    - type information encoded via `|int`, `|float`, `|str` header suffixes
+
+- simple long format table object
+- type information encoded via `|int`, `|float`, `|str` header suffixes
 
 
 ## Usage
 
-Create your model as a subclass of Model.  Each model variable is defined as a method:
+### Model Class
+
+Create your model as a subclass of `heavylight.Model``.  Each model variable is defined as a method:
 
 ```python
-class Annuity(Model):
+import heavylight
+
+class Annuity(heavylight.Model):
     def t(self, t):
         return t
 
     def expected_claim(self, t):
         return self.number_alive(t) * self.data["annuity_per_period"]
 
     def number_alive(self, t):
@@ -38,14 +46,27 @@
             return self.number_alive(t - 1) - self.deaths(t - 1)
     
     def deaths(self, t):
         return self.number_alive(t) * self.mortality_rate(t)
 
     def mortality_rate(self, t):
         return 0.02
+
+    def v(self, t):
+        """discount factor from time t to time 0"""
+        if t == 0:
+            return 1
+        else:
+            return self.v(t - 1) / (1 + self.forward_rate(t))
+    
+    def forward_rate(self, t):
+        return 0.04
+
+    def pv_expected_claim(self, t):
+        return self.expected_claim(t) * self.v(t)
 ```
 
 Define input data as a dictionary
 
 ```python
 policy_data = {
     "initial_policies": 10,
@@ -58,28 +79,32 @@
 ```python
 model = Annuity(data = policy_data,
                 do_run = True,
                 proj_len = 20,
                 )
 ```
 
-display result as a pandas table
+Get the sum of `pv_expected_claim`:
 
 ```python
-model_cashflows = model.ToDataFrame()
+print(model.pv_expected_claim.sum())
 ```
 
-Use numpy_financial or another package to calculate NPVs.
 
-## Notes
 
-### Projecting vs. discounting
+Display result as a pandas table
+
+```python
+model_cashflows = model.ToDataFrame()
+```
+
+## Notes
 
  - This package is designed for projecting actuarial variables, and calculates t=0, 1... in order.
 
  - Actuarial models are generally highly recursive.
 
  - If you create a method which refers to future t value (such as an NPV function) you may hit the python stack limit.
 
- - The recommended solution is to project forward first, and then calculate T0 metrics based on the result.
+ - The recommended solution is to project forward first, and then calculate T0 metrics based on the result, for example using an `npv()`` function
```

### Comparing `heavylight-1.0.2/pyproject.toml` & `heavylight-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "heavylight"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Lewis Fogden", email="lewisfogden@gmail.com" },
 ]
 description = "Heavylight Actuarial Modelling Framework"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `heavylight-1.0.2/PKG-INFO` & `heavylight-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heavylight
-Version: 1.0.2
+Version: 1.0.3
 Summary: Heavylight Actuarial Modelling Framework
 Project-URL: Homepage, https://github.com/lewisfogden/heavylight/
 Project-URL: Bug Tracker, https://github.com/lewisfogden/heavylight/issues
 Author-email: Lewis Fogden <lewisfogden@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,30 +20,38 @@
 - single script
 - installation optional: package with your models.
 - only depends on `pandas`
 
 ## Components
 
 Model:
-    - projection controller
-    - class to subclass with your proprietary models
-    - `BeforeRun` and `AfterRun` methods
+
+- projection controller
+- class to subclass with your proprietary models
+- `BeforeRun` and `AfterRun` methods
+- get all values as a list with `values` attribute
+- get the sum of all values with `sum()` method
 
 
 Table:
-    - simple long format table object
-    - type information encoded via `|int`, `|float`, `|str` header suffixes
+
+- simple long format table object
+- type information encoded via `|int`, `|float`, `|str` header suffixes
 
 
 ## Usage
 
-Create your model as a subclass of Model.  Each model variable is defined as a method:
+### Model Class
+
+Create your model as a subclass of `heavylight.Model``.  Each model variable is defined as a method:
 
 ```python
-class Annuity(Model):
+import heavylight
+
+class Annuity(heavylight.Model):
     def t(self, t):
         return t
 
     def expected_claim(self, t):
         return self.number_alive(t) * self.data["annuity_per_period"]
 
     def number_alive(self, t):
@@ -53,14 +61,27 @@
             return self.number_alive(t - 1) - self.deaths(t - 1)
     
     def deaths(self, t):
         return self.number_alive(t) * self.mortality_rate(t)
 
     def mortality_rate(self, t):
         return 0.02
+
+    def v(self, t):
+        """discount factor from time t to time 0"""
+        if t == 0:
+            return 1
+        else:
+            return self.v(t - 1) / (1 + self.forward_rate(t))
+    
+    def forward_rate(self, t):
+        return 0.04
+
+    def pv_expected_claim(self, t):
+        return self.expected_claim(t) * self.v(t)
 ```
 
 Define input data as a dictionary
 
 ```python
 policy_data = {
     "initial_policies": 10,
@@ -73,28 +94,32 @@
 ```python
 model = Annuity(data = policy_data,
                 do_run = True,
                 proj_len = 20,
                 )
 ```
 
-display result as a pandas table
+Get the sum of `pv_expected_claim`:
 
 ```python
-model_cashflows = model.ToDataFrame()
+print(model.pv_expected_claim.sum())
 ```
 
-Use numpy_financial or another package to calculate NPVs.
 
-## Notes
 
-### Projecting vs. discounting
+Display result as a pandas table
+
+```python
+model_cashflows = model.ToDataFrame()
+```
+
+## Notes
 
  - This package is designed for projecting actuarial variables, and calculates t=0, 1... in order.
 
  - Actuarial models are generally highly recursive.
 
  - If you create a method which refers to future t value (such as an NPV function) you may hit the python stack limit.
 
- - The recommended solution is to project forward first, and then calculate T0 metrics based on the result.
+ - The recommended solution is to project forward first, and then calculate T0 metrics based on the result, for example using an `npv()`` function
```


# Comparing `tmp/fastgplearn-0.0.8.tar.gz` & `tmp/fastgplearn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgplearn-0.0.8.tar", last modified: Tue Nov  9 04:14:43 2021, max compression
+gzip compressed data, was "fastgplearn-0.0.9.tar", last modified: Tue Nov  9 08:08:34 2021, max compression
```

## Comparing `fastgplearn-0.0.8.tar` & `fastgplearn-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2021-11-09 04:14:43.011988 fastgplearn-0.0.8/
--rw-rw-rw-   0        0        0     1088 2021-11-04 09:15:19.000000 fastgplearn-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      174 2021-11-08 06:29:00.000000 fastgplearn-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2545 2021-11-09 04:14:43.011015 fastgplearn-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1379 2021-11-09 03:56:21.000000 fastgplearn-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-11-09 04:14:42.956162 fastgplearn-0.0.8/fastgplearn/
--rw-rw-rw-   0        0        0      220 2021-11-07 15:05:02.000000 fastgplearn-0.0.8/fastgplearn/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:14:42.987055 fastgplearn-0.0.8/fastgplearn/backend/
--rw-rw-rw-   0        0        0     1150 2021-11-07 15:35:30.000000 fastgplearn-0.0.8/fastgplearn/backend/__init__.py
--rw-rw-rw-   0        0        0     1610 2021-11-07 12:19:54.000000 fastgplearn-0.0.8/fastgplearn/backend/c_numpy.py
--rw-rw-rw-   0        0        0     2300 2021-11-07 12:19:54.000000 fastgplearn-0.0.8/fastgplearn/backend/c_torch.py
--rw-rw-rw-   0        0        0     7889 2021-11-07 12:19:54.000000 fastgplearn-0.0.8/fastgplearn/backend/p_numpy.py
--rw-rw-rw-   0        0        0     5123 2021-11-07 12:19:54.000000 fastgplearn-0.0.8/fastgplearn/backend/p_torch.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:14:42.997052 fastgplearn-0.0.8/fastgplearn/cli/
--rw-rw-rw-   0        0        0      188 2021-11-05 07:07:01.000000 fastgplearn-0.0.8/fastgplearn/cli/__init__.py
--rw-rw-rw-   0        0        0      827 2021-11-07 16:38:54.000000 fastgplearn-0.0.8/fastgplearn/cli/cc_numpy.py
--rw-rw-rw-   0        0        0      888 2021-11-07 16:38:54.000000 fastgplearn-0.0.8/fastgplearn/cli/cc_torch.py
--rw-rw-rw-   0        0        0     3898 2021-11-07 16:41:18.000000 fastgplearn-0.0.8/fastgplearn/cli/main.py
--rw-rw-rw-   0        0        0     9705 2021-11-07 15:23:33.000000 fastgplearn-0.0.8/fastgplearn/gp.py
--rw-rw-rw-   0        0        0      415 2021-11-04 15:18:55.000000 fastgplearn-0.0.8/fastgplearn/sci_formula.py
--rw-rw-rw-   0        0        0    29342 2021-11-09 03:24:23.000000 fastgplearn-0.0.8/fastgplearn/skflow.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:14:43.003012 fastgplearn-0.0.8/fastgplearn/source/
--rw-rw-rw-   0        0        0     4145 2021-11-07 12:19:54.000000 fastgplearn-0.0.8/fastgplearn/source/np_tool.pyx
--rw-rw-rw-   0        0        0     5037 2021-11-07 10:25:29.000000 fastgplearn-0.0.8/fastgplearn/source/torch_tool.cpp
--rw-rw-rw-   0        0        0     4704 2021-11-09 03:22:58.000000 fastgplearn-0.0.8/fastgplearn/tools.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:14:42.974107 fastgplearn-0.0.8/fastgplearn.egg-info/
--rw-rw-rw-   0        0        0     2545 2021-11-09 04:14:42.000000 fastgplearn-0.0.8/fastgplearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2021-11-09 04:14:42.000000 fastgplearn-0.0.8/fastgplearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-09 04:14:42.000000 fastgplearn-0.0.8/fastgplearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2021-11-09 04:14:42.000000 fastgplearn-0.0.8/fastgplearn.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2021-11-09 04:14:42.000000 fastgplearn-0.0.8/fastgplearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-11-09 04:14:42.000000 fastgplearn-0.0.8/fastgplearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2021-11-08 09:36:02.000000 fastgplearn-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-11-09 04:14:43.012986 fastgplearn-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1749 2021-11-09 04:14:35.000000 fastgplearn-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-09 04:14:43.009016 fastgplearn-0.0.8/test/
--rw-rw-rw-   0        0        0     1168 2021-11-07 08:12:44.000000 fastgplearn-0.0.8/test/test_classfier_general.py
--rw-rw-rw-   0        0        0     1076 2021-11-07 07:43:52.000000 fastgplearn-0.0.8/test/test_regressor_general.py
+drwxrwxrwx   0        0        0        0 2021-11-09 08:08:34.544968 fastgplearn-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2021-11-04 09:15:19.000000 fastgplearn-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      174 2021-11-08 06:29:00.000000 fastgplearn-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2545 2021-11-09 08:08:34.544968 fastgplearn-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1379 2021-11-09 03:56:21.000000 fastgplearn-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-11-09 08:08:34.491130 fastgplearn-0.0.9/fastgplearn/
+-rw-rw-rw-   0        0        0      220 2021-11-07 15:05:02.000000 fastgplearn-0.0.9/fastgplearn/__init__.py
+drwxrwxrwx   0        0        0        0 2021-11-09 08:08:34.520034 fastgplearn-0.0.9/fastgplearn/backend/
+-rw-rw-rw-   0        0        0     1150 2021-11-07 15:35:30.000000 fastgplearn-0.0.9/fastgplearn/backend/__init__.py
+-rw-rw-rw-   0        0        0     1610 2021-11-07 12:19:54.000000 fastgplearn-0.0.9/fastgplearn/backend/c_numpy.py
+-rw-rw-rw-   0        0        0     2300 2021-11-07 12:19:54.000000 fastgplearn-0.0.9/fastgplearn/backend/c_torch.py
+-rw-rw-rw-   0        0        0     7889 2021-11-07 12:19:54.000000 fastgplearn-0.0.9/fastgplearn/backend/p_numpy.py
+-rw-rw-rw-   0        0        0     5123 2021-11-07 12:19:54.000000 fastgplearn-0.0.9/fastgplearn/backend/p_torch.py
+drwxrwxrwx   0        0        0        0 2021-11-09 08:08:34.531006 fastgplearn-0.0.9/fastgplearn/cli/
+-rw-rw-rw-   0        0        0      188 2021-11-05 07:07:01.000000 fastgplearn-0.0.9/fastgplearn/cli/__init__.py
+-rw-rw-rw-   0        0        0      827 2021-11-07 16:38:54.000000 fastgplearn-0.0.9/fastgplearn/cli/cc_numpy.py
+-rw-rw-rw-   0        0        0      888 2021-11-07 16:38:54.000000 fastgplearn-0.0.9/fastgplearn/cli/cc_torch.py
+-rw-rw-rw-   0        0        0     3898 2021-11-07 16:41:18.000000 fastgplearn-0.0.9/fastgplearn/cli/main.py
+-rw-rw-rw-   0        0        0     9705 2021-11-07 15:23:33.000000 fastgplearn-0.0.9/fastgplearn/gp.py
+-rw-rw-rw-   0        0        0      415 2021-11-04 15:18:55.000000 fastgplearn-0.0.9/fastgplearn/sci_formula.py
+-rw-rw-rw-   0        0        0    29325 2021-11-09 08:08:05.000000 fastgplearn-0.0.9/fastgplearn/skflow.py
+drwxrwxrwx   0        0        0        0 2021-11-09 08:08:34.535992 fastgplearn-0.0.9/fastgplearn/source/
+-rw-rw-rw-   0        0        0     4145 2021-11-07 12:19:54.000000 fastgplearn-0.0.9/fastgplearn/source/np_tool.pyx
+-rw-rw-rw-   0        0        0     5037 2021-11-07 10:25:29.000000 fastgplearn-0.0.9/fastgplearn/source/torch_tool.cpp
+-rw-rw-rw-   0        0        0     4704 2021-11-09 03:22:58.000000 fastgplearn-0.0.9/fastgplearn/tools.py
+drwxrwxrwx   0        0        0        0 2021-11-09 08:08:34.507070 fastgplearn-0.0.9/fastgplearn.egg-info/
+-rw-rw-rw-   0        0        0     2545 2021-11-09 08:08:34.000000 fastgplearn-0.0.9/fastgplearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2021-11-09 08:08:34.000000 fastgplearn-0.0.9/fastgplearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-11-09 08:08:34.000000 fastgplearn-0.0.9/fastgplearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2021-11-09 08:08:34.000000 fastgplearn-0.0.9/fastgplearn.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2021-11-09 08:08:34.000000 fastgplearn-0.0.9/fastgplearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2021-11-09 08:08:34.000000 fastgplearn-0.0.9/fastgplearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2021-11-08 09:36:02.000000 fastgplearn-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2021-11-09 08:08:34.545966 fastgplearn-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2021-11-09 08:08:25.000000 fastgplearn-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-11-09 08:08:34.541976 fastgplearn-0.0.9/test/
+-rw-rw-rw-   0        0        0     1168 2021-11-07 08:12:44.000000 fastgplearn-0.0.9/test/test_classfier_general.py
+-rw-rw-rw-   0        0        0     1076 2021-11-07 07:43:52.000000 fastgplearn-0.0.9/test/test_regressor_general.py
```

### Comparing `fastgplearn-0.0.8/LICENSE` & `fastgplearn-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/PKG-INFO` & `fastgplearn-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgplearn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fast fitting formula.
 Home-page: https://github.com/boliqq07/fastgplearn
 Author: wangchangxin
 Author-email: 986798607@qq.com
 Maintainer: wangchangxin
 License: UNKNOWN
 Description: [![Fastgplearn](./img.jpg)](https://gitee.com/boliqq07/fastgplearn)
```

### Comparing `fastgplearn-0.0.8/README.md` & `fastgplearn-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/backend/__init__.py` & `fastgplearn-0.0.9/fastgplearn/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/backend/c_numpy.py` & `fastgplearn-0.0.9/fastgplearn/backend/c_numpy.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/backend/c_torch.py` & `fastgplearn-0.0.9/fastgplearn/backend/c_torch.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/backend/p_numpy.py` & `fastgplearn-0.0.9/fastgplearn/backend/p_numpy.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/backend/p_torch.py` & `fastgplearn-0.0.9/fastgplearn/backend/p_torch.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/cli/cc_numpy.py` & `fastgplearn-0.0.9/fastgplearn/cli/cc_numpy.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/cli/cc_torch.py` & `fastgplearn-0.0.9/fastgplearn/cli/cc_torch.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/cli/main.py` & `fastgplearn-0.0.9/fastgplearn/cli/main.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/gp.py` & `fastgplearn-0.0.9/fastgplearn/gp.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/skflow.py` & `fastgplearn-0.0.9/fastgplearn/skflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
             func_p (np.ndarray,tuple): with shape (n_function,), probability values of each function.
             sci_preset (str,list): None, "default" or user self-defined list template, default None.
 
 
         """
 
         assert population_size > 100 and generations >= 1
-        # assert store_of_fame <= 0.01 * population_size
         assert tournament_size <= 30 and hall_of_fame <= store_of_fame
         assert hall_of_fame >= 1
         assert store_of_fame >= 10
+        assert depth[1] <= 8
         try:
             self.func_names, self._str_name, self._score_mp, self._score, self._cal = backend[method_backend]
         except KeyError:
             raise NotImplementedError(
                 f"The {method_backend} is just accessible after be compiled, see more in 'Install'.")
         self.population_size = self.pop_n = population_size
         self.hall_of_fame = hall_of_fame
@@ -461,15 +461,15 @@
             n (int): calculate by the n_ed expression.
 
         Returns:
             score (float): Mean r2 of ``self.predict(X)`` wrt. `y`.
         """
         return super().score(X, y, scoring, n=n)
 
-    def top_n(self, n, scoring="r2"):
+    def top_n(self, n=0, scoring="r2"):
         """Print the top n result. The best one is index 0.
 
         Args:
             scoring (str): see also sklearn.metrics.
             n (int): calculate by the n_ed expression.
 
         """
@@ -478,15 +478,15 @@
         func = scorer._score_func
         sign = scorer._sign
 
         self.logs.record_and_print(" ")
         self.logs.record_and_print(f"The top {n} result:")
         self.logs.record_and_print(f"Scoring by {scoring}: ( score, expression, coef, intercept )")
 
-        for ni in range(n):
+        for ni in range(1,n+1):
             pre_y, coef_, intercept_ = self.single_cal(n=n, with_coef=True)
             msg = str((sign * func(self.y, pre_y), self.single_name(ni), coef_, intercept_))
             self.logs.record_and_print(msg)
 
     def best_expression(self, scoring="r2"):
         """Print the best expression."""
         self.top_n(n=0, scoring=scoring)
@@ -650,15 +650,15 @@
         scorer = get_scorer(scoring=scoring)
         func = scorer._score_func
         sign = scorer._sign
 
         self.logs.record_and_print(f"The top {n} result:")
         self.logs.record_and_print(f"Scoring by {scoring}: ( score, expression, coef, intercept )")
 
-        for ni in range(n):
+        for ni in range(1, n+1):
             pre_y, coef_, intercept_ = self.single_cal(n=n, with_coef=True)
             msg = str((sign * func(self.y, self.cla(pre_y)), self.single_name(ni), coef_, intercept_))
             self.logs.record_and_print(msg)
 
     def best_expression(self, scoring="accuracy"):
         """Print the best expression."""
         self.top_n(n=0, scoring=scoring)
```

### Comparing `fastgplearn-0.0.8/fastgplearn/source/np_tool.pyx` & `fastgplearn-0.0.9/fastgplearn/source/np_tool.pyx`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/source/torch_tool.cpp` & `fastgplearn-0.0.9/fastgplearn/source/torch_tool.cpp`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn/tools.py` & `fastgplearn-0.0.9/fastgplearn/tools.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/fastgplearn.egg-info/PKG-INFO` & `fastgplearn-0.0.9/fastgplearn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgplearn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fast fitting formula.
 Home-page: https://github.com/boliqq07/fastgplearn
 Author: wangchangxin
 Author-email: 986798607@qq.com
 Maintainer: wangchangxin
 License: UNKNOWN
 Description: [![Fastgplearn](./img.jpg)](https://gitee.com/boliqq07/fastgplearn)
```

### Comparing `fastgplearn-0.0.8/fastgplearn.egg-info/SOURCES.txt` & `fastgplearn-0.0.9/fastgplearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/setup.py` & `fastgplearn-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
 
     name='fastgplearn',
-    version='0.0.08',
+    version='0.0.09',
     keywords=['genetic programming","symbolic learning'],
     description='Fast fitting formula.',
     install_requires=['pandas', 'numpy', 'scipy', 'scikit-learn', 'joblib', 'deprecated',
                       "mgetool"],
     include_package_data=True,
     author='wangchangxin',
     author_email='986798607@qq.com',
```

### Comparing `fastgplearn-0.0.8/test/test_classfier_general.py` & `fastgplearn-0.0.9/test/test_classfier_general.py`

 * *Files identical despite different names*

### Comparing `fastgplearn-0.0.8/test/test_regressor_general.py` & `fastgplearn-0.0.9/test/test_regressor_general.py`

 * *Files identical despite different names*


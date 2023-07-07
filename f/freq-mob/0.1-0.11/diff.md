# Comparing `tmp/freq_mob-0.1.tar.gz` & `tmp/freq_mob-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freq_mob-0.1.tar", last modified: Wed Jul  5 02:14:54 2023, max compression
+gzip compressed data, was "freq_mob-0.11.tar", last modified: Fri Jul  7 03:54:04 2023, max compression
```

## Comparing `freq_mob-0.1.tar` & `freq_mob-0.11.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-05 02:14:54.070870 freq_mob-0.1/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2020-05-13 21:48:18.000000 freq_mob-0.1/LICENSE.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1718 2023-07-05 02:14:54.065334 freq_mob-0.1/PKG-INFO
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1295 2023-07-05 01:58:22.000000 freq_mob-0.1/README.md
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-05 02:14:54.033049 freq_mob-0.1/freq_mob/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       69 2023-07-04 21:48:53.000000 freq_mob-0.1/freq_mob/__init__.py
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    15954 2023-07-05 02:00:23.000000 freq_mob-0.1/freq_mob/freq_mob.py
-drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-05 02:14:54.065334 freq_mob-0.1/freq_mob.egg-info/
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1718 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/PKG-INFO
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/SOURCES.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/dependency_links.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/requires.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-07-05 02:14:53.000000 freq_mob-0.1/freq_mob.egg-info/top_level.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-05 02:14:54.070870 freq_mob-0.1/setup.cfg
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      692 2023-07-04 22:00:04.000000 freq_mob-0.1/setup.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-07 03:54:04.267164 freq_mob-0.11/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2020-05-13 21:48:18.000000 freq_mob-0.11/LICENSE.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1863 2023-07-07 03:54:04.267164 freq_mob-0.11/PKG-INFO
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1439 2023-07-05 19:45:19.000000 freq_mob-0.11/README.md
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-07 03:54:04.251525 freq_mob-0.11/freq_mob/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       69 2023-07-04 21:48:53.000000 freq_mob-0.11/freq_mob/__init__.py
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    16178 2023-07-06 01:34:22.000000 freq_mob-0.11/freq_mob/freq_mob.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-07 03:54:04.267164 freq_mob-0.11/freq_mob.egg-info/
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1863 2023-07-07 03:54:04.000000 freq_mob-0.11/freq_mob.egg-info/PKG-INFO
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-07-07 03:54:04.000000 freq_mob-0.11/freq_mob.egg-info/SOURCES.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-07-07 03:54:04.000000 freq_mob-0.11/freq_mob.egg-info/dependency_links.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-07 03:54:04.000000 freq_mob-0.11/freq_mob.egg-info/requires.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-07-07 03:54:04.000000 freq_mob-0.11/freq_mob.egg-info/top_level.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-07 03:54:04.267164 freq_mob-0.11/setup.cfg
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      693 2023-07-05 19:37:49.000000 freq_mob-0.11/setup.py
```

### Comparing `freq_mob-0.1/LICENSE.txt` & `freq_mob-0.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `freq_mob-0.1/PKG-INFO` & `freq_mob-0.11/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: freq_mob
-Version: 0.1
+Version: 0.11
 Summary: Monotonic Optimal Binning for Frequency Models
 Home-page: https://github.com/statcompute/freq_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 #### Introduction
 
 To mimic the py\_mob package (https://pypi.org/project/py-mob) for binary outcomes, the freq\_mob is a collection of python functions that would generate the monotonic binning and perform the variable transformation for frequency outcomes such that the Pearson correlation between the transformed X and Ln(Y) is equal to 1. 
 
+Should you have any question or suggestion about the freq\_mob package, please feel free to drop me a line. 
+
 #### Core Functions
 
 ```
 freq_mob
   |-- qtl_bin()  : An iterative discretization based on quantiles of X.  
   |-- cnt_bin()  : A revised iterative discretization for records with Y > 0.
   |-- iso_bin()  : A discretization algorthm driven by the isotonic regression between X and Y. 
-  |-- rng_bin()  : A revised iterative discretization based on the range of X values.  
+  |-- rng_bin()  : A revised iterative discretization based on the value range of X.  
   |-- kmn_bin()  : A discretization algorthm based on the kmeans clustering of X.  
   |-- gbm_bin()  : A discretization algorthm based on the gradient boosting machine.  
   |-- view_bin() : Displays the binning outcome in a tabular form. 
   `-- cal_newx() : Applies the variable transformation to a numeric vector based on the binning outcome.
 ```
 
 ###  Authors
 
 [WenSui Liu](mailto:liuwensui@gmail.com) is a seasoned data scientist with 15-year experience in the financial service industry. 
-[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student major in Mathematics. 
+
+[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student majoring in Mathematics with a passion for data science.
```

### Comparing `freq_mob-0.1/README.md` & `freq_mob-0.11/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #### Introduction
 
 To mimic the py\_mob package (https://pypi.org/project/py-mob) for binary outcomes, the freq\_mob is a collection of python functions that would generate the monotonic binning and perform the variable transformation for frequency outcomes such that the Pearson correlation between the transformed X and Ln(Y) is equal to 1. 
 
+Should you have any question or suggestion about the freq\_mob package, please feel free to drop me a line. 
+
 #### Core Functions
 
 ```
 freq_mob
   |-- qtl_bin()  : An iterative discretization based on quantiles of X.  
   |-- cnt_bin()  : A revised iterative discretization for records with Y > 0.
   |-- iso_bin()  : A discretization algorthm driven by the isotonic regression between X and Y. 
-  |-- rng_bin()  : A revised iterative discretization based on the range of X values.  
+  |-- rng_bin()  : A revised iterative discretization based on the value range of X.  
   |-- kmn_bin()  : A discretization algorthm based on the kmeans clustering of X.  
   |-- gbm_bin()  : A discretization algorthm based on the gradient boosting machine.  
   |-- view_bin() : Displays the binning outcome in a tabular form. 
   `-- cal_newx() : Applies the variable transformation to a numeric vector based on the binning outcome.
 ```
 
 ###  Authors
 
 [WenSui Liu](mailto:liuwensui@gmail.com) is a seasoned data scientist with 15-year experience in the financial service industry. 
-[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student major in Mathematics. 
+
+[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student majoring in Mathematics with a passion for data science.
```

### Comparing `freq_mob-0.1/freq_mob/freq_mob.py` & `freq_mob-0.11/freq_mob/freq_mob.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # freq_mob/freq_mob.py
-# version 0.1
+# version 0.11
 # import freq_mob
 
 import tabulate, numpy
 from scipy.stats import spearmanr
 from sklearn.isotonic import IsotonicRegression as isoreg
 from sklearn.cluster import KMeans as kmeans
 from sklearn import metrics 
@@ -201,15 +201,29 @@
   _tbl = [{**(lambda v: {k: v[k] for k in _sel})(_), "rule": _["rule"].ljust(45)} for _ in x["tbl"]]
 
   print(tabulate.tabulate(_tbl, headers = "keys", tablefmt = "github",
                           colalign = ["center"] + ["right"] * (len(_sel) - 1),
                           floatfmt = (".0f", ".0f", ".0f", ".4f", ".4f", ".4f")))
 
 
-########## 09. qtl_bin() ##########
+########## 09. head() ##########
+
+def head(seq, n = 3):
+  """
+  It shows first n (3 by default) items in a sequence.
+  Parameters:
+    seq : A list.
+    n   : A non-zero integer.
+  """
+
+  for _ in range(n):
+    print(seq[_])
+
+
+########## 11. qtl_bin() ##########
 
 def qtl_bin(x, y):
   """
   It discretizes the x vector based on percentiles and summarizes
   over the y vector to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
@@ -217,15 +231,14 @@
   Returns:
     A dictionary with two keys:
       "cut" : A numeric vector with cut points applied to the x vector.
       "tbl" : A list of dictionaries summarizing the binning outcome.
   """
 
   _data = [_ for _ in zip(x, y, ~numpy.isnan(x))]
-
   _x = [_[0] for _ in _data if _[2] == 1]
   _y = [_[1] for _ in _data if _[2] == 1]
 
   _n = numpy.arange(2, max(3, min(100, len(numpy.unique(_x)) - 1)))
   _p = set(tuple(qcut(_x, _)) for _ in _n)
 
   _l1 = [[_, manual_bin(_x, _y, _)] for _ in _p]
@@ -241,15 +254,15 @@
 
   _l4 = sorted(*[l[1] for l in _l1 if l[0] == _l3], key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _l3, "tbl": gen_rule(gen_newx(_l5), _l3)})
 
-########## 10. iso_bin() ##########
+########## 12. iso_bin() ##########
 
 def iso_bin(x, y):
   """
   It discretizes the x vector based on the isotonic regression and summarizes
   over the y vector to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
@@ -257,15 +270,14 @@
   Returns:
     A dictionary with two keys:
       "cut" : A numeric vector with cut points applied to the x vector.
       "tbl" : A list of dictionaries summarizing the binning outcome.
   """
 
   _data = [_ for _ in zip(x, y, ~numpy.isnan(x))]
-
   _x = [_[0] for _ in _data if _[2] == 1]
   _y = [_[1] for _ in _data if _[2] == 1]
 
   _cor = spearmanr(_x, _y)[0]
   _reg = isoreg()
 
   _f = numpy.abs(_reg.fit_transform(_x, list(map(lambda y:  y * _cor / numpy.abs(_cor), _y))))
@@ -284,15 +296,15 @@
 
   _l4 = sorted(manual_bin(_x, _y, _p), key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _p, "tbl": gen_rule(gen_newx(_l5), _p)})
 
-########## 11. gbm_bin() ##########
+########## 13. gbm_bin() ##########
 
 def gbm_bin(x, y):
   """
   It discretizes the x vector based on the gradient boosting machine and
   summarizes over the y vector to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize. It is a list, 1-D numpy array,
@@ -302,15 +314,14 @@
   Returns:
     A dictionary with two keys:
       "cut" : A numeric vector with cut points applied to the x vector.
       "tbl" : A list of dictionaries summarizing the binning outcome.
   """
 
   _data = [_ for _ in zip(x, y, ~numpy.isnan(x))]
-
   _x = [_[0] for _ in _data if _[2] == 1]
   _y = [_[1] for _ in _data if _[2] == 1]
 
   _cor = spearmanr(_x, _y)[0]
   _con = "1" if _cor > 0 else "-1"
 
   _gbm = gbmreg(num_leaves = 100, min_child_samples = 3, n_estimators = 1,
@@ -334,19 +345,19 @@
 
   _l4 = sorted(manual_bin(_x, _y, _p), key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _p, "tbl": gen_rule(gen_newx(_l5), _p)})
 
-########## 12. rng_bin() ##########
+########## 14. rng_bin() ##########
 
 def rng_bin(x, y):
   """
-  It discretizes the x vector based on the range of x values and summarizes over
+  It discretizes the x vector based on the value range of x and summarizes over
   the y vector to derive the variable transformaton.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
     y : A numeric vector of frequency outcomes with the same length of x.
   Returns:
     A dictionary with two keys:
       "cut" : A numeric vector with cut points applied to the x vector.
@@ -377,15 +388,15 @@
 
   _l4 = sorted(*[l[1] for l in _l1 if l[0] == _l3], key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _l3, "tbl": gen_rule(gen_newx(_l5), _l3)})
 
-########## 13. kmn_bin() ##########
+########## 15. kmn_bin() ##########
 
 def kmn_bin(x, y):
   """
   It discretizes the x vector based on the kmeans clustering and summarizes over 
   the y vector to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
@@ -428,15 +439,15 @@
 
   _l4 = sorted(*[l[1] for l in _l1 if l[0] == _l3], key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _l3, "tbl": gen_rule(gen_newx(_l5), _l3)})
 
-########## 14. cnt_bin() ##########
+########## 16. cnt_bin() ##########
 
 def cnt_bin(x, y):
   """
   It discretizes the x vector based on percentiles and summarizes over
   the y vector with y > 0, i.e. nonzero count, to derive the variable transformation.
   Parameters:
     x : A numeric vector to discretize, e.g. list, numpy array, or pandas series.
```

### Comparing `freq_mob-0.1/freq_mob.egg-info/PKG-INFO` & `freq_mob-0.11/freq_mob.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: freq-mob
-Version: 0.1
+Version: 0.11
 Summary: Monotonic Optimal Binning for Frequency Models
 Home-page: https://github.com/statcompute/freq_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 #### Introduction
 
 To mimic the py\_mob package (https://pypi.org/project/py-mob) for binary outcomes, the freq\_mob is a collection of python functions that would generate the monotonic binning and perform the variable transformation for frequency outcomes such that the Pearson correlation between the transformed X and Ln(Y) is equal to 1. 
 
+Should you have any question or suggestion about the freq\_mob package, please feel free to drop me a line. 
+
 #### Core Functions
 
 ```
 freq_mob
   |-- qtl_bin()  : An iterative discretization based on quantiles of X.  
   |-- cnt_bin()  : A revised iterative discretization for records with Y > 0.
   |-- iso_bin()  : A discretization algorthm driven by the isotonic regression between X and Y. 
-  |-- rng_bin()  : A revised iterative discretization based on the range of X values.  
+  |-- rng_bin()  : A revised iterative discretization based on the value range of X.  
   |-- kmn_bin()  : A discretization algorthm based on the kmeans clustering of X.  
   |-- gbm_bin()  : A discretization algorthm based on the gradient boosting machine.  
   |-- view_bin() : Displays the binning outcome in a tabular form. 
   `-- cal_newx() : Applies the variable transformation to a numeric vector based on the binning outcome.
 ```
 
 ###  Authors
 
 [WenSui Liu](mailto:liuwensui@gmail.com) is a seasoned data scientist with 15-year experience in the financial service industry. 
-[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student major in Mathematics. 
+
+[Joyce Liu](mailto:jcl4482@my.utexas.edu) is a college student majoring in Mathematics with a passion for data science.
```

### Comparing `freq_mob-0.1/setup.py` & `freq_mob-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r") as fh:
   long_description = fh.read()
  
 setuptools.setup(
   name = "freq_mob",
-  version = "0.1",
+  version = "0.11",
   author = "WenSui Liu",
   author_email = "liuwensui@gmail.com",
   description = "Monotonic Optimal Binning for Frequency Models",
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = "https://github.com/statcompute/freq_mob",
   packages = setuptools.find_packages(),
```


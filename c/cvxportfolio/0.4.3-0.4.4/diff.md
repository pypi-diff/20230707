# Comparing `tmp/cvxportfolio-0.4.3.tar.gz` & `tmp/cvxportfolio-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.4.3.tar", last modified: Wed Jul  5 16:26:18 2023, max compression
+gzip compressed data, was "cvxportfolio-0.4.4.tar", last modified: Fri Jul  7 06:00:21 2023, max compression
```

## Comparing `cvxportfolio-0.4.3.tar` & `cvxportfolio-0.4.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-05 16:26:18.261479 cvxportfolio-0.4.3/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.4.3/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.4.3/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)     5442 2023-07-05 16:26:18.261158 cvxportfolio-0.4.3/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     5072 2023-07-03 17:30:09.000000 cvxportfolio-0.4.3/README.md
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-05 16:26:18.248103 cvxportfolio-0.4.3/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)     1018 2023-07-05 16:23:56.000000 cvxportfolio-0.4.3/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     2638 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/benchmark.py
--rw-r--r--   0 enzo       (501) staff       (20)    11909 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    19207 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    20371 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/data.py
--rw-r--r--   0 enzo       (501) staff       (20)     1001 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    15860 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)     4167 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/hyperparameters.py
--rw-r--r--   0 enzo       (501) staff       (20)    22839 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     7060 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)     8648 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    14416 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    33741 2023-07-05 16:21:09.000000 cvxportfolio-0.4.3/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-05 16:26:18.260609 cvxportfolio-0.4.3/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)        0 2023-07-05 16:23:56.000000 cvxportfolio-0.4.3/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1680 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/base.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.4.3/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.4.3/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)    10279 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    10139 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     7182 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     8995 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)     3725 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_hyperparameters.py
--rw-r--r--   0 enzo       (501) staff       (20)    22397 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     5996 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     9361 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    25890 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.4.3/cvxportfolio/tests/volumes.csv
--rw-r--r--   0 enzo       (501) staff       (20)     1325 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/utils.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-05 16:26:18.250368 cvxportfolio-0.4.3/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)     5442 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     1094 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)       65 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)       38 2023-07-05 16:26:18.261562 cvxportfolio-0.4.3/setup.cfg
--rw-r--r--   0 enzo       (501) staff       (20)     1032 2023-07-05 16:23:56.000000 cvxportfolio-0.4.3/setup.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-07 06:00:21.937893 cvxportfolio-0.4.4/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.4.4/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.4.4/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)     6461 2023-07-07 06:00:21.937534 cvxportfolio-0.4.4/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     6091 2023-07-07 05:51:38.000000 cvxportfolio-0.4.4/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-07 06:00:21.922005 cvxportfolio-0.4.4/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)     1018 2023-07-07 05:54:53.000000 cvxportfolio-0.4.4/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     2638 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/benchmark.py
+-rw-r--r--   0 enzo       (501) staff       (20)    11909 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)    19207 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    20371 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1001 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    15914 2023-07-07 05:51:38.000000 cvxportfolio-0.4.4/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)     4167 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/hyperparameters.py
+-rw-r--r--   0 enzo       (501) staff       (20)    22839 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     7060 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8648 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    14416 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    33774 2023-07-07 05:51:38.000000 cvxportfolio-0.4.4/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-07 06:00:21.936930 cvxportfolio-0.4.4/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-07-07 05:54:53.000000 cvxportfolio-0.4.4/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1680 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.4.4/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.4.4/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)    10279 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10139 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     7171 2023-07-07 05:51:38.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8995 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)     3725 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_hyperparameters.py
+-rw-r--r--   0 enzo       (501) staff       (20)    22397 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     5996 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9361 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    25890 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.4.4/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     1325 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-07 06:00:21.924106 cvxportfolio-0.4.4/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)     6461 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     1094 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       65 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-07-07 06:00:21.938017 cvxportfolio-0.4.4/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)     1032 2023-07-07 05:54:53.000000 cvxportfolio-0.4.4/setup.py
```

### Comparing `cvxportfolio-0.4.3/LICENSE` & `cvxportfolio-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/PKG-INFO` & `cvxportfolio-0.4.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: cvxportfolio
-Version: 0.4.3
-Summary: Portfolio optimization.
-Home-page: https://cvxportfolio.readthedocs.io
-Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
-Author-email: enzo.busseti@gmail.com
-Maintainer: Enzo Busseti
-License: Apache 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
 # Cvxportfolio
 
 [![CVXportfolio on PyPI](https://img.shields.io/pypi/v/cvxportfolio.svg)](https://pypi.org/project/cvxportfolio/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cvxportfolio?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cvxportfolio)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/cvxportfolio/badge.svg?branch=master)](https://coveralls.io/github/cvxgrp/cvxportfolio?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/cvxportfolio/badge/?version=latest)](https://cvxportfolio.readthedocs.io/en/latest/?badge=latest)
 
@@ -40,16 +27,16 @@
 We ship our unit test suite with the pip package. After installing you can test in you local environment by
 
 ```
 python -m unittest discover cvxportfolio
 ```
 
 
-Example
-------------
+Simplest Example
+----------------
 In the following example market data is downloaded by a public source
 (Yahoo finance) and the forecasts are computed iteratively, at each point in the backtest, from past data. 
 That is, at each point in the backtest,
 the policy object only operates on **past data**, and thus the result you get is a realistic simulation of what the strategy would have performed in the market.
 The simulator by default includes holding and transaction costs, using the models described in the book, and default parameters that are typical for the US stock market.
 The logic used
 matches what is described in Chapter 7 of the book. For example, returns are forecasted as the historical mean returns 
@@ -77,14 +64,29 @@
 # print backtest result statistics
 print(result)
 
 # plot backtest results
 result.plot()
 ```
 
+Some Other Examples
+-------------------
+We show in the example on [user-provided forecasters](https://github.com/cvxgrp/cvxportfolio/blob/master/examples/user_provided_forecasters.py) how the user can define custom classes to forecast
+the expected returns and covariances. These provide callbacks that are
+executed at each point in time during the backtest. The system enforces 
+causality and safety against numerical errors. 
+We recommend to always include 
+the default forecasters that we provide in any analysis you may do, 
+since they are very robust and well-tested. 
+
+We show in the examples on [DOW30 components](https://github.com/cvxgrp/cvxportfolio/blob/master/examples/dow30_example.py) and [wide assets-classes ETFs](https://github.com/cvxgrp/cvxportfolio/blob/master/examples/etfs_example.py) how a
+simple sweep over hyper-parameters, taking advantage of our sophisticated parallel backtest machinery, quickly provides results on the best strategy
+to apply to any given selection of assets.
+
+
 Development
 -----------
 To set up a development environment locally you should
 
 ```
 git clone https://github.com/cvxgrp/cvxportfolio.git
 cd cvxportfolio
```

### Comparing `cvxportfolio-0.4.3/cvxportfolio/__init__.py` & `cvxportfolio-0.4.4/cvxportfolio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Cvxportfolio __init__ module.
 
 This module only republishes the api of a selection of cvxportfolio modules.
 The __all__ attribute of each is used.
 """
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 from .simulator import *
 from .policies import *
 from .constraints import *
 from .costs import *
 from .returns import *
 from .risks import *
```

### Comparing `cvxportfolio-0.4.3/cvxportfolio/benchmark.py` & `cvxportfolio-0.4.4/cvxportfolio/benchmark.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/constraints.py` & `cvxportfolio-0.4.4/cvxportfolio/constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/costs.py` & `cvxportfolio-0.4.4/cvxportfolio/costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/data.py` & `cvxportfolio-0.4.4/cvxportfolio/data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/errors.py` & `cvxportfolio-0.4.4/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/estimator.py` & `cvxportfolio-0.4.4/cvxportfolio/estimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,27 +189,27 @@
         raise DataError(
             f"{self.__class__.__name__}._recursive_values_in_time result is not a scalar or array."
         )
 
     def internal__recursive_values_in_time(self, t, *args, **kwargs):
         """Internal method called by `self._recursive_values_in_time`."""
 
-        if hasattr(self.data, "_recursive_values_in_time"):
-            return self.value_checker(
-                self.data._recursive_values_in_time(
-                    t, *args, **kwargs))
+        if hasattr(self.data, "values_in_time"):
+            _ = self.data.values_in_time(t=t, *args, **kwargs)
+            if hasattr(_, 'values'):
+                return self.value_checker(_.values)
+            else:
+                return self.value_checker(_)
+                                
 
-        if (
-            hasattr(self.data, "loc")
-            and hasattr(self.data, "index")
-            and (
-                isinstance(self.data.index, pd.DatetimeIndex)
+        if (hasattr(self.data, "loc") and hasattr(self.data, "index")
+            and (isinstance(self.data.index, pd.DatetimeIndex)
                 or (
-                    isinstance(self.data.index, pd.MultiIndex)
-                    and isinstance(self.data.index.levels[0], pd.DatetimeIndex)
+                isinstance(self.data.index, pd.MultiIndex)
+                and isinstance(self.data.index.levels[0], pd.DatetimeIndex)
                 )
             )
         ):
             try:
                 if self.use_last_available_time:
                     if isinstance(self.data.index, pd.MultiIndex):
                         newt = self.data.index.levels[0][
```

### Comparing `cvxportfolio-0.4.3/cvxportfolio/forecast.py` & `cvxportfolio-0.4.4/cvxportfolio/forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/hyperparameters.py` & `cvxportfolio-0.4.4/cvxportfolio/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/policies.py` & `cvxportfolio-0.4.4/cvxportfolio/policies.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/result.py` & `cvxportfolio-0.4.4/cvxportfolio/result.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/returns.py` & `cvxportfolio-0.4.4/cvxportfolio/returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/risks.py` & `cvxportfolio-0.4.4/cvxportfolio/risks.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/simulator.py` & `cvxportfolio-0.4.4/cvxportfolio/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,19 +125,19 @@
             self._get_market_data(universe, datasource)
             self._add_cash_column(self.cash_key)
             self._remove_missing_recent()
         else:
             if returns is None:
                 raise SyntaxError(
                     "If you don't specify a universe you should pass `returns`.")
-            self.returns = pd.DataFrame(returns, copy=copy)
+            self.returns = pd.DataFrame(returns, copy=copy_dataframes)
             self.volumes = volumes if volumes is None else \
-                pd.DataFrame(volumes, copy=copy)
+                pd.DataFrame(volumes, copy=copy_dataframes)
             self.prices = prices if prices is None else \
-                pd.DataFrame(prices, copy=copy)
+                pd.DataFrame(prices, copy=copy_dataframes)
             if cash_key != returns.columns[-1]:
                 self._add_cash_column(cash_key)
 
         if trading_frequency:
             self._downsample(trading_frequency)
 
         self._set_read_only()
@@ -422,15 +422,15 @@
                  min_history=pd.Timedelta('365d'),
                  datasource='YFinance',
                  cash_key="USDOLLAR", base_location=BASE_LOCATION,
                  trading_frequency=None, **kwargs):
         """Initialize the Simulator and download data if necessary."""
         self.base_location = Path(base_location)
         
-        self.enable_caching = not len(universe)
+        self.enable_caching = len(universe) > 0
 
         self.market_data = MarketData(
             universe=universe, returns=returns,
             volumes=volumes, prices=prices,
             cash_key=cash_key, base_location=base_location,
             trading_frequency=trading_frequency,
             min_history=min_history,
```

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/base.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/base.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/returns.csv` & `cvxportfolio-0.4.4/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-0.4.4/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_costs.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_data.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from cvxportfolio.errors import MissingValuesError, DataError
 
 
 class PlaceholderCallable:
     def __init__(self, value):
         self.value = value
 
-    def _recursive_values_in_time(self, t, **kwargs):
+    def values_in_time(self, t, **kwargs):
         return self.value
 
 
 class TestEstimators(unittest.TestCase):
 
     def test_callable(self):
         estimator = DataEstimator(PlaceholderCallable(1.0))
```

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_hyperparameters.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_policies.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_policies.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_returns.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_risks.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_risks.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-0.4.4/cvxportfolio/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/tests/volumes.csv` & `cvxportfolio-0.4.4/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio/utils.py` & `cvxportfolio-0.4.4/cvxportfolio/utils.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/cvxportfolio.egg-info/PKG-INFO` & `cvxportfolio-0.4.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 0.4.3
+Version: 0.4.4
 Summary: Portfolio optimization.
 Home-page: https://cvxportfolio.readthedocs.io
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Author-email: enzo.busseti@gmail.com
 Maintainer: Enzo Busseti
 License: Apache 2.0
 Description-Content-Type: text/markdown
@@ -40,16 +40,16 @@
 We ship our unit test suite with the pip package. After installing you can test in you local environment by
 
 ```
 python -m unittest discover cvxportfolio
 ```
 
 
-Example
-------------
+Simplest Example
+----------------
 In the following example market data is downloaded by a public source
 (Yahoo finance) and the forecasts are computed iteratively, at each point in the backtest, from past data. 
 That is, at each point in the backtest,
 the policy object only operates on **past data**, and thus the result you get is a realistic simulation of what the strategy would have performed in the market.
 The simulator by default includes holding and transaction costs, using the models described in the book, and default parameters that are typical for the US stock market.
 The logic used
 matches what is described in Chapter 7 of the book. For example, returns are forecasted as the historical mean returns 
@@ -77,14 +77,29 @@
 # print backtest result statistics
 print(result)
 
 # plot backtest results
 result.plot()
 ```
 
+Some Other Examples
+-------------------
+We show in the example on [user-provided forecasters](https://github.com/cvxgrp/cvxportfolio/blob/master/examples/user_provided_forecasters.py) how the user can define custom classes to forecast
+the expected returns and covariances. These provide callbacks that are
+executed at each point in time during the backtest. The system enforces 
+causality and safety against numerical errors. 
+We recommend to always include 
+the default forecasters that we provide in any analysis you may do, 
+since they are very robust and well-tested. 
+
+We show in the examples on [DOW30 components](https://github.com/cvxgrp/cvxportfolio/blob/master/examples/dow30_example.py) and [wide assets-classes ETFs](https://github.com/cvxgrp/cvxportfolio/blob/master/examples/etfs_example.py) how a
+simple sweep over hyper-parameters, taking advantage of our sophisticated parallel backtest machinery, quickly provides results on the best strategy
+to apply to any given selection of assets.
+
+
 Development
 -----------
 To set up a development environment locally you should
 
 ```
 git clone https://github.com/cvxgrp/cvxportfolio.git
 cd cvxportfolio
```

### Comparing `cvxportfolio-0.4.3/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-0.4.4/cvxportfolio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.3/setup.py` & `cvxportfolio-0.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_descr = ''.join(f.readlines())
 
 setup(
     name='cvxportfolio',
-    version='0.4.3',
+    version='0.4.4',
     author='Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.',
     maintainer='Enzo Busseti',
     author_email='enzo.busseti@gmail.com',
     packages=['cvxportfolio',
               'cvxportfolio.tests'],
     package_dir={'cvxportfolio': 'cvxportfolio'},
     package_data={'cvxportfolio': [
```


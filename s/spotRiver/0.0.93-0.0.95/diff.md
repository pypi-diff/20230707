# Comparing `tmp/spotRiver-0.0.93.tar.gz` & `tmp/spotRiver-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotRiver-0.0.93.tar", last modified: Sat Jun 10 19:47:21 2023, max compression
+gzip compressed data, was "spotRiver-0.0.95.tar", last modified: Fri Jul  7 07:12:45 2023, max compression
```

## Comparing `spotRiver-0.0.93.tar` & `spotRiver-0.0.95.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.367777 spotRiver-0.0.93/
--rw-r--r--   0 bartz      (501) staff       (20)     1520 2023-01-29 11:49:35.000000 spotRiver-0.0.93/LICENSE
--rw-r--r--   0 bartz      (501) staff       (20)      164 2023-03-22 20:43:16.000000 spotRiver-0.0.93/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-06-10 19:47:21.367651 spotRiver-0.0.93/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-01-29 16:41:52.000000 spotRiver-0.0.93/README.md
--rw-r--r--   0 bartz      (501) staff       (20)     1046 2023-06-08 18:54:56.000000 spotRiver-0.0.93/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-06-10 19:47:21.367816 spotRiver-0.0.93/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.361489 spotRiver-0.0.93/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.362091 spotRiver-0.0.93/src/spotRiver/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.365472 spotRiver-0.0.93/src/spotRiver/data/
--rw-r--r--   0 bartz      (501) staff       (20)      413 2023-01-29 11:52:00.000000 spotRiver-0.0.93/src/spotRiver/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2182 2023-01-17 12:39:58.000000 spotRiver-0.0.93/src/spotRiver/data/airline-passengers.csv
--rw-r--r--   0 bartz      (501) staff       (20)     1023 2023-03-27 20:31:30.000000 spotRiver-0.0.93/src/spotRiver/data/airline_passengers.py
--rw-r--r--   0 bartz      (501) staff       (20)    13646 2023-03-22 20:37:51.000000 spotRiver-0.0.93/src/spotRiver/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)     1113 2023-03-13 20:26:53.000000 spotRiver-0.0.93/src/spotRiver/data/bike_sharing.py
--rw-r--r--   0 bartz      (501) staff       (20)     1870 2023-03-07 16:50:39.000000 spotRiver-0.0.93/src/spotRiver/data/generic.py
--rw-r--r--   0 bartz      (501) staff       (20)     7751 2023-03-07 16:50:39.000000 spotRiver-0.0.93/src/spotRiver/data/opm.py
--rw-r--r--   0 bartz      (501) staff       (20)    17554 2023-04-08 14:44:16.000000 spotRiver-0.0.93/src/spotRiver/data/river_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-03-31 21:04:02.000000 spotRiver-0.0.93/src/spotRiver/data/river_hyper_dict.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.365708 spotRiver-0.0.93/src/spotRiver/data/synth/
--rw-r--r--   0 bartz      (501) staff       (20)      328 2023-01-18 17:25:51.000000 spotRiver-0.0.93/src/spotRiver/data/synth/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2442 2023-02-20 15:46:37.000000 spotRiver-0.0.93/src/spotRiver/data/synth/sea.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.365829 spotRiver-0.0.93/src/spotRiver/drift/
--rw-r--r--   0 bartz      (501) staff       (20)      767 2023-02-20 15:46:37.000000 spotRiver-0.0.93/src/spotRiver/drift/drift_generator.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.366408 spotRiver-0.0.93/src/spotRiver/evaluation/
--rw-r--r--   0 bartz      (501) staff       (20)    29393 2023-04-06 12:46:27.000000 spotRiver-0.0.93/src/spotRiver/evaluation/eval_bml.py
--rw-r--r--   0 bartz      (501) staff       (20)     3958 2023-02-26 22:39:12.000000 spotRiver-0.0.93/src/spotRiver/evaluation/eval_nowcast.py
--rw-r--r--   0 bartz      (501) staff       (20)     6752 2023-04-06 12:44:54.000000 spotRiver-0.0.93/src/spotRiver/evaluation/eval_oml.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.366746 spotRiver-0.0.93/src/spotRiver/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     5391 2023-06-10 18:01:21.000000 spotRiver-0.0.93/src/spotRiver/fun/hyperriver.py
--rw-r--r--   0 bartz      (501) staff       (20)    32460 2023-04-22 19:31:59.000000 spotRiver-0.0.93/src/spotRiver/fun/hyperriver_old.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.366908 spotRiver-0.0.93/src/spotRiver/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1340 2023-03-11 14:52:45.000000 spotRiver-0.0.93/src/spotRiver/plot/stats.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.367061 spotRiver-0.0.93/src/spotRiver/preprocess/
--rw-r--r--   0 bartz      (501) staff       (20)     2488 2023-03-07 16:50:39.000000 spotRiver-0.0.93/src/spotRiver/preprocess/impute.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.367331 spotRiver-0.0.93/src/spotRiver/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2033 2023-04-04 17:58:20.000000 spotRiver-0.0.93/src/spotRiver/utils/data_conversion.py
--rw-r--r--   0 bartz      (501) staff       (20)     5549 2023-04-13 20:07:21.000000 spotRiver-0.0.93/src/spotRiver/utils/features.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.363601 spotRiver-0.0.93/src/spotRiver.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-06-10 19:47:21.000000 spotRiver-0.0.93/src/spotRiver.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)      987 2023-06-10 19:47:21.000000 spotRiver-0.0.93/src/spotRiver.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-06-10 19:47:21.000000 spotRiver-0.0.93/src/spotRiver.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       20 2023-06-10 19:47:21.000000 spotRiver-0.0.93/src/spotRiver.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       10 2023-06-10 19:47:21.000000 spotRiver-0.0.93/src/spotRiver.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-10 19:47:21.367470 spotRiver-0.0.93/test/
--rw-r--r--   0 bartz      (501) staff       (20)      510 2023-02-25 09:55:05.000000 spotRiver-0.0.93/test/test_features.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.069869 spotRiver-0.0.95/
+-rw-r--r--   0 bartz      (501) staff       (20)     1520 2023-01-29 11:49:35.000000 spotRiver-0.0.95/LICENSE
+-rw-r--r--   0 bartz      (501) staff       (20)      164 2023-03-22 20:43:16.000000 spotRiver-0.0.95/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-07-07 07:12:45.069758 spotRiver-0.0.95/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-01-29 16:41:52.000000 spotRiver-0.0.95/README.md
+-rw-r--r--   0 bartz      (501) staff       (20)     1046 2023-07-06 18:58:29.000000 spotRiver-0.0.95/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-07-07 07:12:45.069908 spotRiver-0.0.95/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.064656 spotRiver-0.0.95/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.065341 spotRiver-0.0.95/src/spotRiver/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.068029 spotRiver-0.0.95/src/spotRiver/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      413 2023-01-29 11:52:00.000000 spotRiver-0.0.95/src/spotRiver/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2182 2023-01-17 12:39:58.000000 spotRiver-0.0.95/src/spotRiver/data/airline-passengers.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     1023 2023-03-27 20:31:30.000000 spotRiver-0.0.95/src/spotRiver/data/airline_passengers.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13646 2023-03-22 20:37:51.000000 spotRiver-0.0.95/src/spotRiver/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1113 2023-03-13 20:26:53.000000 spotRiver-0.0.95/src/spotRiver/data/bike_sharing.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1870 2023-03-07 16:50:39.000000 spotRiver-0.0.95/src/spotRiver/data/generic.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7751 2023-03-07 16:50:39.000000 spotRiver-0.0.95/src/spotRiver/data/opm.py
+-rw-r--r--   0 bartz      (501) staff       (20)    17554 2023-04-08 14:44:16.000000 spotRiver-0.0.95/src/spotRiver/data/river_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-03-31 21:04:02.000000 spotRiver-0.0.95/src/spotRiver/data/river_hyper_dict.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.068256 spotRiver-0.0.95/src/spotRiver/data/synth/
+-rw-r--r--   0 bartz      (501) staff       (20)      328 2023-01-18 17:25:51.000000 spotRiver-0.0.95/src/spotRiver/data/synth/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2442 2023-02-20 15:46:37.000000 spotRiver-0.0.95/src/spotRiver/data/synth/sea.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.068368 spotRiver-0.0.95/src/spotRiver/drift/
+-rw-r--r--   0 bartz      (501) staff       (20)      767 2023-02-20 15:46:37.000000 spotRiver-0.0.95/src/spotRiver/drift/drift_generator.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.068718 spotRiver-0.0.95/src/spotRiver/evaluation/
+-rw-r--r--   0 bartz      (501) staff       (20)    29393 2023-04-06 12:46:27.000000 spotRiver-0.0.95/src/spotRiver/evaluation/eval_bml.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3958 2023-02-26 22:39:12.000000 spotRiver-0.0.95/src/spotRiver/evaluation/eval_nowcast.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6752 2023-04-06 12:44:54.000000 spotRiver-0.0.95/src/spotRiver/evaluation/eval_oml.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.068942 spotRiver-0.0.95/src/spotRiver/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     5391 2023-06-10 18:01:21.000000 spotRiver-0.0.95/src/spotRiver/fun/hyperriver.py
+-rw-r--r--   0 bartz      (501) staff       (20)    32460 2023-04-22 19:31:59.000000 spotRiver-0.0.95/src/spotRiver/fun/hyperriver_old.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.069059 spotRiver-0.0.95/src/spotRiver/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1340 2023-03-11 14:52:45.000000 spotRiver-0.0.95/src/spotRiver/plot/stats.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.069158 spotRiver-0.0.95/src/spotRiver/preprocess/
+-rw-r--r--   0 bartz      (501) staff       (20)     2488 2023-03-07 16:50:39.000000 spotRiver-0.0.95/src/spotRiver/preprocess/impute.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.069393 spotRiver-0.0.95/src/spotRiver/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2284 2023-07-06 19:04:13.000000 spotRiver-0.0.95/src/spotRiver/utils/data_conversion.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5549 2023-04-13 20:07:21.000000 spotRiver-0.0.95/src/spotRiver/utils/features.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.066568 spotRiver-0.0.95/src/spotRiver.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-07-07 07:12:45.000000 spotRiver-0.0.95/src/spotRiver.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)      987 2023-07-07 07:12:45.000000 spotRiver-0.0.95/src/spotRiver.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-07-07 07:12:45.000000 spotRiver-0.0.95/src/spotRiver.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       20 2023-07-07 07:12:45.000000 spotRiver-0.0.95/src/spotRiver.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       10 2023-07-07 07:12:45.000000 spotRiver-0.0.95/src/spotRiver.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-07 07:12:45.069511 spotRiver-0.0.95/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      510 2023-02-25 09:55:05.000000 spotRiver-0.0.95/test/test_features.py
```

### Comparing `spotRiver-0.0.93/LICENSE` & `spotRiver-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/PKG-INFO` & `spotRiver-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotRiver
-Version: 0.0.93
+Version: 0.0.95
 Summary: spotRiver - Sequential Parameter Optimization Interface to River
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 Project-URL: Homepage, https://www.spotseven.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotRiver-0.0.93/README.md` & `spotRiver-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/pyproject.toml` & `spotRiver-0.0.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
             "numpy",
             "scikit-learn",
             "matplotlib"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotRiver"
-version = "0.0.93"
+version = "0.0.95"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotRiver - Sequential Parameter Optimization Interface to River"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `spotRiver-0.0.93/src/spotRiver/data/airline-passengers.csv` & `spotRiver-0.0.95/src/spotRiver/data/airline-passengers.csv`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/data/airline_passengers.py` & `spotRiver-0.0.95/src/spotRiver/data/airline_passengers.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/data/base.py` & `spotRiver-0.0.95/src/spotRiver/data/base.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/data/bike_sharing.py` & `spotRiver-0.0.95/src/spotRiver/data/bike_sharing.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/data/generic.py` & `spotRiver-0.0.95/src/spotRiver/data/generic.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/data/opm.py` & `spotRiver-0.0.95/src/spotRiver/data/opm.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/data/river_hyper_dict.json` & `spotRiver-0.0.95/src/spotRiver/data/river_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/data/synth/sea.py` & `spotRiver-0.0.95/src/spotRiver/data/synth/sea.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/drift/drift_generator.py` & `spotRiver-0.0.95/src/spotRiver/drift/drift_generator.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/evaluation/eval_bml.py` & `spotRiver-0.0.95/src/spotRiver/evaluation/eval_bml.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/evaluation/eval_nowcast.py` & `spotRiver-0.0.95/src/spotRiver/evaluation/eval_nowcast.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/evaluation/eval_oml.py` & `spotRiver-0.0.95/src/spotRiver/evaluation/eval_oml.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/fun/hyperriver.py` & `spotRiver-0.0.95/src/spotRiver/fun/hyperriver.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/fun/hyperriver_old.py` & `spotRiver-0.0.95/src/spotRiver/fun/hyperriver_old.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/plot/stats.py` & `spotRiver-0.0.95/src/spotRiver/plot/stats.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/preprocess/impute.py` & `spotRiver-0.0.95/src/spotRiver/preprocess/impute.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver/utils/data_conversion.py` & `spotRiver-0.0.95/src/spotRiver/utils/data_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from river import datasets
 import pandas as pd
 from tabulate import tabulate
 
 
-def convert_to_df(dataset: datasets.base.Dataset, target_column: str) -> pd.DataFrame:
+def convert_to_df(dataset: datasets.base.Dataset, target_column: str, n_total=None) -> pd.DataFrame:
     """Converts a river dataset into a pandas DataFrame.
 
     Args:
         dataset (datasets.base.Dataset): The river dataset to be converted.
         target_column (str): The name of the target column in the resulting DataFrame.
 
     Returns:
@@ -25,20 +25,26 @@
                 'Rasmussen': 'rasmussen',
                 'YouGov': 'you_gov'},
                 inplace=True)
             # Split the data into train and test sets
             train = df[:500]
             test = df[500:]
     """
-    data_dict = {key: [] for key in list(dataset)[0][0].keys()}
+    data_dict = {key: [] for key in list(dataset.take(1))[0][0].keys()}
     data_dict[target_column] = []
-    for x in dataset:
-        for key, value in x[0].items():
-            data_dict[key].append(value)
-        data_dict[target_column].append(x[1])
+    if n_total is None:
+        for x in dataset:
+            for key, value in x[0].items():
+                data_dict[key].append(value)
+            data_dict[target_column].append(x[1])
+    else:
+        for x in dataset.take(n_total):
+            for key, value in x[0].items():
+                data_dict[key].append(value)
+            data_dict[target_column].append(x[1])
     df = pd.DataFrame(data_dict)
     return df
 
 
 def compare_two_tree_models(model1, model2, headers=["Parameter", "Default", "Spot"]):
     """Compares two tree models and returns a table of the differences.
     Args:
```

### Comparing `spotRiver-0.0.93/src/spotRiver/utils/features.py` & `spotRiver-0.0.95/src/spotRiver/utils/features.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.93/src/spotRiver.egg-info/PKG-INFO` & `spotRiver-0.0.95/src/spotRiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotRiver
-Version: 0.0.93
+Version: 0.0.95
 Summary: spotRiver - Sequential Parameter Optimization Interface to River
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 Project-URL: Homepage, https://www.spotseven.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotRiver-0.0.93/src/spotRiver.egg-info/SOURCES.txt` & `spotRiver-0.0.95/src/spotRiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*


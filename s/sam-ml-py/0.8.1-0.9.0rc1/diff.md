# Comparing `tmp/sam_ml-py-0.8.1.tar.gz` & `tmp/sam_ml-py-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.8.1.tar", last modified: Wed Jul  5 18:02:38 2023, max compression
+gzip compressed data, was "sam_ml-py-0.9.0rc1.tar", last modified: Thu Jul  6 12:01:15 2023, max compression
```

## Comparing `sam_ml-py-0.8.1.tar` & `sam_ml-py-0.9.0rc1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.003584 sam_ml-py-0.8.1/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.003584 sam_ml-py-0.8.1/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/config/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.003584 sam_ml-py-0.8.1/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/XGBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 18:02:37.000000 sam_ml-py-0.8.1/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:38.007584 sam_ml-py-0.8.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/test/test_CTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/test/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-05 18:02:28.000000 sam_ml-py-0.8.1/test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.539675 sam_ml-py-0.9.0rc1/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.539675 sam_ml-py-0.9.0rc1/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/config/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.543675 sam_ml-py-0.9.0rc1/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.547675 sam_ml-py-0.9.0rc1/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21838 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/XGBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/test/test_CTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/test/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/test/test_pipeline.py
```

### Comparing `sam_ml-py-0.8.1/LICENSE` & `sam_ml-py-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/PKG-INFO` & `sam_ml-py-0.9.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam_ml-py
-Version: 0.8.1
+Version: 0.9.0rc1
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: with_swig
```

### Comparing `sam_ml-py-0.8.1/README.md` & `sam_ml-py-0.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/config/global_variables.py` & `sam_ml-py-0.9.0rc1/sam_ml/config/global_variables.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/config/logging.py` & `sam_ml-py-0.9.0rc1/sam_ml/config/logging.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/data/embeddings.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/data/feature_selection.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/data/sampling.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         """
         self.algorithm = algorithm
         self._grid: dict[str, list] = {} # for pipeline structure
 
         if algorithm == "SMOTE":
             self.sampler = SMOTE(random_state=random_state, **kwargs)
         elif algorithm == "rus":
-            self.sampler = RandomUnderSampler(random_state=random_state, replacement=True, **kwargs)
+            self.sampler = RandomUnderSampler(random_state=random_state, **kwargs)
         elif algorithm == "ros":
             self.sampler = RandomOverSampler(random_state=random_state, **kwargs)
         elif algorithm == "tl":
             self.sampler = TomekLinks(sampling_strategy="majority", **kwargs)
         elif algorithm == "nm":
             self.sampler = NearMiss(**kwargs)
         else:
```

### Comparing `sam_ml-py-0.8.1/sam_ml/data/scaler.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/scaler.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/AdaBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/BaggingClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/BernoulliNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/ClassifierTest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 import sys
+import time
 import warnings
+from datetime import timedelta
 from typing import Union
 
+import numpy as np
 import pandas as pd
 
 # to deactivate pygame promt 
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
 
 import pygame
 from pkg_resources import resource_filename
@@ -43,15 +46,15 @@
     warnings.simplefilter("ignore")
     os.environ["PYTHONWARNINGS"] = "ignore" # Also affects subprocesses
 
 
 class CTest:
     """ AutoML class """
 
-    def __init__(self, models: Union[str, list[Classifier]] = "all", vectorizer: Union[str, Embeddings_builder] = None, scaler: Union[str, Scaler] = None, selector: Union[str, Selector] = None, sampler: Union[str, Sampler] = None):
+    def __init__(self, models: str | list[Classifier] = "all", vectorizer: str | Embeddings_builder | None | list[str | Embeddings_builder | None] = None, scaler: str | Scaler | None  | list[str | Scaler | None] = None, selector: str | Selector | None  | list[str | Selector | None] = None, sampler: str | Sampler | None  | list[str | Sampler | None] = None):
         """
         @params:
             models:
 
                 - list of Wrapperclass models from this library
 
                 - 'all': use all Wrapperclass models (18+ models)
@@ -64,22 +67,35 @@
             sampling: type of "data.sampling.Sampler" or Sampler class object for sampling the train data (None for no sampling)
         """
         self.__models_input = models
 
         if type(models) == str:
             models = self.model_combs(models)
 
-        self.models: dict = {}
-        for i in range(len(models)):
-            self.models[models[i].model_name] = Pipeline(vectorizer,  scaler, selector, sampler, models[i], models[i].model_name+" (pipeline)")
+        if type(vectorizer) in (str, Embeddings_builder) or vectorizer is None:
+            vectorizer = [vectorizer]
+
+        if type(scaler) in (str, Scaler) or scaler is None:
+            scaler = [scaler]
+
+        if type(selector) in (str, Selector) or selector is None:
+            selector = [selector]
+
+        if type(sampler) in (str, Sampler) or sampler is None:
+            sampler = [sampler]
 
         self._vectorizer = vectorizer
         self._scaler = scaler
         self._selector = selector
         self._sampler = sampler
+
+        self.models: dict = {}
+        for model in models:
+            self.add_model(model)
+
         self.best_model: Pipeline
         self.scores: dict = {}
 
     def __repr__(self) -> str:
         params: str = ""
 
         if type(self.__models_input) == str:
@@ -126,15 +142,26 @@
 
         return f"CTest({params})"
 
     def remove_model(self, model_name: str):
         del self.models[model_name]
 
     def add_model(self, model: Classifier):
-        self.models[model.model_name] = Pipeline(self._vectorizer, self._scaler, self._selector, self._sampler, model, model.model_name+" (pipeline)")
+        for vec in self._vectorizer:
+            for scal in self._scaler:
+                for sel in self._selector:
+                    for sam in self._sampler:
+                        sampling_problems = ["QDA", "LDA", "LR", "MLPC", "LSVC"]
+                        if model.model_type in sampling_problems and sam == "SMOTE":
+                            model_pipe_name = model.model_name+f" (vec={vec}, scaler={scal}, selector={sel}, sampler=ros)"
+                        elif model.model_type in sampling_problems and sam in ("nm", "tl"):
+                            model_pipe_name = model.model_name+f" (vec={vec}, scaler={scal}, selector={sel}, sampler=rus)"
+                        else:
+                            model_pipe_name = model.model_name+f" (vec={vec}, scaler={scal}, selector={sel}, sampler={sam})"
+                        self.models[model_pipe_name] = Pipeline(vec,  scal, sel, sam, model, model_pipe_name)
 
     def model_combs(self, kind: str):
         """
         @params:
             kind:
                 "all": use all models
                 "basic": use a simple combination (LogisticRegression, MLP Classifier, LinearSVC, DecisionTreeClassifier, RandomForestClassifier, SVC, Gradientboostingmachine, AdaboostClassifier, KNeighborsClassifier)
@@ -248,15 +275,15 @@
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
             strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return:
             saves metrics in dict self.scores and also outputs them
         """
         try:
-            for key in tqdm(self.models.keys(), desc="Crossvalidation"):
+            for key in tqdm(self.models.keys(), desc="Evaluation"):
                 tscore, ttime = self.models[key].train(x_train, y_train, console_out=False)
                 score = self.models[key].evaluate(
                     x_test, y_test, avg=avg, pos_label=pos_label, console_out=False, secondary_scoring=secondary_scoring, strength=strength,
                 )
                 score["train_score"] = tscore
                 score["train_time"] = ttime
                 self.scores[key] = score
@@ -368,7 +395,101 @@
         sorted_scores = self.output_scores_as_pd(sort_by=[scoring, "s_score", "train_time"], console_out=False)
         best_model_type = sorted_scores.iloc[0].name
         best_model_value = sorted_scores.iloc[0][scoring]
         best_model_hyperparameters = sorted_scores.iloc[0]["best_hyperparameters (rCVs)"]
         logger.info(f"best model type {best_model_type} - {scoring}: {best_model_value} - parameters: {best_model_hyperparameters}")
         self.__finish_sound()
         return self.scores
+    
+    def find_best_model_mass_search(self,
+        x_train: pd.DataFrame,
+        y_train: pd.Series,
+        x_test: pd.DataFrame,
+        y_test: pd.Series,
+        n_trails: int = 10,
+        scoring: str = "accuracy",
+        avg: str = "macro",
+        pos_label: Union[int, str] = -1,
+        secondary_scoring: str = None,
+        strength: int = 3,
+        leave_loadbar: bool = True,
+        save_results_path: str | None = "find_best_model_mass_search_results.csv",
+    ) -> dict:
+        model_dict = {}
+        for key in self.models.keys():
+            model = self.models[key]
+            configs = model.get_random_configs(n_trails)
+            try:
+                for config in configs:
+                    model_new = model.get_deepcopy()
+                    model_new = model_new.set_params(**config)
+                    if model_new.model_type != "XGBC":
+                        model_new = model_new.set_params(**{"warm_start": True})
+                    model_name = f"{key} {dict(config)}"
+                    model_dict[model_name] = model_new
+            except:
+                logger.warning(f"modeltype in '{key}' is not supported for this search -> will be skipped")
+
+        total_model_num = len(model_dict)
+        logger.info(f"total number of models: {total_model_num}")
+        split_num = int(np.log2(total_model_num))+1
+        split_size =int(1/split_num*len(x_train))
+        if split_size < 300:
+            raise RuntimeError(f"not enough data for the amout of models. Data per split should be over 300, but {split_size} < 300")
+        logger.info(f"split number: {split_num}, split_size (x_train): {split_size}")
+
+        # shuffle x_train/y_train
+        x_train = x_train.sample(frac=1, random_state=42)
+        y_train = y_train.sample(frac=1, random_state=42)
+
+        for split_idx in tqdm(range(split_num-1), desc="splits"):
+            x_train_train = x_train[split_idx*split_size:(split_idx+1)*split_size]
+            x_train_test = x_train[(split_idx+1)*split_size:]
+            y_train_train = y_train[split_idx*split_size:(split_idx+1)*split_size]
+            y_train_test = y_train[(split_idx+1)*split_size:]
+            logger.info(f"length x_train/y_train {len(x_train_train)}/{len(y_train_train)}, length x_test/y_test {len(x_train_test)}/{len(y_train_test)}")
+            split_scores: dict = {}
+            # train models in model_dict
+            for key in tqdm(model_dict.keys(), desc=f"split {split_idx+1}", leave=leave_loadbar):
+                # train data classes in first split on all train data
+                if split_idx == 0:
+                    model_dict[key]._Pipeline__data_prepare(x_train, y_train)
+
+                # XGBoostClassifier has different warm_start implementation
+                if model_dict[key].model_type != "XGBC" or split_idx==0:
+                    tscore, ttime = model_dict[key].train_warm_start(x_train_train, y_train_train, console_out=False)
+                else:
+                    start = time.time()
+                    model_dict[key].fit_warm_start(x_train_train, y_train_train, xgb_model=model_dict[key].model)
+                    end = time.time()
+                    tscore, ttime = model_dict[key].get_train_score(x_train_train, y_train_train), str(timedelta(seconds=int(end-start)))
+                
+                score = model_dict[key].evaluate(x_train_test, y_train_test, avg=avg, pos_label=pos_label, console_out=False, secondary_scoring=secondary_scoring, strength=strength)
+                score["train_score"] = tscore
+                score["train_time"] = ttime
+                split_scores[key] = score
+            sorted_split_scores = dict(sorted(split_scores.items(), key=lambda item: (item[1][scoring], item[1]["s_score"], item[1]["train_time"]), reverse=True))
+            sorted_split_scores_pd = pd.DataFrame(sorted_split_scores).transpose()
+
+            # save model scores
+            if save_results_path is not None:
+                sorted_split_scores_pd.to_csv(save_results_path.split(".")[0]+f"_split{split_idx}."+save_results_path.split(".")[1])
+
+            logger.info(f"Split scores (top 5): \n{sorted_split_scores_pd.head(5)}")
+
+            # only keep better half of the models
+            for key in list(sorted_split_scores.keys())[int(len(sorted_split_scores)/2):]:
+                del model_dict[key]
+
+            logger.info(f"removed {len(sorted_split_scores)-len(model_dict)} models")
+            
+            best_model_name = list(sorted_split_scores.keys())[0]
+            best_model = model_dict[list(sorted_split_scores.keys())[0]]
+
+        logger.info(f"Evaluating best model: \n\n{best_model_name}\n")
+        x_train_train = x_train[int(split_idx*1/split_num*len(x_train)):]
+        y_train_train = y_train[int(split_idx*1/split_num*len(y_train)):]
+        tscore, ttime = best_model.train_warm_start(x_train_train, y_train_train, console_out=False)
+        score = best_model.evaluate(x_test, y_test, avg=avg, pos_label=pos_label, console_out=True, secondary_scoring=secondary_scoring, strength=strength)
+        score["train_score"] = tscore
+        score["train_time"] = ttime
+        return best_model_name, score
```

### Comparing `sam_ml-py-0.8.1/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/ExtraTreesClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/GaussianNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/GaussianProcessClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/GradientBoostingMachine.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/MLPClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/SupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/XGBoostClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/XGBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/__init__.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/main_classifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/main_classifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml/models/main_model.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/main_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         if console_out:
             print("Train score: ", self.train_score, " - Train time: ", self.train_time)
             
         logger.debug(f"training {self.model_name} - finished")
 
         return self.train_score, self.train_time
 
-    def fit(self, x_train: pd.DataFrame, y_train: pd.Series):
-        self.model.fit(x_train, y_train)
+    def fit(self, x_train: pd.DataFrame, y_train: pd.Series, **kwargs):
+        self.model.fit(x_train, y_train, **kwargs)
         return self
 
     def predict(self, x_test: pd.DataFrame) -> list:
         """
         @return:
             list with predictions
         """
@@ -65,14 +65,18 @@
 
     def get_params(self, deep: bool = True):
         return self.model.get_params(deep)
 
     def set_params(self, **params):
         self.model.set_params(**params)
         return self
+    
+    def get_train_score(self, x_train: pd.DataFrame, y_train: pd.Series) -> float:
+        score = self.model.score(x_train, y_train)
+        return score
 
     def evaluate(self, x_test: pd.DataFrame, y_test: pd.Series, console_out: bool = True) -> float:
         self.test_score = self.model.score(x_test, y_test)
         if console_out:
             print("Test score: ", self.test_score)
         return self.test_score
```

### Comparing `sam_ml-py-0.8.1/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/main_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -77,14 +77,17 @@
                 self.sampler = Sampler(algorithm="ros")
             elif self.sampler.algorithm in ("nm", "tl") and self.model_type in sampling_problems:
                 logger.warning(self.model_type+f" does not work with sampling='{self.sampler.algorithm}' --> going on with sampling='rus'")
                 self.sampler = Sampler(algorithm="rus")
 
         self.vectorizer_dict: dict[str, Embeddings_builder] = {}
 
+        # keep track if model was trained for warm_start
+        self.data_classes_trained: bool = False
+
     def __repr__(self) -> str:
         params: str = ""
         data_steps = ("vectorizer", self.vectorizer), ("scaler", self.scaler), ("selector", self.selector), ("sampler", self.sampler)
         for step in data_steps:
             params += step[0]+"="+step[1].__str__()+", "
 
         params += f"model={self.model.__str__()}, "
@@ -116,23 +119,36 @@
             X = self.__auto_vectorizing(X, train_on=train_on)
         if self.scaler is not None:
             X = self.scaler.scale(X, train_on=train_on)
         if self.selector is not None:
             X = self.selector.select(X, y, train_on=train_on)
         if self.sampler is not None and train_on:
             X, y = self.sampler.sample(X, y)
+        self.data_classes_trained = True
         return X, y
 
     def train(self, x_train: pd.DataFrame, y_train: pd.Series, console_out: bool = True) -> tuple[float, str]:
         x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on=True)
         return super().train(x_train_pre, y_train_pre, console_out)
+    
+    def train_warm_start(self, x_train: pd.DataFrame, y_train: pd.Series, console_out: bool = True) -> tuple[float, str]:
+        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self.data_classes_trained)
+        return super().train(x_train_pre, y_train_pre, console_out)
 
-    def fit(self, x_train: pd.DataFrame, y_train: pd.Series):
+    def fit(self, x_train: pd.DataFrame, y_train: pd.Series, **kwargs):
         x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on=True)
-        return super().fit(x_train_pre, y_train_pre)
+        return super().fit(x_train_pre, y_train_pre, **kwargs)
+    
+    def fit_warm_start(self, x_train: pd.DataFrame, y_train: pd.Series, **kwargs):
+        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self.data_classes_trained)
+        return super().fit(x_train_pre, y_train_pre, **kwargs)
+    
+    def get_train_score(self, x_train: pd.DataFrame, y_train: pd.Series) -> float:
+        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self.data_classes_trained)
+        return super().get_train_score(x_train_pre, y_train_pre)
 
     def predict(self, x_test: pd.DataFrame) -> list:
         x_test_pre, _ = self.__data_prepare(x_test, None, train_on=False)
         return super().predict(x_test_pre)
 
     def get_params(self, deep: bool = True) -> dict[str, any]:
         return dict(self.steps)
```

### Comparing `sam_ml-py-0.8.1/sam_ml/models/scorer.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam-ml-py
-Version: 0.8.1
+Version: 0.9.0rc1
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: with_swig
```

### Comparing `sam_ml-py-0.8.1/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/setup.py` & `sam_ml-py-0.9.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.8.1",
+    version="0.9.0rc1",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
```

### Comparing `sam_ml-py-0.8.1/test/test_CTest.py` & `sam_ml-py-0.9.0rc1/test/test_CTest.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/test/test_classifier.py` & `sam_ml-py-0.9.0rc1/test/test_classifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.8.1/test/test_pipeline.py` & `sam_ml-py-0.9.0rc1/test/test_pipeline.py`

 * *Files identical despite different names*


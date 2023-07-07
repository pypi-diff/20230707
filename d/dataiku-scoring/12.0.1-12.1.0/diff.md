# Comparing `tmp/dataiku-scoring-12.0.1.tar.gz` & `tmp/dataiku-scoring-12.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dataiku-scoring-12.0.1.tar", last modified: Wed Jul  5 08:18:34 2023, max compression
+gzip compressed data, was "dist/dataiku-scoring-12.1.0.tar", last modified: Fri Jul  7 15:17:20 2023, max compression
```

## Comparing `dataiku-scoring-12.0.1.tar` & `dataiku-scoring-12.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/
--rw-r--r--   0 kevinremy   (502) staff       (20)     1222 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/PKG-INFO
--rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/requirements.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)       65 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/MANIFEST.in
--rw-r--r--   0 kevinremy   (502) staff       (20)      214 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/README.md
--rw-r--r--   0 kevinremy   (502) staff       (20)       27 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/NOTICE.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)      876 2023-07-04 13:43:10.000000 dataiku-scoring-12.0.1/setup.py
--rw-r--r--   0 kevinremy   (502) staff       (20)       38 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/setup.cfg
--rw-r--r--   0 kevinremy   (502) staff       (20)      245 2023-07-04 13:43:10.000000 dataiku-scoring-12.0.1/HISTORY.txt
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/
--rw-r--r--   0 kevinremy   (502) staff       (20)     1222 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/PKG-INFO
--rw-r--r--   0 kevinremy   (502) staff       (20)     2506 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/SOURCES.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/requires.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)       15 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/top_level.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)        1 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/dependency_links.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)      524 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/LICENSE.txt
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/
--rw-r--r--   0 kevinremy   (502) staff       (20)     1103 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/gradient_boosting_regressor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     4771 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/decision_tree_model.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1157 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/generic_mlp.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1597 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/logistic.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      672 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/forest_regressor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      903 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      848 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/mlp_classifier.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1581 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/gradient_boosting_classifier.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      576 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/common.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      429 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/linear_regression.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      258 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/mlp_regressor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      708 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/forest_classifier.py
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/
--rw-r--r--   0 kevinremy   (502) staff       (20)     2469 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/regression.py
--rw-r--r--   0 kevinremy   (502) staff       (20)    10845 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/classification.py
--rw-r--r--   0 kevinremy   (502) staff       (20)    11000 2023-07-04 13:20:45.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/dss_flavor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      681 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     7867 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/common.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1069 2023-07-04 13:20:45.000000 dataiku-scoring-12.0.1/dataikuscoring/__init__.py
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/
--rw-r--r--   0 kevinremy   (502) staff       (20)      239 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/math_utils.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      242 2023-06-15 08:28:03.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     6491 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/prediction_result.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1413 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/tokenizer.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1379 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/scoring_data.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2323 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/indexed_matrix.py
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/models/
--rw-r--r--   0 kevinremy   (502) staff       (20)      880 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/binary.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      205 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/regression.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2457 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/mlflow.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      334 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/multiclass.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      635 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     6240 2023-06-30 10:38:01.000000 dataiku-scoring-12.0.1/dataikuscoring/models/partitioned.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     3964 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/model.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2409 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/common.py
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/
--rw-r--r--   0 kevinremy   (502) staff       (20)      928 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/rescale.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2080 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/derive_rescale.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      759 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/flag.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2471 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/vectorize_tfidf.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      783 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/vectors_unfold.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1399 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/categorical_encode.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1423 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/normalize.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1047 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/cat_cat_interaction.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1290 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/derive.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1241 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1205 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/impute.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      996 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/preprocessor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1023 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/num_num_interaction.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1131 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/dummify.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      711 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/binarize.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1679 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/selection.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      864 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/num_cat_interaction.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2098 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/datetime_cyclical.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1302 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/preprocessings.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      995 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/drop_rows.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     5038 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/prepare_input.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2863 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/calibration.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1246 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/vectorize_word_count.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     9455 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/load.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-07 15:17:20.000000 dataiku-scoring-12.1.0/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1468 2023-07-07 15:17:20.000000 dataiku-scoring-12.1.0/PKG-INFO
+-rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-04-06 10:00:29.000000 dataiku-scoring-12.1.0/requirements.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)       65 2023-04-06 10:00:29.000000 dataiku-scoring-12.1.0/MANIFEST.in
+-rw-r--r--   0 kevinremy   (502) staff       (20)      214 2023-04-06 10:00:29.000000 dataiku-scoring-12.1.0/README.md
+-rw-r--r--   0 kevinremy   (502) staff       (20)       27 2023-04-06 10:00:29.000000 dataiku-scoring-12.1.0/NOTICE.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)      876 2023-07-07 15:17:08.000000 dataiku-scoring-12.1.0/setup.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)       38 2023-07-07 15:17:20.000000 dataiku-scoring-12.1.0/setup.cfg
+-rw-r--r--   0 kevinremy   (502) staff       (20)      395 2023-07-07 15:17:08.000000 dataiku-scoring-12.1.0/HISTORY.txt
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-07 15:17:19.000000 dataiku-scoring-12.1.0/dataiku_scoring.egg-info/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1468 2023-07-07 15:17:19.000000 dataiku-scoring-12.1.0/dataiku_scoring.egg-info/PKG-INFO
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2506 2023-07-07 15:17:19.000000 dataiku-scoring-12.1.0/dataiku_scoring.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-07-07 15:17:19.000000 dataiku-scoring-12.1.0/dataiku_scoring.egg-info/requires.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)       15 2023-07-07 15:17:19.000000 dataiku-scoring-12.1.0/dataiku_scoring.egg-info/top_level.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)        1 2023-07-07 15:17:19.000000 dataiku-scoring-12.1.0/dataiku_scoring.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)      524 2023-04-06 10:00:29.000000 dataiku-scoring-12.1.0/LICENSE.txt
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-07 15:17:19.000000 dataiku-scoring-12.1.0/dataikuscoring/
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-07 15:17:20.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1103 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/gradient_boosting_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     4771 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/decision_tree_model.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1157 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/generic_mlp.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1597 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/logistic.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      672 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/forest_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      903 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      848 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/mlp_classifier.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1581 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/gradient_boosting_classifier.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      576 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/common.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      429 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/linear_regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      258 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/mlp_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      708 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/algorithms/forest_classifier.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-07 15:17:20.000000 dataiku-scoring-12.1.0/dataikuscoring/mlflow/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2656 2023-07-07 15:17:08.000000 dataiku-scoring-12.1.0/dataikuscoring/mlflow/regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)    11841 2023-07-07 15:17:08.000000 dataiku-scoring-12.1.0/dataikuscoring/mlflow/classification.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)    11000 2023-07-04 13:20:45.000000 dataiku-scoring-12.1.0/dataikuscoring/mlflow/dss_flavor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      681 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/mlflow/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     7939 2023-07-07 15:17:08.000000 dataiku-scoring-12.1.0/dataikuscoring/mlflow/common.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1069 2023-07-04 13:20:45.000000 dataiku-scoring-12.1.0/dataikuscoring/__init__.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-07 15:17:20.000000 dataiku-scoring-12.1.0/dataikuscoring/utils/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      239 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/utils/math_utils.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      242 2023-06-15 08:28:03.000000 dataiku-scoring-12.1.0/dataikuscoring/utils/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     6491 2023-07-06 14:06:22.000000 dataiku-scoring-12.1.0/dataikuscoring/utils/prediction_result.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1413 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/utils/tokenizer.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1379 2023-07-06 14:06:22.000000 dataiku-scoring-12.1.0/dataikuscoring/utils/scoring_data.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2323 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/utils/indexed_matrix.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-07 15:17:20.000000 dataiku-scoring-12.1.0/dataikuscoring/models/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      880 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/models/binary.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      205 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/models/regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2457 2023-07-06 14:36:41.000000 dataiku-scoring-12.1.0/dataikuscoring/models/mlflow.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      334 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/models/multiclass.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      635 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/models/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     7552 2023-07-07 15:17:08.000000 dataiku-scoring-12.1.0/dataikuscoring/models/partitioned.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     3964 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/models/model.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2409 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/models/common.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-07 15:17:20.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      928 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/rescale.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2080 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/derive_rescale.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      759 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/flag.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2471 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/vectorize_tfidf.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      783 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/vectors_unfold.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1399 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/categorical_encode.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1423 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/normalize.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1047 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/cat_cat_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1290 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/derive.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1241 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1205 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/impute.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      996 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/preprocessor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1023 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/num_num_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1131 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/dummify.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      711 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/binarize.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1679 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/selection.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      864 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/num_cat_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2098 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/datetime_cyclical.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1302 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/preprocessings.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      995 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/drop_rows.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     5038 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/prepare_input.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2863 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/calibration.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1246 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/processors/vectorize_word_count.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     9455 2023-04-07 20:10:33.000000 dataiku-scoring-12.1.0/dataikuscoring/load.py
```

### Comparing `dataiku-scoring-12.0.1/PKG-INFO` & `dataiku-scoring-12.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dataiku-scoring
-Version: 12.0.1
+Version: 12.1.0
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
 Description: # Dataiku ML Scoring Python library
         
@@ -13,24 +13,36 @@
         To use this library, you need to first export your model to Python from Dataiku.
         
         
         Changelog
         ==========
         
         
+        
+        12.1.0 (2023-07-06)
+        -------------------
+        
+        * Initial release for DSS 12.1.0
+        
         12.0.1 (2023-07-04)
         -------------------
         
         * Initial release for DSS 12.0.1
         
         11.4.4 (2023-07-04)
         -------------------
         
         * Initial release for DSS 11.4.4
         
+        11.4.0 (2023-03-16)
+        -------------------
+        
+        * Initial release for DSS 11.4
+        
+        
         11.1.0 (2022-10-20)
         -------------------
         
         * Initial release for DSS 11.1
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dataiku-scoring-12.0.1/setup.py` & `dataiku-scoring-12.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 
 long_description = (open('README.md').read() + '\n\n' +
                     open('HISTORY.txt').read())
 
-VERSION = "12.0.1"
+VERSION = "12.1.0"
 
 setuptools.setup(
     name='dataiku-scoring',
     version=VERSION,
     license="Apache Software License",
     packages=setuptools.find_packages(),
     description="Dataiku ML Scoring Python library",
```

### Comparing `dataiku-scoring-12.0.1/dataiku_scoring.egg-info/PKG-INFO` & `dataiku-scoring-12.1.0/dataiku_scoring.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dataiku-scoring
-Version: 12.0.1
+Version: 12.1.0
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
 Description: # Dataiku ML Scoring Python library
         
@@ -13,24 +13,36 @@
         To use this library, you need to first export your model to Python from Dataiku.
         
         
         Changelog
         ==========
         
         
+        
+        12.1.0 (2023-07-06)
+        -------------------
+        
+        * Initial release for DSS 12.1.0
+        
         12.0.1 (2023-07-04)
         -------------------
         
         * Initial release for DSS 12.0.1
         
         11.4.4 (2023-07-04)
         -------------------
         
         * Initial release for DSS 11.4.4
         
+        11.4.0 (2023-03-16)
+        -------------------
+        
+        * Initial release for DSS 11.4
+        
+        
         11.1.0 (2022-10-20)
         -------------------
         
         * Initial release for DSS 11.1
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dataiku-scoring-12.0.1/dataiku_scoring.egg-info/SOURCES.txt` & `dataiku-scoring-12.1.0/dataiku_scoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/LICENSE.txt` & `dataiku-scoring-12.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/gradient_boosting_regressor.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/decision_tree_model.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/decision_tree_model.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/generic_mlp.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/generic_mlp.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/logistic.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/logistic.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/forest_regressor.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/forest_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/__init__.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/mlp_classifier.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/gradient_boosting_classifier.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/gradient_boosting_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/common.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/algorithms/forest_classifier.py` & `dataiku-scoring-12.1.0/dataikuscoring/algorithms/forest_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/mlflow/regression.py` & `dataiku-scoring-12.1.0/dataikuscoring/mlflow/regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     convert_date_features(imported_model_meta, input_df)
 
     logging.info("Predicting it")
 
     with DisableMLflowTypeEnforcement():
         output = mlflow_model.predict(input_df)
 
+    if isinstance(output, list):
+        output = np.array(output)
+
     if isinstance(output, pd.DataFrame):
         logging.info("MLflow model returned a dataframe with columns: %s" % (output.columns))
         if "predictions" in output.columns and "target" in output.columns:
             logging.info("Using Fast.AI adapter on: %s" % (output))
             # This is the fastai output. Each "predictions" is an array of probas
             mlflow_raw_preds = output["target"]
 
@@ -45,14 +48,17 @@
             raise Exception("Can't handle model output of shape=%s" % (shape,))
     else:
         raise Exception("Can't handle model output: %s" % type(output))
 
     if mlflow_raw_preds.shape[0] == 0:
         raise Exception("Cannot work with no data at input")
 
+    if not pd.api.types.is_numeric_dtype(mlflow_raw_preds):
+        mlflow_raw_preds = mlflow_raw_preds.astype(float)
+
     preds = mlflow_raw_preds
     pred_df = pd.DataFrame({"prediction": preds})
 
     if np.isnan(pred_df.to_numpy()).any():
         raise Exception("MLflow model predicted NaN probabilities")
 
     logger.debug("Final pred_df: %s " % pred_df)
```

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/mlflow/classification.py` & `dataiku-scoring-12.1.0/dataikuscoring/mlflow/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,28 +85,34 @@
 
     mlflow_raw_preds = None  # raw prediction Serie or array (can be label or values)
     probas = None  # dataframe with the probabilities as proba_value0, proba_value1 etc.
     probas_raw = None  # the probabilities as np.array in the same order as lavels_list
     if imported_model_meta.get("proxyModelsConfiguration") is not None:
         with DisableMLflowTypeEnforcement():
             output_df = mlflow_model.predict(input_df)
-        mlflow_raw_preds = output_df["prediction"]
-        probas_df = output_df.drop("prediction", axis=1)
+        if "prediction" in output_df:
+            mlflow_raw_preds = output_df["prediction"]
+            probas_df = output_df.drop("prediction", axis=1)
+        else:
+            probas_df = output_df
         if not probas_df.empty:
             probas = probas_df
             proba_columns = ["proba_{}".format(int_to_label_map[i]) for i in labels_list]
             probas_raw = probas_df[proba_columns].values  # reorder and dump as numpy
 
     if probas is None:
         probas, probas_raw = mlflow_try_to_get_probas(input_df, mlflow_model, int_to_label_map)
 
     if probas_raw is None and mlflow_raw_preds is None:
         with DisableMLflowTypeEnforcement():
             output = mlflow_model.predict(input_df)
 
+        if isinstance(output, list):
+            output = np.array(output)
+
         if isinstance(output, pd.DataFrame):
             logging.info("MLflow model returned a dataframe with columns: %s" % (output.columns))
             if "predictions" in output.columns and "target" in output.columns:
                 logging.info("Using Fast.AI adapter on: %s" % (output))
                 # This is the fastai output. Each "predictions" is an array of probas
                 mlflow_raw_preds = output["target"]
                 probas_raw = np.stack(output["predictions"].tolist())
@@ -115,15 +121,21 @@
             elif len(output.columns) == 1:
                 # case where probas are flatten
                 if len(labels_list) and output.shape[0] / len(labels_list) == input_df.shape[0]:
                     probas_raw = output.to_numpy().reshape(-1, len(labels_list))
                 else:
                     mlflow_raw_preds = output[output.columns[0]]
             elif len(output.columns) == len(labels_list):
-                # It is outputting probas, but not the actual prediction
+                # It is outputting probas, but not the actual prediction.
+                # Let's make sure we are dealing with floats first: when the df is coming
+                # from proxy models, it is easy to lose the initial type, for example
+                # when we communicate using CSV.
+                output_non_numeric_cols = output.select_dtypes(exclude=[np.number]).columns
+                for col in output_non_numeric_cols:
+                    output[col] = output[col].astype(float)
                 probas_raw = output.to_numpy()
             else:
                 raise Exception("Can't handle model output of shape=%s" % (output.shape,))
 
         elif isinstance(output, np.ndarray):
             logging.info("MLflow model returned a ndarray with shape %s" % (output.shape,))
             shape = output.shape
@@ -145,17 +157,23 @@
             mlflow_raw_preds = probas_raw[:, 1]
         else:
             mlflow_raw_preds = probas_raw.argmax(1)
 
     if mlflow_raw_preds.shape[0] == 0:
         raise Exception("Cannot work with no data at input")
 
+    if imported_model_meta["predictionType"] == "BINARY_CLASSIFICATION" and \
+            not pd.api.types.is_numeric_dtype(mlflow_raw_preds):
+        # let's check if mlflow_raw_preds are actually floats and use that if yes
+        raw_preds_numeric = pd.to_numeric(mlflow_raw_preds, errors="ignore")
+        if raw_preds_numeric.dtype == float:
+            mlflow_raw_preds = raw_preds_numeric
+
     first_value = mlflow_raw_preds.iloc[0] if isinstance(mlflow_raw_preds, pd.Series) else mlflow_raw_preds[0]
     # Then determine if we already have labels, or if we have class indices
-
     if isinstance(first_value, str):
         logger.info("MLflow outputs labels, converting")
         # Model outputs labels
         preds = pd.Series(mlflow_raw_preds).replace(label_to_int_map)
         pred_df = pd.DataFrame({"prediction": mlflow_raw_preds})
     elif isinstance(first_value, int) or isinstance(first_value, np.integer):
         # Model outputs integers
```

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/mlflow/dss_flavor.py` & `dataiku-scoring-12.1.0/dataikuscoring/mlflow/dss_flavor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/mlflow/__init__.py` & `dataiku-scoring-12.1.0/dataikuscoring/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/mlflow/common.py` & `dataiku-scoring-12.1.0/dataikuscoring/mlflow/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,14 +138,17 @@
             if force_json_tensors_output:
                 tensors_list = [json.dumps(tensor.tolist()) for tensor in list(output)]
             else:
                 tensors_list = [tensor.tolist() for tensor in list(output)]
             return pd.DataFrame({"prediction": tensors_list})
         else:
             raise Exception("Can't handle MLflow model output of shape=%s" % (shape,))
+    elif isinstance(output, list):
+        return pd.DataFrame(output)
+
 
     else:
         raise Exception("Can't handle MLflow model output: %s" % type(output))
 
 
 def convert_date_features(imported_model_meta, input_df):
     """
```

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/__init__.py` & `dataiku-scoring-12.1.0/dataikuscoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/utils/prediction_result.py` & `dataiku-scoring-12.1.0/dataikuscoring/utils/prediction_result.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/utils/tokenizer.py` & `dataiku-scoring-12.1.0/dataikuscoring/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/utils/scoring_data.py` & `dataiku-scoring-12.1.0/dataikuscoring/utils/scoring_data.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/utils/indexed_matrix.py` & `dataiku-scoring-12.1.0/dataikuscoring/utils/indexed_matrix.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/models/binary.py` & `dataiku-scoring-12.1.0/dataikuscoring/models/binary.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/models/mlflow.py` & `dataiku-scoring-12.1.0/dataikuscoring/models/mlflow.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/models/__init__.py` & `dataiku-scoring-12.1.0/dataikuscoring/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/models/partitioned.py` & `dataiku-scoring-12.1.0/dataikuscoring/models/partitioned.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,113 @@
 from datetime import datetime
 import re
 import numpy as np
 
 from .common import PredictionModelMixin, ProbabilisticModelMixin
 
 
+def get_dimension_value(value, dimension_name, dimension_type, dimensions_values=None):
+    """Extract the exact partition dimension value from the dimension type.
+
+    Args:
+        :param str/int/float/datetime value: value of the partition dimension, can be of many form (str, date, timestamp, ...)
+        :param str dimension_name: name of the partition dimension
+        :param str dimension_type: type of the partition dimension
+        :param dict dimensions_values: dict of list of dimension values per dimension name. Defaults to None.
+
+        :return: str
+    """    
+    if dimension_type == "DISCRETE":
+        return value
+    else:
+        return _get_time_dimension_value(value, dimension_name, dimension_type, dimensions_values=dimensions_values)
+
+
+def _get_time_dimension_value(value, dimension_name, dimension_type, dimensions_values=None):
+    """
+    This is basically a copy of what is done in Java (PartitionedPipeline.getTimeDimensionValue).
+    """
+    def _get_time_dimension_value_from_timestamp(value, dimension_type, milliseconds=True):
+        datetime_value = datetime.fromtimestamp(value / 1000) if milliseconds else datetime.fromtimestamp(value)
+        return _get_time_dimension_value_from_datetime(datetime_value, dimension_type)
+    
+    def _get_time_dimension_value_from_datetime(value, dimension_type):
+        dimension_value = ""
+        if dimension_type == "HOUR":
+            dimension_value = "-%02d" % value.hour
+        if dimension_type in ("HOUR", "DAY"):
+            dimension_value = "-%02d" % value.day + dimension_value
+        if dimension_type in ("HOUR", "DAY", "MONTH"):
+            dimension_value = "-%02d" % value.month + dimension_value
+        if dimension_type in ("HOUR", "DAY", "MONTH", "YEAR"):
+            dimension_value = "%02d" % value.year + dimension_value
+        return dimension_value
+
+    if isinstance(value, (str)):
+        if dimensions_values and value in dimensions_values[dimension_name]:
+            return value
+        elif dimension_type == "YEAR" and re.match(r"^\d{4}$", value):
+            # a YEAR value of format "yyyy" should not be interpreted as an epoch even though it can be parsed as an int
+            return value
+        elif value.isdigit() or (value[0] in ("-", "+") and value[1:].isdigit()):
+            epoch = int(value)
+            return _get_time_dimension_value_from_timestamp(epoch, dimension_type)
+        elif re.match(
+            r"^\d{4}-\d\d-\d\dT\d\d:\d\d:\d\d(\.\d+)?(([+-]\d\d:\d\d)|Z)?$",
+            value,
+        ):  # "yyyy-MM-dd'T'HH:mm:ss.SSSXXX"
+            return _get_time_dimension_value_from_timestamp(
+                (
+                    datetime.strptime(value, "%Y-%m-%dT%H:%M:%S.%fZ") - datetime(1970, 1, 1)
+                ).total_seconds(), dimension_type, milliseconds=False
+            )
+        else:
+            return value
+
+    elif isinstance(value, (float, int)):
+        return _get_time_dimension_value_from_timestamp(value, dimension_type)
+    
+    elif isinstance(value, datetime):  # works also with pd.Timestamp
+        return _get_time_dimension_value_from_datetime(value, dimension_type)
+
+    else:
+        raise ValueError("Unknown dimension value type for {} / {} : {}".format(dimension_name, dimension_type, type(value)))
+
+
 class PartitionedModel(object):
 
     def __init__(self, models, resources):
         self.models = models
         self.dimensions = resources["meta"]["partitioning"]
         self.dimensions_types = ["DISCRETE"] * len(self.dimensions) if resources["meta"]["partitioningTypes"] is None else resources["meta"]["partitioningTypes"]
         self.dimensions_values = {dimension: [] for dimension in self.dimensions}
         for partition in self.models.keys():
             for partition_dimension, dimension in zip(partition.split("|"), self.dimensions):
                 self.dimensions_values[dimension].append(partition_dimension)
 
-    def _get_time_dimension_value(self, value, dimension, dimension_type):
-
-        def _get_time_dimension_value_from_timestamp(value, dimension_type, milliseconds=True):
-            dimension_value = ""
-            cal = datetime.fromtimestamp(value / 1000) if milliseconds else datetime.fromtimestamp(value)
-
-            if dimension_type == "HOUR":
-                dimension_value = "-%02d" % cal.hour
-            if dimension_type in ("HOUR", "DAY"):
-                dimension_value = "-%02d" % cal.day + dimension_value
-            if dimension_type in ("HOUR", "DAY", "MONTH"):
-                dimension_value = "-%02d" % cal.month + dimension_value
-            if dimension_type in ("HOUR", "DAY", "MONTH", "YEAR"):
-                dimension_value = "%02d" % cal.year + dimension_value
-            return dimension_value
-
-        if isinstance(value, (str)):
-            if value in self.dimensions_values[dimension]:
-                return value
-            elif value.isdigit() or (value[0] in ("-", "+") and value[1:].isdigit()):
-                epoch = int(value)
-                return _get_time_dimension_value_from_timestamp(epoch, dimension_type)
-
-            elif re.match(
-                r"^\d{4}-\d\d-\d\dT\d\d:\d\d:\d\d(\.\d+)?(([+-]\d\d:\d\d)|Z)?$",
-                value,
-            ):  # "yyyy-MM-dd'T'HH:mm:ss.SSSXXX"
-                return _get_time_dimension_value_from_timestamp(
-                    (
-                        datetime.strptime(value, "%Y-%m-%dT%H:%M:%S.%fZ") - datetime(1970, 1, 1)
-                    ).total_seconds(), dimension_type, milliseconds=False
-                )
-            else:
-                return value
-
-        elif isinstance(value, (float, int)):
-            return _get_time_dimension_value_from_timestamp(value, dimension_type)
-
-        else:
-            raise ValueError("Unknown dimension value type for {} / {} : {}".format(dimension, dimension_type, type(value)))
-
     def get_partition_for_dict(self, data):
         for dimension in self.dimensions:
             assert dimension in data, (
                 "Data is missing dimension {} required for partitioning".format(dimension))
 
         partition = "|".join([
-            str(data[dimension]) if dimension_type == "DISCRETE" else
-            self._get_time_dimension_value(data[dimension], dimension, dimension_type)
+            str(get_dimension_value(
+                data[dimension], dimension, dimension_type, dimensions_values=self.dimensions_values
+            ))
             for dimension, dimension_type in zip(self.dimensions, self.dimensions_types)
         ])
 
         return partition
 
     def get_partition_for_list(self, data):
         input_column_names = self.prepare_input.input_column_names
         partition = "|".join([
-            str(data[input_column_names.index(dimension)]) if dimension_type == "DISCRETE" else
-            self._get_time_dimension_value(data[input_column_names.index(dimension)], dimension, dimension_type)
+            str(get_dimension_value(
+                data[input_column_names.index(dimension)], dimension, dimension_type, dimensions_values=self.dimensions_values
+            ))
             for dimension, dimension_type in zip(self.dimensions, self.dimensions_types)
         ])
 
         return partition
 
     def _compute(self, X, method):
         """ Separate in sub batch per model and then sort to match the original order """
```

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/models/model.py` & `dataiku-scoring-12.1.0/dataikuscoring/models/model.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/models/common.py` & `dataiku-scoring-12.1.0/dataikuscoring/models/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/rescale.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/derive_rescale.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/derive_rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/flag.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/flag.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/vectorize_tfidf.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/vectorize_tfidf.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/vectors_unfold.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/vectors_unfold.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/categorical_encode.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/categorical_encode.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/normalize.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/normalize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/cat_cat_interaction.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/cat_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/derive.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/derive.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/__init__.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/impute.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/impute.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/preprocessor.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/num_num_interaction.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/num_num_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/dummify.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/dummify.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/binarize.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/binarize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/selection.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/selection.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/num_cat_interaction.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/num_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/datetime_cyclical.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/datetime_cyclical.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/preprocessings.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/preprocessings.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/drop_rows.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/drop_rows.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/prepare_input.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/prepare_input.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/calibration.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/calibration.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/processors/vectorize_word_count.py` & `dataiku-scoring-12.1.0/dataikuscoring/processors/vectorize_word_count.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.0.1/dataikuscoring/load.py` & `dataiku-scoring-12.1.0/dataikuscoring/load.py`

 * *Files identical despite different names*


# Comparing `tmp/gurobi-machinelearning-1.3.1.tar.gz` & `tmp/gurobi-machinelearning-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gurobi-machinelearning-1.3.1.tar", last modified: Thu Jul  6 10:36:37 2023, max compression
+gzip compressed data, was "gurobi-machinelearning-1.3.2.tar", last modified: Fri Jul  7 11:59:40 2023, max compression
```

## Comparing `gurobi-machinelearning-1.3.1.tar` & `gurobi-machinelearning-1.3.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 10:36:37.000000 gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/gurobi_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-06 10:36:30.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/add_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.715664 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/_var_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/base_predictor_constr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/get_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/neural_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/submodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/register_user_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/registered_predictors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/base_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/mlpregressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/predictors_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/skgetter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:36:37.719664 gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-07-06 10:36:28.000000 gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/xgboost_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.990282 gurobi-machinelearning-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-07 11:59:40.990282 gurobi-machinelearning-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 11:59:40.990282 gurobi-machinelearning-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.982282 gurobi-machinelearning-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.982282 gurobi-machinelearning-1.3.2/src/gurobi_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-07 11:59:40.000000 gurobi-machinelearning-1.3.2/src/gurobi_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-07 11:59:40.000000 gurobi-machinelearning-1.3.2/src/gurobi_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:59:40.000000 gurobi-machinelearning-1.3.2/src/gurobi_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 11:59:40.000000 gurobi-machinelearning-1.3.2/src/gurobi_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 11:59:40.000000 gurobi-machinelearning-1.3.2/src/gurobi_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.986282 gurobi-machinelearning-1.3.2/src/gurobi_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-07 11:59:32.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/add_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.986282 gurobi-machinelearning-1.3.2/src/gurobi_ml/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/keras/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.986282 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/_var_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/base_predictor_constr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.986282 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/decision_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/decision_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/get_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.986282 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/neural_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/submodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/register_user_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/registered_predictors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.990282 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/base_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/mlpregressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/predictors_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/skgetter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.990282 gurobi-machinelearning-1.3.2/src/gurobi_ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:59:40.990282 gurobi-machinelearning-1.3.2/src/gurobi_ml/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/xgboost/xgboost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-07 11:59:30.000000 gurobi-machinelearning-1.3.2/src/gurobi_ml/xgboost_sklearn_api.py
```

### Comparing `gurobi-machinelearning-1.3.1/LICENSE` & `gurobi-machinelearning-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/PKG-INFO` & `gurobi-machinelearning-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.3.1
+Version: 1.3.2
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
```

### Comparing `gurobi-machinelearning-1.3.1/README.md` & `gurobi-machinelearning-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/pyproject.toml` & `gurobi-machinelearning-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gurobi-machinelearning"
-version = "1.3.1"
+version = "1.3.2"
 description = "package to insert ML models in Gurobi"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="Apache-2.0"}
 keywords = ["mathematical optimization", "gurobi", "scikit-learn", "pytorch", "tensorflow", "ml"]
 authors = [
   {name = "Gurobi Optimization LLC"}
```

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/PKG-INFO` & `gurobi-machinelearning-1.3.2/src/gurobi_machinelearning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.3.1
+Version: 1.3.2
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
```

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_machinelearning.egg-info/SOURCES.txt` & `gurobi-machinelearning-1.3.2/src/gurobi_machinelearning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/gurobi_machinelearning.egg-info/top_level.txt
 src/gurobi_ml/__init__.py
 src/gurobi_ml/_version.py
 src/gurobi_ml/add_predictor.py
 src/gurobi_ml/exceptions.py
 src/gurobi_ml/register_user_predictor.py
 src/gurobi_ml/registered_predictors.py
+src/gurobi_ml/xgboost_sklearn_api.py
 src/gurobi_ml/keras/__init__.py
 src/gurobi_ml/keras/keras.py
 src/gurobi_ml/modeling/__init__.py
 src/gurobi_ml/modeling/_var_utils.py
 src/gurobi_ml/modeling/base_predictor_constr.py
 src/gurobi_ml/modeling/get_convertor.py
 src/gurobi_ml/modeling/submodel.py
```

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/__init__.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/_version.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from importlib import metadata
 
 try:
     __version__ = metadata.version("gurobi_machinelearning")
 except metadata.PackageNotFoundError:
     __version__ = "dev"
 
-GIT_HASH = "208bf12d2e054b02c2462de6446318be3e461520"
+GIT_HASH = "c0b69ba52b4cc23985adb88bf4488895bbfe7199"
 
 
 def get_versions():
     """Get package version."""
     # Downloaded package with inserted git hash.
     if "Format" not in GIT_HASH:
         git_hash = f"-{GIT_HASH}"
```

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/add_predictor.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/add_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/exceptions.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/__init__.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/keras/keras.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/keras/keras.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/__init__.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/_var_utils.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/_var_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/base_predictor_constr.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/base_predictor_constr.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/__init__.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/decision_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/get_convertor.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/get_convertor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/__init__.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/activations.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/activations.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/layers.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/layers.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/neuralnet/neural_net.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/neuralnet/neural_net.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/modeling/submodel.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/modeling/submodel.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/register_user_predictor.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/register_user_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/registered_predictors.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/registered_predictors.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,20 +58,20 @@
 def xgboost_convertors():
     """Collect known PyTorch objects that can be formulated and the conversion class."""
     if "xgboost" in sys.modules:
         import xgboost as xgb  # pylint: disable=import-outside-toplevel
 
         from .xgboost import (  # pylint: disable=import-outside-toplevel
             add_xgboost_regressor_constr,
-            add_xgbrfregressor_constr,
+            add_xgbregressor_constr,
         )
 
         return {
             xgb.core.Booster: add_xgboost_regressor_constr,
-            xgb.XGBRFRegressor: add_xgbrfregressor_constr,
+            xgb.XGBRegressor: add_xgbregressor_constr,
         }
     return {}
 
 
 def keras_convertors():
     """Collect known Keras objects that can be embedded and the conversion class."""
     if "tensorflow" in sys.modules:
```

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/__init__.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/base_regressions.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/base_regressions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/column_transformer.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/column_transformer.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/decision_tree_regressor.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/linear_regression.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/linear_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/logistic_regression.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/mlpregressor.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/mlpregressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/pipeline.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 """
 
 
 from ..exceptions import NoModel
 from ..modeling.base_predictor_constr import AbstractPredictorConstr
 from ..modeling.get_convertor import get_convertor
 from ..register_user_predictor import user_predictors
+from ..xgboost_sklearn_api import xgboost_sklearn_convertors
 from .column_transformer import add_column_transformer_constr
 from .predictors_list import sklearn_predictors
 from .preprocessing import sklearn_transformers
 from .skgetter import SKgetter
 
 
 def add_pipeline_constr(gp_model, pipeline, input_vars, output_vars=None, **kwargs):
@@ -111,14 +112,15 @@
                     f"I don't know how to deal with that object: {transformer}",
                 )
             steps.append(convertor(gp_model, transformer, input_vars, **kwargs))
             input_vars = steps[-1].output
 
         predictor = pipeline[-1]
         predictors = sklearn_predictors() | user_predictors()
+        predictors |= xgboost_sklearn_convertors()
         convertor = get_convertor(predictor, predictors)
         if convertor is None:
             raise NoModel(
                 self.predictor,
                 f"I don't know how to deal with that object: {predictor}",
             )
         steps.append(convertor(gp_model, predictor, input_vars, output_vars, **kwargs))
```

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/pls_regression.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/pls_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/predictors_list.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/predictors_list.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/preprocessing.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/random_forest_regressor.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/sklearn/skgetter.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/sklearn/skgetter.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/__init__.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/torch/sequential.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/torch/sequential.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/__init__.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/xgboost/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from .xgboost_regressor import add_xgboost_regressor_constr, add_xgbrfregressor_constr
+from .xgboost_regressor import add_xgboost_regressor_constr, add_xgbregressor_constr
```

### Comparing `gurobi-machinelearning-1.3.1/src/gurobi_ml/xgboost/xgboost_regressor.py` & `gurobi-machinelearning-1.3.2/src/gurobi_ml/xgboost/xgboost_regressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from gurobipy import GRB
 
 from ..exceptions import NoModel, NoSolution
 from ..modeling import AbstractPredictorConstr
 from ..modeling.decision_tree import leaf_formulation
 
 
-def add_xgbrfregressor_constr(
+def add_xgbregressor_constr(
     gp_model, xgboost_regressor, input_vars, output_vars=None, epsilon=0.0, **kwargs
 ):
     """Formulate xgboost_regressor into gp_model.
 
     The formulation predicts the values of output_vars using input_vars
     according to xgboost_regressor. See our :ref:`User's Guide
     <Gradient Boosting Regression>` for details on the mip formulation used.
```


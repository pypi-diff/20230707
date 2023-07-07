# Comparing `tmp/mlpype-0.4.7.tar.gz` & `tmp/mlpype-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-0.4.7.tar", last modified: Fri Jul  7 12:43:39 2023, max compression
+gzip compressed data, was "mlpype-0.4.8.tar", last modified: Fri Jul  7 14:00:24 2023, max compression
```

## Comparing `mlpype-0.4.7.tar` & `mlpype-0.4.8.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.287841 mlpype-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 12:39:43.000000 mlpype-0.4.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-07 12:43:39.287841 mlpype-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-07 12:39:43.000000 mlpype-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.235839 mlpype-0.4.7/mlpype/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.239840 mlpype-0.4.7/mlpype/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.239840 mlpype-0.4.7/mlpype/base/data/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/data/data_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/data/data_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/data/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.239840 mlpype-0.4.7/mlpype/base/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/deploy/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.243840 mlpype-0.4.7/mlpype/base/deploy/wheel/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/deploy/wheel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/deploy/wheel/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/deploy/wheel/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.243840 mlpype-0.4.7/mlpype/base/deploy/wheel/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/deploy/wheel/helpers/setup_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/deploy/wheel/helpers/wheel_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/deploy/wheel/wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.247840 mlpype-0.4.7/mlpype/base/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/evaluate/base_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/evaluate/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.247840 mlpype-0.4.7/mlpype/base/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/experiment/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/experiment/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.247840 mlpype-0.4.7/mlpype/base/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/logger/experiment_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/logger/local_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.251840 mlpype-0.4.7/mlpype/base/model/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.251840 mlpype-0.4.7/mlpype/base/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/pipeline/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/pipeline/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/pipeline/type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.255840 mlpype-0.4.7/mlpype/base/serialiser/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/serialiser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/serialiser/joblib_serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/serialiser/serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.255840 mlpype-0.4.7/mlpype/base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/base/utils/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.255840 mlpype-0.4.7/mlpype/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.259840 mlpype-0.4.7/mlpype/fastapi/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/fastapi/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/fastapi/deploy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.259840 mlpype-0.4.7/mlpype/fastapi/deploy/wheel/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/fastapi/deploy/wheel/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/fastapi/deploy/wheel_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/fastapi/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.259840 mlpype-0.4.7/mlpype/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/hyperopt/optimise.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/hyperopt/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.263840 mlpype-0.4.7/mlpype/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/mlflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.263840 mlpype-0.4.7/mlpype/mlflow/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/mlflow/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/mlflow/deploy/load_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.263840 mlpype-0.4.7/mlpype/mlflow/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/mlflow/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/mlflow/logger/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/mlflow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.263840 mlpype-0.4.7/mlpype/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.267840 mlpype-0.4.7/mlpype/sklearn/data/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/data/data_frame_source.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/data/sklearn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/data/sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.267840 mlpype-0.4.7/mlpype/sklearn/model/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/model/linear_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/model/logistic_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/model/sklearn_base_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/model/sklearn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.271841 mlpype-0.4.7/mlpype/sklearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/pipeline/numpy_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/pipeline/pandas_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/sklearn/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.271841 mlpype-0.4.7/mlpype/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.271841 mlpype-0.4.7/mlpype/spark/data/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/data/spark_data_frame_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/data/spark_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/data/spark_sql_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.275841 mlpype-0.4.7/mlpype/spark/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/evaluate/spark_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.275841 mlpype-0.4.7/mlpype/spark/model/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/model/linear_spark_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/model/spark_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.275841 mlpype-0.4.7/mlpype/spark/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/pipeline/spark_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/pipeline/spark_type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.279841 mlpype-0.4.7/mlpype/spark/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/serialisation/spark_serialiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/spark/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.279841 mlpype-0.4.7/mlpype/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.279841 mlpype-0.4.7/mlpype/tensorflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/data/tensor_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.283841 mlpype-0.4.7/mlpype/tensorflow/model/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/model/keras_pype_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/model/mlp_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/model/mlp_pype_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.283841 mlpype-0.4.7/mlpype/tensorflow/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/pipeline/tensor_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/tensorflow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.283841 mlpype-0.4.7/mlpype/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/xgboost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.283841 mlpype-0.4.7/mlpype/xgboost/model/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/xgboost/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/xgboost/model/xgboost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/xgboost/model/xgboost_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-07 12:39:43.000000 mlpype-0.4.7/mlpype/xgboost/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:43:39.235839 mlpype-0.4.7/mlpype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-07 12:43:39.000000 mlpype-0.4.7/mlpype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-07 12:43:39.000000 mlpype-0.4.7/mlpype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:43:39.000000 mlpype-0.4.7/mlpype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 12:43:39.000000 mlpype-0.4.7/mlpype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 12:39:43.000000 mlpype-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 12:43:39.287841 mlpype-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 12:39:43.000000 mlpype-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.565422 mlpype-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 13:57:33.000000 mlpype-0.4.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-07 14:00:24.565422 mlpype-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-07 13:57:33.000000 mlpype-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.529422 mlpype-0.4.8/mlpype/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.533422 mlpype-0.4.8/mlpype/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.533422 mlpype-0.4.8/mlpype/base/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/data/data_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/data/data_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/data/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.533422 mlpype-0.4.8/mlpype/base/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/deploy/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.537422 mlpype-0.4.8/mlpype/base/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/deploy/wheel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/deploy/wheel/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/deploy/wheel/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.537422 mlpype-0.4.8/mlpype/base/deploy/wheel/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/deploy/wheel/helpers/setup_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/deploy/wheel/helpers/wheel_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/deploy/wheel/wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.537422 mlpype-0.4.8/mlpype/base/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/evaluate/base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/evaluate/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.537422 mlpype-0.4.8/mlpype/base/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/experiment/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.541422 mlpype-0.4.8/mlpype/base/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/logger/experiment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/logger/local_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.541422 mlpype-0.4.8/mlpype/base/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.541422 mlpype-0.4.8/mlpype/base/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/pipeline/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/pipeline/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/pipeline/type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.545422 mlpype-0.4.8/mlpype/base/serialiser/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/serialiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/serialiser/joblib_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/serialiser/serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.545422 mlpype-0.4.8/mlpype/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/base/utils/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.545422 mlpype-0.4.8/mlpype/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.545422 mlpype-0.4.8/mlpype/fastapi/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/fastapi/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/fastapi/deploy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.545422 mlpype-0.4.8/mlpype/fastapi/deploy/wheel/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/fastapi/deploy/wheel/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/fastapi/deploy/wheel_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/fastapi/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.549422 mlpype-0.4.8/mlpype/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/hyperopt/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/hyperopt/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.549422 mlpype-0.4.8/mlpype/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/mlflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.549422 mlpype-0.4.8/mlpype/mlflow/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/mlflow/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/mlflow/deploy/load_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.549422 mlpype-0.4.8/mlpype/mlflow/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/mlflow/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/mlflow/logger/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/mlflow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.549422 mlpype-0.4.8/mlpype/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.553422 mlpype-0.4.8/mlpype/sklearn/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/data/data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/data/sklearn_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/data/sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.553422 mlpype-0.4.8/mlpype/sklearn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/model/linear_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/model/logistic_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/model/sklearn_base_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/model/sklearn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.553422 mlpype-0.4.8/mlpype/sklearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/pipeline/numpy_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/pipeline/pandas_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/sklearn/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.553422 mlpype-0.4.8/mlpype/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.557422 mlpype-0.4.8/mlpype/spark/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/data/spark_data_frame_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/data/spark_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/data/spark_sql_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.557422 mlpype-0.4.8/mlpype/spark/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/evaluate/spark_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.557422 mlpype-0.4.8/mlpype/spark/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/model/linear_spark_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/model/spark_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.561422 mlpype-0.4.8/mlpype/spark/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/pipeline/spark_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/pipeline/spark_type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.561422 mlpype-0.4.8/mlpype/spark/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/serialisation/spark_serialiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/spark/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.561422 mlpype-0.4.8/mlpype/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.561422 mlpype-0.4.8/mlpype/tensorflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/data/tensor_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.561422 mlpype-0.4.8/mlpype/tensorflow/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/model/keras_pype_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/model/mlp_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/model/mlp_pype_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.565422 mlpype-0.4.8/mlpype/tensorflow/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/pipeline/tensor_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/tensorflow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.565422 mlpype-0.4.8/mlpype/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/xgboost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.565422 mlpype-0.4.8/mlpype/xgboost/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/xgboost/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/xgboost/model/xgboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/xgboost/model/xgboost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-07 13:57:33.000000 mlpype-0.4.8/mlpype/xgboost/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:00:24.529422 mlpype-0.4.8/mlpype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-07 14:00:24.000000 mlpype-0.4.8/mlpype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-07 14:00:24.000000 mlpype-0.4.8/mlpype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:00:24.000000 mlpype-0.4.8/mlpype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 14:00:24.000000 mlpype-0.4.8/mlpype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-07 13:57:33.000000 mlpype-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 14:00:24.565422 mlpype-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 13:57:33.000000 mlpype-0.4.8/setup.py
```

### Comparing `mlpype-0.4.7/LICENSE.txt` & `mlpype-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/PKG-INFO` & `mlpype-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.4.7
+Version: 0.4.8
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.4.7/README.md` & `mlpype-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/data/data_catalog.py` & `mlpype-0.4.8/mlpype/base/data/data_catalog.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/data/dataset.py` & `mlpype-0.4.8/mlpype/base/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
             dct (Dict[str, Data]): The dictionary containing data.
 
         Returns:
             DataSet[Data]: A DataSet based on the given dict.
         """
         return cls(**dct)
 
-    def set_all(self, keys: List[str], data: Iterable[Data]) -> None:
+    def set_all(self, keys: Iterable[str], data: Iterable[Data]) -> None:
         """Set all data to the given keys, in order.
 
         This assumes the keys and data set are of the same length.
 
         Args:
-            keys (List[str]): The keys of the given data.
+            keys (Iterable[str]): The keys of the given data.
             data (Iterable[Data]): The data to store.
         """
         for key, d in zip(keys, data):
             self[key] = d
 
     def copy(self) -> "DataSet[Data]":
         """Create a shallow copy of this DataSet.
```

### Comparing `mlpype-0.4.7/mlpype/base/deploy/inference.py` & `mlpype-0.4.8/mlpype/base/deploy/inference.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,30 +30,38 @@
             output_type_checker (TypeCheckerPipe): The type checker used to determine outgoing types.
         """
         self.model = model
         self.pipeline = pipeline
         self.input_type_checker = input_type_checker
         self.output_type_checker = output_type_checker
 
-    def predict(self, data: Union[DataSet, DataCatalog]) -> DataSet:
+    def predict(self, data: Union[DataSet, DataCatalog], return_transformed_data: bool = False) -> DataSet:
         """Predicts using the given data using the Pipeline and Model.
 
         Args:
             data (Union[DataSet, DataCatalog]): The data to predict for.
+            return_transformed_data (bool): Flag indicating if transformed data
+                also needs to be returned. If set to True, we still only return one
+                dataset, but we'll add the data after the pipeline has run to it.
 
         Returns:
-            DataSet: The predictions from Model.
+            DataSet: The predictions from Model, with transformed data from the Pipeline if
+                requested.
         """
         # TODO: inverse transformation after prediction
         if isinstance(data, DataCatalog):
             data = data.read()
         self.input_type_checker.transform(data)
         transformed = self.pipeline.transform(data, is_inference=True)
         predicted = self.model.transform(transformed)
         self.output_type_checker.transform(predicted)
+
+        if return_transformed_data:
+            transformed.set_all(predicted.keys(), predicted.values())
+            return transformed
         return predicted
 
     @classmethod
     def from_folder(cls: Type["Inferencer"], folder: Path, serialiser: Optional[Serialiser] = None) -> "Inferencer":
         """Loads a Inferencer from the results of an Experiment.
 
         We use the absolute version of the path to try and prevent loading issues.
```

### Comparing `mlpype-0.4.7/mlpype/base/deploy/wheel/builder.py` & `mlpype-0.4.8/mlpype/base/deploy/wheel/builder.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/deploy/wheel/extensions.py` & `mlpype-0.4.8/mlpype/base/deploy/wheel/extensions.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/deploy/wheel/helpers/setup_template.py` & `mlpype-0.4.8/mlpype/base/deploy/wheel/helpers/setup_template.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/deploy/wheel/wheel.py` & `mlpype-0.4.8/mlpype/base/deploy/wheel/wheel.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/evaluate/base_evaluator.py` & `mlpype-0.4.8/mlpype/base/evaluate/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/evaluate/evaluator.py` & `mlpype-0.4.8/mlpype/base/evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/experiment/argument_parsing.py` & `mlpype-0.4.8/mlpype/base/experiment/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/experiment/experiment.py` & `mlpype-0.4.8/mlpype/base/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/logger/experiment_logger.py` & `mlpype-0.4.8/mlpype/base/logger/experiment_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/logger/local_logger.py` & `mlpype-0.4.8/mlpype/base/logger/local_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/model/model.py` & `mlpype-0.4.8/mlpype/base/model/model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/pipeline/operator.py` & `mlpype-0.4.8/mlpype/base/pipeline/operator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/pipeline/pipe.py` & `mlpype-0.4.8/mlpype/base/pipeline/pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/pipeline/pipeline.py` & `mlpype-0.4.8/mlpype/base/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/pipeline/type_checker.py` & `mlpype-0.4.8/mlpype/base/pipeline/type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/serialiser/joblib_serialiser.py` & `mlpype-0.4.8/mlpype/base/serialiser/joblib_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/serialiser/serialiser.py` & `mlpype-0.4.8/mlpype/base/serialiser/serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/setup.py` & `mlpype-0.4.8/mlpype/base/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
 
     dev_deps = ["pre-commit", "build==0.8.0", "pypiserver==1.5.1", "twine==4.0.1", "pdoc==13.1.0"]
     test_deps = ["pytest", "pytest-cov"]
     deps = [
         f"mlpype=={version}",
         "docstring_parser>=0.14.1",
         "pydantic>=1.9.1",
```

### Comparing `mlpype-0.4.7/mlpype/base/utils/parsing.py` & `mlpype-0.4.8/mlpype/base/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/base/utils/workspace.py` & `mlpype-0.4.8/mlpype/base/utils/workspace.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/fastapi/deploy/app.py` & `mlpype-0.4.8/mlpype/fastapi/deploy/app.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/fastapi/deploy/wheel/helpers.py` & `mlpype-0.4.8/mlpype/fastapi/deploy/wheel/helpers.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/fastapi/setup.py` & `mlpype-0.4.8/mlpype/fastapi/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
     deps: List[str] = [f"mlpype-base=={version}", "fastapi>=0.79.0"]
     dev_deps = ["uvicorn==0.18.2"]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
         name="mlpype-fastapi",
         install_requires=deps,
```

### Comparing `mlpype-0.4.7/mlpype/hyperopt/optimise.py` & `mlpype-0.4.8/mlpype/hyperopt/optimise.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/mlflow/deploy/load_experiment.py` & `mlpype-0.4.8/mlpype/mlflow/deploy/load_experiment.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/mlflow/logger/mlflow_logger.py` & `mlpype-0.4.8/mlpype/mlflow/logger/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/mlflow/setup.py` & `mlpype-0.4.8/mlpype/spark/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
 
     deps = [
         f"mlpype-base=={version}",
-        "mlflow>=1.28.0, <2.0",
-        "GitPython>=3.1.27",
+        # We will provide absolute no guarantees that our integration will work with
+        # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
+        "pyspark>=3.2.1",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
+    test_deps = ["pandas"]
 
     setup(
-        name="mlpype-mlflow",
+        name="mlpype-spark",
         install_requires=deps,
-        extras_require={"dev": strict_deps, "strict": strict_deps},
+        extras_require={"dev": strict_deps + test_deps, "test": strict_deps + test_deps, "strict": strict_deps},
         packages=find_namespace_packages(include=["mlpype.*"]),
         version=version,
     )
```

### Comparing `mlpype-0.4.7/mlpype/sklearn/data/data_frame_source.py` & `mlpype-0.4.8/mlpype/sklearn/data/data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/sklearn/data/sql_source.py` & `mlpype-0.4.8/mlpype/sklearn/data/sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/sklearn/model/sklearn_model.py` & `mlpype-0.4.8/mlpype/sklearn/model/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/sklearn/pipeline/numpy_type_checker.py` & `mlpype-0.4.8/mlpype/sklearn/pipeline/numpy_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/sklearn/pipeline/pandas_type_checker.py` & `mlpype-0.4.8/mlpype/sklearn/pipeline/pandas_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/sklearn/setup.py` & `mlpype-0.4.8/mlpype/sklearn/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
 
     deps = [
         f"mlpype-base=={version}",
         "numpy>=1.23.0",
         "scikit-learn>=1.1.1",
         "pandas>=1.4.3",
     ]
```

### Comparing `mlpype-0.4.7/mlpype/spark/data/spark_data_frame_source.py` & `mlpype-0.4.8/mlpype/spark/data/spark_data_frame_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/spark/data/spark_read.py` & `mlpype-0.4.8/mlpype/spark/data/spark_read.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/spark/data/spark_sql_source.py` & `mlpype-0.4.8/mlpype/spark/data/spark_sql_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/spark/evaluate/spark_evaluator.py` & `mlpype-0.4.8/mlpype/spark/evaluate/spark_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/spark/model/spark_model.py` & `mlpype-0.4.8/mlpype/spark/model/spark_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/spark/pipeline/spark_pipe.py` & `mlpype-0.4.8/mlpype/spark/pipeline/spark_pipe.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/spark/pipeline/spark_type_checker.py` & `mlpype-0.4.8/mlpype/spark/pipeline/spark_type_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/spark/serialisation/spark_serialiser.py` & `mlpype-0.4.8/mlpype/spark/serialisation/spark_serialiser.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/spark/setup.py` & `mlpype-0.4.8/mlpype/tensorflow/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
 
     deps = [
         f"mlpype-base=={version}",
-        # We will provide absolute no guarantees that our integration will work with
-        # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
-        "pyspark>=3.2.1",
+        # on mac, it is recommended to use conda/mamba or source to install tensorflow
+        "tensorflow>=2.12",
+        "numpy>=1.23.0",
+        "protobuf>=3.20.3",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
-    test_deps = ["pandas"]
 
     setup(
-        name="mlpype-spark",
+        name="mlpype-tensorflow",
         install_requires=deps,
-        extras_require={"dev": strict_deps + test_deps, "test": strict_deps + test_deps, "strict": strict_deps},
+        extras_require={"dev": strict_deps, "strict": strict_deps},
         packages=find_namespace_packages(include=["mlpype.*"]),
         version=version,
     )
```

### Comparing `mlpype-0.4.7/mlpype/tensorflow/data/tensor_source.py` & `mlpype-0.4.8/mlpype/tensorflow/data/tensor_source.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/tensorflow/model/keras_pype_model.py` & `mlpype-0.4.8/mlpype/tensorflow/model/keras_pype_model.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/tensorflow/model/mlp_keras.py` & `mlpype-0.4.8/mlpype/tensorflow/model/mlp_keras.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/tensorflow/pipeline/tensor_checker.py` & `mlpype-0.4.8/mlpype/tensorflow/pipeline/tensor_checker.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/tensorflow/setup.py` & `mlpype-0.4.8/mlpype/mlflow/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.7"
+    version = "0.4.8"
 
     deps = [
         f"mlpype-base=={version}",
-        # on mac, it is recommended to use conda/mamba or source to install tensorflow
-        "tensorflow>=2.12",
-        "numpy>=1.23.0",
-        "protobuf>=3.20.3",
+        "mlflow>=1.28.0, <2.0",
+        "GitPython>=3.1.27",
     ]
     strict_deps = [s.replace(">=", "==") for s in deps]
 
     setup(
-        name="mlpype-tensorflow",
+        name="mlpype-mlflow",
         install_requires=deps,
         extras_require={"dev": strict_deps, "strict": strict_deps},
         packages=find_namespace_packages(include=["mlpype.*"]),
         version=version,
     )
```

### Comparing `mlpype-0.4.7/mlpype/xgboost/model/xgboost_classifier.py` & `mlpype-0.4.8/mlpype/xgboost/model/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype/xgboost/model/xgboost_regressor.py` & `mlpype-0.4.8/mlpype/xgboost/model/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/mlpype.egg-info/PKG-INFO` & `mlpype-0.4.8/mlpype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpype
-Version: 0.4.7
+Version: 0.4.8
 Summary: Standardise model training across libraries
 Home-page: https://github.com/jeroenvdhoven/mlpype
 Author: Jeroen van den Hoven
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `mlpype-0.4.7/mlpype.egg-info/SOURCES.txt` & `mlpype-0.4.8/mlpype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpype-0.4.7/pyproject.toml` & `mlpype-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "mlpype"
 authors = [
     {name = "Jeroen van den Hoven"},
 ]
 description = "Standardise model training across libraries"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.4.7"
+version = "0.4.8"
 dynamic = ["license"]
 
 [tool.kedro]
 package_name = "data_cube_pipeline"
 project_name = "Data Cube Pipeline"
 project_version = "0.17.0"
```


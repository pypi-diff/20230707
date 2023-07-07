# Comparing `tmp/bluecast-0.8.tar.gz` & `tmp/bluecast-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecast-0.8.tar", max compression
+gzip compressed data, was "bluecast-0.9.tar", max compression
```

## Comparing `bluecast-0.8.tar` & `bluecast-0.9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.8/LICENSE
--rw-r--r--   0        0        0    21843 2023-07-04 12:34:21.155729 bluecast-0.8/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.8/bluecast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.8/bluecast/blueprints/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.8/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.8/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    12784 2023-07-04 05:47:32.922473 bluecast-0.8/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
--rw-r--r--   0        0        0    12771 2023-07-04 05:55:24.921932 bluecast-0.8/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
--rw-r--r--   0        0        0     3288 2023-07-04 05:48:22.227257 bluecast-0.8/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc
--rw-r--r--   0        0        0     3889 2023-07-04 08:06:47.096758 bluecast-0.8/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc
--rw-r--r--   0        0        0    18655 2023-07-04 04:45:52.998854 bluecast-0.8/bluecast/blueprints/cast.py
--rw-r--r--   0        0        0     6015 2023-07-04 09:07:51.456141 bluecast-0.8/bluecast/blueprints/cast_cv.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.8/bluecast/config/__init__.py
--rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.8/bluecast/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.8/bluecast/config/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3792 2023-07-04 05:47:32.926473 bluecast-0.8/bluecast/config/__pycache__/training_config.cpython-310.pyc
--rw-r--r--   0        0        0     3684 2023-07-04 04:33:16.382858 bluecast-0.8/bluecast/config/__pycache__/training_config.cpython-38.pyc
--rw-r--r--   0        0        0     4815 2023-07-05 03:56:09.501654 bluecast-0.8/bluecast/config/training_config.py
--rw-r--r--   0        0        0        0 2023-06-30 06:22:16.681826 bluecast-0.8/bluecast/eda/__init__.py
--rw-r--r--   0        0        0      152 2023-07-04 05:47:32.270463 bluecast-0.8/bluecast/eda/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3051 2023-07-04 05:47:32.270463 bluecast-0.8/bluecast/eda/__pycache__/analyse.cpython-310.pyc
--rw-r--r--   0        0        0     3708 2023-06-30 06:22:16.681826 bluecast-0.8/bluecast/eda/analyse.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.8/bluecast/evaluation/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.8/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.8/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1955 2023-06-29 10:24:22.109350 bluecast-0.8/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     1957 2023-06-29 13:35:03.129236 bluecast-0.8/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
--rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.8/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
--rw-r--r--   0        0        0     1321 2023-06-27 07:43:47.497769 bluecast-0.8/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
--rw-r--r--   0        0        0     2212 2023-06-28 11:13:13.084298 bluecast-0.8/bluecast/evaluation/eval_metrics.py
--rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.8/bluecast/evaluation/shap_values.py
--rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.8/bluecast/general_utils/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.8/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.8/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.8/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.8/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.8/bluecast/general_utils/general_utils.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.8/bluecast/ml_modelling/__init__.py
--rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.8/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.8/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.8/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.8/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
--rw-r--r--   0        0        0     9075 2023-07-04 05:47:33.326480 bluecast-0.8/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
--rw-r--r--   0        0        0     9009 2023-07-03 13:08:03.868811 bluecast-0.8/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
--rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/ml_modelling/base_classes.py
--rw-r--r--   0        0        0    14435 2023-07-03 13:07:54.936762 bluecast-0.8/bluecast/ml_modelling/xgboost.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.8/bluecast/preprocessing/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.8/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.8/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.8/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
--rw-r--r--   0        0        0     1919 2023-06-27 07:43:47.497769 bluecast-0.8/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc
--rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.8/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
--rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.8/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
--rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.8/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
--rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.8/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
--rw-r--r--   0        0        0     2239 2023-06-27 04:06:05.910063 bluecast-0.8/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
--rw-r--r--   0        0        0     2228 2023-06-27 07:43:47.497769 bluecast-0.8/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc
--rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.8/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
--rw-r--r--   0        0        0     4561 2023-06-27 07:43:47.501769 bluecast-0.8/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
--rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.8/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
--rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.8/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
--rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.8/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
--rw-r--r--   0        0        0     1982 2023-06-27 07:43:47.505769 bluecast-0.8/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
--rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.8/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.8/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
--rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.8/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
--rw-r--r--   0        0        0     2332 2023-06-27 07:43:47.505769 bluecast-0.8/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
--rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.8/bluecast/preprocessing/custom.py
--rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/preprocessing/datetime_features.py
--rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/preprocessing/encode_target_labels.py
--rw-r--r--   0        0        0     1890 2023-06-27 03:46:28.907353 bluecast-0.8/bluecast/preprocessing/feature_selection.py
--rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.8/bluecast/preprocessing/feature_types.py
--rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/preprocessing/nulls_and_infs.py
--rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.8/bluecast/preprocessing/schema_checks.py
--rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/preprocessing/target_encoding.py
--rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.8/bluecast/preprocessing/train_test_split.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.8/bluecast/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.8/bluecast/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1797 2023-07-04 05:47:32.018459 bluecast-0.8/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     8753 2023-07-04 05:47:32.846472 bluecast-0.8/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2412 2023-07-04 05:47:33.582484 bluecast-0.8/bluecast/tests/__pycache__/test_cast_cv.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.8/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.8/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.8/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.8/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.8/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.8/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.8/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.8/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.8/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4064 2023-06-27 04:06:05.962063 bluecast-0.8/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.8/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.8/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.8/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.8/bluecast/tests/make_data/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.8/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.8/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
--rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.8/bluecast/tests/make_data/create_data.py
--rw-r--r--   0        0        0     1176 2023-06-30 06:22:16.681826 bluecast-0.8/bluecast/tests/test_analyse.py
--rw-r--r--   0        0        0     6677 2023-06-30 06:22:16.681826 bluecast-0.8/bluecast/tests/test_cast.py
--rw-r--r--   0        0        0     1357 2023-07-04 05:47:13.522164 bluecast-0.8/bluecast/tests/test_cast_cv.py
--rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.8/bluecast/tests/test_check_gpu_support.py
--rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.8/bluecast/tests/test_custom_processing_base_class.py
--rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.8/bluecast/tests/test_datetime_features.py
--rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.8/bluecast/tests/test_encode_target_labels.py
--rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.8/bluecast/tests/test_feature_type_detector.py
--rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.8/bluecast/tests/test_load_for_production.py
--rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.8/bluecast/tests/test_nulls_and_infs.py
--rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.8/bluecast/tests/test_save_to_production.py
--rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.8/bluecast/tests/test_schema_checks.py
--rw-r--r--   0        0        0     2296 2023-06-27 03:46:28.907353 bluecast-0.8/bluecast/tests/test_shap_explanations.py
--rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.8/bluecast/tests/test_target_encoding_binary.py
--rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.8/bluecast/tests/test_target_encoding_multiclass.py
--rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.8/bluecast/tests/test_train_test_split.py
--rw-r--r--   0        0        0     1478 2023-07-02 15:26:48.016156 bluecast-0.8/pyproject.toml
--rw-r--r--   0        0        0    22993 1970-01-01 00:00:00.000000 bluecast-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.9/LICENSE
+-rw-r--r--   0        0        0    22150 2023-07-06 04:36:03.818725 bluecast-0.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.9/bluecast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.9/bluecast/blueprints/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.9/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.9/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    12784 2023-07-05 10:48:05.571979 bluecast-0.9/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
+-rw-r--r--   0        0        0    12771 2023-07-04 05:55:24.921932 bluecast-0.9/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
+-rw-r--r--   0        0        0     4354 2023-07-05 10:48:06.115987 bluecast-0.9/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc
+-rw-r--r--   0        0        0     3889 2023-07-04 08:06:47.096758 bluecast-0.9/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc
+-rw-r--r--   0        0        0    18655 2023-07-05 06:07:39.547549 bluecast-0.9/bluecast/blueprints/cast.py
+-rw-r--r--   0        0        0     6244 2023-07-06 03:40:08.782319 bluecast-0.9/bluecast/blueprints/cast_cv.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.9/bluecast/config/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.9/bluecast/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.9/bluecast/config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5690 2023-07-05 10:48:05.571979 bluecast-0.9/bluecast/config/__pycache__/training_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3684 2023-07-04 04:33:16.382858 bluecast-0.9/bluecast/config/__pycache__/training_config.cpython-38.pyc
+-rw-r--r--   0        0        0     4823 2023-07-05 11:13:08.171327 bluecast-0.9/bluecast/config/training_config.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:22:16.681826 bluecast-0.9/bluecast/eda/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-04 05:47:32.270463 bluecast-0.9/bluecast/eda/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4727 2023-07-06 04:32:26.415879 bluecast-0.9/bluecast/eda/__pycache__/analyse.cpython-310.pyc
+-rw-r--r--   0        0        0     5566 2023-07-06 04:35:35.374354 bluecast-0.9/bluecast/eda/analyse.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.9/bluecast/evaluation/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.9/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.9/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1955 2023-06-29 10:24:22.109350 bluecast-0.9/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     1957 2023-06-29 13:35:03.129236 bluecast-0.9/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.9/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
+-rw-r--r--   0        0        0     1321 2023-06-27 07:43:47.497769 bluecast-0.9/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
+-rw-r--r--   0        0        0     2212 2023-06-28 11:13:13.084298 bluecast-0.9/bluecast/evaluation/eval_metrics.py
+-rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.9/bluecast/evaluation/shap_values.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.9/bluecast/general_utils/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.9/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.9/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.9/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.9/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.9/bluecast/general_utils/general_utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.9/bluecast/ml_modelling/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.9/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.9/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.9/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.9/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
+-rw-r--r--   0        0        0     9075 2023-07-05 10:48:05.895984 bluecast-0.9/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
+-rw-r--r--   0        0        0     9009 2023-07-03 13:08:03.868811 bluecast-0.9/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
+-rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.9/bluecast/ml_modelling/base_classes.py
+-rw-r--r--   0        0        0    14435 2023-07-05 06:07:39.547549 bluecast-0.9/bluecast/ml_modelling/xgboost.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.9/bluecast/preprocessing/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.9/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.9/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.9/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
+-rw-r--r--   0        0        0     1919 2023-06-27 07:43:47.497769 bluecast-0.9/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc
+-rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.9/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
+-rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.9/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
+-rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.9/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
+-rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.9/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     2239 2023-06-27 04:06:05.910063 bluecast-0.9/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     2228 2023-06-27 07:43:47.497769 bluecast-0.9/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc
+-rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.9/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
+-rw-r--r--   0        0        0     4561 2023-06-27 07:43:47.501769 bluecast-0.9/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
+-rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.9/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
+-rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.9/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
+-rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.9/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     1982 2023-06-27 07:43:47.505769 bluecast-0.9/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
+-rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.9/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.9/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
+-rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.9/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
+-rw-r--r--   0        0        0     2332 2023-06-27 07:43:47.505769 bluecast-0.9/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
+-rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.9/bluecast/preprocessing/custom.py
+-rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.9/bluecast/preprocessing/datetime_features.py
+-rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.9/bluecast/preprocessing/encode_target_labels.py
+-rw-r--r--   0        0        0     1890 2023-06-27 03:46:28.907353 bluecast-0.9/bluecast/preprocessing/feature_selection.py
+-rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.9/bluecast/preprocessing/feature_types.py
+-rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.9/bluecast/preprocessing/nulls_and_infs.py
+-rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.9/bluecast/preprocessing/schema_checks.py
+-rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.9/bluecast/preprocessing/target_encoding.py
+-rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.9/bluecast/preprocessing/train_test_split.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.9/bluecast/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.9/bluecast/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2298 2023-07-06 04:31:30.823147 bluecast-0.9/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     9445 2023-07-05 10:48:05.511978 bluecast-0.9/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4202 2023-07-05 10:48:06.115987 bluecast-0.9/bluecast/tests/__pycache__/test_cast_cv.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.9/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.9/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.9/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.9/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.9/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.9/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.9/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.9/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.9/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4064 2023-06-27 04:06:05.962063 bluecast-0.9/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.9/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.9/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.9/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.9/bluecast/tests/make_data/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.9/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.9/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.9/bluecast/tests/make_data/create_data.py
+-rw-r--r--   0        0        0     1938 2023-07-06 04:35:19.978153 bluecast-0.9/bluecast/tests/test_analyse.py
+-rw-r--r--   0        0        0     6677 2023-07-05 11:13:08.171327 bluecast-0.9/bluecast/tests/test_cast.py
+-rw-r--r--   0        0        0     1357 2023-07-05 11:13:08.171327 bluecast-0.9/bluecast/tests/test_cast_cv.py
+-rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.9/bluecast/tests/test_check_gpu_support.py
+-rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.9/bluecast/tests/test_custom_processing_base_class.py
+-rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.9/bluecast/tests/test_datetime_features.py
+-rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.9/bluecast/tests/test_encode_target_labels.py
+-rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.9/bluecast/tests/test_feature_type_detector.py
+-rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.9/bluecast/tests/test_load_for_production.py
+-rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.9/bluecast/tests/test_nulls_and_infs.py
+-rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.9/bluecast/tests/test_save_to_production.py
+-rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.9/bluecast/tests/test_schema_checks.py
+-rw-r--r--   0        0        0     2296 2023-06-27 03:46:28.907353 bluecast-0.9/bluecast/tests/test_shap_explanations.py
+-rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.9/bluecast/tests/test_target_encoding_binary.py
+-rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.9/bluecast/tests/test_target_encoding_multiclass.py
+-rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.9/bluecast/tests/test_train_test_split.py
+-rw-r--r--   0        0        0     1478 2023-07-05 11:15:09.817603 bluecast-0.9/pyproject.toml
+-rw-r--r--   0        0        0    23300 1970-01-01 00:00:00.000000 bluecast-0.9/PKG-INFO
```

### Comparing `bluecast-0.8/LICENSE` & `bluecast-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/README.md` & `bluecast-0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,24 @@
             :, feat_type_detector.num_columns])
 
 # show correlation to target
 correlation_to_target(train_data.loc[
             :, feat_type_detector.num_columns
         ],
         "EC1",)
+
+# show feature space after principal component analysis
+plot_pca(train_data.loc[
+            :, feat_type_detector.num_columns
+        ], "target")
+
+# show feature space after t-SNE
+plot_tsne(train_data.loc[
+            :, feat_type_detector.num_columns
+        ], "target", perplexity=30, random_state=0)
 ```
 
 #### Enable cross-validation
 
 While the default behaviour of BlueCast is to use a simple
 train-test-split, cross-validation can be enabled easily:
```

### Comparing `bluecast-0.8/bluecast/blueprints/__pycache__/cast.cpython-310.pyc` & `bluecast-0.9/bluecast/blueprints/__pycache__/cast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 04:45:52 2023 UTC, .py size: 18655 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 00a4 a364 df48 0000  o..........d.H..
+00000000: 6f0d 0d0a 0000 0000 ab08 a564 df48 0000  o..........d.H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 0100 6401 6404 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6402 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0c 6401 6402 6c0d 5a0e 6401 6405 6c0f  Z.d.d.l.Z.d.d.l.
```

### Comparing `bluecast-0.8/bluecast/blueprints/__pycache__/cast.cpython-38.pyc` & `bluecast-0.9/bluecast/blueprints/__pycache__/cast.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc` & `bluecast-0.9/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 05:48:18 2023 UTC, .py size: 4146 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,244 @@
-00000000: 6f0d 0d0a 0000 0000 a2b2 a364 3210 0000  o..........d2...
+00000000: 550d 0d0a 0000 0000 5bce a364 9513 0000  U.......[..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 5a08 6400 6403 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  d.l.m.Z.m.Z.m.Z.
 00000080: 0100 4700 6406 6407 8400 6407 8302 5a11  ..G.d.d...d...Z.
 00000090: 6402 5300 2908 e900 0000 0029 06da 0341  d.S.)......)...A
 000000a0: 6e79 da04 4c69 7374 da07 4c69 7465 7261  ny..List..Litera
 000000b0: 6cda 084f 7074 696f 6e61 6cda 0554 7570  l..Optional..Tup
-000000c0: 6c65 da05 556e 696f 6e4e 2901 da17 5265  le..UnionN)...Re
-000000d0: 7065 6174 6564 5374 7261 7469 6669 6564  peatedStratified
-000000e0: 4b46 6f6c 6429 01da 0842 6c75 6543 6173  KFold)...BlueCas
-000000f0: 7429 03da 0e54 7261 696e 696e 6743 6f6e  t)...TrainingCon
-00000100: 6669 67da 1758 6762 6f6f 7374 4669 6e61  fig..XgboostFina
-00000110: 6c50 6172 616d 436f 6e66 6967 da17 5867  lParamConfig..Xg
-00000120: 626f 6f73 7454 756e 6550 6172 616d 7343  boostTuneParamsC
-00000130: 6f6e 6669 6763 0000 0000 0000 0000 0000  onfigc..........
-00000140: 0000 0000 0000 0a00 0000 4000 0000 73d0  ..........@...s.
-00000150: 0000 0065 005a 0164 005a 0209 0109 0209  ...e.Z.d.Z......
-00000160: 0209 0264 1964 0365 0364 0419 0064 0565  ...d.d.e.d...d.e
-00000170: 0465 0519 0064 0665 0465 0619 0064 0765  .e...d.e.e...d.e
-00000180: 0465 0719 0066 0864 0864 0984 055a 0864  .e...f.d.d...Z.d
-00000190: 0a65 096a 0a64 0b65 0b64 0c65 0c65 096a  .e.j.d.e.d.e.e.j
-000001a0: 0a65 096a 0d66 0219 0066 0664 0d64 0e84  .e.j.f...f.d.d..
-000001b0: 045a 0e64 0a65 096a 0a64 0b65 0b64 0f65  .Z.d.e.j.d.e.d.e
-000001c0: 0465 0f19 0064 0c64 0266 0864 1064 1184  .e...d.d.f.d.d..
-000001d0: 045a 1009 0264 1a64 0a65 096a 0a64 1265  .Z...d.d.e.j.d.e
-000001e0: 0b64 0f65 0465 0f19 0064 0c64 0266 0864  .d.e.e...d.d.f.d
-000001f0: 1364 1484 055a 1109 1564 1b64 0a65 096a  .d...Z...d.d.e.j
-00000200: 0a64 1665 1264 0c65 1365 096a 0a65 096a  .d.e.d.e.e.j.e.j
-00000210: 0d66 0219 0066 0664 1764 1884 055a 1464  .f...f.d.d...Z.d
-00000220: 0253 0029 1cda 0a42 6c75 6543 6173 7443  .S.)...BlueCastC
-00000230: 56da 0662 696e 6172 794e da0d 636c 6173  V..binaryN..clas
-00000240: 735f 7072 6f62 6c65 6d29 0272 0e00 0000  s_problem).r....
-00000250: da0a 6d75 6c74 6963 6c61 7373 da0d 636f  ..multiclass..co
-00000260: 6e66 5f74 7261 696e 696e 67da 0c63 6f6e  nf_training..con
-00000270: 665f 7867 626f 6f73 74da 1363 6f6e 665f  f_xgboost..conf_
-00000280: 7061 7261 6d73 5f78 6762 6f6f 7374 6305  params_xgboostc.
-00000290: 0000 0000 0000 0000 0000 0005 0000 0002  ................
-000002a0: 0000 0043 0000 0073 2200 0000 7c01 7c00  ...C...s"...|.|.
-000002b0: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 7c04  _.|.|._.|.|._.|.
-000002c0: 7c00 5f03 6700 7c00 5f04 6400 5300 a901  |._.g.|._.d.S...
-000002d0: 4e29 0572 0f00 0000 7211 0000 0072 1200  N).r....r....r..
-000002e0: 0000 7213 0000 00da 0f62 6c75 6563 6173  ..r......bluecas
-000002f0: 745f 6d6f 6465 6c73 2905 da04 7365 6c66  t_models)...self
-00000300: 720f 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00000310: 1300 0000 a900 7217 0000 00fa 412f 686f  ......r.....A/ho
-00000320: 6d65 2f74 686f 6d61 732f 4964 6561 5072  me/thomas/IdeaPr
-00000330: 6f6a 6563 7473 2f42 6c75 6543 6173 742f  ojects/BlueCast/
-00000340: 626c 7565 6361 7374 2f62 6c75 6570 7269  bluecast/bluepri
-00000350: 6e74 732f 6361 7374 5f63 762e 7079 da08  nts/cast_cv.py..
-00000360: 5f5f 696e 6974 5f5f 0f00 0000 730a 0000  __init__....s...
-00000370: 0006 0706 0106 0106 010a 017a 1342 6c75  ...........z.Blu
-00000380: 6543 6173 7443 562e 5f5f 696e 6974 5f5f  eCastCV.__init__
-00000390: da02 6466 da06 7461 7267 6574 da06 7265  ..df..target..re
-000003a0: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
-000003b0: 0005 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
-000003c0: 0000 7c01 7c02 1900 7d03 7c01 6a00 7c02  ..|.|...}.|.j.|.
-000003d0: 6401 6402 8d02 7d04 7c04 7c03 6602 5300  d.d...}.|.|.f.S.
-000003e0: 2903 4ee9 0100 0000 a901 da04 6178 6973  ).N.........axis
-000003f0: a901 da04 6472 6f70 2905 7216 0000 0072  ....drop).r....r
-00000400: 1a00 0000 721b 0000 00da 0179 da01 5872  ....r......y..Xr
-00000410: 1700 0000 7217 0000 0072 1800 0000 da0c  ....r....r......
-00000420: 7072 6570 6172 655f 6461 7461 1c00 0000  prepare_data....
-00000430: 7306 0000 0008 030e 0108 017a 1742 6c75  s..........z.Blu
-00000440: 6543 6173 7443 562e 7072 6570 6172 655f  eCastCV.prepare_
-00000450: 6461 7461 da0a 7374 7261 7469 6669 6572  data..stratifier
-00000460: 6304 0000 0000 0000 0000 0000 000f 0000  c...............
-00000470: 0008 0000 0043 0000 0073 0e01 0000 7c00  .....C...s....|.
-00000480: a000 7c01 7c02 a102 5c02 7d04 7d05 7c00  ..|.|...\.}.}.|.
-00000490: 6a01 730f 7402 8300 7c00 5f01 7c03 731a  j.s.t...|._.|.s.
-000004a0: 7403 6401 6402 7c00 6a01 6a04 6403 8d03  t.d.d.|.j.j.d...
-000004b0: 7d03 7405 7c03 a006 7c04 7c05 a102 8301  }.t.|...|.|.....
-000004c0: 4400 5d62 5c02 7d06 5c02 7d07 7d08 7c04  D.]b\.}.\.}.}.|.
-000004d0: 6a07 7c07 1900 7c04 6a07 7c08 1900 0202  j.|...|.j.|.....
-000004e0: 7d09 7d0a 7c05 6a07 7c07 1900 7c05 6a07  }.}.|.j.|...|.j.
-000004f0: 7c08 1900 0202 7d0b 7d0c 7408 6a09 7c09  |.....}.}.t.j.|.
-00000500: 7c0a 6702 6404 6405 8d02 7d0d 7408 6a09  |.g.d.d...}.t.j.
-00000510: 7c0b 7c0c 6702 6404 6405 8d02 7d0b 7c0d  |.|.g.d.d...}.|.
-00000520: 6a0a 6406 6407 8d01 7d0d 7c0b 6a0a 6406  j.d.d...}.|.j.d.
-00000530: 6407 8d01 7d0b 7c0b 7c02 1900 7c0d 7c02  d...}.|.|...|.|.
-00000540: 3c00 7c00 6a01 0400 6a04 7c06 3700 0200  <.|.j...j.|.7...
-00000550: 5f04 740b 7c00 6a0c 7c02 7c00 6a01 7c00  _.t.|.j.|.|.j.|.
-00000560: 6a0d 7c00 6a0e 6408 8d05 7d0e 7c0e 6a0f  j.|.j.d...}.|.j.
-00000570: 7c09 7c02 6409 8d02 0100 7c00 6a10 a011  |.|.d.....|.j...
-00000580: 7c0e a101 0100 7122 6400 5300 290a 4ee9  |.....q"d.S.).N.
-00000590: 0500 0000 e903 0000 00a9 03da 086e 5f73  .............n_s
-000005a0: 706c 6974 73da 096e 5f72 6570 6561 7473  plits..n_repeats
-000005b0: da0c 7261 6e64 6f6d 5f73 7461 7465 721d  ..random_stater.
-000005c0: 0000 0072 1e00 0000 5472 2000 0000 a905  ...r....Tr .....
-000005d0: 720f 0000 00da 0d74 6172 6765 745f 636f  r......target_co
-000005e0: 6c75 6d6e 7211 0000 0072 1200 0000 7213  lumnr....r....r.
-000005f0: 0000 00a9 01da 0a74 6172 6765 745f 636f  .......target_co
-00000600: 6c29 1272 2400 0000 7211 0000 0072 0a00  l).r$...r....r..
-00000610: 0000 7208 0000 00da 1367 6c6f 6261 6c5f  ..r......global_
-00000620: 7261 6e64 6f6d 5f73 7461 7465 da09 656e  random_state..en
-00000630: 756d 6572 6174 65da 0573 706c 6974 da04  umerate..split..
-00000640: 696c 6f63 da02 7064 da06 636f 6e63 6174  iloc..pd..concat
-00000650: da0b 7265 7365 745f 696e 6465 7872 0900  ..reset_indexr..
-00000660: 0000 720f 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00000670: 00da 0366 6974 7215 0000 00da 0661 7070  ...fitr......app
-00000680: 656e 6429 0f72 1600 0000 721a 0000 0072  end).r....r....r
-00000690: 1b00 0000 7225 0000 0072 2300 0000 7222  ....r%...r#...r"
-000006a0: 0000 00da 0266 6eda 0774 726e 5f69 6478  .....fn..trn_idx
-000006b0: da07 7661 6c5f 6964 78da 0758 5f74 7261  ..val_idx..X_tra
-000006c0: 696e da05 585f 7661 6cda 0779 5f74 7261  in..X_val..y_tra
-000006d0: 696e da05 795f 7661 6cda 0778 5f74 7261  in..y_val..x_tra
-000006e0: 696e da06 6175 746f 6d6c 7217 0000 0072  in..automlr....r
-000006f0: 1700 0000 7218 0000 0072 3700 0000 2300  ....r....r7...#.
-00000700: 0000 7338 0000 0010 0106 0208 0104 0202  ..s8............
-00000710: 0102 0102 0106 0106 fd1c 0616 0116 0112  ................
-00000720: 0112 010c 020c 010c 0110 0202 0204 0102  ................
-00000730: 0104 0104 0104 0106 fb0e 070e 0104 ec7a  ...............z
-00000740: 0e42 6c75 6543 6173 7443 562e 6669 7472  .BlueCastCV.fitr
-00000750: 2f00 0000 6304 0000 0000 0000 0000 0000  /...c...........
-00000760: 000e 0000 0008 0000 0043 0000 0073 d200  .........C...s..
-00000770: 0000 7c00 a000 7c01 7c02 a102 5c02 7d04  ..|...|.|...\.}.
-00000780: 7d05 7c00 6a01 730f 7402 8300 7c00 5f01  }.|.j.s.t...|._.
-00000790: 7c03 731a 7403 6401 6402 7c00 6a01 6a04  |.s.t.d.d.|.j.j.
-000007a0: 6403 8d03 7d03 7405 7c03 a006 7c04 7c05  d...}.t.|...|.|.
-000007b0: a102 8301 4400 5d44 5c02 7d06 5c02 7d07  ....D.]D\.}.\.}.
-000007c0: 7d08 7c04 6a07 7c07 1900 7c04 6a07 7c08  }.|.j.|...|.j.|.
-000007d0: 1900 0202 7d09 7d0a 7c05 6a07 7c07 1900  ....}.}.|.j.|...
-000007e0: 7c05 6a07 7c08 1900 0202 7d0b 7d0c 7c0b  |.j.|.....}.}.|.
-000007f0: 7c09 7c02 3c00 7c00 6a01 0400 6a04 7c06  |.|.<.|.j...j.|.
-00000800: 3700 0200 5f04 7408 7c00 6a09 7c02 7c00  7..._.t.|.j.|.|.
-00000810: 6a01 7c00 6a0a 7c00 6a0b 6404 8d05 7d0d  j.|.j.|.j.d...}.
-00000820: 7c0d 6a0c 7c09 7c0a 7c0c 7c02 6405 8d04  |.j.|.|.|.|.d...
-00000830: 0100 7c00 6a0d a00e 7c0d a101 0100 7122  ..|.j...|.....q"
-00000840: 6400 5300 2906 4e72 2600 0000 7227 0000  d.S.).Nr&...r'..
-00000850: 0072 2800 0000 722c 0000 0072 2e00 0000  .r(...r,...r....
-00000860: 290f 7224 0000 0072 1100 0000 720a 0000  ).r$...r....r...
-00000870: 0072 0800 0000 7230 0000 0072 3100 0000  .r....r0...r1...
-00000880: 7232 0000 0072 3300 0000 7209 0000 0072  r2...r3...r....r
-00000890: 0f00 0000 7212 0000 0072 1300 0000 da08  ....r....r......
-000008a0: 6669 745f 6576 616c 7215 0000 0072 3800  fit_evalr....r8.
-000008b0: 0000 290e 7216 0000 0072 1a00 0000 722f  ..).r....r....r/
-000008c0: 0000 0072 2500 0000 7223 0000 0072 2200  ...r%...r#...r".
-000008d0: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
-000008e0: 0072 3c00 0000 723d 0000 0072 3e00 0000  .r<...r=...r>...
-000008f0: 723f 0000 0072 4100 0000 7217 0000 0072  r?...rA...r....r
-00000900: 1700 0000 7218 0000 0072 4200 0000 4600  ....r....rB...F.
-00000910: 0000 7330 0000 0010 0306 0208 0104 0202  ..s0............
-00000920: 0102 0102 0106 0106 fd1c 0616 0116 0108  ................
-00000930: 0210 0202 0204 0102 0104 0104 0104 0106  ................
-00000940: fb12 070e 0104 f07a 1342 6c75 6543 6173  .......z.BlueCas
-00000950: 7443 562e 6669 745f 6576 616c 46da 1872  tCV.fit_evalF..r
-00000960: 6574 7572 6e5f 7375 625f 6d6f 6465 6c73  eturn_sub_models
-00000970: 5f70 726f 6261 7363 0300 0000 0000 0000  _probasc........
-00000980: 0000 0000 0900 0000 0600 0000 4300 0000  ............C...
-00000990: 7388 0000 007c 016a 007d 0367 007d 0474  s....|.j.}.g.}.t
-000009a0: 017c 006a 0283 0144 005d 215c 027d 057d  .|.j...D.]!\.}.}
-000009b0: 067c 06a0 037c 016a 0464 0064 0085 027c  .|...|.j.d.d...|
-000009c0: 0366 0219 00a1 015c 027d 077d 087c 077c  .f.....\.}.}.|.|
-000009d0: 0164 017c 059b 009d 023c 007c 04a0 0564  .d.|.....<.|...d
-000009e0: 017c 059b 009d 02a1 0101 0071 0a7c 0272  .|.........q.|.r
-000009f0: 377c 016a 0464 0064 0085 027c 0466 0219  7|.j.d.d...|.f..
-00000a00: 0053 007c 016a 0464 0064 0085 027c 0466  .S.|.j.d.d...|.f
-00000a10: 0219 006a 0664 0264 038d 0153 0029 044e  ...j.d.d...S.).N
-00000a20: 5a06 7072 6f62 615f 721d 0000 0072 1e00  Z.proba_r....r..
-00000a30: 0000 2907 da07 636f 6c75 6d6e 7372 3100  ..)...columnsr1.
-00000a40: 0000 7215 0000 00da 0770 7265 6469 6374  ..r......predict
-00000a50: da03 6c6f 6372 3800 0000 da04 6d65 616e  ..locr8.....mean
-00000a60: 2909 7216 0000 0072 1a00 0000 7243 0000  ).r....r....rC..
-00000a70: 005a 076f 725f 636f 6c73 5a09 7072 6564  .Z.or_colsZ.pred
-00000a80: 5f63 6f6c 7372 3900 0000 da08 7069 7065  _colsr9.....pipe
-00000a90: 6c69 6e65 da07 795f 7072 6f62 73da 0979  line..y_probs..y
-00000aa0: 5f63 6c61 7373 6573 7217 0000 0072 1700  _classesr....r..
-00000ab0: 0000 7218 0000 0072 4500 0000 6700 0000  ..r....rE...g...
-00000ac0: 7312 0000 0006 0304 0112 011c 010e 0112  s...............
-00000ad0: 0104 0212 011a 027a 1242 6c75 6543 6173  .......z.BlueCas
-00000ae0: 7443 562e 7072 6564 6963 7429 0472 0e00  tCV.predict).r..
-00000af0: 0000 4e4e 4e72 1400 0000 2901 4629 15da  ..NNNr....).F)..
-00000b00: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000b10: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000b20: 655f 5f72 0400 0000 7205 0000 0072 0a00  e__r....r....r..
-00000b30: 0000 720c 0000 0072 0b00 0000 7219 0000  ..r....r....r...
-00000b40: 0072 3400 0000 da09 4461 7461 4672 616d  .r4.....DataFram
-00000b50: 65da 0373 7472 7206 0000 00da 0653 6572  e..strr......Ser
-00000b60: 6965 7372 2400 0000 7202 0000 0072 3700  iesr$...r....r7.
-00000b70: 0000 7242 0000 00da 0462 6f6f 6c72 0700  ..rB.....boolr..
-00000b80: 0000 7245 0000 0072 1700 0000 7217 0000  ..rE...r....r...
-00000b90: 0072 1700 0000 7218 0000 0072 0d00 0000  .r....r....r....
-00000ba0: 0e00 0000 7350 0000 0008 0002 0302 0102  ....sP..........
-00000bb0: 0102 0104 fb06 0202 fe06 0302 fd06 0402  ................
-00000bc0: fc06 050a fb02 0d04 0102 ff02 0102 ff0e  ................
-00000bd0: 020a fe20 0702 2404 ff04 0102 ff02 0102  ... ..$.........
-00000be0: ff06 0102 ff02 020a fe02 2204 ff04 0102  ..........".....
-00000bf0: ff02 0102 ff0e 020e fe72 0d00 0000 2912  .........r....).
-00000c00: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000c10: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
-00000c20: 0072 0700 0000 da06 7061 6e64 6173 7234  .r......pandasr4
-00000c30: 0000 00da 1773 6b6c 6561 726e 2e6d 6f64  .....sklearn.mod
-00000c40: 656c 5f73 656c 6563 7469 6f6e 7208 0000  el_selectionr...
-00000c50: 00da 1862 6c75 6563 6173 742e 626c 7565  ...bluecast.blue
-00000c60: 7072 696e 7473 2e63 6173 7472 0900 0000  prints.castr....
-00000c70: da1f 626c 7565 6361 7374 2e63 6f6e 6669  ..bluecast.confi
-00000c80: 672e 7472 6169 6e69 6e67 5f63 6f6e 6669  g.training_confi
-00000c90: 6772 0a00 0000 720b 0000 0072 0c00 0000  gr....r....r....
-00000ca0: 720d 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-00000cb0: 1700 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
-00000cc0: 6c65 3e01 0000 0073 0c00 0000 2000 0802  le>....s.... ...
-00000cd0: 0c01 0c02 1401 1207                      ........
+000000c0: 6c65 da05 556e 696f 6e4e 2901 da0f 5374  le..UnionN)...St
+000000d0: 7261 7469 6669 6564 4b46 6f6c 6429 01da  ratifiedKFold)..
+000000e0: 0842 6c75 6543 6173 7429 03da 0e54 7261  .BlueCast)...Tra
+000000f0: 696e 696e 6743 6f6e 6669 67da 1758 6762  iningConfig..Xgb
+00000100: 6f6f 7374 4669 6e61 6c50 6172 616d 436f  oostFinalParamCo
+00000110: 6e66 6967 da17 5867 626f 6f73 7454 756e  nfig..XgboostTun
+00000120: 6550 6172 616d 7343 6f6e 6669 6763 0000  eParamsConfigc..
+00000130: 0000 0000 0000 0000 0000 0000 0000 0800  ................
+00000140: 0000 4000 0000 73ba 0000 0065 005a 0164  ..@...s....e.Z.d
+00000150: 005a 0264 015a 0364 1465 0464 0419 0065  .Z.d.Z.d.e.d...e
+00000160: 0565 0619 0065 0565 0719 0065 0565 0819  .e...e.e...e.e..
+00000170: 0065 0565 0919 0064 059c 0564 0664 0784  .e.e...d...d.d..
+00000180: 055a 0a65 0b6a 0c65 0d65 0e65 0b6a 0c65  .Z.e.j.e.e.e.j.e
+00000190: 0b6a 0f66 0219 0064 089c 0364 0964 0a84  .j.f...d...d.d..
+000001a0: 045a 1065 0b6a 0c65 0d64 0364 0b9c 0364  .Z.e.j.e.d.d...d
+000001b0: 0c64 0d84 045a 1165 0b6a 0c65 0d64 0364  .d...Z.e.j.e.d.d
+000001c0: 0b9c 0364 0e64 0f84 045a 1264 1565 0b6a  ...d.d...Z.d.e.j
+000001d0: 0c65 1365 0e65 1465 0b6a 0c65 0b6a 0f66  .e.e.e.e.j.e.j.f
+000001e0: 0219 0065 1465 0b6a 0c65 0b6a 0f66 0219  ...e.e.j.e.j.f..
+000001f0: 0066 0219 0064 119c 0364 1264 1384 055a  .f...d...d.d...Z
+00000200: 1564 0353 0029 16da 0a42 6c75 6543 6173  .d.S.)...BlueCas
+00000210: 7443 567a 6157 7261 7070 6572 2074 6f20  tCVzaWrapper to 
+00000220: 7472 6169 6e20 616e 6420 7072 6564 6963  train and predic
+00000230: 7420 6d75 6c74 6970 6c65 2062 6c75 6543  t multiple blueC
+00000240: 6173 7420 696e 7473 616e 6365 732e 0a0a  ast intsances...
+00000250: 2020 2020 4120 6375 7374 6f6d 2073 706c      A custom spl
+00000260: 6974 7465 7220 6361 6e20 6265 2070 726f  itter can be pro
+00000270: 7669 6465 642e da06 6269 6e61 7279 4e29  vided...binaryN)
+00000280: 0272 0e00 0000 da0a 6d75 6c74 6963 6c61  .r......multicla
+00000290: 7373 2905 da0d 636c 6173 735f 7072 6f62  ss)...class_prob
+000002a0: 6c65 6dda 0a73 7472 6174 6966 6965 72da  lem..stratifier.
+000002b0: 0d63 6f6e 665f 7472 6169 6e69 6e67 da0c  .conf_training..
+000002c0: 636f 6e66 5f78 6762 6f6f 7374 da13 636f  conf_xgboost..co
+000002d0: 6e66 5f70 6172 616d 735f 7867 626f 6f73  nf_params_xgboos
+000002e0: 7463 0600 0000 0000 0000 0000 0000 0600  tc..............
+000002f0: 0000 0200 0000 4300 0000 7328 0000 007c  ......C...s(...|
+00000300: 017c 005f 007c 047c 005f 017c 037c 005f  .|._.|.|._.|.|._
+00000310: 027c 057c 005f 0367 007c 005f 047c 027c  .|.|._.g.|._.|.|
+00000320: 005f 0564 0053 0029 014e 2906 7210 0000  ._.d.S.).N).r...
+00000330: 0072 1300 0000 7212 0000 0072 1400 0000  .r....r....r....
+00000340: da0f 626c 7565 6361 7374 5f6d 6f64 656c  ..bluecast_model
+00000350: 7372 1100 0000 2906 da04 7365 6c66 7210  sr....)...selfr.
+00000360: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+00000370: 0000 7214 0000 00a9 0072 1700 0000 fa41  ..r......r.....A
+00000380: 2f68 6f6d 652f 7468 6f6d 6173 2f49 6465  /home/thomas/Ide
+00000390: 6150 726f 6a65 6374 732f 426c 7565 4361  aProjects/BlueCa
+000003a0: 7374 2f62 6c75 6563 6173 742f 626c 7565  st/bluecast/blue
+000003b0: 7072 696e 7473 2f63 6173 745f 6376 2e70  prints/cast_cv.p
+000003c0: 79da 085f 5f69 6e69 745f 5f13 0000 0073  y..__init__....s
+000003d0: 0c00 0000 0008 0601 0601 0601 0601 0601  ................
+000003e0: 7a13 426c 7565 4361 7374 4356 2e5f 5f69  z.BlueCastCV.__i
+000003f0: 6e69 745f 5f29 03da 0264 66da 0674 6172  nit__)...df..tar
+00000400: 6765 74da 0672 6574 7572 6e63 0300 0000  get..returnc....
+00000410: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+00000420: 4300 0000 732a 0000 007c 016a 0064 0164  C...s*...|.j.d.d
+00000430: 028d 017d 017c 017c 0219 007d 037c 016a  ...}.|.|...}.|.j
+00000440: 017c 0264 0364 048d 027d 047c 047c 0366  .|.d.d...}.|.|.f
+00000450: 0253 0029 054e 54a9 01da 0464 726f 70e9  .S.).NT....drop.
+00000460: 0100 0000 a901 da04 6178 6973 2902 da0b  ........axis)...
+00000470: 7265 7365 745f 696e 6465 7872 1e00 0000  reset_indexr....
+00000480: 2905 7216 0000 0072 1a00 0000 721b 0000  ).r....r....r...
+00000490: 00da 0179 da01 5872 1700 0000 7217 0000  ...y..Xr....r...
+000004a0: 0072 1800 0000 da0c 7072 6570 6172 655f  .r......prepare_
+000004b0: 6461 7461 2200 0000 7308 0000 0000 030c  data"...s.......
+000004c0: 0108 010e 017a 1742 6c75 6543 6173 7443  .....z.BlueCastC
+000004d0: 562e 7072 6570 6172 655f 6461 7461 2903  V.prepare_data).
+000004e0: 721a 0000 00da 0a74 6172 6765 745f 636f  r......target_co
+000004f0: 6c72 1c00 0000 6303 0000 0000 0000 0000  lr....c.........
+00000500: 0000 000e 0000 0008 0000 0043 0000 0073  ...........C...s
+00000510: 1201 0000 7c00 a000 7c01 7c02 a102 5c02  ....|...|.|...\.
+00000520: 7d03 7d04 7c00 6a01 731e 7402 8300 7c00  }.}.|.j.s.t...|.
+00000530: 5f01 7c00 6a03 7338 7404 6401 6402 7c00  _.|.j.s8t.d.d.|.
+00000540: 6a01 6a05 6403 8d03 7c00 5f03 7406 7c00  j.j.d...|._.t.|.
+00000550: 6a03 a007 7c03 7c04 a102 8301 4400 5dc2  j...|.|.....D.].
+00000560: 5c02 7d05 5c02 7d06 7d07 7c03 6a08 7c06  \.}.\.}.}.|.j.|.
+00000570: 1900 7c03 6a08 7c07 1900 0200 7d08 7d09  ..|.j.|.....}.}.
+00000580: 7c04 6a08 7c06 1900 7c04 6a08 7c07 1900  |.j.|...|.j.|...
+00000590: 0200 7d0a 7d0b 7409 6a0a 7c08 7c09 6702  ..}.}.t.j.|.|.g.
+000005a0: 6402 6404 8d02 7d0c 7409 6a0a 7c0a 7c0b  d.d...}.t.j.|.|.
+000005b0: 6702 6402 6404 8d02 7d0a 7c0c 6a0b 6402  g.d.d...}.|.j.d.
+000005c0: 6405 8d01 7d08 7c0a 6a0b 6402 6405 8d01  d...}.|.j.d.d...
+000005d0: 7d0a 7c0a 6a0c 7c08 7c02 3c00 7c00 6a01  }.|.j.|.|.<.|.j.
+000005e0: 0400 6a05 7c05 3700 0200 5f05 740d 7c00  ..j.|.7..._.t.|.
+000005f0: 6a0e 7c02 7c00 6a01 7c00 6a0f 7c00 6a10  j.|.|.j.|.j.|.j.
+00000600: 6406 8d05 7d0d 7c0d 6a11 7c08 7c02 6407  d...}.|.j.|.|.d.
+00000610: 8d02 0100 7c00 6a12 a013 7c0d a101 0100  ....|.j...|.....
+00000620: 714a 6408 5300 2909 7a6a 4669 7420 6d75  qJd.S.).zjFit mu
+00000630: 6c74 6970 6c65 2042 6c75 6543 6173 7420  ltiple BlueCast 
+00000640: 696e 7374 616e 6365 7320 6f6e 2064 6966  instances on dif
+00000650: 6665 7265 6e74 2064 6174 6120 7370 6c69  ferent data spli
+00000660: 7473 2e0a 0a20 2020 2020 2020 2049 6e70  ts...        Inp
+00000670: 7574 2064 6620 6973 2065 7870 6563 7465  ut df is expecte
+00000680: 6420 7468 6520 7461 7267 6574 2063 6f6c  d the target col
+00000690: 756d 6e2e e905 0000 0054 a903 da08 6e5f  umn......T....n_
+000006a0: 7370 6c69 7473 da07 7368 7566 666c 65da  splits..shuffle.
+000006b0: 0c72 616e 646f 6d5f 7374 6174 6529 01da  .random_state)..
+000006c0: 0c69 676e 6f72 655f 696e 6465 7872 1d00  .ignore_indexr..
+000006d0: 0000 a905 7210 0000 00da 0d74 6172 6765  ....r......targe
+000006e0: 745f 636f 6c75 6d6e 7212 0000 0072 1300  t_columnr....r..
+000006f0: 0000 7214 0000 00a9 0172 2600 0000 4e29  ..r......r&...N)
+00000700: 1472 2500 0000 7212 0000 0072 0a00 0000  .r%...r....r....
+00000710: 7211 0000 0072 0800 0000 da13 676c 6f62  r....r......glob
+00000720: 616c 5f72 616e 646f 6d5f 7374 6174 65da  al_random_state.
+00000730: 0965 6e75 6d65 7261 7465 da05 7370 6c69  .enumerate..spli
+00000740: 74da 0469 6c6f 63da 0270 64da 0663 6f6e  t..iloc..pd..con
+00000750: 6361 7472 2200 0000 da06 7661 6c75 6573  catr".....values
+00000760: 7209 0000 0072 1000 0000 7213 0000 0072  r....r....r....r
+00000770: 1400 0000 da03 6669 7472 1500 0000 da06  ......fitr......
+00000780: 6170 7065 6e64 290e 7216 0000 0072 1a00  append).r....r..
+00000790: 0000 7226 0000 0072 2400 0000 7223 0000  ..r&...r$...r#..
+000007a0: 00da 0266 6eda 0774 726e 5f69 6478 da07  ...fn..trn_idx..
+000007b0: 7661 6c5f 6964 78da 0758 5f74 7261 696e  val_idx..X_train
+000007c0: da05 585f 7661 6cda 0779 5f74 7261 696e  ..X_val..y_train
+000007d0: da05 795f 7661 6cda 0778 5f74 7261 696e  ..y_val..x_train
+000007e0: da06 6175 746f 6d6c 7217 0000 0072 1700  ..automlr....r..
+000007f0: 0000 7218 0000 0072 3700 0000 2a00 0000  ..r....r7...*...
+00000800: 7336 0000 0000 0410 0206 0108 0206 0102  s6..............
+00000810: 0102 0102 0106 fd08 061e 0116 0116 0112  ................
+00000820: 0112 020c 010c 010a 0210 0202 0104 0102  ................
+00000830: 0104 0104 0104 fb06 070e 017a 0e42 6c75  ...........z.Blu
+00000840: 6543 6173 7443 562e 6669 7463 0300 0000  eCastCV.fitc....
+00000850: 0000 0000 0000 0000 0d00 0000 0800 0000  ................
+00000860: 4300 0000 73d8 0000 007c 00a0 007c 017c  C...s....|...|.|
+00000870: 02a1 025c 027d 037d 047c 006a 0173 1e74  ...\.}.}.|.j.s.t
+00000880: 0283 007c 005f 017c 006a 0373 3874 0464  ...|._.|.j.s8t.d
+00000890: 0164 027c 006a 016a 0564 038d 037c 005f  .d.|.j.j.d...|._
+000008a0: 0374 067c 006a 03a0 077c 037c 04a1 0283  .t.|.j...|.|....
+000008b0: 0144 005d 885c 027d 055c 027d 067d 077c  .D.].\.}.\.}.}.|
+000008c0: 036a 087c 0619 007c 036a 087c 0719 0002  .j.|...|.j.|....
+000008d0: 007d 087d 097c 046a 087c 0619 007c 046a  .}.}.|.j.|...|.j
+000008e0: 087c 0719 0002 007d 0a7d 0b7c 0a7c 087c  .|.....}.}.|.|.|
+000008f0: 023c 007c 006a 0104 006a 057c 0537 0002  .<.|.j...j.|.7..
+00000900: 005f 0574 097c 006a 0a7c 027c 006a 017c  ._.t.|.j.|.|.j.|
+00000910: 006a 0b7c 006a 0c64 048d 057d 0c7c 0c6a  .j.|.j.d...}.|.j
+00000920: 0d7c 087c 097c 0b7c 0264 058d 0401 007c  .|.|.|.|.d.....|
+00000930: 006a 0ea0 0f7c 0ca1 0101 0071 4a64 0653  .j...|.....qJd.S
+00000940: 0029 077a af46 6974 206d 756c 7469 706c  .).z.Fit multipl
+00000950: 6520 426c 7565 4361 7374 2069 6e73 7461  e BlueCast insta
+00000960: 6e63 6573 206f 6e20 6469 6666 6572 656e  nces on differen
+00000970: 7420 6461 7461 2073 706c 6974 732e 0a0a  t data splits...
+00000980: 2020 2020 2020 2020 496e 7075 7420 6466          Input df
+00000990: 2069 7320 6578 7065 6374 6564 2074 6865   is expected the
+000009a0: 2074 6172 6765 7420 636f 6c75 6d6e 2e20   target column. 
+000009b0: 4576 616c 7561 7469 6f6e 2069 7320 6578  Evaluation is ex
+000009c0: 6563 7574 6564 206f 6e20 6f75 742d 6f66  ecuted on out-of
+000009d0: 2d66 6f6c 6420 6461 7461 7365 740a 2020  -fold dataset.  
+000009e0: 2020 2020 2020 696e 2065 6163 6820 7370        in each sp
+000009f0: 6c69 742e 7227 0000 0054 7228 0000 0072  lit.r'...Tr(...r
+00000a00: 2d00 0000 722f 0000 004e 2910 7225 0000  -...r/...N).r%..
+00000a10: 0072 1200 0000 720a 0000 0072 1100 0000  .r....r....r....
+00000a20: 7208 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
+00000a30: 3200 0000 7233 0000 0072 0900 0000 7210  2...r3...r....r.
+00000a40: 0000 0072 1300 0000 7214 0000 00da 0866  ...r....r......f
+00000a50: 6974 5f65 7661 6c72 1500 0000 7238 0000  it_evalr....r8..
+00000a60: 0029 0d72 1600 0000 721a 0000 0072 2600  .).r....r....r&.
+00000a70: 0000 7224 0000 0072 2300 0000 7239 0000  ..r$...r#...r9..
+00000a80: 0072 3a00 0000 723b 0000 0072 3c00 0000  .r:...r;...r<...
+00000a90: 723d 0000 0072 3e00 0000 723f 0000 0072  r=...r>...r?...r
+00000aa0: 4100 0000 7217 0000 0072 1700 0000 7218  A...r....r....r.
+00000ab0: 0000 0072 4200 0000 5000 0000 732e 0000  ...rB...P...s...
+00000ac0: 0000 0510 0206 0108 0206 0102 0102 0102  ................
+00000ad0: 0106 fd08 061e 0116 0116 0208 0210 0202  ................
+00000ae0: 0104 0102 0104 0104 0104 fb06 0712 017a  ...............z
+00000af0: 1342 6c75 6543 6173 7443 562e 6669 745f  .BlueCastCV.fit_
+00000b00: 6576 616c 4629 0372 1a00 0000 da17 7265  evalF).r......re
+00000b10: 7475 726e 5f73 7562 5f6d 6f64 656c 735f  turn_sub_models_
+00000b20: 7072 6564 7372 1c00 0000 6303 0000 0000  predsr....c.....
+00000b30: 0000 0000 0000 000a 0000 0006 0000 0043  ...............C
+00000b40: 0000 0073 de00 0000 7c01 6a00 7d03 6700  ...s....|.j.}.g.
+00000b50: 7d04 6700 7d05 7401 7c00 6a02 8301 4400  }.g.}.t.|.j...D.
+00000b60: 5d60 5c02 7d06 7d07 7c07 a003 7c01 6a04  ]`\.}.}.|...|.j.
+00000b70: 6401 6401 8502 7c03 6602 1900 a101 5c02  d.d...|.f.....\.
+00000b80: 7d08 7d09 7c08 7c01 6402 7c06 9b00 9d02  }.}.|.|.d.|.....
+00000b90: 3c00 7c09 7c01 6403 7c06 9b00 9d02 3c00  <.|.|.d.|.....<.
+00000ba0: 7c04 a005 6402 7c06 9b00 9d02 a101 0100  |...d.|.........
+00000bb0: 7c05 a005 6403 7c06 9b00 9d02 a101 0100  |...d.|.........
+00000bc0: 7118 7c02 72a2 7c01 6a04 6401 6401 8502  q.|.r.|.j.d.d...
+00000bd0: 7c04 6602 1900 7c01 6a04 6401 6401 8502  |.f...|.j.d.d...
+00000be0: 7c05 6602 1900 6602 5300 7c01 6a04 6401  |.f...f.S.|.j.d.
+00000bf0: 6401 8502 7c04 6602 1900 6a06 6404 6405  d...|.f...j.d.d.
+00000c00: 8d01 7c01 6a04 6401 6401 8502 7c04 6602  ..|.j.d.d...|.f.
+00000c10: 1900 6a06 6404 6405 8d01 6406 6b04 6602  ..j.d.d...d.k.f.
+00000c20: 5300 6401 5300 2907 7a40 5072 6564 6963  S.d.S.).z@Predic
+00000c30: 7420 6f6e 2075 6e73 6565 6e20 6461 7461  t on unseen data
+00000c40: 2075 7369 6e67 206d 756c 7469 706c 6520   using multiple 
+00000c50: 7472 6169 6e65 6420 426c 7565 4361 7374  trained BlueCast
+00000c60: 2069 6e73 7461 6e63 6573 4e5a 0670 726f   instancesNZ.pro
+00000c70: 6261 5fda 0863 6c61 7373 6573 5f72 1f00  ba_..classes_r..
+00000c80: 0000 7220 0000 0067 0000 0000 0000 e03f  ..r ...g.......?
+00000c90: 2907 da07 636f 6c75 6d6e 7372 3100 0000  )...columnsr1...
+00000ca0: 7215 0000 00da 0770 7265 6469 6374 da03  r......predict..
+00000cb0: 6c6f 6372 3800 0000 da04 6d65 616e 290a  locr8.....mean).
+00000cc0: 7216 0000 0072 1a00 0000 7243 0000 00da  r....r....rC....
+00000cd0: 076f 725f 636f 6c73 5a09 7072 6f62 5f63  .or_colsZ.prob_c
+00000ce0: 6f6c 735a 0a63 6c61 7373 5f63 6f6c 7372  olsZ.class_colsr
+00000cf0: 3900 0000 da08 7069 7065 6c69 6e65 da07  9.....pipeline..
+00000d00: 795f 7072 6f62 73da 0979 5f63 6c61 7373  y_probs..y_class
+00000d10: 6573 7217 0000 0072 1700 0000 7218 0000  esr....r....r...
+00000d20: 0072 4600 0000 7300 0000 731c 0000 0000  .rF...s...s.....
+00000d30: 0406 0104 0104 0112 011c 010e 010e 0110  ................
+00000d40: 0112 0204 0124 0318 011c fe7a 1242 6c75  .....$.....z.Blu
+00000d50: 6543 6173 7443 562e 7072 6564 6963 7429  eCastCV.predict)
+00000d60: 0572 0e00 0000 4e4e 4e4e 2901 4629 16da  .r....NNNN).F)..
+00000d70: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000d80: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000d90: 655f 5fda 075f 5f64 6f63 5f5f 7204 0000  e__..__doc__r...
+00000da0: 0072 0500 0000 7202 0000 0072 0a00 0000  .r....r....r....
+00000db0: 720c 0000 0072 0b00 0000 7219 0000 0072  r....r....r....r
+00000dc0: 3400 0000 da09 4461 7461 4672 616d 65da  4.....DataFrame.
+00000dd0: 0373 7472 7206 0000 00da 0653 6572 6965  .strr......Serie
+00000de0: 7372 2500 0000 7237 0000 0072 4200 0000  sr%...r7...rB...
+00000df0: da04 626f 6f6c 7207 0000 0072 4600 0000  ..boolr....rF...
+00000e00: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00000e10: 1800 0000 720d 0000 000e 0000 0073 3200  ....r........s2.
+00000e20: 0000 0801 0406 0001 0001 0001 0001 00fa  ................
+00000e30: 0202 0601 0601 0601 0601 06fa 0c10 0400  ................
+00000e40: 0201 0efe 0c08 1426 1424 00ff 0201 0400  .......&.$......
+00000e50: 0201 22fe 720d 0000 0029 12da 0674 7970  ..".r....)...typ
+00000e60: 696e 6772 0200 0000 7203 0000 0072 0400  ingr....r....r..
+00000e70: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
+00000e80: 00da 0670 616e 6461 7372 3400 0000 da17  ...pandasr4.....
+00000e90: 736b 6c65 6172 6e2e 6d6f 6465 6c5f 7365  sklearn.model_se
+00000ea0: 6c65 6374 696f 6e72 0800 0000 da18 626c  lectionr......bl
+00000eb0: 7565 6361 7374 2e62 6c75 6570 7269 6e74  uecast.blueprint
+00000ec0: 732e 6361 7374 7209 0000 00da 1f62 6c75  s.castr......blu
+00000ed0: 6563 6173 742e 636f 6e66 6967 2e74 7261  ecast.config.tra
+00000ee0: 696e 696e 675f 636f 6e66 6967 720a 0000  ining_configr...
+00000ef0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000f00: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00000f10: 1800 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000f20: 0000 730a 0000 0020 0208 010c 020c 0114  ..s.... ........
+00000f30: 07                                       .
```

### Comparing `bluecast-0.8/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc` & `bluecast-0.9/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jul  4 07:46:35 2023 UTC, .py size: 5013 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,244 +1,273 @@
-00000000: 550d 0d0a 0000 0000 5bce a364 9513 0000  U.......[..d....
+00000000: 6f0d 0d0a 0000 0000 ab08 a564 7f17 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
+00000020: 0003 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 5a08 6400 6403 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  d.l.m.Z.m.Z.m.Z.
-00000080: 0100 4700 6406 6407 8400 6407 8302 5a11  ..G.d.d...d...Z.
-00000090: 6402 5300 2908 e900 0000 0029 06da 0341  d.S.)......)...A
-000000a0: 6e79 da04 4c69 7374 da07 4c69 7465 7261  ny..List..Litera
-000000b0: 6cda 084f 7074 696f 6e61 6cda 0554 7570  l..Optional..Tup
-000000c0: 6c65 da05 556e 696f 6e4e 2901 da0f 5374  le..UnionN)...St
-000000d0: 7261 7469 6669 6564 4b46 6f6c 6429 01da  ratifiedKFold)..
-000000e0: 0842 6c75 6543 6173 7429 03da 0e54 7261  .BlueCast)...Tra
-000000f0: 696e 696e 6743 6f6e 6669 67da 1758 6762  iningConfig..Xgb
-00000100: 6f6f 7374 4669 6e61 6c50 6172 616d 436f  oostFinalParamCo
-00000110: 6e66 6967 da17 5867 626f 6f73 7454 756e  nfig..XgboostTun
-00000120: 6550 6172 616d 7343 6f6e 6669 6763 0000  eParamsConfigc..
-00000130: 0000 0000 0000 0000 0000 0000 0000 0800  ................
-00000140: 0000 4000 0000 73ba 0000 0065 005a 0164  ..@...s....e.Z.d
-00000150: 005a 0264 015a 0364 1465 0464 0419 0065  .Z.d.Z.d.e.d...e
-00000160: 0565 0619 0065 0565 0719 0065 0565 0819  .e...e.e...e.e..
-00000170: 0065 0565 0919 0064 059c 0564 0664 0784  .e.e...d...d.d..
-00000180: 055a 0a65 0b6a 0c65 0d65 0e65 0b6a 0c65  .Z.e.j.e.e.e.j.e
-00000190: 0b6a 0f66 0219 0064 089c 0364 0964 0a84  .j.f...d...d.d..
-000001a0: 045a 1065 0b6a 0c65 0d64 0364 0b9c 0364  .Z.e.j.e.d.d...d
-000001b0: 0c64 0d84 045a 1165 0b6a 0c65 0d64 0364  .d...Z.e.j.e.d.d
-000001c0: 0b9c 0364 0e64 0f84 045a 1264 1565 0b6a  ...d.d...Z.d.e.j
-000001d0: 0c65 1365 0e65 1465 0b6a 0c65 0b6a 0f66  .e.e.e.e.j.e.j.f
-000001e0: 0219 0065 1465 0b6a 0c65 0b6a 0f66 0219  ...e.e.j.e.j.f..
-000001f0: 0066 0219 0064 119c 0364 1264 1384 055a  .f...d...d.d...Z
-00000200: 1564 0353 0029 16da 0a42 6c75 6543 6173  .d.S.)...BlueCas
-00000210: 7443 567a 6157 7261 7070 6572 2074 6f20  tCVzaWrapper to 
-00000220: 7472 6169 6e20 616e 6420 7072 6564 6963  train and predic
-00000230: 7420 6d75 6c74 6970 6c65 2062 6c75 6543  t multiple blueC
-00000240: 6173 7420 696e 7473 616e 6365 732e 0a0a  ast intsances...
-00000250: 2020 2020 4120 6375 7374 6f6d 2073 706c      A custom spl
-00000260: 6974 7465 7220 6361 6e20 6265 2070 726f  itter can be pro
-00000270: 7669 6465 642e da06 6269 6e61 7279 4e29  vided...binaryN)
-00000280: 0272 0e00 0000 da0a 6d75 6c74 6963 6c61  .r......multicla
-00000290: 7373 2905 da0d 636c 6173 735f 7072 6f62  ss)...class_prob
-000002a0: 6c65 6dda 0a73 7472 6174 6966 6965 72da  lem..stratifier.
-000002b0: 0d63 6f6e 665f 7472 6169 6e69 6e67 da0c  .conf_training..
-000002c0: 636f 6e66 5f78 6762 6f6f 7374 da13 636f  conf_xgboost..co
-000002d0: 6e66 5f70 6172 616d 735f 7867 626f 6f73  nf_params_xgboos
-000002e0: 7463 0600 0000 0000 0000 0000 0000 0600  tc..............
-000002f0: 0000 0200 0000 4300 0000 7328 0000 007c  ......C...s(...|
-00000300: 017c 005f 007c 047c 005f 017c 037c 005f  .|._.|.|._.|.|._
-00000310: 027c 057c 005f 0367 007c 005f 047c 027c  .|.|._.g.|._.|.|
-00000320: 005f 0564 0053 0029 014e 2906 7210 0000  ._.d.S.).N).r...
-00000330: 0072 1300 0000 7212 0000 0072 1400 0000  .r....r....r....
-00000340: da0f 626c 7565 6361 7374 5f6d 6f64 656c  ..bluecast_model
-00000350: 7372 1100 0000 2906 da04 7365 6c66 7210  sr....)...selfr.
-00000360: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00000370: 0000 7214 0000 00a9 0072 1700 0000 fa41  ..r......r.....A
-00000380: 2f68 6f6d 652f 7468 6f6d 6173 2f49 6465  /home/thomas/Ide
-00000390: 6150 726f 6a65 6374 732f 426c 7565 4361  aProjects/BlueCa
-000003a0: 7374 2f62 6c75 6563 6173 742f 626c 7565  st/bluecast/blue
-000003b0: 7072 696e 7473 2f63 6173 745f 6376 2e70  prints/cast_cv.p
-000003c0: 79da 085f 5f69 6e69 745f 5f13 0000 0073  y..__init__....s
-000003d0: 0c00 0000 0008 0601 0601 0601 0601 0601  ................
-000003e0: 7a13 426c 7565 4361 7374 4356 2e5f 5f69  z.BlueCastCV.__i
-000003f0: 6e69 745f 5f29 03da 0264 66da 0674 6172  nit__)...df..tar
-00000400: 6765 74da 0672 6574 7572 6e63 0300 0000  get..returnc....
-00000410: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00000420: 4300 0000 732a 0000 007c 016a 0064 0164  C...s*...|.j.d.d
-00000430: 028d 017d 017c 017c 0219 007d 037c 016a  ...}.|.|...}.|.j
-00000440: 017c 0264 0364 048d 027d 047c 047c 0366  .|.d.d...}.|.|.f
-00000450: 0253 0029 054e 54a9 01da 0464 726f 70e9  .S.).NT....drop.
-00000460: 0100 0000 a901 da04 6178 6973 2902 da0b  ........axis)...
-00000470: 7265 7365 745f 696e 6465 7872 1e00 0000  reset_indexr....
-00000480: 2905 7216 0000 0072 1a00 0000 721b 0000  ).r....r....r...
-00000490: 00da 0179 da01 5872 1700 0000 7217 0000  ...y..Xr....r...
-000004a0: 0072 1800 0000 da0c 7072 6570 6172 655f  .r......prepare_
-000004b0: 6461 7461 2200 0000 7308 0000 0000 030c  data"...s.......
-000004c0: 0108 010e 017a 1742 6c75 6543 6173 7443  .....z.BlueCastC
-000004d0: 562e 7072 6570 6172 655f 6461 7461 2903  V.prepare_data).
-000004e0: 721a 0000 00da 0a74 6172 6765 745f 636f  r......target_co
-000004f0: 6c72 1c00 0000 6303 0000 0000 0000 0000  lr....c.........
-00000500: 0000 000e 0000 0008 0000 0043 0000 0073  ...........C...s
-00000510: 1201 0000 7c00 a000 7c01 7c02 a102 5c02  ....|...|.|...\.
-00000520: 7d03 7d04 7c00 6a01 731e 7402 8300 7c00  }.}.|.j.s.t...|.
-00000530: 5f01 7c00 6a03 7338 7404 6401 6402 7c00  _.|.j.s8t.d.d.|.
-00000540: 6a01 6a05 6403 8d03 7c00 5f03 7406 7c00  j.j.d...|._.t.|.
-00000550: 6a03 a007 7c03 7c04 a102 8301 4400 5dc2  j...|.|.....D.].
-00000560: 5c02 7d05 5c02 7d06 7d07 7c03 6a08 7c06  \.}.\.}.}.|.j.|.
-00000570: 1900 7c03 6a08 7c07 1900 0200 7d08 7d09  ..|.j.|.....}.}.
-00000580: 7c04 6a08 7c06 1900 7c04 6a08 7c07 1900  |.j.|...|.j.|...
-00000590: 0200 7d0a 7d0b 7409 6a0a 7c08 7c09 6702  ..}.}.t.j.|.|.g.
-000005a0: 6402 6404 8d02 7d0c 7409 6a0a 7c0a 7c0b  d.d...}.t.j.|.|.
-000005b0: 6702 6402 6404 8d02 7d0a 7c0c 6a0b 6402  g.d.d...}.|.j.d.
-000005c0: 6405 8d01 7d08 7c0a 6a0b 6402 6405 8d01  d...}.|.j.d.d...
-000005d0: 7d0a 7c0a 6a0c 7c08 7c02 3c00 7c00 6a01  }.|.j.|.|.<.|.j.
-000005e0: 0400 6a05 7c05 3700 0200 5f05 740d 7c00  ..j.|.7..._.t.|.
-000005f0: 6a0e 7c02 7c00 6a01 7c00 6a0f 7c00 6a10  j.|.|.j.|.j.|.j.
-00000600: 6406 8d05 7d0d 7c0d 6a11 7c08 7c02 6407  d...}.|.j.|.|.d.
-00000610: 8d02 0100 7c00 6a12 a013 7c0d a101 0100  ....|.j...|.....
-00000620: 714a 6408 5300 2909 7a6a 4669 7420 6d75  qJd.S.).zjFit mu
-00000630: 6c74 6970 6c65 2042 6c75 6543 6173 7420  ltiple BlueCast 
-00000640: 696e 7374 616e 6365 7320 6f6e 2064 6966  instances on dif
-00000650: 6665 7265 6e74 2064 6174 6120 7370 6c69  ferent data spli
-00000660: 7473 2e0a 0a20 2020 2020 2020 2049 6e70  ts...        Inp
-00000670: 7574 2064 6620 6973 2065 7870 6563 7465  ut df is expecte
-00000680: 6420 7468 6520 7461 7267 6574 2063 6f6c  d the target col
-00000690: 756d 6e2e e905 0000 0054 a903 da08 6e5f  umn......T....n_
-000006a0: 7370 6c69 7473 da07 7368 7566 666c 65da  splits..shuffle.
-000006b0: 0c72 616e 646f 6d5f 7374 6174 6529 01da  .random_state)..
-000006c0: 0c69 676e 6f72 655f 696e 6465 7872 1d00  .ignore_indexr..
-000006d0: 0000 a905 7210 0000 00da 0d74 6172 6765  ....r......targe
-000006e0: 745f 636f 6c75 6d6e 7212 0000 0072 1300  t_columnr....r..
-000006f0: 0000 7214 0000 00a9 0172 2600 0000 4e29  ..r......r&...N)
-00000700: 1472 2500 0000 7212 0000 0072 0a00 0000  .r%...r....r....
-00000710: 7211 0000 0072 0800 0000 da13 676c 6f62  r....r......glob
-00000720: 616c 5f72 616e 646f 6d5f 7374 6174 65da  al_random_state.
-00000730: 0965 6e75 6d65 7261 7465 da05 7370 6c69  .enumerate..spli
-00000740: 74da 0469 6c6f 63da 0270 64da 0663 6f6e  t..iloc..pd..con
-00000750: 6361 7472 2200 0000 da06 7661 6c75 6573  catr".....values
-00000760: 7209 0000 0072 1000 0000 7213 0000 0072  r....r....r....r
-00000770: 1400 0000 da03 6669 7472 1500 0000 da06  ......fitr......
-00000780: 6170 7065 6e64 290e 7216 0000 0072 1a00  append).r....r..
-00000790: 0000 7226 0000 0072 2400 0000 7223 0000  ..r&...r$...r#..
-000007a0: 00da 0266 6eda 0774 726e 5f69 6478 da07  ...fn..trn_idx..
-000007b0: 7661 6c5f 6964 78da 0758 5f74 7261 696e  val_idx..X_train
-000007c0: da05 585f 7661 6cda 0779 5f74 7261 696e  ..X_val..y_train
-000007d0: da05 795f 7661 6cda 0778 5f74 7261 696e  ..y_val..x_train
-000007e0: da06 6175 746f 6d6c 7217 0000 0072 1700  ..automlr....r..
-000007f0: 0000 7218 0000 0072 3700 0000 2a00 0000  ..r....r7...*...
-00000800: 7336 0000 0000 0410 0206 0108 0206 0102  s6..............
-00000810: 0102 0102 0106 fd08 061e 0116 0116 0112  ................
-00000820: 0112 020c 010c 010a 0210 0202 0104 0102  ................
-00000830: 0104 0104 0104 fb06 070e 017a 0e42 6c75  ...........z.Blu
-00000840: 6543 6173 7443 562e 6669 7463 0300 0000  eCastCV.fitc....
-00000850: 0000 0000 0000 0000 0d00 0000 0800 0000  ................
-00000860: 4300 0000 73d8 0000 007c 00a0 007c 017c  C...s....|...|.|
-00000870: 02a1 025c 027d 037d 047c 006a 0173 1e74  ...\.}.}.|.j.s.t
-00000880: 0283 007c 005f 017c 006a 0373 3874 0464  ...|._.|.j.s8t.d
-00000890: 0164 027c 006a 016a 0564 038d 037c 005f  .d.|.j.j.d...|._
-000008a0: 0374 067c 006a 03a0 077c 037c 04a1 0283  .t.|.j...|.|....
-000008b0: 0144 005d 885c 027d 055c 027d 067d 077c  .D.].\.}.\.}.}.|
-000008c0: 036a 087c 0619 007c 036a 087c 0719 0002  .j.|...|.j.|....
-000008d0: 007d 087d 097c 046a 087c 0619 007c 046a  .}.}.|.j.|...|.j
-000008e0: 087c 0719 0002 007d 0a7d 0b7c 0a7c 087c  .|.....}.}.|.|.|
-000008f0: 023c 007c 006a 0104 006a 057c 0537 0002  .<.|.j...j.|.7..
-00000900: 005f 0574 097c 006a 0a7c 027c 006a 017c  ._.t.|.j.|.|.j.|
-00000910: 006a 0b7c 006a 0c64 048d 057d 0c7c 0c6a  .j.|.j.d...}.|.j
-00000920: 0d7c 087c 097c 0b7c 0264 058d 0401 007c  .|.|.|.|.d.....|
-00000930: 006a 0ea0 0f7c 0ca1 0101 0071 4a64 0653  .j...|.....qJd.S
-00000940: 0029 077a af46 6974 206d 756c 7469 706c  .).z.Fit multipl
-00000950: 6520 426c 7565 4361 7374 2069 6e73 7461  e BlueCast insta
-00000960: 6e63 6573 206f 6e20 6469 6666 6572 656e  nces on differen
-00000970: 7420 6461 7461 2073 706c 6974 732e 0a0a  t data splits...
-00000980: 2020 2020 2020 2020 496e 7075 7420 6466          Input df
-00000990: 2069 7320 6578 7065 6374 6564 2074 6865   is expected the
-000009a0: 2074 6172 6765 7420 636f 6c75 6d6e 2e20   target column. 
-000009b0: 4576 616c 7561 7469 6f6e 2069 7320 6578  Evaluation is ex
-000009c0: 6563 7574 6564 206f 6e20 6f75 742d 6f66  ecuted on out-of
-000009d0: 2d66 6f6c 6420 6461 7461 7365 740a 2020  -fold dataset.  
-000009e0: 2020 2020 2020 696e 2065 6163 6820 7370        in each sp
-000009f0: 6c69 742e 7227 0000 0054 7228 0000 0072  lit.r'...Tr(...r
-00000a00: 2d00 0000 722f 0000 004e 2910 7225 0000  -...r/...N).r%..
-00000a10: 0072 1200 0000 720a 0000 0072 1100 0000  .r....r....r....
-00000a20: 7208 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
-00000a30: 3200 0000 7233 0000 0072 0900 0000 7210  2...r3...r....r.
-00000a40: 0000 0072 1300 0000 7214 0000 00da 0866  ...r....r......f
-00000a50: 6974 5f65 7661 6c72 1500 0000 7238 0000  it_evalr....r8..
-00000a60: 0029 0d72 1600 0000 721a 0000 0072 2600  .).r....r....r&.
-00000a70: 0000 7224 0000 0072 2300 0000 7239 0000  ..r$...r#...r9..
-00000a80: 0072 3a00 0000 723b 0000 0072 3c00 0000  .r:...r;...r<...
-00000a90: 723d 0000 0072 3e00 0000 723f 0000 0072  r=...r>...r?...r
-00000aa0: 4100 0000 7217 0000 0072 1700 0000 7218  A...r....r....r.
-00000ab0: 0000 0072 4200 0000 5000 0000 732e 0000  ...rB...P...s...
-00000ac0: 0000 0510 0206 0108 0206 0102 0102 0102  ................
-00000ad0: 0106 fd08 061e 0116 0116 0208 0210 0202  ................
-00000ae0: 0104 0102 0104 0104 0104 fb06 0712 017a  ...............z
-00000af0: 1342 6c75 6543 6173 7443 562e 6669 745f  .BlueCastCV.fit_
-00000b00: 6576 616c 4629 0372 1a00 0000 da17 7265  evalF).r......re
-00000b10: 7475 726e 5f73 7562 5f6d 6f64 656c 735f  turn_sub_models_
-00000b20: 7072 6564 7372 1c00 0000 6303 0000 0000  predsr....c.....
-00000b30: 0000 0000 0000 000a 0000 0006 0000 0043  ...............C
-00000b40: 0000 0073 de00 0000 7c01 6a00 7d03 6700  ...s....|.j.}.g.
-00000b50: 7d04 6700 7d05 7401 7c00 6a02 8301 4400  }.g.}.t.|.j...D.
-00000b60: 5d60 5c02 7d06 7d07 7c07 a003 7c01 6a04  ]`\.}.}.|...|.j.
-00000b70: 6401 6401 8502 7c03 6602 1900 a101 5c02  d.d...|.f.....\.
-00000b80: 7d08 7d09 7c08 7c01 6402 7c06 9b00 9d02  }.}.|.|.d.|.....
-00000b90: 3c00 7c09 7c01 6403 7c06 9b00 9d02 3c00  <.|.|.d.|.....<.
-00000ba0: 7c04 a005 6402 7c06 9b00 9d02 a101 0100  |...d.|.........
-00000bb0: 7c05 a005 6403 7c06 9b00 9d02 a101 0100  |...d.|.........
-00000bc0: 7118 7c02 72a2 7c01 6a04 6401 6401 8502  q.|.r.|.j.d.d...
-00000bd0: 7c04 6602 1900 7c01 6a04 6401 6401 8502  |.f...|.j.d.d...
-00000be0: 7c05 6602 1900 6602 5300 7c01 6a04 6401  |.f...f.S.|.j.d.
-00000bf0: 6401 8502 7c04 6602 1900 6a06 6404 6405  d...|.f...j.d.d.
-00000c00: 8d01 7c01 6a04 6401 6401 8502 7c04 6602  ..|.j.d.d...|.f.
-00000c10: 1900 6a06 6404 6405 8d01 6406 6b04 6602  ..j.d.d...d.k.f.
-00000c20: 5300 6401 5300 2907 7a40 5072 6564 6963  S.d.S.).z@Predic
-00000c30: 7420 6f6e 2075 6e73 6565 6e20 6461 7461  t on unseen data
-00000c40: 2075 7369 6e67 206d 756c 7469 706c 6520   using multiple 
-00000c50: 7472 6169 6e65 6420 426c 7565 4361 7374  trained BlueCast
-00000c60: 2069 6e73 7461 6e63 6573 4e5a 0670 726f   instancesNZ.pro
-00000c70: 6261 5fda 0863 6c61 7373 6573 5f72 1f00  ba_..classes_r..
-00000c80: 0000 7220 0000 0067 0000 0000 0000 e03f  ..r ...g.......?
-00000c90: 2907 da07 636f 6c75 6d6e 7372 3100 0000  )...columnsr1...
-00000ca0: 7215 0000 00da 0770 7265 6469 6374 da03  r......predict..
-00000cb0: 6c6f 6372 3800 0000 da04 6d65 616e 290a  locr8.....mean).
-00000cc0: 7216 0000 0072 1a00 0000 7243 0000 00da  r....r....rC....
-00000cd0: 076f 725f 636f 6c73 5a09 7072 6f62 5f63  .or_colsZ.prob_c
-00000ce0: 6f6c 735a 0a63 6c61 7373 5f63 6f6c 7372  olsZ.class_colsr
-00000cf0: 3900 0000 da08 7069 7065 6c69 6e65 da07  9.....pipeline..
-00000d00: 795f 7072 6f62 73da 0979 5f63 6c61 7373  y_probs..y_class
-00000d10: 6573 7217 0000 0072 1700 0000 7218 0000  esr....r....r...
-00000d20: 0072 4600 0000 7300 0000 731c 0000 0000  .rF...s...s.....
-00000d30: 0406 0104 0104 0112 011c 010e 010e 0110  ................
-00000d40: 0112 0204 0124 0318 011c fe7a 1242 6c75  .....$.....z.Blu
-00000d50: 6543 6173 7443 562e 7072 6564 6963 7429  eCastCV.predict)
-00000d60: 0572 0e00 0000 4e4e 4e4e 2901 4629 16da  .r....NNNN).F)..
-00000d70: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000d80: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000d90: 655f 5fda 075f 5f64 6f63 5f5f 7204 0000  e__..__doc__r...
-00000da0: 0072 0500 0000 7202 0000 0072 0a00 0000  .r....r....r....
-00000db0: 720c 0000 0072 0b00 0000 7219 0000 0072  r....r....r....r
-00000dc0: 3400 0000 da09 4461 7461 4672 616d 65da  4.....DataFrame.
-00000dd0: 0373 7472 7206 0000 00da 0653 6572 6965  .strr......Serie
-00000de0: 7372 2500 0000 7237 0000 0072 4200 0000  sr%...r7...rB...
-00000df0: da04 626f 6f6c 7207 0000 0072 4600 0000  ..boolr....rF...
-00000e00: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-00000e10: 1800 0000 720d 0000 000e 0000 0073 3200  ....r........s2.
-00000e20: 0000 0801 0406 0001 0001 0001 0001 00fa  ................
-00000e30: 0202 0601 0601 0601 0601 06fa 0c10 0400  ................
-00000e40: 0201 0efe 0c08 1426 1424 00ff 0201 0400  .......&.$......
-00000e50: 0201 22fe 720d 0000 0029 12da 0674 7970  ..".r....)...typ
-00000e60: 696e 6772 0200 0000 7203 0000 0072 0400  ingr....r....r..
-00000e70: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
-00000e80: 00da 0670 616e 6461 7372 3400 0000 da17  ...pandasr4.....
-00000e90: 736b 6c65 6172 6e2e 6d6f 6465 6c5f 7365  sklearn.model_se
-00000ea0: 6c65 6374 696f 6e72 0800 0000 da18 626c  lectionr......bl
-00000eb0: 7565 6361 7374 2e62 6c75 6570 7269 6e74  uecast.blueprint
-00000ec0: 732e 6361 7374 7209 0000 00da 1f62 6c75  s.castr......blu
-00000ed0: 6563 6173 742e 636f 6e66 6967 2e74 7261  ecast.config.tra
-00000ee0: 696e 696e 675f 636f 6e66 6967 720a 0000  ining_configr...
-00000ef0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000f00: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-00000f10: 1800 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000f20: 0000 730a 0000 0020 0208 010c 020c 0114  ..s.... ........
-00000f30: 07                                       .
+00000080: 0100 6400 6406 6c11 6d12 5a12 0100 6400  ..d.d.l.m.Z...d.
+00000090: 6407 6c13 6d14 5a14 0100 4700 6408 6409  d.l.m.Z...G.d.d.
+000000a0: 8400 6409 8302 5a15 6402 5300 290a e900  ..d...Z.d.S.)...
+000000b0: 0000 0029 06da 0341 6e79 da04 4c69 7374  ...)...Any..List
+000000c0: da07 4c69 7465 7261 6cda 084f 7074 696f  ..Literal..Optio
+000000d0: 6e61 6cda 0554 7570 6c65 da05 556e 696f  nal..Tuple..Unio
+000000e0: 6e4e 2901 da0f 5374 7261 7469 6669 6564  nN)...Stratified
+000000f0: 4b46 6f6c 6429 01da 0842 6c75 6543 6173  KFold)...BlueCas
+00000100: 7429 03da 0e54 7261 696e 696e 6743 6f6e  t)...TrainingCon
+00000110: 6669 67da 1758 6762 6f6f 7374 4669 6e61  fig..XgboostFina
+00000120: 6c50 6172 616d 436f 6e66 6967 da17 5867  lParamConfig..Xg
+00000130: 626f 6f73 7454 756e 6550 6172 616d 7343  boostTuneParamsC
+00000140: 6f6e 6669 6729 01da 1343 7573 746f 6d50  onfig)...CustomP
+00000150: 7265 7072 6f63 6573 7369 6e67 2901 da0d  reprocessing)...
+00000160: 5246 4543 5653 656c 6563 746f 7263 0000  RFECVSelectorc..
+00000170: 0000 0000 0000 0000 0000 0000 0000 1400  ................
+00000180: 0000 4000 0000 7304 0100 0065 005a 0164  ..@...s....e.Z.d
+00000190: 005a 0264 015a 0309 0209 0309 0309 0309  .Z.d.Z..........
+000001a0: 0309 0309 0309 0364 1d64 0465 0464 0519  .......d.d.e.d..
+000001b0: 0064 0665 0565 0619 0064 0765 0565 0719  .d.e.e...d.e.e..
+000001c0: 0064 0865 0565 0819 0064 0965 0565 0919  .d.e.e...d.e.e..
+000001d0: 0064 0a65 0565 0a19 0064 0b65 0565 0a19  .d.e.e...d.e.e..
+000001e0: 0064 0c65 0565 0b65 0c65 0a66 0219 0019  .d.e.e.e.e.f....
+000001f0: 0066 1064 0d64 0e84 055a 0d64 0f65 0e6a  .f.d.d...Z.d.e.j
+00000200: 0f64 1065 1064 1165 1165 0e6a 0f65 0e6a  .d.e.d.e.e.j.e.j
+00000210: 1266 0219 0066 0664 1264 1384 045a 1364  .f...f.d.d...Z.d
+00000220: 0f65 0e6a 0f64 1465 1064 1164 0366 0664  .e.j.d.e.d.d.f.d
+00000230: 1564 1684 045a 1464 0f65 0e6a 0f64 1465  .d...Z.d.e.j.d.e
+00000240: 1064 1164 0366 0664 1764 1884 045a 1509  .d.d.f.d.d...Z..
+00000250: 1964 1e64 0f65 0e6a 0f64 1a65 1664 1165  .d.d.e.j.d.e.d.e
+00000260: 1165 0b65 0e6a 0f65 0e6a 1266 0219 0065  .e.e.j.e.j.f...e
+00000270: 0b65 0e6a 0f65 0e6a 1266 0219 0066 0219  .e.j.e.j.f...f..
+00000280: 0066 0664 1b64 1c84 055a 1764 0353 0029  .f.d.d...Z.d.S.)
+00000290: 1fda 0a42 6c75 6543 6173 7443 567a 6157  ...BlueCastCVzaW
+000002a0: 7261 7070 6572 2074 6f20 7472 6169 6e20  rapper to train 
+000002b0: 616e 6420 7072 6564 6963 7420 6d75 6c74  and predict mult
+000002c0: 6970 6c65 2062 6c75 6543 6173 7420 696e  iple blueCast in
+000002d0: 7473 616e 6365 732e 0a0a 2020 2020 4120  tsances...    A 
+000002e0: 6375 7374 6f6d 2073 706c 6974 7465 7220  custom splitter 
+000002f0: 6361 6e20 6265 2070 726f 7669 6465 642e  can be provided.
+00000300: da06 6269 6e61 7279 4eda 0d63 6c61 7373  ..binaryN..class
+00000310: 5f70 726f 626c 656d 2902 7210 0000 00da  _problem).r.....
+00000320: 0a6d 756c 7469 636c 6173 73da 0a73 7472  .multiclass..str
+00000330: 6174 6966 6965 72da 0d63 6f6e 665f 7472  atifier..conf_tr
+00000340: 6169 6e69 6e67 da0c 636f 6e66 5f78 6762  aining..conf_xgb
+00000350: 6f6f 7374 da13 636f 6e66 5f70 6172 616d  oost..conf_param
+00000360: 735f 7867 626f 6f73 74da 1c63 7573 746f  s_xgboost..custo
+00000370: 6d5f 6c61 7374 5f6d 696c 655f 636f 6d70  m_last_mile_comp
+00000380: 7574 6174 696f 6eda 1363 7573 746f 6d5f  utation..custom_
+00000390: 7072 6570 726f 6365 7373 6f72 da17 6375  preprocessor..cu
+000003a0: 7374 6f6d 5f66 6561 7475 7265 5f73 656c  stom_feature_sel
+000003b0: 6563 746f 7263 0900 0000 0000 0000 0000  ectorc..........
+000003c0: 0000 0900 0000 0200 0000 4300 0000 733a  ..........C...s:
+000003d0: 0000 007c 017c 005f 007c 047c 005f 017c  ...|.|._.|.|._.|
+000003e0: 037c 005f 027c 057c 005f 037c 077c 005f  .|._.|.|._.|.|._
+000003f0: 047c 087c 005f 057c 067c 005f 0667 007c  .|.|._.|.|._.g.|
+00000400: 005f 077c 027c 005f 0864 0053 0029 014e  ._.|.|._.d.S.).N
+00000410: 2909 7211 0000 0072 1500 0000 7214 0000  ).r....r....r...
+00000420: 0072 1600 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000430: 7217 0000 00da 0f62 6c75 6563 6173 745f  r......bluecast_
+00000440: 6d6f 6465 6c73 7213 0000 0029 09da 0473  modelsr....)...s
+00000450: 656c 6672 1100 0000 7213 0000 0072 1400  elfr....r....r..
+00000460: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000470: 0072 1800 0000 7219 0000 00a9 0072 1c00  .r....r......r..
+00000480: 0000 fa41 2f68 6f6d 652f 7468 6f6d 6173  ...A/home/thomas
+00000490: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
+000004a0: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
+000004b0: 626c 7565 7072 696e 7473 2f63 6173 745f  blueprints/cast_
+000004c0: 6376 2e70 79da 085f 5f69 6e69 745f 5f15  cv.py..__init__.
+000004d0: 0000 0073 1200 0000 060d 0601 0601 0601  ...s............
+000004e0: 0601 0601 0601 0601 0a01 7a13 426c 7565  ..........z.Blue
+000004f0: 4361 7374 4356 2e5f 5f69 6e69 745f 5fda  CastCV.__init__.
+00000500: 0264 66da 0674 6172 6765 74da 0672 6574  .df..target..ret
+00000510: 7572 6e63 0300 0000 0000 0000 0000 0000  urnc............
+00000520: 0500 0000 0400 0000 4300 0000 732a 0000  ........C...s*..
+00000530: 007c 016a 0064 0164 028d 017d 017c 017c  .|.j.d.d...}.|.|
+00000540: 0219 007d 037c 016a 017c 0264 0364 048d  ...}.|.j.|.d.d..
+00000550: 027d 047c 047c 0366 0253 0029 054e 54a9  .}.|.|.f.S.).NT.
+00000560: 01da 0464 726f 70e9 0100 0000 a901 da04  ...drop.........
+00000570: 6178 6973 2902 da0b 7265 7365 745f 696e  axis)...reset_in
+00000580: 6465 7872 2300 0000 2905 721b 0000 0072  dexr#...).r....r
+00000590: 1f00 0000 7220 0000 00da 0179 da01 5872  ....r .....y..Xr
+000005a0: 1c00 0000 721c 0000 0072 1d00 0000 da0c  ....r....r......
+000005b0: 7072 6570 6172 655f 6461 7461 2c00 0000  prepare_data,...
+000005c0: 7308 0000 000c 0308 010e 0108 017a 1742  s............z.B
+000005d0: 6c75 6543 6173 7443 562e 7072 6570 6172  lueCastCV.prepar
+000005e0: 655f 6461 7461 da0a 7461 7267 6574 5f63  e_data..target_c
+000005f0: 6f6c 6303 0000 0000 0000 0000 0000 000e  olc.............
+00000600: 0000 000b 0000 0043 0000 0073 1e01 0000  .......C...s....
+00000610: 7c00 a000 7c01 7c02 a102 5c02 7d03 7d04  |...|.|...\.}.}.
+00000620: 7c00 6a01 730f 7402 8300 7c00 5f01 7c00  |.j.s.t...|._.|.
+00000630: 6a03 731c 7404 6401 6402 7c00 6a01 6a05  j.s.t.d.d.|.j.j.
+00000640: 6403 8d03 7c00 5f03 7406 7c00 6a03 a007  d...|._.t.|.j...
+00000650: 7c03 7c04 a102 8301 4400 5d67 5c02 7d05  |.|.....D.]g\.}.
+00000660: 5c02 7d06 7d07 7c03 6a08 7c06 1900 7c03  \.}.}.|.j.|...|.
+00000670: 6a08 7c07 1900 0202 7d08 7d09 7c04 6a08  j.|.....}.}.|.j.
+00000680: 7c06 1900 7c04 6a08 7c07 1900 0202 7d0a  |...|.j.|.....}.
+00000690: 7d0b 7409 6a0a 7c08 7c09 6702 6402 6404  }.t.j.|.|.g.d.d.
+000006a0: 8d02 7d0c 7409 6a0a 7c0a 7c0b 6702 6402  ..}.t.j.|.|.g.d.
+000006b0: 6404 8d02 7d0a 7c0c 6a0b 6402 6405 8d01  d...}.|.j.d.d...
+000006c0: 7d08 7c0a 6a0b 6402 6405 8d01 7d0a 7c0a  }.|.j.d.d...}.|.
+000006d0: 6a0c 7c08 7c02 3c00 7c00 6a01 0400 6a05  j.|.|.<.|.j...j.
+000006e0: 7c05 3700 0200 5f05 740d 7c00 6a0e 7c02  |.7..._.t.|.j.|.
+000006f0: 7c00 6a01 7c00 6a0f 7c00 6a10 7c00 6a11  |.j.|.j.|.j.|.j.
+00000700: 7c00 6a12 7c00 6a13 6406 8d08 7d0d 7c0d  |.j.|.j.d...}.|.
+00000710: 6a14 7c08 7c02 6407 8d02 0100 7c00 6a15  j.|.|.d.....|.j.
+00000720: a016 7c0d a101 0100 7125 6408 5300 2909  ..|.....q%d.S.).
+00000730: 7a6a 4669 7420 6d75 6c74 6970 6c65 2042  zjFit multiple B
+00000740: 6c75 6543 6173 7420 696e 7374 616e 6365  lueCast instance
+00000750: 7320 6f6e 2064 6966 6665 7265 6e74 2064  s on different d
+00000760: 6174 6120 7370 6c69 7473 2e0a 0a20 2020  ata splits...   
+00000770: 2020 2020 2049 6e70 7574 2064 6620 6973       Input df is
+00000780: 2065 7870 6563 7465 6420 7468 6520 7461   expected the ta
+00000790: 7267 6574 2063 6f6c 756d 6e2e e905 0000  rget column.....
+000007a0: 0054 a903 da08 6e5f 7370 6c69 7473 da07  .T....n_splits..
+000007b0: 7368 7566 666c 65da 0c72 616e 646f 6d5f  shuffle..random_
+000007c0: 7374 6174 6529 01da 0c69 676e 6f72 655f  state)...ignore_
+000007d0: 696e 6465 7872 2200 0000 a908 7211 0000  indexr".....r...
+000007e0: 00da 0d74 6172 6765 745f 636f 6c75 6d6e  ...target_column
+000007f0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000800: 1800 0000 7219 0000 0072 1700 0000 a901  ....r....r......
+00000810: 722b 0000 004e 2917 722a 0000 0072 1400  r+...N).r*...r..
+00000820: 0000 720a 0000 0072 1300 0000 7208 0000  ..r....r....r...
+00000830: 00da 1367 6c6f 6261 6c5f 7261 6e64 6f6d  ...global_random
+00000840: 5f73 7461 7465 da09 656e 756d 6572 6174  _state..enumerat
+00000850: 65da 0573 706c 6974 da04 696c 6f63 da02  e..split..iloc..
+00000860: 7064 da06 636f 6e63 6174 7227 0000 00da  pd..concatr'....
+00000870: 0676 616c 7565 7372 0900 0000 7211 0000  .valuesr....r...
+00000880: 0072 1500 0000 7216 0000 0072 1800 0000  .r....r....r....
+00000890: 7219 0000 0072 1700 0000 da03 6669 7472  r....r......fitr
+000008a0: 1a00 0000 da06 6170 7065 6e64 290e 721b  ......append).r.
+000008b0: 0000 0072 1f00 0000 722b 0000 0072 2900  ...r....r+...r).
+000008c0: 0000 7228 0000 00da 0266 6eda 0774 726e  ..r(.....fn..trn
+000008d0: 5f69 6478 da07 7661 6c5f 6964 78da 0758  _idx..val_idx..X
+000008e0: 5f74 7261 696e da05 585f 7661 6cda 0779  _train..X_val..y
+000008f0: 5f74 7261 696e da05 795f 7661 6cda 0778  _train..y_val..x
+00000900: 5f74 7261 696e da06 6175 746f 6d6c 721c  _train..automlr.
+00000910: 0000 0072 1c00 0000 721d 0000 0072 3c00  ...r....r....r<.
+00000920: 0000 3400 0000 733e 0000 0010 0406 0208  ..4...s>........
+00000930: 0106 0202 0102 0102 0106 0108 fd1e 0616  ................
+00000940: 0116 0112 0112 010c 020c 010a 0110 0202  ................
+00000950: 0204 0102 0104 0104 0104 0104 0104 0104  ................
+00000960: 0106 f80e 0a0e 0104 e97a 0e42 6c75 6543  .........z.BlueC
+00000970: 6173 7443 562e 6669 7463 0300 0000 0000  astCV.fitc......
+00000980: 0000 0000 0000 0d00 0000 0b00 0000 4300  ..............C.
+00000990: 0000 73e4 0000 007c 00a0 007c 017c 02a1  ..s....|...|.|..
+000009a0: 025c 027d 037d 047c 006a 0173 0f74 0283  .\.}.}.|.j.s.t..
+000009b0: 007c 005f 017c 006a 0373 1c74 0464 0164  .|._.|.j.s.t.d.d
+000009c0: 027c 006a 016a 0564 038d 037c 005f 0374  .|.j.j.d...|._.t
+000009d0: 067c 006a 03a0 077c 037c 04a1 0283 0144  .|.j...|.|.....D
+000009e0: 005d 4a5c 027d 055c 027d 067d 077c 036a  .]J\.}.\.}.}.|.j
+000009f0: 087c 0619 007c 036a 087c 0719 0002 027d  .|...|.j.|.....}
+00000a00: 087d 097c 046a 087c 0619 007c 046a 087c  .}.|.j.|...|.j.|
+00000a10: 0719 0002 027d 0a7d 0b7c 0a7c 087c 023c  .....}.}.|.|.|.<
+00000a20: 007c 006a 0104 006a 057c 0537 0002 005f  .|.j...j.|.7..._
+00000a30: 0574 097c 006a 0a7c 027c 006a 017c 006a  .t.|.j.|.|.j.|.j
+00000a40: 0b7c 006a 0c7c 006a 0d7c 006a 0e7c 006a  .|.j.|.j.|.j.|.j
+00000a50: 0f64 048d 087d 0c7c 0c6a 107c 087c 097c  .d...}.|.j.|.|.|
+00000a60: 0b7c 0264 058d 0401 007c 006a 11a0 127c  .|.d.....|.j...|
+00000a70: 0ca1 0101 0071 2564 0653 0029 077a af46  .....q%d.S.).z.F
+00000a80: 6974 206d 756c 7469 706c 6520 426c 7565  it multiple Blue
+00000a90: 4361 7374 2069 6e73 7461 6e63 6573 206f  Cast instances o
+00000aa0: 6e20 6469 6666 6572 656e 7420 6461 7461  n different data
+00000ab0: 2073 706c 6974 732e 0a0a 2020 2020 2020   splits...      
+00000ac0: 2020 496e 7075 7420 6466 2069 7320 6578    Input df is ex
+00000ad0: 7065 6374 6564 2074 6865 2074 6172 6765  pected the targe
+00000ae0: 7420 636f 6c75 6d6e 2e20 4576 616c 7561  t column. Evalua
+00000af0: 7469 6f6e 2069 7320 6578 6563 7574 6564  tion is executed
+00000b00: 206f 6e20 6f75 742d 6f66 2d66 6f6c 6420   on out-of-fold 
+00000b10: 6461 7461 7365 740a 2020 2020 2020 2020  dataset.        
+00000b20: 696e 2065 6163 6820 7370 6c69 742e 722c  in each split.r,
+00000b30: 0000 0054 722d 0000 0072 3200 0000 7234  ...Tr-...r2...r4
+00000b40: 0000 004e 2913 722a 0000 0072 1400 0000  ...N).r*...r....
+00000b50: 720a 0000 0072 1300 0000 7208 0000 0072  r....r....r....r
+00000b60: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
+00000b70: 0000 0072 0900 0000 7211 0000 0072 1500  ...r....r....r..
+00000b80: 0000 7216 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000b90: 0072 1700 0000 da08 6669 745f 6576 616c  .r......fit_eval
+00000ba0: 721a 0000 0072 3d00 0000 290d 721b 0000  r....r=...).r...
+00000bb0: 0072 1f00 0000 722b 0000 0072 2900 0000  .r....r+...r)...
+00000bc0: 7228 0000 0072 3e00 0000 723f 0000 0072  r(...r>...r?...r
+00000bd0: 4000 0000 7241 0000 0072 4200 0000 7243  @...rA...rB...rC
+00000be0: 0000 0072 4400 0000 7246 0000 0072 1c00  ...rD...rF...r..
+00000bf0: 0000 721c 0000 0072 1d00 0000 7247 0000  ..r....r....rG..
+00000c00: 005d 0000 0073 3600 0000 1005 0602 0801  .]...s6.........
+00000c10: 0602 0201 0201 0201 0601 08fd 1e06 1601  ................
+00000c20: 1601 0802 1002 0202 0401 0201 0401 0401  ................
+00000c30: 0401 0401 0401 0401 06f8 120a 0e01 04ed  ................
+00000c40: 7a13 426c 7565 4361 7374 4356 2e66 6974  z.BlueCastCV.fit
+00000c50: 5f65 7661 6c46 da17 7265 7475 726e 5f73  _evalF..return_s
+00000c60: 7562 5f6d 6f64 656c 735f 7072 6564 7363  ub_models_predsc
+00000c70: 0300 0000 0000 0000 0000 0000 0a00 0000  ................
+00000c80: 0600 0000 4300 0000 73da 0000 007c 016a  ....C...s....|.j
+00000c90: 007d 0367 007d 0467 007d 0574 017c 006a  .}.g.}.g.}.t.|.j
+00000ca0: 0283 0144 005d 305c 027d 067d 077c 07a0  ...D.]0\.}.}.|..
+00000cb0: 037c 016a 0464 0164 0185 027c 0366 0219  .|.j.d.d...|.f..
+00000cc0: 00a1 015c 027d 087d 097c 087c 0164 027c  ...\.}.}.|.|.d.|
+00000cd0: 069b 009d 023c 007c 097c 0164 037c 069b  .....<.|.|.d.|..
+00000ce0: 009d 023c 007c 04a0 0564 027c 069b 009d  ...<.|...d.|....
+00000cf0: 02a1 0101 007c 05a0 0564 037c 069b 009d  .....|...d.|....
+00000d00: 02a1 0101 0071 0c7c 0272 517c 016a 0464  .....q.|.rQ|.j.d
+00000d10: 0164 0185 027c 0466 0219 007c 016a 0464  .d...|.f...|.j.d
+00000d20: 0164 0185 027c 0566 0219 0066 0253 007c  .d...|.f...f.S.|
+00000d30: 016a 0464 0164 0185 027c 0466 0219 006a  .j.d.d...|.f...j
+00000d40: 0664 0464 058d 017c 016a 0464 0164 0185  .d.d...|.j.d.d..
+00000d50: 027c 0466 0219 006a 0664 0464 058d 0164  .|.f...j.d.d...d
+00000d60: 066b 0466 0253 0029 077a 4050 7265 6469  .k.f.S.).z@Predi
+00000d70: 6374 206f 6e20 756e 7365 656e 2064 6174  ct on unseen dat
+00000d80: 6120 7573 696e 6720 6d75 6c74 6970 6c65  a using multiple
+00000d90: 2074 7261 696e 6564 2042 6c75 6543 6173   trained BlueCas
+00000da0: 7420 696e 7374 616e 6365 734e 5a06 7072  t instancesNZ.pr
+00000db0: 6f62 615f da08 636c 6173 7365 735f 7224  oba_..classes_r$
+00000dc0: 0000 0072 2500 0000 6700 0000 0000 00e0  ...r%...g.......
+00000dd0: 3f29 07da 0763 6f6c 756d 6e73 7236 0000  ?)...columnsr6..
+00000de0: 0072 1a00 0000 da07 7072 6564 6963 74da  .r......predict.
+00000df0: 036c 6f63 723d 0000 00da 046d 6561 6e29  .locr=.....mean)
+00000e00: 0a72 1b00 0000 721f 0000 0072 4800 0000  .r....r....rH...
+00000e10: 5a07 6f72 5f63 6f6c 735a 0970 726f 625f  Z.or_colsZ.prob_
+00000e20: 636f 6c73 5a0a 636c 6173 735f 636f 6c73  colsZ.class_cols
+00000e30: 723e 0000 00da 0870 6970 656c 696e 65da  r>.....pipeline.
+00000e40: 0779 5f70 726f 6273 da09 795f 636c 6173  .y_probs..y_clas
+00000e50: 7365 7372 1c00 0000 721c 0000 0072 1d00  sesr....r....r..
+00000e60: 0000 724b 0000 0083 0000 0073 1c00 0000  ..rK.......s....
+00000e70: 0604 0401 0401 1201 1c01 0e01 0e01 1001  ................
+00000e80: 1201 0402 2401 1803 1c01 04fe 7a12 426c  ....$.......z.Bl
+00000e90: 7565 4361 7374 4356 2e70 7265 6469 6374  ueCastCV.predict
+00000ea0: 2908 7210 0000 004e 4e4e 4e4e 4e4e 2901  ).r....NNNNNNN).
+00000eb0: 4629 18da 085f 5f6e 616d 655f 5fda 0a5f  F)...__name__.._
+00000ec0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000ed0: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000ee0: 7204 0000 0072 0500 0000 7202 0000 0072  r....r....r....r
+00000ef0: 0a00 0000 720c 0000 0072 0b00 0000 720d  ....r....r....r.
+00000f00: 0000 0072 0700 0000 720e 0000 0072 1e00  ...r....r....r..
+00000f10: 0000 7239 0000 00da 0944 6174 6146 7261  ..r9.....DataFra
+00000f20: 6d65 da03 7374 7272 0600 0000 da06 5365  me..strr......Se
+00000f30: 7269 6573 722a 0000 0072 3c00 0000 7247  riesr*...r<...rG
+00000f40: 0000 00da 0462 6f6f 6c72 4b00 0000 721c  .....boolrK...r.
+00000f50: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
+00000f60: 0000 720f 0000 0010 0000 0073 5c00 0000  ..r........s\...
+00000f70: 0800 0401 0206 0201 0201 0201 0201 0201  ................
+00000f80: 0201 0203 04f5 0602 02fe 0603 02fd 0604  ................
+00000f90: 02fc 0605 02fb 0606 02fa 0607 02f9 0608  ................
+00000fa0: 02f8 0209 0a01 02ff 0af7 0217 0401 02ff  ................
+00000fb0: 0201 02ff 0e02 0afe 1808 1829 0227 04ff  ...........).'..
+00000fc0: 0401 02ff 0201 02ff 2202 0efe 720f 0000  ........"...r...
+00000fd0: 0029 16da 0674 7970 696e 6772 0200 0000  .)...typingr....
+00000fe0: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+00000ff0: 0600 0000 7207 0000 00da 0670 616e 6461  ....r......panda
+00001000: 7372 3900 0000 da17 736b 6c65 6172 6e2e  sr9.....sklearn.
+00001010: 6d6f 6465 6c5f 7365 6c65 6374 696f 6e72  model_selectionr
+00001020: 0800 0000 da18 626c 7565 6361 7374 2e62  ......bluecast.b
+00001030: 6c75 6570 7269 6e74 732e 6361 7374 7209  lueprints.castr.
+00001040: 0000 00da 1f62 6c75 6563 6173 742e 636f  .....bluecast.co
+00001050: 6e66 6967 2e74 7261 696e 696e 675f 636f  nfig.training_co
+00001060: 6e66 6967 720a 0000 0072 0b00 0000 720c  nfigr....r....r.
+00001070: 0000 00da 1d62 6c75 6563 6173 742e 7072  .....bluecast.pr
+00001080: 6570 726f 6365 7373 696e 672e 6375 7374  eprocessing.cust
+00001090: 6f6d 720d 0000 00da 2862 6c75 6563 6173  omr.....(bluecas
+000010a0: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
+000010b0: 6665 6174 7572 655f 7365 6c65 6374 696f  feature_selectio
+000010c0: 6e72 0e00 0000 720f 0000 0072 1c00 0000  nr....r....r....
+000010d0: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
+000010e0: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
+000010f0: 0000 2000 0802 0c01 0c02 1401 0c05 0c01  .. .............
+00001100: 1203                                     ..
```

### Comparing `bluecast-0.8/bluecast/blueprints/cast.py` & `bluecast-0.9/bluecast/blueprints/cast.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/blueprints/cast_cv.py` & `bluecast-0.9/bluecast/blueprints/cast_cv.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from bluecast.blueprints.cast import BlueCast
 from bluecast.config.training_config import (
     TrainingConfig,
     XgboostFinalParamConfig,
     XgboostTuneParamsConfig,
 )
+from bluecast.ml_modelling.xgboost import XgboostModel
 from bluecast.preprocessing.custom import CustomPreprocessing
 from bluecast.preprocessing.feature_selection import RFECVSelector
 
 
 class BlueCastCV:
     """Wrapper to train and predict multiple blueCast intsances.
 
@@ -26,24 +27,26 @@
         conf_xgboost: Optional[XgboostTuneParamsConfig] = None,
         conf_params_xgboost: Optional[XgboostFinalParamConfig] = None,
         custom_last_mile_computation: Optional[CustomPreprocessing] = None,
         custom_preprocessor: Optional[CustomPreprocessing] = None,
         custom_feature_selector: Optional[
             Union[RFECVSelector, CustomPreprocessing]
         ] = None,
+        ml_model: Optional[Union[XgboostModel, Any]] = None,
     ):
         self.class_problem = class_problem
         self.conf_xgboost = conf_xgboost
         self.conf_training = conf_training
         self.conf_params_xgboost = conf_params_xgboost
         self.custom_preprocessor = custom_preprocessor
         self.custom_feature_selector = custom_feature_selector
         self.custom_last_mile_computation = custom_last_mile_computation
         self.bluecast_models: List[BlueCast] = []
         self.stratifier = stratifier
+        self.ml_model = ml_model
 
     def prepare_data(
         self, df: pd.DataFrame, target: str
     ) -> Tuple[pd.DataFrame, pd.Series]:
         df = df.reset_index(drop=True)
         y = df[target]
         X = df.drop(target, axis=1)
@@ -82,14 +85,15 @@
                 target_column=target_col,
                 conf_training=self.conf_training,
                 conf_xgboost=self.conf_xgboost,
                 conf_params_xgboost=self.conf_params_xgboost,
                 custom_preprocessor=self.custom_preprocessor,
                 custom_feature_selector=self.custom_feature_selector,
                 custom_last_mile_computation=self.custom_last_mile_computation,
+                ml_model=self.ml_model,
             )
             automl.fit(X_train, target_col=target_col)
             self.bluecast_models.append(automl)
 
     def fit_eval(self, df: pd.DataFrame, target_col: str) -> None:
         """Fit multiple BlueCast instances on different data splits.
 
@@ -120,14 +124,15 @@
                 target_column=target_col,
                 conf_training=self.conf_training,
                 conf_xgboost=self.conf_xgboost,
                 conf_params_xgboost=self.conf_params_xgboost,
                 custom_preprocessor=self.custom_preprocessor,
                 custom_feature_selector=self.custom_feature_selector,
                 custom_last_mile_computation=self.custom_last_mile_computation,
+                ml_model=self.ml_model,
             )
             automl.fit_eval(X_train, X_val, y_val, target_col=target_col)
             self.bluecast_models.append(automl)
 
     def predict(
         self, df: pd.DataFrame, return_sub_models_preds: bool = False
     ) -> Tuple[Union[pd.DataFrame, pd.Series], Union[pd.DataFrame, pd.Series]]:
```

### Comparing `bluecast-0.8/bluecast/config/__pycache__/training_config.cpython-310.pyc` & `bluecast-0.9/bluecast/config/__pycache__/training_config.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 04:32:39 2023 UTC, .py size: 2932 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e7a0 a364 740b 0000  o..........dt...
+00000000: 550d 0d0a 0000 0000 e7a0 a364 740b 0000  U..........dt...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a06 6505 4700  d.d...d...Z.e.G.
 00000060: 6406 6407 8400 6407 8302 8301 5a07 6505  d.d...d.....Z.e.
 00000070: 4700 6408 6409 8400 6409 8302 8301 5a08  G.d.d...d.....Z.
@@ -41,197 +41,191 @@
 00000280: da04 4469 6374 da08 4f70 7469 6f6e 616c  ..Dict..Optional
 00000290: 2901 da09 6461 7461 636c 6173 7363 0000  )...dataclassc..
 000002a0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
 000002b0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
 000002c0: 005a 0264 015a 0364 0253 0029 03da 0643  .Z.d.Z.d.S.)...C
 000002d0: 6f6e 6669 6754 4e29 04da 085f 5f6e 616d  onfigTN)...__nam
 000002e0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000002f0: 0c5f 5f71 7561 6c6e 616d 655f 5f5a 1761  .__qualname__Z.a
+000002f0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 1761  .__qualname__..a
 00000300: 7262 6974 7261 7279 5f74 7970 6573 5f61  rbitrary_types_a
-00000310: 6c6c 6f77 6564 a900 7209 0000 0072 0900  llowed..r....r..
+00000310: 6c6c 6f77 6564 a900 720a 0000 0072 0a00  llowed..r....r..
 00000320: 0000 fa45 2f68 6f6d 652f 7468 6f6d 6173  ...E/home/thomas
 00000330: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
 00000340: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
 00000350: 636f 6e66 6967 2f74 7261 696e 696e 675f  config/training_
 00000360: 636f 6e66 6967 2e70 7972 0500 0000 0d00  config.pyr......
-00000370: 0000 7304 0000 0008 0008 0172 0500 0000  ..s........r....
-00000380: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000390: 0003 0000 0040 0000 0073 ba00 0000 6500  .....@...s....e.
-000003a0: 5a01 6400 5a02 5500 6401 5a03 6402 5a04  Z.d.Z.U.d.Z.d.Z.
-000003b0: 6505 6506 6403 3c00 6404 5a07 6508 6506  e.e.d.<.d.Z.e.e.
-000003c0: 6405 3c00 6406 5a09 6505 6506 6407 3c00  d.<.d.Z.e.e.d.<.
-000003d0: 6408 5a0a 6505 6506 6409 3c00 640a 5a0b  d.Z.e.e.d.<.d.Z.
-000003e0: 6505 6506 640b 3c00 6402 5a0c 6505 6506  e.e.d.<.d.Z.e.e.
-000003f0: 640c 3c00 6404 5a0d 6508 6506 640d 3c00  d.<.d.Z.e.e.d.<.
-00000400: 640e 5a0e 6508 6506 640f 3c00 6404 5a0f  d.Z.e.e.d.<.d.Z.
-00000410: 6508 6506 6410 3c00 6411 5a10 6511 6506  e.e.d.<.d.Z.e.e.
-00000420: 6412 3c00 6404 5a12 6508 6506 6413 3c00  d.<.d.Z.e.e.d.<.
-00000430: 640e 5a13 6508 6506 6414 3c00 6415 5a14  d.Z.e.e.d.<.d.Z.
-00000440: 6505 6506 6416 3c00 640e 5a15 6508 6506  e.e.d.<.d.Z.e.e.
-00000450: 6417 3c00 6418 5300 2919 da0e 5472 6169  d.<.d.S.)...Trai
-00000460: 6e69 6e67 436f 6e66 6967 7a23 4465 6669  ningConfigz#Defi
-00000470: 6e65 2067 656e 6572 616c 2074 7261 696e  ne general train
-00000480: 696e 6720 7061 7261 6d65 7465 7273 2ee9  ing parameters..
-00000490: 0a00 0000 da13 676c 6f62 616c 5f72 616e  ......global_ran
-000004a0: 646f 6d5f 7374 6174 6554 da17 7368 7566  dom_stateT..shuf
-000004b0: 666c 655f 6475 7269 6e67 5f74 7261 696e  fle_during_train
-000004c0: 696e 67e9 6400 0000 da1c 6879 7065 7270  ing.d.....hyperp
-000004d0: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
-000004e0: 726f 756e 6473 6910 0e00 00da 2668 7970  roundsi.....&hyp
-000004f0: 6572 7061 7261 6d65 7465 725f 7475 6e69  erparameter_tuni
-00000500: 6e67 5f6d 6178 5f72 756e 7469 6d65 5f73  ng_max_runtime_s
-00000510: 6563 73e9 0100 0000 da14 6879 7065 7274  ecs.......hypert
-00000520: 756e 696e 675f 6376 5f66 6f6c 6473 da15  uning_cv_folds..
-00000530: 6561 726c 795f 7374 6f70 7069 6e67 5f72  early_stopping_r
-00000540: 6f75 6e64 73da 0e61 7574 6f74 756e 655f  ounds..autotune_
-00000550: 6d6f 6465 6c46 da18 656e 6162 6c65 5f66  modelF..enable_f
-00000560: 6561 7475 7265 5f73 656c 6563 7469 6f6e  eature_selection
-00000570: da15 6361 6c63 756c 6174 655f 7368 6170  ..calculate_shap
-00000580: 5f76 616c 7565 73e7 9a99 9999 9999 e93f  _values........?
-00000590: da0a 7472 6169 6e5f 7369 7a65 da14 7472  ..train_size..tr
-000005a0: 6169 6e5f 7370 6c69 745f 7374 7261 7469  ain_split_strati
-000005b0: 6679 da1d 7573 655f 6675 6c6c 5f64 6174  fy..use_full_dat
-000005c0: 615f 666f 725f 6669 6e61 6c5f 6d6f 6465  a_for_final_mode
-000005d0: 6ce9 0500 0000 da16 6d69 6e5f 6665 6174  l.......min_feat
-000005e0: 7572 6573 5f74 6f5f 7365 6c65 6374 da1d  ures_to_select..
-000005f0: 6361 745f 656e 636f 6469 6e67 5f76 6961  cat_encoding_via
-00000600: 5f6d 6c5f 616c 676f 7269 7468 6d4e 2916  _ml_algorithmN).
-00000610: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
-00000620: 075f 5f64 6f63 5f5f 720d 0000 00da 0369  .__doc__r......i
-00000630: 6e74 da0f 5f5f 616e 6e6f 7461 7469 6f6e  nt..__annotation
-00000640: 735f 5f72 0e00 0000 da04 626f 6f6c 7210  s__r......boolr.
-00000650: 0000 0072 1100 0000 7213 0000 0072 1400  ...r....r....r..
-00000660: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000670: 0072 1900 0000 da05 666c 6f61 7472 1a00  .r......floatr..
-00000680: 0000 721b 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00000690: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-000006a0: 720a 0000 0072 0b00 0000 1100 0000 7320  r....r........s 
-000006b0: 0000 000a 0004 020c 020c 010c 010c 010c  ................
-000006c0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-000006d0: 0110 0172 0b00 0000 6300 0000 0000 0000  ...r....c.......
-000006e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000006f0: 0073 3201 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
-00000700: 6401 5a03 6402 5a04 6505 6506 6403 3c00  d.Z.d.Z.e.e.d.<.
-00000710: 6404 5a07 6505 6506 6405 3c00 6406 5a08  d.Z.e.e.d.<.d.Z.
-00000720: 6509 6506 6407 3c00 6408 5a0a 6509 6506  e.e.d.<.d.Z.e.e.
-00000730: 6409 3c00 6406 5a0b 6509 6506 640a 3c00  d.<.d.Z.e.e.d.<.
-00000740: 6408 5a0c 6509 6506 640b 3c00 6402 5a0d  d.Z.e.e.d.<.d.Z.
-00000750: 6505 6506 640c 3c00 640d 5a0e 6505 6506  e.e.d.<.d.Z.e.e.
-00000760: 640e 3c00 640f 5a0f 6509 6506 6410 3c00  d.<.d.Z.e.e.d.<.
-00000770: 6411 5a10 6509 6506 6412 3c00 640f 5a11  d.Z.e.e.d.<.d.Z.
-00000780: 6509 6506 6413 3c00 6411 5a12 6509 6506  e.e.d.<.d.Z.e.e.
-00000790: 6414 3c00 640f 5a13 6509 6506 6415 3c00  d.<.d.Z.e.e.d.<.
-000007a0: 6411 5a14 6509 6506 6416 3c00 6406 5a15  d.Z.e.e.d.<.d.Z.
-000007b0: 6509 6506 6417 3c00 6408 5a16 6509 6506  e.e.d.<.d.Z.e.e.
-000007c0: 6418 3c00 6419 5a17 6509 6506 641a 3c00  d.<.d.Z.e.e.d.<.
-000007d0: 640f 5a18 6509 6506 641b 3c00 6402 5a19  d.Z.e.e.d.<.d.Z.
-000007e0: 6505 6506 641c 3c00 641d 5a1a 6505 6506  e.e.d.<.d.Z.e.e.
-000007f0: 641e 3c00 641f 5a1b 6505 6506 6420 3c00  d.<.d.Z.e.e.d <.
-00000800: 6421 5a1c 651d 6506 6422 3c00 6423 5a1e  d!Z.e.e.d"<.d#Z.
-00000810: 651d 6506 6424 3c00 6425 5a1f 651d 6506  e.e.d$<.d%Z.e.e.
-00000820: 6426 3c00 6427 5300 2928 da17 5867 626f  d&<.d'S.)(..Xgbo
-00000830: 6f73 7454 756e 6550 6172 616d 7343 6f6e  ostTuneParamsCon
-00000840: 6669 677a 2a44 6566 696e 6520 6879 7065  figz*Define hype
-00000850: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
-00000860: 6720 7365 6172 6368 2073 7061 6365 2ee9  g search space..
-00000870: 0200 0000 da0d 6d61 785f 6465 7074 685f  ......max_depth_
-00000880: 6d69 6ee9 0600 0000 da0d 6d61 785f 6465  min.......max_de
-00000890: 7074 685f 6d61 7867 0000 0000 0000 0000  pth_maxg........
-000008a0: da09 616c 7068 615f 6d69 6e67 0000 0000  ..alpha_ming....
-000008b0: 0000 2440 da09 616c 7068 615f 6d61 78da  ..$@..alpha_max.
-000008c0: 0a6c 616d 6264 615f 6d69 6eda 0a6c 616d  .lambda_min..lam
-000008d0: 6264 615f 6d61 78da 0e6e 756d 5f6c 6561  bda_max..num_lea
-000008e0: 7665 735f 6d69 6ee9 4000 0000 da0e 6e75  ves_min.@.....nu
-000008f0: 6d5f 6c65 6176 6573 5f6d 6178 6733 3333  m_leaves_maxg333
-00000900: 3333 33d3 3fda 0e73 7562 5f73 616d 706c  333.?..sub_sampl
-00000910: 655f 6d69 6e67 0000 0000 0000 f03f da0e  e_ming.......?..
-00000920: 7375 625f 7361 6d70 6c65 5f6d 6178 da16  sub_sample_max..
-00000930: 636f 6c5f 7361 6d70 6c65 5f62 795f 7472  col_sample_by_tr
-00000940: 6565 5f6d 696e da16 636f 6c5f 7361 6d70  ee_min..col_samp
-00000950: 6c65 5f62 795f 7472 6565 5f6d 6178 da17  le_by_tree_max..
-00000960: 636f 6c5f 7361 6d70 6c65 5f62 795f 6c65  col_sample_by_le
-00000970: 7665 6c5f 6d69 6eda 1763 6f6c 5f73 616d  vel_min..col_sam
-00000980: 706c 655f 6279 5f6c 6576 656c 5f6d 6178  ple_by_level_max
-00000990: da14 6d69 6e5f 6368 696c 645f 7765 6967  ..min_child_weig
-000009a0: 6874 5f6d 696e da14 6d69 6e5f 6368 696c  ht_min..min_chil
-000009b0: 645f 7765 6967 6874 5f6d 6178 67fc a9f1  d_weight_maxg...
-000009c0: d24d 6250 3fda 0765 7461 5f6d 696e da07  .MbP?..eta_min..
-000009d0: 6574 615f 6d61 78da 0973 7465 7073 5f6d  eta_max..steps_m
-000009e0: 696e e9e8 0300 00da 0973 7465 7073 5f6d  in.......steps_m
-000009f0: 6178 7201 0000 00da 0f6d 6f64 656c 5f76  axr......model_v
-00000a00: 6572 626f 7369 7479 fa0e 6d75 6c74 693a  erbosity..multi:
-00000a10: 736f 6674 7072 6f62 da0f 6d6f 6465 6c5f  softprob..model_
-00000a20: 6f62 6a65 6374 6976 65da 086d 6c6f 676c  objective..mlogl
-00000a30: 6f73 73da 116d 6f64 656c 5f65 7661 6c5f  oss..model_eval_
-00000a40: 6d65 7472 6963 da06 6762 7472 6565 da07  metric..gbtree..
-00000a50: 626f 6f73 7465 724e 2920 7206 0000 0072  boosterN) r....r
-00000a60: 0700 0000 7208 0000 0072 1f00 0000 7226  ....r....r....r&
-00000a70: 0000 0072 2000 0000 7221 0000 0072 2800  ...r ...r!...r(.
-00000a80: 0000 7229 0000 0072 2300 0000 722a 0000  ..r)...r#...r*..
-00000a90: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
-00000aa0: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
-00000ab0: 3200 0000 7233 0000 0072 3400 0000 7235  2...r3...r4...r5
-00000ac0: 0000 0072 3600 0000 7237 0000 0072 3800  ...r6...r7...r8.
-00000ad0: 0000 7239 0000 0072 3a00 0000 723c 0000  ..r9...r:...r<..
-00000ae0: 0072 3d00 0000 723f 0000 00da 0373 7472  .r=...r?.....str
-00000af0: 7241 0000 0072 4300 0000 7209 0000 0072  rA...rC...r....r
-00000b00: 0900 0000 7209 0000 0072 0a00 0000 7224  ....r....r....r$
-00000b10: 0000 0025 0000 0073 3400 0000 0a00 0402  ...%...s4.......
-00000b20: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000370: 0000 7302 0000 0008 0172 0500 0000 6300  ..s......r....c.
+00000380: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000390: 0000 0040 0000 0073 ba00 0000 6500 5a01  ...@...s....e.Z.
+000003a0: 6400 5a02 5500 6401 5a03 6402 5a04 6505  d.Z.U.d.Z.d.Z.e.
+000003b0: 6506 6403 3c00 6404 5a07 6508 6506 6405  e.d.<.d.Z.e.e.d.
+000003c0: 3c00 6406 5a09 6505 6506 6407 3c00 6408  <.d.Z.e.e.d.<.d.
+000003d0: 5a0a 6505 6506 6409 3c00 640a 5a0b 6505  Z.e.e.d.<.d.Z.e.
+000003e0: 6506 640b 3c00 6402 5a0c 6505 6506 640c  e.d.<.d.Z.e.e.d.
+000003f0: 3c00 6404 5a0d 6508 6506 640d 3c00 640e  <.d.Z.e.e.d.<.d.
+00000400: 5a0e 6508 6506 640f 3c00 6404 5a0f 6508  Z.e.e.d.<.d.Z.e.
+00000410: 6506 6410 3c00 6411 5a10 6511 6506 6412  e.d.<.d.Z.e.e.d.
+00000420: 3c00 6404 5a12 6508 6506 6413 3c00 640e  <.d.Z.e.e.d.<.d.
+00000430: 5a13 6508 6506 6414 3c00 6415 5a14 6505  Z.e.e.d.<.d.Z.e.
+00000440: 6506 6416 3c00 640e 5a15 6508 6506 6417  e.d.<.d.Z.e.e.d.
+00000450: 3c00 6418 5300 2919 da0e 5472 6169 6e69  <.d.S.)...Traini
+00000460: 6e67 436f 6e66 6967 7a23 4465 6669 6e65  ngConfigz#Define
+00000470: 2067 656e 6572 616c 2074 7261 696e 696e   general trainin
+00000480: 6720 7061 7261 6d65 7465 7273 2ee9 0a00  g parameters....
+00000490: 0000 da13 676c 6f62 616c 5f72 616e 646f  ....global_rando
+000004a0: 6d5f 7374 6174 6554 da17 7368 7566 666c  m_stateT..shuffl
+000004b0: 655f 6475 7269 6e67 5f74 7261 696e 696e  e_during_trainin
+000004c0: 67e9 6400 0000 da1c 6879 7065 7270 6172  g.d.....hyperpar
+000004d0: 616d 6574 6572 5f74 756e 696e 675f 726f  ameter_tuning_ro
+000004e0: 756e 6473 6910 0e00 00da 2668 7970 6572  undsi.....&hyper
+000004f0: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
+00000500: 5f6d 6178 5f72 756e 7469 6d65 5f73 6563  _max_runtime_sec
+00000510: 73e9 0100 0000 da14 6879 7065 7274 756e  s.......hypertun
+00000520: 696e 675f 6376 5f66 6f6c 6473 da15 6561  ing_cv_folds..ea
+00000530: 726c 795f 7374 6f70 7069 6e67 5f72 6f75  rly_stopping_rou
+00000540: 6e64 73da 0e61 7574 6f74 756e 655f 6d6f  nds..autotune_mo
+00000550: 6465 6c46 da18 656e 6162 6c65 5f66 6561  delF..enable_fea
+00000560: 7475 7265 5f73 656c 6563 7469 6f6e da15  ture_selection..
+00000570: 6361 6c63 756c 6174 655f 7368 6170 5f76  calculate_shap_v
+00000580: 616c 7565 73e7 9a99 9999 9999 e93f da0a  alues........?..
+00000590: 7472 6169 6e5f 7369 7a65 da14 7472 6169  train_size..trai
+000005a0: 6e5f 7370 6c69 745f 7374 7261 7469 6679  n_split_stratify
+000005b0: da1d 7573 655f 6675 6c6c 5f64 6174 615f  ..use_full_data_
+000005c0: 666f 725f 6669 6e61 6c5f 6d6f 6465 6ce9  for_final_model.
+000005d0: 0500 0000 da16 6d69 6e5f 6665 6174 7572  ......min_featur
+000005e0: 6573 5f74 6f5f 7365 6c65 6374 da1d 6361  es_to_select..ca
+000005f0: 745f 656e 636f 6469 6e67 5f76 6961 5f6d  t_encoding_via_m
+00000600: 6c5f 616c 676f 7269 7468 6d4e 2916 7206  l_algorithmN).r.
+00000610: 0000 0072 0700 0000 7208 0000 00da 075f  ...r....r......_
+00000620: 5f64 6f63 5f5f 720e 0000 00da 0369 6e74  _doc__r......int
+00000630: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+00000640: 5f72 0f00 0000 da04 626f 6f6c 7211 0000  _r......boolr...
+00000650: 0072 1200 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000660: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000670: 1a00 0000 da05 666c 6f61 7472 1b00 0000  ......floatr....
+00000680: 721c 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000690: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+000006a0: 0000 0072 0c00 0000 1100 0000 731e 0000  ...r........s...
+000006b0: 000a 0204 020c 010c 010c 010c 010c 010c  ................
+000006c0: 010c 010c 010c 010c 010c 010c 010c 0172  ...............r
+000006d0: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000006e0: 0000 0000 0003 0000 0040 0000 0073 3201  .........@...s2.
+000006f0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000700: 6402 5a04 6505 6506 6403 3c00 6404 5a07  d.Z.e.e.d.<.d.Z.
+00000710: 6505 6506 6405 3c00 6406 5a08 6509 6506  e.e.d.<.d.Z.e.e.
+00000720: 6407 3c00 6408 5a0a 6509 6506 6409 3c00  d.<.d.Z.e.e.d.<.
+00000730: 6406 5a0b 6509 6506 640a 3c00 6408 5a0c  d.Z.e.e.d.<.d.Z.
+00000740: 6509 6506 640b 3c00 6402 5a0d 6505 6506  e.e.d.<.d.Z.e.e.
+00000750: 640c 3c00 640d 5a0e 6505 6506 640e 3c00  d.<.d.Z.e.e.d.<.
+00000760: 640f 5a0f 6509 6506 6410 3c00 6411 5a10  d.Z.e.e.d.<.d.Z.
+00000770: 6509 6506 6412 3c00 640f 5a11 6509 6506  e.e.d.<.d.Z.e.e.
+00000780: 6413 3c00 6411 5a12 6509 6506 6414 3c00  d.<.d.Z.e.e.d.<.
+00000790: 640f 5a13 6509 6506 6415 3c00 6411 5a14  d.Z.e.e.d.<.d.Z.
+000007a0: 6509 6506 6416 3c00 6406 5a15 6509 6506  e.e.d.<.d.Z.e.e.
+000007b0: 6417 3c00 6408 5a16 6509 6506 6418 3c00  d.<.d.Z.e.e.d.<.
+000007c0: 6419 5a17 6509 6506 641a 3c00 640f 5a18  d.Z.e.e.d.<.d.Z.
+000007d0: 6509 6506 641b 3c00 6402 5a19 6505 6506  e.e.d.<.d.Z.e.e.
+000007e0: 641c 3c00 641d 5a1a 6505 6506 641e 3c00  d.<.d.Z.e.e.d.<.
+000007f0: 641f 5a1b 6505 6506 6420 3c00 6421 5a1c  d.Z.e.e.d <.d!Z.
+00000800: 651d 6506 6422 3c00 6423 5a1e 651d 6506  e.e.d"<.d#Z.e.e.
+00000810: 6424 3c00 6425 5a1f 651d 6506 6426 3c00  d$<.d%Z.e.e.d&<.
+00000820: 6427 5300 2928 da17 5867 626f 6f73 7454  d'S.)(..XgboostT
+00000830: 756e 6550 6172 616d 7343 6f6e 6669 677a  uneParamsConfigz
+00000840: 2a44 6566 696e 6520 6879 7065 7270 6172  *Define hyperpar
+00000850: 616d 6574 6572 2074 756e 696e 6720 7365  ameter tuning se
+00000860: 6172 6368 2073 7061 6365 2ee9 0200 0000  arch space......
+00000870: da0d 6d61 785f 6465 7074 685f 6d69 6ee9  ..max_depth_min.
+00000880: 0600 0000 da0d 6d61 785f 6465 7074 685f  ......max_depth_
+00000890: 6d61 7867 0000 0000 0000 0000 da09 616c  maxg..........al
+000008a0: 7068 615f 6d69 6e67 0000 0000 0000 2440  pha_ming......$@
+000008b0: da09 616c 7068 615f 6d61 78da 0a6c 616d  ..alpha_max..lam
+000008c0: 6264 615f 6d69 6eda 0a6c 616d 6264 615f  bda_min..lambda_
+000008d0: 6d61 78da 0e6e 756d 5f6c 6561 7665 735f  max..num_leaves_
+000008e0: 6d69 6ee9 4000 0000 da0e 6e75 6d5f 6c65  min.@.....num_le
+000008f0: 6176 6573 5f6d 6178 6733 3333 3333 33d3  aves_maxg333333.
+00000900: 3fda 0e73 7562 5f73 616d 706c 655f 6d69  ?..sub_sample_mi
+00000910: 6e67 0000 0000 0000 f03f da0e 7375 625f  ng.......?..sub_
+00000920: 7361 6d70 6c65 5f6d 6178 da16 636f 6c5f  sample_max..col_
+00000930: 7361 6d70 6c65 5f62 795f 7472 6565 5f6d  sample_by_tree_m
+00000940: 696e da16 636f 6c5f 7361 6d70 6c65 5f62  in..col_sample_b
+00000950: 795f 7472 6565 5f6d 6178 da17 636f 6c5f  y_tree_max..col_
+00000960: 7361 6d70 6c65 5f62 795f 6c65 7665 6c5f  sample_by_level_
+00000970: 6d69 6eda 1763 6f6c 5f73 616d 706c 655f  min..col_sample_
+00000980: 6279 5f6c 6576 656c 5f6d 6178 da14 6d69  by_level_max..mi
+00000990: 6e5f 6368 696c 645f 7765 6967 6874 5f6d  n_child_weight_m
+000009a0: 696e da14 6d69 6e5f 6368 696c 645f 7765  in..min_child_we
+000009b0: 6967 6874 5f6d 6178 67fc a9f1 d24d 6250  ight_maxg....MbP
+000009c0: 3fda 0765 7461 5f6d 696e da07 6574 615f  ?..eta_min..eta_
+000009d0: 6d61 78da 0973 7465 7073 5f6d 696e e9e8  max..steps_min..
+000009e0: 0300 00da 0973 7465 7073 5f6d 6178 7201  .....steps_maxr.
+000009f0: 0000 00da 0f6d 6f64 656c 5f76 6572 626f  .....model_verbo
+00000a00: 7369 7479 fa0e 6d75 6c74 693a 736f 6674  sity..multi:soft
+00000a10: 7072 6f62 da0f 6d6f 6465 6c5f 6f62 6a65  prob..model_obje
+00000a20: 6374 6976 65da 086d 6c6f 676c 6f73 73da  ctive..mlogloss.
+00000a30: 116d 6f64 656c 5f65 7661 6c5f 6d65 7472  .model_eval_metr
+00000a40: 6963 da06 6762 7472 6565 da07 626f 6f73  ic..gbtree..boos
+00000a50: 7465 724e 2920 7206 0000 0072 0700 0000  terN) r....r....
+00000a60: 7208 0000 0072 2000 0000 7227 0000 0072  r....r ...r'...r
+00000a70: 2100 0000 7222 0000 0072 2900 0000 722a  !...r"...r)...r*
+00000a80: 0000 0072 2400 0000 722b 0000 0072 2c00  ...r$...r+...r,.
+00000a90: 0000 722d 0000 0072 2e00 0000 7230 0000  ..r-...r....r0..
+00000aa0: 0072 3100 0000 7232 0000 0072 3300 0000  .r1...r2...r3...
+00000ab0: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
+00000ac0: 3700 0000 7238 0000 0072 3900 0000 723a  7...r8...r9...r:
+00000ad0: 0000 0072 3b00 0000 723d 0000 0072 3e00  ...r;...r=...r>.
+00000ae0: 0000 7240 0000 00da 0373 7472 7242 0000  ..r@.....strrB..
+00000af0: 0072 4400 0000 720a 0000 0072 0a00 0000  .rD...r....r....
+00000b00: 720a 0000 0072 0b00 0000 7225 0000 0025  r....r....r%...%
+00000b10: 0000 0073 3200 0000 0a02 0402 0c01 0c01  ...s2...........
+00000b20: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
 00000b30: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000b40: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 1001  ................
-00000b50: 7224 0000 0063 0000 0000 0000 0000 0000  r$...c..........
-00000b60: 0000 0000 0000 0400 0000 4000 0000 73a0  ..........@...s.
-00000b70: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000b80: 0369 0064 0264 0393 0164 0464 0593 0164  .i.d.d...d.d...d
-00000b90: 0664 0793 0164 0864 0993 0164 0a64 0b93  .d...d.d...d.d..
-00000ba0: 0164 0c64 0d93 0164 0e64 0f93 0164 1064  .d.d...d.d...d.d
-00000bb0: 0f93 0164 1164 1293 0164 1364 1493 0164  ...d.d...d.d...d
-00000bc0: 1564 1493 0164 1664 1493 0164 1764 1493  .d...d.d...d.d..
-00000bd0: 0164 1864 1993 0164 1a64 0f93 0164 1b64  .d.d...d.d...d.d
-00000be0: 1c93 0164 1d64 1e93 015a 0464 1f5a 0565  ...d.d...Z.d.Z.e
-00000bf0: 0665 0765 0865 0966 0219 0019 0065 0a64  .e.e.e.f.....e.d
-00000c00: 203c 0064 215a 0b65 0965 0a64 223c 0064   <.d!Z.e.e.d"<.d
-00000c10: 1f53 0029 23da 1758 6762 6f6f 7374 4669  .S.)#..XgboostFi
-00000c20: 6e61 6c50 6172 616d 436f 6e66 6967 7a1e  nalParamConfigz.
-00000c30: 4465 6669 6e65 2066 696e 616c 2068 7970  Define final hyp
-00000c40: 6572 2070 6172 616d 6574 6572 732e da09  er parameters...
-00000c50: 6f62 6a65 6374 6976 6572 3e00 0000 da0b  objectiver>.....
-00000c60: 6576 616c 5f6d 6574 7269 6372 4000 0000  eval_metricr@...
-00000c70: da07 7665 7262 6f73 6572 0100 0000 da0b  ..verboser......
-00000c80: 7472 6565 5f6d 6574 686f 64da 0565 7861  tree_method..exa
-00000c90: 6374 da09 6e75 6d5f 636c 6173 7372 2500  ct..num_classr%.
-00000ca0: 0000 da09 6d61 785f 6465 7074 68e9 0300  ....max_depth...
-00000cb0: 0000 da05 616c 7068 6167 9a99 9999 9999  ....alphag......
-00000cc0: b93f da06 6c61 6d62 6461 da0a 6e75 6d5f  .?..lambda..num_
-00000cd0: 6c65 6176 6573 e910 0000 00da 0973 7562  leaves.......sub
-00000ce0: 7361 6d70 6c65 7218 0000 00da 1063 6f6c  sampler......col
-00000cf0: 7361 6d70 6c65 5f62 7974 7265 65da 1163  sample_bytree..c
-00000d00: 6f6c 7361 6d70 6c65 5f62 796c 6576 656c  olsample_bylevel
-00000d10: da10 636f 6c73 616d 706c 655f 6279 6e6f  ..colsample_byno
-00000d20: 6465 da11 6d69 6e5f 6368 696c 645f 7361  de..min_child_sa
-00000d30: 6d70 6c65 7372 0f00 0000 da03 6574 61da  mplesr......eta.
-00000d40: 0573 7465 7073 723b 0000 00da 116e 756d  .stepsr;.....num
-00000d50: 5f70 6172 616c 6c65 6c5f 7472 6565 7212  _parallel_treer.
-00000d60: 0000 004e da0d 7361 6d70 6c65 5f77 6569  ...N..sample_wei
-00000d70: 6768 7467 0000 0000 0000 e03f da18 636c  ghtg.......?..cl
-00000d80: 6173 7369 6669 6361 7469 6f6e 5f74 6872  assification_thr
-00000d90: 6573 686f 6c64 290c 7206 0000 0072 0700  eshold).r....r..
-00000da0: 0000 7208 0000 0072 1f00 0000 da06 7061  ..r....r......pa
-00000db0: 7261 6d73 725a 0000 0072 0300 0000 7202  ramsrZ...r....r.
-00000dc0: 0000 0072 4400 0000 7223 0000 0072 2100  ...rD...r#...r!.
-00000dd0: 0000 725b 0000 0072 0900 0000 7209 0000  ..r[...r....r...
-00000de0: 0072 0900 0000 720a 0000 0072 4500 0000  .r....r....rE...
-00000df0: 4300 0000 734e 0000 000a 0004 0202 0204  C...sN..........
-00000e00: 0102 ff04 0202 fe04 0302 fd04 0402 fc04  ................
-00000e10: 0502 fb04 0602 fa04 0702 f904 0802 f804  ................
-00000e20: 0902 f704 0a02 f604 0b02 f504 0c02 f404  ................
-00000e30: 0d02 f304 0e02 f204 0f02 f104 1002 f004  ................
-00000e40: 1104 ef18 1310 0172 4500 0000 4e29 0a72  .......rE...N).r
-00000e50: 1f00 0000 da06 7479 7069 6e67 7202 0000  ......typingr...
-00000e60: 0072 0300 0000 5a14 7079 6461 6e74 6963  .r....Z.pydantic
-00000e70: 2e64 6174 6163 6c61 7373 6573 7204 0000  .dataclassesr...
-00000e80: 0072 0500 0000 720b 0000 0072 2400 0000  .r....r....r$...
-00000e90: 7245 0000 0072 0900 0000 7209 0000 0072  rE...r....r....r
-00000ea0: 0900 0000 720a 0000 00da 083c 6d6f 6475  ....r......<modu
-00000eb0: 6c65 3e01 0000 0073 1400 0000 0400 1007  le>....s........
-00000ec0: 0c02 0e03 0204 1001 0213 1001 021d 1401  ................
+00000b40: 0c01 0c01 0c01 0c01 0c01 7225 0000 0063  ..........r%...c
+00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b60: 1200 0000 4000 0000 735e 0000 0065 005a  ....@...s^...e.Z
+00000b70: 0164 005a 0255 0064 015a 0364 0264 0364  .d.Z.U.d.Z.d.d.d
+00000b80: 0464 0564 0664 0764 0864 0864 0964 0a64  .d.d.d.d.d.d.d.d
+00000b90: 0a64 0a64 0a64 0b64 0864 0c64 0d64 0e9c  .d.d.d.d.d.d.d..
+00000ba0: 115a 0464 0f5a 0565 0665 0765 0865 0966  .Z.d.Z.e.e.e.e.f
+00000bb0: 0219 0019 0065 0a64 103c 0064 115a 0b65  .....e.d.<.d.Z.e
+00000bc0: 0965 0a64 123c 0064 0f53 0029 13da 1758  .e.d.<.d.S.)...X
+00000bd0: 6762 6f6f 7374 4669 6e61 6c50 6172 616d  gboostFinalParam
+00000be0: 436f 6e66 6967 7a1e 4465 6669 6e65 2066  Configz.Define f
+00000bf0: 696e 616c 2068 7970 6572 2070 6172 616d  inal hyper param
+00000c00: 6574 6572 732e 723f 0000 0072 4100 0000  eters.r?...rA...
+00000c10: 7201 0000 00da 0565 7861 6374 7226 0000  r......exactr&..
+00000c20: 00e9 0300 0000 679a 9999 9999 99b9 3fe9  ......g.......?.
+00000c30: 1000 0000 7219 0000 0072 1000 0000 723c  ....r....r....r<
+00000c40: 0000 0072 1300 0000 2911 da09 6f62 6a65  ...r....)...obje
+00000c50: 6374 6976 65da 0b65 7661 6c5f 6d65 7472  ctive..eval_metr
+00000c60: 6963 da07 7665 7262 6f73 65da 0b74 7265  ic..verbose..tre
+00000c70: 655f 6d65 7468 6f64 da09 6e75 6d5f 636c  e_method..num_cl
+00000c80: 6173 73da 096d 6178 5f64 6570 7468 da05  ass..max_depth..
+00000c90: 616c 7068 61da 066c 616d 6264 61da 0a6e  alpha..lambda..n
+00000ca0: 756d 5f6c 6561 7665 73da 0973 7562 7361  um_leaves..subsa
+00000cb0: 6d70 6c65 da10 636f 6c73 616d 706c 655f  mple..colsample_
+00000cc0: 6279 7472 6565 da11 636f 6c73 616d 706c  bytree..colsampl
+00000cd0: 655f 6279 6c65 7665 6cda 1063 6f6c 7361  e_bylevel..colsa
+00000ce0: 6d70 6c65 5f62 796e 6f64 65da 116d 696e  mple_bynode..min
+00000cf0: 5f63 6869 6c64 5f73 616d 706c 6573 da03  _child_samples..
+00000d00: 6574 61da 0573 7465 7073 da11 6e75 6d5f  eta..steps..num_
+00000d10: 7061 7261 6c6c 656c 5f74 7265 654e da0d  parallel_treeN..
+00000d20: 7361 6d70 6c65 5f77 6569 6768 7467 0000  sample_weightg..
+00000d30: 0000 0000 e03f da18 636c 6173 7369 6669  .....?..classifi
+00000d40: 6361 7469 6f6e 5f74 6872 6573 686f 6c64  cation_threshold
+00000d50: 290c 7206 0000 0072 0700 0000 7208 0000  ).r....r....r...
+00000d60: 0072 2000 0000 da06 7061 7261 6d73 725b  .r .....paramsr[
+00000d70: 0000 0072 0300 0000 7202 0000 0072 4500  ...r....r....rE.
+00000d80: 0000 7224 0000 0072 2200 0000 725c 0000  ..r$...r"...r\..
+00000d90: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00000da0: 720b 0000 0072 4600 0000 4300 0000 732a  r....rF...C...s*
+00000db0: 0000 000a 0204 0302 0102 0102 0102 0102  ................
+00000dc0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000dd0: 0102 0102 0102 0102 ef06 1318 0172 4600  .............rF.
+00000de0: 0000 4e29 0a72 2000 0000 da06 7479 7069  ..N).r .....typi
+00000df0: 6e67 7202 0000 0072 0300 0000 da14 7079  ngr....r......py
+00000e00: 6461 6e74 6963 2e64 6174 6163 6c61 7373  dantic.dataclass
+00000e10: 6573 7204 0000 0072 0500 0000 720c 0000  esr....r....r...
+00000e20: 0072 2500 0000 7246 0000 0072 0a00 0000  .r%...rF...r....
+00000e30: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
+00000e40: 083c 6d6f 6475 6c65 3e01 0000 0073 1200  .<module>....s..
+00000e50: 0000 0407 1002 0c03 0e04 0201 1013 0201  ................
+00000e60: 101d 0201                                ....
```

### Comparing `bluecast-0.8/bluecast/config/training_config.py` & `bluecast-0.9/bluecast/config/training_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         custom ML model is passed.
     :param hypertuning_cv_folds: Number of cross-validation folds to use for hyperparameter tuning. Not used when
         custom ML model is passed.
     :param early_stopping_rounds: Number of early stopping rounds. Not used when custom ML model is passed.
     :param autotune_model: Whether to autotune the model. Not used when custom ML model is passed.
     :param enable_feature_selection: Whether to enable recursive feature selection.
     :param calculate_shap_values: Whether to calculate shap values. Also used when custom ML model is passed. Not
-    compatible with all ML models. See SHAP documentation for more details.
+        compatible with all ML models. See the SHAP documentation for more details.
     :param train_size: Train size to use for train-test split.
     :param train_split_stratify: Whether to stratify the train-test split. Not used when custom ML model is passed.
     :param use_full_data_for_final_model: Whether to use the full data for the final model. This might cause overfitting.
     Not used when custom ML model is passed.
     :param min_features_to_select: Minimum number of features to select. Only used when enable_feature_selection is
         True.
     :param cat_encoding_via_ml_algorithm: Whether to use an ML algorithm for categorical encoding. If True, the
```

### Comparing `bluecast-0.8/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc` & `bluecast-0.9/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc` & `bluecast-0.9/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc` & `bluecast-0.9/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc` & `bluecast-0.9/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/evaluation/eval_metrics.py` & `bluecast-0.9/bluecast/evaluation/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/evaluation/shap_values.py` & `bluecast-0.9/bluecast/evaluation/shap_values.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc` & `bluecast-0.9/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc` & `bluecast-0.9/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/general_utils/general_utils.py` & `bluecast-0.9/bluecast/general_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc` & `bluecast-0.9/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc` & `bluecast-0.9/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc` & `bluecast-0.9/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul  3 13:07:54 2023 UTC, .py size: 14435 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2ac8 a264 6338 0000  o.......*..dc8..
+00000000: 6f0d 0d0a 0000 0000 ab08 a564 6338 0000  o..........dc8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 5a09 6401 6404 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
```

### Comparing `bluecast-0.8/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc` & `bluecast-0.9/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/ml_modelling/base_classes.py` & `bluecast-0.9/bluecast/ml_modelling/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/ml_modelling/xgboost.py` & `bluecast-0.9/bluecast/ml_modelling/xgboost.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc` & `bluecast-0.9/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/custom.py` & `bluecast-0.9/bluecast/preprocessing/custom.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/datetime_features.py` & `bluecast-0.9/bluecast/preprocessing/datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/encode_target_labels.py` & `bluecast-0.9/bluecast/preprocessing/encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/feature_selection.py` & `bluecast-0.9/bluecast/preprocessing/feature_selection.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/feature_types.py` & `bluecast-0.9/bluecast/preprocessing/feature_types.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/nulls_and_infs.py` & `bluecast-0.9/bluecast/preprocessing/nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/schema_checks.py` & `bluecast-0.9/bluecast/preprocessing/schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/target_encoding.py` & `bluecast-0.9/bluecast/preprocessing/target_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/preprocessing/train_test_split.py` & `bluecast-0.9/bluecast/preprocessing/train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 06:22:16 2023 UTC, .py size: 1176 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,113 +1,144 @@
-00000000: 6f0d 0d0a 0000 0000 9874 9e64 9804 0000  o........t.d....
+00000000: 6f0d 0d0a 0000 0000 a043 a664 a806 0000  o........C.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a09 6400 6401  Z...d.d.l.Z.d.d.
 00000060: 6c0a 5a0a 6400 6403 6c0b 6d0c 5a0c 6d0d  l.Z.d.d.l.m.Z.m.
-00000070: 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6400 6404  Z.m.Z.m.Z...d.d.
-00000080: 6c10 6d11 5a11 0100 650a 6a12 6405 6507  l.m.Z...e.j.d.e.
-00000090: 6509 6a13 6509 6a13 6602 1900 6602 6406  e.j.e.j.f...f.d.
-000000a0: 6407 8404 8301 5a14 6408 6409 8400 5a15  d.....Z.d.d...Z.
-000000b0: 640a 640b 8400 5a16 640c 640d 8400 5a17  d.d...Z.d.d...Z.
-000000c0: 640e 640f 8400 5a18 6401 5300 2910 e900  d.d...Z.d.S.)...
-000000d0: 0000 004e 2901 da05 5475 706c 6529 04da  ...N)...Tuple)..
-000000e0: 1062 695f 7661 7269 6174 655f 706c 6f74  .bi_variate_plot
-000000f0: 73da 1363 6f72 7265 6c61 7469 6f6e 5f68  s..correlation_h
-00000100: 6561 746d 6170 da15 636f 7272 656c 6174  eatmap..correlat
-00000110: 696f 6e5f 746f 5f74 6172 6765 74da 1075  ion_to_target..u
-00000120: 6e69 7661 7269 6174 655f 706c 6f74 73a9  nivariate_plots.
-00000130: 01da 1a63 7265 6174 655f 7379 6e74 6865  ...create_synthe
-00000140: 7469 635f 6461 7461 6672 616d 65da 0672  tic_dataframe..r
-00000150: 6574 7572 6e63 0000 0000 0000 0000 0000  eturnc..........
-00000160: 0000 0200 0000 0400 0000 4300 0000 7320  ..........C...s 
-00000170: 0000 0074 0064 0164 0264 038d 027d 0074  ...t.d.d.d...}.t
-00000180: 0064 0164 0464 038d 027d 017c 007c 0166  .d.d.d...}.|.|.f
-00000190: 0253 0029 054e 69d0 0700 00e9 1400 0000  .S.).Ni.........
-000001a0: 2901 5a0c 7261 6e64 6f6d 5f73 7461 7465  ).Z.random_state
-000001b0: e9c8 0000 0072 0700 0000 2902 5a08 6466  .....r....).Z.df
-000001c0: 5f74 7261 696e 5a06 6466 5f76 616c a900  _trainZ.df_val..
-000001d0: 720c 0000 00fa 412f 686f 6d65 2f74 686f  r.....A/home/tho
-000001e0: 6d61 732f 4964 6561 5072 6f6a 6563 7473  mas/IdeaProjects
-000001f0: 2f42 6c75 6543 6173 742f 626c 7565 6361  /BlueCast/blueca
-00000200: 7374 2f74 6573 7473 2f74 6573 745f 616e  st/tests/test_an
-00000210: 616c 7973 652e 7079 da19 7379 6e74 6865  alyse.py..synthe
-00000220: 7469 635f 7472 6169 6e5f 7465 7374 5f64  tic_train_test_d
-00000230: 6174 610f 0000 0073 0600 0000 0c02 0c01  ata....s........
-00000240: 0801 720e 0000 0063 0100 0000 0000 0000  ..r....c........
-00000250: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
-00000260: 7350 0000 0074 007c 0064 0119 006a 0164  sP...t.|.d...j.d
-00000270: 0064 0085 0267 0064 02a2 0166 0219 0064  .d...g.d...f...d
-00000280: 0383 0201 0064 047d 017c 0173 2464 0564  .....d.}.|.s$d.d
-00000290: 0674 02a0 037c 01a1 0169 0116 007d 0274  .t...|...i...}.t
-000002a0: 0474 02a0 057c 02a1 0183 0182 0164 007d  .t...|.......d.}
-000002b0: 0164 0053 0029 074e 7201 0000 0029 035a  .d.S.).Nr....).Z
-000002c0: 136e 756d 6572 6963 616c 5f66 6561 7475  .numerical_featu
-000002d0: 7265 5f31 5a13 6e75 6d65 7269 6361 6c5f  re_1Z.numerical_
-000002e0: 6665 6174 7572 655f 325a 136e 756d 6572  feature_2Z.numer
-000002f0: 6963 616c 5f66 6561 7475 7265 5f33 da06  ical_feature_3..
-00000300: 7461 7267 6574 54fa 0e61 7373 6572 7420  targetT..assert 
-00000310: 2528 7079 3129 73da 0370 7931 2906 7206  %(py1)s..py1).r.
-00000320: 0000 00da 036c 6f63 da0a 4070 7974 6573  .....loc..@pytes
-00000330: 745f 6172 da09 5f73 6166 6572 6570 72da  t_ar.._saferepr.
-00000340: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000350: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
-00000360: 7469 6f6e a903 720e 0000 005a 0b40 7079  tion..r....Z.@py
-00000370: 5f61 7373 6572 7430 5a0b 4070 795f 666f  _assert0Z.@py_fo
-00000380: 726d 6174 3272 0c00 0000 720c 0000 0072  rmat2r....r....r
-00000390: 0d00 0000 da15 7465 7374 5f75 6e69 7661  ......test_univa
-000003a0: 7269 6174 655f 706c 6f74 7316 0000 0073  riate_plots....s
-000003b0: 0e00 0000 0201 0801 0e01 02ff 0203 04fc  ................
-000003c0: 3006 7218 0000 0063 0100 0000 0000 0000  0.r....c........
-000003d0: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
-000003e0: f33e 0000 0074 007c 0064 0119 0064 0283  .>...t.|.d...d..
-000003f0: 0201 0064 037d 017c 0173 1b64 0464 0574  ...d.}.|.s.d.d.t
-00000400: 01a0 027c 01a1 0169 0116 007d 0274 0374  ...|...i...}.t.t
-00000410: 01a0 047c 02a1 0183 0182 0164 007d 0164  ...|.......d.}.d
-00000420: 0053 00a9 064e 7201 0000 0072 0f00 0000  .S...Nr....r....
-00000430: 5472 1000 0000 7211 0000 0029 0572 0300  Tr....r....).r..
-00000440: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000450: 0072 1600 0000 7217 0000 0072 0c00 0000  .r....r....r....
-00000460: 720c 0000 0072 0d00 0000 da15 7465 7374  r....r......test
-00000470: 5f62 695f 7661 7269 6174 655f 706c 6f74  _bi_variate_plot
-00000480: 7320 0000 00f3 0400 0000 0e01 3001 721b  s ..........0.r.
-00000490: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000004a0: 0300 0000 0500 0000 4300 0000 733c 0000  ........C...s<..
-000004b0: 0074 007c 0064 0119 0083 0101 0064 027d  .t.|.d.......d.}
-000004c0: 017c 0173 1a64 0364 0474 01a0 027c 01a1  .|.s.d.d.t...|..
-000004d0: 0169 0116 007d 0274 0374 01a0 047c 02a1  .i...}.t.t...|..
-000004e0: 0183 0182 0164 007d 0164 0053 0029 054e  .....d.}.d.S.).N
-000004f0: 7201 0000 0054 7210 0000 0072 1100 0000  r....Tr....r....
-00000500: 2905 7204 0000 0072 1300 0000 7214 0000  ).r....r....r...
-00000510: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000520: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000530: 1874 6573 745f 636f 7272 656c 6174 696f  .test_correlatio
-00000540: 6e5f 6865 6174 6d61 7025 0000 0073 0400  n_heatmap%...s..
-00000550: 0000 0c01 3001 721d 0000 0063 0100 0000  ....0.r....c....
-00000560: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00000570: 4300 0000 7219 0000 0072 1a00 0000 2905  C...r....r....).
-00000580: 7205 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000590: 1500 0000 7216 0000 0072 1700 0000 720c  ....r....r....r.
-000005a0: 0000 0072 0c00 0000 720d 0000 00da 1a74  ...r....r......t
-000005b0: 6573 745f 636f 7272 656c 6174 696f 6e5f  est_correlation_
-000005c0: 746f 5f74 6172 6765 742a 0000 0072 1c00  to_target*...r..
-000005d0: 0000 721e 0000 0029 19da 0862 7569 6c74  ..r....)...built
-000005e0: 696e 73da 0c40 7079 5f62 7569 6c74 696e  ins..@py_builtin
-000005f0: 73da 195f 7079 7465 7374 2e61 7373 6572  s.._pytest.asser
-00000600: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
-00000610: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
-00000620: 7213 0000 00da 0674 7970 696e 6772 0200  r......typingr..
-00000630: 0000 5a06 7061 6e64 6173 da02 7064 da06  ..Z.pandas..pd..
-00000640: 7079 7465 7374 5a14 626c 7565 6361 7374  pytestZ.bluecast
-00000650: 2e65 6461 2e61 6e61 6c79 7365 7203 0000  .eda.analyser...
-00000660: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-00000670: 5a24 626c 7565 6361 7374 2e74 6573 7473  Z$bluecast.tests
-00000680: 2e6d 616b 655f 6461 7461 2e63 7265 6174  .make_data.creat
-00000690: 655f 6461 7461 7208 0000 00da 0766 6978  e_datar......fix
-000006a0: 7475 7265 5a09 4461 7461 4672 616d 6572  tureZ.DataFramer
-000006b0: 0e00 0000 7218 0000 0072 1b00 0000 721d  ....r....r....r.
-000006c0: 0000 0072 1e00 0000 720c 0000 0072 0c00  ...r....r....r..
-000006d0: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
-000006e0: 6f64 756c 653e 0100 0000 7316 0000 0026  odule>....s....&
-000006f0: 0008 0208 0118 020c 0604 031c 0108 0608  ................
-00000700: 0a08 050c 05                             .....
+00000070: 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11  Z.m.Z.m.Z.m.Z.m.
+00000080: 5a11 0100 6400 6404 6c12 6d13 5a13 0100  Z...d.d.l.m.Z...
+00000090: 650a 6a14 6405 6507 6509 6a15 6509 6a15  e.j.d.e.e.j.e.j.
+000000a0: 6602 1900 6602 6406 6407 8404 8301 5a16  f...f.d.d.....Z.
+000000b0: 6408 6409 8400 5a17 640a 640b 8400 5a18  d.d...Z.d.d...Z.
+000000c0: 640c 640d 8400 5a19 640e 640f 8400 5a1a  d.d...Z.d.d...Z.
+000000d0: 6410 6411 8400 5a1b 6412 6413 8400 5a1c  d.d...Z.d.d...Z.
+000000e0: 6401 5300 2914 e900 0000 004e 2901 da05  d.S.)......N)...
+000000f0: 5475 706c 6529 06da 1062 695f 7661 7269  Tuple)...bi_vari
+00000100: 6174 655f 706c 6f74 73da 1363 6f72 7265  ate_plots..corre
+00000110: 6c61 7469 6f6e 5f68 6561 746d 6170 da15  lation_heatmap..
+00000120: 636f 7272 656c 6174 696f 6e5f 746f 5f74  correlation_to_t
+00000130: 6172 6765 74da 0870 6c6f 745f 7063 61da  arget..plot_pca.
+00000140: 0970 6c6f 745f 7473 6e65 da10 756e 6976  .plot_tsne..univ
+00000150: 6172 6961 7465 5f70 6c6f 7473 a901 da1a  ariate_plots....
+00000160: 6372 6561 7465 5f73 796e 7468 6574 6963  create_synthetic
+00000170: 5f64 6174 6166 7261 6d65 da06 7265 7475  _dataframe..retu
+00000180: 726e 6300 0000 0000 0000 0000 0000 0002  rnc.............
+00000190: 0000 0004 0000 0043 0000 0073 2000 0000  .......C...s ...
+000001a0: 7400 6401 6402 6403 8d02 7d00 7400 6401  t.d.d.d...}.t.d.
+000001b0: 6404 6403 8d02 7d01 7c00 7c01 6602 5300  d.d...}.|.|.f.S.
+000001c0: 2905 4e69 d007 0000 e914 0000 0029 01da  ).Ni.........)..
+000001d0: 0c72 616e 646f 6d5f 7374 6174 65e9 c800  .random_state...
+000001e0: 0000 7209 0000 0029 025a 0864 665f 7472  ..r....).Z.df_tr
+000001f0: 6169 6e5a 0664 665f 7661 6ca9 0072 0f00  ainZ.df_val..r..
+00000200: 0000 fa41 2f68 6f6d 652f 7468 6f6d 6173  ...A/home/thomas
+00000210: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
+00000220: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
+00000230: 7465 7374 732f 7465 7374 5f61 6e61 6c79  tests/test_analy
+00000240: 7365 2e70 79da 1973 796e 7468 6574 6963  se.py..synthetic
+00000250: 5f74 7261 696e 5f74 6573 745f 6461 7461  _train_test_data
+00000260: 1100 0000 7306 0000 000c 020c 0108 0172  ....s..........r
+00000270: 1100 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000280: 0003 0000 0005 0000 0043 0000 00f3 5000  .........C....P.
+00000290: 0000 7400 7c00 6401 1900 6a01 6400 6400  ..t.|.d...j.d.d.
+000002a0: 8502 6700 6402 a201 6602 1900 6403 8302  ..g.d...f...d...
+000002b0: 0100 6404 7d01 7c01 7324 6405 6406 7402  ..d.}.|.s$d.d.t.
+000002c0: a003 7c01 a101 6901 1600 7d02 7404 7402  ..|...i...}.t.t.
+000002d0: a005 7c02 a101 8301 8201 6400 7d01 6400  ..|.......d.}.d.
+000002e0: 5300 2907 4e72 0100 0000 2903 da13 6e75  S.).Nr....)...nu
+000002f0: 6d65 7269 6361 6c5f 6665 6174 7572 655f  merical_feature_
+00000300: 31da 136e 756d 6572 6963 616c 5f66 6561  1..numerical_fea
+00000310: 7475 7265 5f32 da13 6e75 6d65 7269 6361  ture_2..numerica
+00000320: 6c5f 6665 6174 7572 655f 33da 0674 6172  l_feature_3..tar
+00000330: 6765 7454 fa0e 6173 7365 7274 2025 2870  getT..assert %(p
+00000340: 7931 2973 da03 7079 3129 0672 0800 0000  y1)s..py1).r....
+00000350: da03 6c6f 63da 0a40 7079 7465 7374 5f61  ..loc..@pytest_a
+00000360: 72da 095f 7361 6665 7265 7072 da0e 4173  r.._saferepr..As
+00000370: 7365 7274 696f 6e45 7272 6f72 da13 5f66  sertionError.._f
+00000380: 6f72 6d61 745f 6578 706c 616e 6174 696f  ormat_explanatio
+00000390: 6ea9 0372 1100 0000 5a0b 4070 795f 6173  n..r....Z.@py_as
+000003a0: 7365 7274 305a 0b40 7079 5f66 6f72 6d61  sert0Z.@py_forma
+000003b0: 7432 720f 0000 0072 0f00 0000 7210 0000  t2r....r....r...
+000003c0: 00da 1574 6573 745f 756e 6976 6172 6961  ...test_univaria
+000003d0: 7465 5f70 6c6f 7473 1800 0000 730e 0000  te_plots....s...
+000003e0: 0002 0108 010e 0102 ff02 0304 fc30 0672  .............0.r
+000003f0: 1f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000400: 0003 0000 0005 0000 0043 0000 00f3 3e00  .........C....>.
+00000410: 0000 7400 7c00 6401 1900 6402 8302 0100  ..t.|.d...d.....
+00000420: 6403 7d01 7c01 731b 6404 6405 7401 a002  d.}.|.s.d.d.t...
+00000430: 7c01 a101 6901 1600 7d02 7403 7401 a004  |...i...}.t.t...
+00000440: 7c02 a101 8301 8201 6400 7d01 6400 5300  |.......d.}.d.S.
+00000450: a906 4e72 0100 0000 7216 0000 0054 7217  ..Nr....r....Tr.
+00000460: 0000 0072 1800 0000 2905 7203 0000 0072  ...r....).r....r
+00000470: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
+00000480: 0000 0072 1e00 0000 720f 0000 0072 0f00  ...r....r....r..
+00000490: 0000 7210 0000 00da 1574 6573 745f 6269  ..r......test_bi
+000004a0: 5f76 6172 6961 7465 5f70 6c6f 7473 2200  _variate_plots".
+000004b0: 0000 f304 0000 000e 0130 0172 2200 0000  .........0.r"...
+000004c0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+000004d0: 0005 0000 0043 0000 0073 3c00 0000 7400  .....C...s<...t.
+000004e0: 7c00 6401 1900 8301 0100 6402 7d01 7c01  |.d.......d.}.|.
+000004f0: 731a 6403 6404 7401 a002 7c01 a101 6901  s.d.d.t...|...i.
+00000500: 1600 7d02 7403 7401 a004 7c02 a101 8301  ..}.t.t...|.....
+00000510: 8201 6400 7d01 6400 5300 2905 4e72 0100  ..d.}.d.S.).Nr..
+00000520: 0000 5472 1700 0000 7218 0000 0029 0572  ..Tr....r....).r
+00000530: 0400 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00000540: 0000 0072 1d00 0000 721e 0000 0072 0f00  ...r....r....r..
+00000550: 0000 720f 0000 0072 1000 0000 da18 7465  ..r....r......te
+00000560: 7374 5f63 6f72 7265 6c61 7469 6f6e 5f68  st_correlation_h
+00000570: 6561 746d 6170 2700 0000 7304 0000 000c  eatmap'...s.....
+00000580: 0130 0172 2400 0000 6301 0000 0000 0000  .0.r$...c.......
+00000590: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
+000005a0: 0072 2000 0000 7221 0000 0029 0572 0500  .r ...r!...).r..
+000005b0: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+000005c0: 0072 1d00 0000 721e 0000 0072 0f00 0000  .r....r....r....
+000005d0: 720f 0000 0072 1000 0000 da1a 7465 7374  r....r......test
+000005e0: 5f63 6f72 7265 6c61 7469 6f6e 5f74 6f5f  _correlation_to_
+000005f0: 7461 7267 6574 2c00 0000 7223 0000 0072  target,...r#...r
+00000600: 2500 0000 6301 0000 0000 0000 0000 0000  %...c...........
+00000610: 0003 0000 0005 0000 0043 0000 0072 1200  .........C...r..
+00000620: 0000 2907 4e72 0100 0000 a904 7213 0000  ..).Nr......r...
+00000630: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000640: 7216 0000 0054 7217 0000 0072 1800 0000  r....Tr....r....
+00000650: 2906 7206 0000 0072 1900 0000 721a 0000  ).r....r....r...
+00000660: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00000670: 721e 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00000680: 1000 0000 da0d 7465 7374 5f70 6361 5f70  ......test_pca_p
+00000690: 6c6f 7431 0000 0073 0c00 0000 0a01 0e01  lot1...s........
+000006a0: 02ff 0202 04fe 3003 7227 0000 0063 0100  ......0.r'...c..
+000006b0: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+000006c0: 0000 4300 0000 7356 0000 0074 007c 0064  ..C...sV...t.|.d
+000006d0: 0119 006a 0164 0064 0085 0267 0064 02a2  ...j.d.d...g.d..
+000006e0: 0166 0219 0064 0364 0464 0164 058d 0401  .f...d.d.d.d....
+000006f0: 0064 067d 017c 0173 2764 0764 0874 02a0  .d.}.|.s'd.d.t..
+00000700: 037c 01a1 0169 0116 007d 0274 0474 02a0  .|...i...}.t.t..
+00000710: 057c 02a1 0183 0182 0164 007d 0164 0053  .|.......d.}.d.S
+00000720: 0029 094e 7201 0000 0072 2600 0000 7216  .).Nr....r&...r.
+00000730: 0000 00e9 1e00 0000 2902 5a0a 7065 7270  ........).Z.perp
+00000740: 6c65 7869 7479 720d 0000 0054 7217 0000  lexityr....Tr...
+00000750: 0072 1800 0000 2906 7207 0000 0072 1900  .r....).r....r..
+00000760: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000770: 0072 1d00 0000 721e 0000 0072 0f00 0000  .r....r....r....
+00000780: 720f 0000 0072 1000 0000 da0e 7465 7374  r....r......test
+00000790: 5f70 6c6f 745f 7473 6e65 3800 0000 730c  _plot_tsne8...s.
+000007a0: 0000 000a 010e 0102 ff06 0206 fe30 0372  .............0.r
+000007b0: 2900 0000 291d da08 6275 696c 7469 6e73  )...)...builtins
+000007c0: da0c 4070 795f 6275 696c 7469 6e73 da19  ..@py_builtins..
+000007d0: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
+000007e0: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
+000007f0: 7469 6f6e da07 7265 7772 6974 6572 1a00  tion..rewriter..
+00000800: 0000 da06 7479 7069 6e67 7202 0000 005a  ....typingr....Z
+00000810: 0670 616e 6461 73da 0270 64da 0670 7974  .pandas..pd..pyt
+00000820: 6573 745a 1462 6c75 6563 6173 742e 6564  estZ.bluecast.ed
+00000830: 612e 616e 616c 7973 6572 0300 0000 7204  a.analyser....r.
+00000840: 0000 0072 0500 0000 7206 0000 0072 0700  ...r....r....r..
+00000850: 0000 7208 0000 005a 2462 6c75 6563 6173  ..r....Z$bluecas
+00000860: 742e 7465 7374 732e 6d61 6b65 5f64 6174  t.tests.make_dat
+00000870: 612e 6372 6561 7465 5f64 6174 6172 0a00  a.create_datar..
+00000880: 0000 da07 6669 7874 7572 655a 0944 6174  ....fixtureZ.Dat
+00000890: 6146 7261 6d65 7211 0000 0072 1f00 0000  aFramer....r....
+000008a0: 7222 0000 0072 2400 0000 7225 0000 0072  r"...r$...r%...r
+000008b0: 2700 0000 7229 0000 0072 0f00 0000 720f  '...r)...r....r.
+000008c0: 0000 0072 0f00 0000 7210 0000 00da 083c  ...r....r......<
+000008d0: 6d6f 6475 6c65 3e01 0000 0073 1a00 0000  module>....s....
+000008e0: 2600 0802 0801 2002 0c08 0403 1c01 0806  &..... .........
+000008f0: 080a 0805 0805 0805 0c07                 ..........
```

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 06:22:16 2023 UTC, .py size: 6677 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9874 9e64 151a 0000  o........t.d....
+00000000: 6f0d 0d0a 0000 0000 ab2f a564 681d 0000  o......../.dh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a0a  Z.m.Z...d.d.l.Z.
 00000060: 6400 6401 6c0b 5a0c 6400 6401 6c0d 5a0d  d.d.l.Z.d.d.l.Z.
 00000070: 6400 6401 6c0e 5a0f 6400 6403 6c10 6d11  d.d.l.Z.d.d.l.m.
@@ -47,502 +47,545 @@
 000002e0: 6f6d 6173 2f49 6465 6150 726f 6a65 6374  omas/IdeaProject
 000002f0: 732f 426c 7565 4361 7374 2f62 6c75 6563  s/BlueCast/bluec
 00000300: 6173 742f 7465 7374 732f 7465 7374 5f63  ast/tests/test_c
 00000310: 6173 742e 7079 da19 7379 6e74 6865 7469  ast.py..syntheti
 00000320: 635f 7472 6169 6e5f 7465 7374 5f64 6174  c_train_test_dat
 00000330: 6117 0000 0073 0600 0000 0c02 0c01 0801  a....s..........
 00000340: 721a 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000350: 0000 1000 0000 0a00 0000 4300 0000 73d0  ..........C...s.
+00000350: 0000 0f00 0000 0a00 0000 4300 0000 73b2  ..........C...s.
 00000360: 0200 007c 0064 0119 007d 017c 0064 0219  ...|.d...}.|.d..
 00000370: 007d 0274 0083 007d 0364 037c 035f 0164  .}.t...}.d.|._.d
-00000380: 047c 035f 0274 0383 007d 0464 057c 045f  .|._.t...}.d.|._
-00000390: 0464 067c 045f 0564 027c 045f 0647 0064  .d.|._.d.|._.G.d
-000003a0: 0764 0884 0064 0874 0783 037d 057c 0583  .d...d.t...}.|..
-000003b0: 007d 0674 0864 0964 0a7c 047c 037c 0664  .}.t.d.d.|.|.|.d
-000003c0: 0b8d 057d 077c 076a 097c 017c 016a 0a64  ...}.|.j.|.|.j.d
-000003d0: 0a64 0264 0c8d 027c 0164 0a19 0064 0a64  .d.d...|.d...d.d
-000003e0: 0d8d 0401 0074 0b64 0e83 0101 007c 07a0  .....t.d.....|..
-000003f0: 0c7c 026a 0a64 0a64 0264 0c8d 02a1 015c  .|.j.d.d.d.....\
-00000400: 027d 087d 0974 0b64 0f83 0101 0074 0d7c  .}.}.t.d.....t.|
-00000410: 0883 017d 0a7c 026a 0e7d 0b74 0d7c 0b83  ...}.|.j.}.t.|..
-00000420: 017d 0c7c 0a7c 0c6b 027d 0d7c 0d73 d174  .}.|.|.k.}.|.s.t
-00000430: 0fa0 1064 107c 0d66 0164 117c 0a7c 0c66  ...d.|.f.d.|.|.f
-00000440: 02a1 0464 1274 11a0 12a1 0076 0073 7b74  ...d.t.....v.s{t
-00000450: 0fa0 1374 0da1 0172 8074 0fa0 1474 0da1  ...t...r.t...t..
-00000460: 016e 0164 1264 1374 11a0 12a1 0076 0073  .n.d.d.t.....v.s
-00000470: 8c74 0fa0 137c 08a1 0172 9174 0fa0 147c  .t...|...r.t...|
-00000480: 08a1 016e 0164 1374 0fa0 147c 0aa1 0164  ...n.d.t...|...d
-00000490: 1274 11a0 12a1 0076 0073 a174 0fa0 1374  .t.....v.s.t...t
-000004a0: 0da1 0172 a674 0fa0 1474 0da1 016e 0164  ...r.t...t...n.d
-000004b0: 1264 1474 11a0 12a1 0076 0073 b274 0fa0  .d.t.....v.s.t..
-000004c0: 137c 02a1 0172 b774 0fa0 147c 02a1 016e  .|...r.t...|...n
-000004d0: 0164 1474 0fa0 147c 0ba1 0174 0fa0 147c  .d.t...|...t...|
-000004e0: 0ca1 0164 159c 0716 007d 0e64 1664 177c  ...d.....}.d.d.|
-000004f0: 0e69 0116 007d 0f74 1574 0fa0 167c 0fa1  .i...}.t.t...|..
-00000500: 0183 0182 0164 1804 007d 0a04 007d 0d04  .....d...}...}..
-00000510: 007d 0b7d 0c74 0d7c 0983 017d 0a7c 026a  .}.}.t.|...}.|.j
-00000520: 0e7d 0b74 0d7c 0b83 017d 0c7c 0a7c 0c6b  .}.t.|...}.|.|.k
-00000530: 027d 0d7c 0d90 0173 5e74 0fa0 1064 107c  .}.|...s^t...d.|
-00000540: 0d66 0164 117c 0a7c 0c66 02a1 0464 1274  .f.d.|.|.f...d.t
-00000550: 11a0 12a1 0076 0090 0173 0274 0fa0 1374  .....v...s.t...t
-00000560: 0da1 0190 0172 0774 0fa0 1474 0da1 016e  .....r.t...t...n
-00000570: 0164 1264 1974 11a0 12a1 0076 0090 0173  .d.d.t.....v...s
-00000580: 1574 0fa0 137c 09a1 0190 0172 1a74 0fa0  .t...|.....r.t..
-00000590: 147c 09a1 016e 0164 1974 0fa0 147c 0aa1  .|...n.d.t...|..
-000005a0: 0164 1274 11a0 12a1 0076 0090 0173 2c74  .d.t.....v...s,t
-000005b0: 0fa0 1374 0da1 0190 0172 3174 0fa0 1474  ...t.....r1t...t
-000005c0: 0da1 016e 0164 1264 1474 11a0 12a1 0076  ...n.d.d.t.....v
-000005d0: 0090 0173 3f74 0fa0 137c 02a1 0190 0172  ...s?t...|.....r
-000005e0: 4474 0fa0 147c 02a1 016e 0164 1474 0fa0  Dt...|...n.d.t..
-000005f0: 147c 0ba1 0174 0fa0 147c 0ca1 0164 159c  .|...t...|...d..
-00000600: 0716 007d 0e64 1664 177c 0e69 0116 007d  ...}.d.d.|.i...}
-00000610: 0f74 1574 0fa0 167c 0fa1 0183 0182 0164  .t.t...|.......d
-00000620: 1804 007d 0a04 007d 0d04 007d 0b7d 0c64  ...}...}...}.}.d
-00000630: 1853 0029 1a7a 2254 6573 7420 7468 6174  .S.).z"Test that
-00000640: 2074 6573 7473 2074 6865 2042 6c75 6543   tests the BlueC
-00000650: 6173 7420 636c 6173 7372 0100 0000 e901  ast classr......
-00000660: 0000 00e9 6400 0000 e910 0000 00e9 0a00  ....d...........
-00000670: 0000 4663 0000 0000 0000 0000 0000 0000  ..Fc............
-00000680: 0000 0000 0c00 0000 4000 0000 7380 0000  ........@...s...
-00000690: 0065 005a 0164 005a 0264 0165 036a 0464  .e.Z.d.Z.d.e.j.d
-000006a0: 0265 036a 0466 0464 0364 0484 045a 0564  .e.j.f.d.d...Z.d
-000006b0: 0165 036a 0464 0565 036a 0664 0265 0765  .e.j.d.e.j.d.e.e
-000006c0: 036a 0465 036a 0666 0219 0066 0664 0664  .j.e.j.f...f.d.d
-000006d0: 0784 045a 0809 0809 0964 0d64 0165 036a  ...Z.....d.d.e.j
-000006e0: 0464 0565 0965 036a 0619 0064 0a65 0a64  .d.e.e.j...d.e.d
-000006f0: 0265 0765 036a 0465 0965 036a 0619 0066  .e.e.j.e.e.j...f
-00000700: 0219 0066 0864 0b64 0c84 055a 0b64 0853  ...f.d.d...Z.d.S
-00000710: 0029 0e7a 3d74 6573 745f 626c 7565 7072  .).z=test_bluepr
-00000720: 696e 745f 7867 626f 6f73 742e 3c6c 6f63  int_xgboost.<loc
-00000730: 616c 733e 2e4d 7943 7573 746f 6d4c 6173  als>.MyCustomLas
-00000740: 744d 696c 6550 7265 7072 6f63 6573 7369  tMilePreprocessi
-00000750: 6e67 da02 6466 7212 0000 0063 0200 0000  ng..dfr....c....
-00000760: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000770: 5300 0000 730c 0000 0064 017c 0164 023c  S...s....d.|.d.<
-00000780: 007c 0153 0029 034e e905 0000 005a 0a63  .|.S.).N.....Z.c
-00000790: 7573 746f 6d5f 636f 6c72 1800 0000 2902  ustom_colr....).
-000007a0: da04 7365 6c66 721f 0000 0072 1800 0000  ..selfr....r....
-000007b0: 7218 0000 0072 1900 0000 da0f 6375 7374  r....r......cust
-000007c0: 6f6d 5f66 756e 6374 696f 6e2c 0000 0073  om_function,...s
-000007d0: 0400 0000 0801 0401 7a4d 7465 7374 5f62  ........zMtest_b
-000007e0: 6c75 6570 7269 6e74 5f78 6762 6f6f 7374  lueprint_xgboost
-000007f0: 2e3c 6c6f 6361 6c73 3e2e 4d79 4375 7374  .<locals>.MyCust
-00000800: 6f6d 4c61 7374 4d69 6c65 5072 6570 726f  omLastMilePrepro
-00000810: 6365 7373 696e 672e 6375 7374 6f6d 5f66  cessing.custom_f
-00000820: 756e 6374 696f 6eda 0674 6172 6765 7463  unction..targetc
-00000830: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00000840: 0300 0000 5300 0000 7326 0000 007c 00a0  ....S...s&...|..
-00000850: 007c 01a1 017d 017c 01a0 0164 01a1 017d  .|...}.|...d...}
-00000860: 017c 02a0 0164 01a1 017d 027c 017c 0266  .|...d...}.|.|.f
-00000870: 0253 0029 024e 69e8 0300 0029 0272 2200  .S.).Ni....).r".
-00000880: 0000 da04 6865 6164 a903 7221 0000 0072  ....head..r!...r
-00000890: 1f00 0000 7223 0000 0072 1800 0000 7218  ....r#...r....r.
-000008a0: 0000 0072 1900 0000 da0d 6669 745f 7472  ...r......fit_tr
-000008b0: 616e 7366 6f72 6d30 0000 0073 0800 0000  ansform0...s....
-000008c0: 0a03 0a01 0a01 0801 7a4b 7465 7374 5f62  ........zKtest_b
-000008d0: 6c75 6570 7269 6e74 5f78 6762 6f6f 7374  lueprint_xgboost
-000008e0: 2e3c 6c6f 6361 6c73 3e2e 4d79 4375 7374  .<locals>.MyCust
-000008f0: 6f6d 4c61 7374 4d69 6c65 5072 6570 726f  omLastMilePrepro
-00000900: 6365 7373 696e 672e 6669 745f 7472 616e  cessing.fit_tran
-00000910: 7366 6f72 6d4e 46da 0e70 7265 6469 6374  sformNF..predict
-00000920: 6f6e 5f6d 6f64 6563 0400 0000 0000 0000  on_modec........
-00000930: 0000 0000 0400 0000 0300 0000 5300 0000  ............S...
-00000940: 7336 0000 007c 00a0 007c 01a1 017d 017c  s6...|...|...}.|
-00000950: 0373 1774 017c 0274 026a 0383 0272 177c  .s.t.|.t.j...r.|
-00000960: 01a0 0464 01a1 017d 017c 02a0 0464 01a1  ...d...}.|...d..
-00000970: 017d 027c 017c 0266 0253 0029 024e 721c  .}.|.|.f.S.).Nr.
-00000980: 0000 0029 0572 2200 0000 da0a 6973 696e  ...).r".....isin
-00000990: 7374 616e 6365 da02 7064 da06 5365 7269  stance..pd..Seri
-000009a0: 6573 7224 0000 00a9 0472 2100 0000 721f  esr$.....r!...r.
-000009b0: 0000 0072 2300 0000 7227 0000 0072 1800  ...r#...r'...r..
-000009c0: 0000 7218 0000 0072 1900 0000 da09 7472  ..r....r......tr
-000009d0: 616e 7366 6f72 6d38 0000 0073 0a00 0000  ansform8...s....
-000009e0: 0a06 1001 0a01 0a01 0801 7a47 7465 7374  ..........zGtest
-000009f0: 5f62 6c75 6570 7269 6e74 5f78 6762 6f6f  _blueprint_xgboo
-00000a00: 7374 2e3c 6c6f 6361 6c73 3e2e 4d79 4375  st.<locals>.MyCu
-00000a10: 7374 6f6d 4c61 7374 4d69 6c65 5072 6570  stomLastMilePrep
-00000a20: 726f 6365 7373 696e 672e 7472 616e 7366  rocessing.transf
-00000a30: 6f72 6da9 024e 4629 0cda 085f 5f6e 616d  orm..NF)...__nam
-00000a40: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000a50: 0c5f 5f71 7561 6c6e 616d 655f 5f72 2900  .__qualname__r).
-00000a60: 0000 da09 4461 7461 4672 616d 6572 2200  ....DataFramer".
-00000a70: 0000 722a 0000 0072 0300 0000 7226 0000  ..r*...r....r&..
-00000a80: 0072 0200 0000 da04 626f 6f6c 722c 0000  .r......boolr,..
-00000a90: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00000aa0: 7219 0000 00da 1d4d 7943 7573 746f 6d4c  r......MyCustomL
-00000ab0: 6173 744d 696c 6550 7265 7072 6f63 6573  astMilePreproces
-00000ac0: 7369 6e67 2b00 0000 7328 0000 0008 0016  sing+...s(......
-00000ad0: 0102 0404 0102 ff04 0102 ff0e 020a fe02  ................
-00000ae0: 0b02 0104 fc04 0202 fe08 0302 fd02 0402  ................
-00000af0: fc12 050e fb72 3300 0000 da06 6269 6e61  .....r3.....bina
-00000b00: 7279 7223 0000 0029 05da 0d63 6c61 7373  ryr#...)...class
-00000b10: 5f70 726f 626c 656d da0d 7461 7267 6574  _problem..target
-00000b20: 5f63 6f6c 756d 6eda 0d63 6f6e 665f 7472  _column..conf_tr
-00000b30: 6169 6e69 6e67 5a0c 636f 6e66 5f78 6762  ainingZ.conf_xgb
-00000b40: 6f6f 7374 da1c 6375 7374 6f6d 5f6c 6173  oost..custom_las
-00000b50: 745f 6d69 6c65 5f63 6f6d 7075 7461 7469  t_mile_computati
-00000b60: 6f6e 2901 da04 6178 6973 2901 5a0a 7461  on)...axis).Z.ta
-00000b70: 7267 6574 5f63 6f6c 7a16 4175 746f 7475  rget_colz.Autotu
-00000b80: 6e69 6e67 2073 7563 6365 7373 6675 6c2e  ning successful.
-00000b90: 7a16 5072 6564 6963 7469 6e67 2073 7563  z.Predicting suc
-00000ba0: 6365 7373 6675 6c2e 2901 fa02 3d3d 2901  cessful.)...==).
-00000bb0: 7a6b 2528 7079 3329 730a 7b25 2870 7933  zk%(py3)s.{%(py3
-00000bc0: 2973 203d 2025 2870 7930 2973 2825 2870  )s = %(py0)s(%(p
-00000bd0: 7931 2973 290a 7d20 3d3d 2025 2870 7931  y1)s).} == %(py1
-00000be0: 3029 730a 7b25 2870 7931 3029 7320 3d20  0)s.{%(py10)s = 
-00000bf0: 2528 7079 3529 7328 2528 7079 3829 730a  %(py5)s(%(py8)s.
-00000c00: 7b25 2870 7938 2973 203d 2025 2870 7936  {%(py8)s = %(py6
-00000c10: 2973 2e69 6e64 6578 0a7d 290a 7dda 036c  )s.index.}).}..l
-00000c20: 656e da07 795f 7072 6f62 7372 1700 0000  en..y_probsr....
-00000c30: 2907 da03 7079 30da 0370 7931 5a03 7079  )...py0..py1Z.py
-00000c40: 335a 0370 7935 da03 7079 365a 0370 7938  3Z.py5..py6Z.py8
-00000c50: 5a04 7079 3130 7a0f 6173 7365 7274 2025  Z.py10z.assert %
-00000c60: 2870 7931 3229 735a 0470 7931 324e da09  (py12)sZ.py12N..
-00000c70: 795f 636c 6173 7365 7329 1772 0b00 0000  y_classes).r....
-00000c80: 5a09 7374 6570 735f 6d61 785a 0e6e 756d  Z.steps_maxZ.num
-00000c90: 5f6c 6561 7665 735f 6d61 7872 0a00 0000  _leaves_maxr....
-00000ca0: da1c 6879 7065 7270 6172 616d 6574 6572  ..hyperparameter
-00000cb0: 5f74 756e 696e 675f 726f 756e 6473 da18  _tuning_rounds..
-00000cc0: 656e 6162 6c65 5f66 6561 7475 7265 5f73  enable_feature_s
-00000cd0: 656c 6563 7469 6f6e da14 6879 7065 7274  election..hypert
-00000ce0: 756e 696e 675f 6376 5f66 6f6c 6473 720f  uning_cv_foldsr.
-00000cf0: 0000 0072 0900 0000 5a08 6669 745f 6576  ...r....Z.fit_ev
-00000d00: 616c da04 6472 6f70 da05 7072 696e 74da  al..drop..print.
-00000d10: 0770 7265 6469 6374 723b 0000 00da 0569  .predictr;.....i
-00000d20: 6e64 6578 da0a 4070 7974 6573 745f 6172  ndex..@pytest_ar
-00000d30: da11 5f63 616c 6c5f 7265 7072 636f 6d70  .._call_reprcomp
-00000d40: 6172 65da 0c40 7079 5f62 7569 6c74 696e  are..@py_builtin
-00000d50: 73da 066c 6f63 616c 73da 185f 7368 6f75  s..locals.._shou
-00000d60: 6c64 5f72 6570 725f 676c 6f62 616c 5f6e  ld_repr_global_n
-00000d70: 616d 65da 095f 7361 6665 7265 7072 da0e  ame.._saferepr..
-00000d80: 4173 7365 7274 696f 6e45 7272 6f72 da13  AssertionError..
-00000d90: 5f66 6f72 6d61 745f 6578 706c 616e 6174  _format_explanat
-00000da0: 696f 6e29 1072 1a00 0000 7216 0000 0072  ion).r....r....r
-00000db0: 1700 0000 5a14 7867 626f 6f73 745f 7061  ....Z.xgboost_pa
-00000dc0: 7261 6d5f 636f 6e66 6967 da0c 7472 6169  ram_config..trai
-00000dd0: 6e5f 636f 6e66 6967 7233 0000 0072 3800  n_configr3...r8.
-00000de0: 0000 5a06 6175 746f 6d6c 723c 0000 0072  ..Z.automlr<...r
-00000df0: 4000 0000 5a0b 4070 795f 6173 7365 7274  @...Z.@py_assert
-00000e00: 325a 0b40 7079 5f61 7373 6572 7437 5a0b  2Z.@py_assert7Z.
-00000e10: 4070 795f 6173 7365 7274 395a 0b40 7079  @py_assert9Z.@py
-00000e20: 5f61 7373 6572 7434 5a0c 4070 795f 666f  _assert4Z.@py_fo
-00000e30: 726d 6174 3131 5a0c 4070 795f 666f 726d  rmat11Z.@py_form
-00000e40: 6174 3133 7218 0000 0072 1800 0000 7219  at13r....r....r.
-00000e50: 0000 00da 1674 6573 745f 626c 7565 7072  .....test_bluepr
-00000e60: 696e 745f 7867 626f 6f73 741e 0000 0073  int_xgboost....s
-00000e70: 3e00 0000 0802 0801 0601 0601 0601 0601  >...............
-00000e80: 0601 0601 0601 1003 0619 0202 0201 0201  ................
-00000e90: 0201 0201 0201 06fb 0407 0201 0c01 0601  ................
-00000ea0: 0201 06fc 0806 1801 0801 fe01 0a00 fe01  ................
-00000eb0: 2000 7251 0000 0063 0000 0000 0000 0000   .rQ...c........
-00000ec0: 0000 0000 0000 0000 0a00 0000 4000 0000  ............@...
-00000ed0: 7356 0000 0065 005a 0164 005a 0264 0164  sV...e.Z.d.Z.d.d
-00000ee0: 0284 005a 0364 0365 046a 0564 0465 046a  ...Z.d.e.j.d.e.j
-00000ef0: 0564 0565 046a 0664 0665 046a 0664 0764  .d.e.j.d.e.j.d.d
-00000f00: 0866 0a64 0964 0a84 045a 0764 0b65 046a  .f.d.d...Z.d.e.j
-00000f10: 0564 0765 0865 0965 0a66 0219 0066 0464  .d.e.e.e.f...f.d
-00000f20: 0c64 0d84 045a 0b64 0853 0029 0eda 0b43  .d...Z.d.S.)...C
-00000f30: 7573 746f 6d4d 6f64 656c 6301 0000 0000  ustomModelc.....
-00000f40: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000f50: 0000 0073 0a00 0000 6400 7c00 5f00 6400  ...s....d.|._.d.
-00000f60: 5300 a901 4e29 01da 056d 6f64 656c 2901  S...N)...model).
-00000f70: 7221 0000 0072 1800 0000 7218 0000 0072  r!...r....r....r
-00000f80: 1900 0000 da08 5f5f 696e 6974 5f5f 5b00  ......__init__[.
-00000f90: 0000 7302 0000 000a 017a 1443 7573 746f  ..s......z.Custo
-00000fa0: 6d4d 6f64 656c 2e5f 5f69 6e69 745f 5fda  mModel.__init__.
-00000fb0: 0778 5f74 7261 696e da06 785f 7465 7374  .x_train..x_test
-00000fc0: da07 795f 7472 6169 6eda 0679 5f74 6573  ..y_train..y_tes
-00000fd0: 7472 1200 0000 4e63 0500 0000 0000 0000  tr....Nc........
-00000fe0: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
-00000ff0: 731a 0000 0074 0083 007c 005f 017c 006a  s....t...|._.|.j
-00001000: 01a0 027c 017c 03a1 0201 0064 0053 0072  ...|.|.....d.S.r
-00001010: 5300 0000 2903 7204 0000 0072 5400 0000  S...).r....rT...
-00001020: da03 6669 7429 0572 2100 0000 7256 0000  ..fit).r!...rV..
-00001030: 0072 5700 0000 7258 0000 0072 5900 0000  .rW...rX...rY...
-00001040: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00001050: 5a00 0000 5e00 0000 7304 0000 0008 0712  Z...^...s.......
-00001060: 017a 0f43 7573 746f 6d4d 6f64 656c 2e66  .z.CustomModel.f
-00001070: 6974 721f 0000 0063 0200 0000 0000 0000  itr....c........
-00001080: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
-00001090: 7320 0000 007c 006a 00a0 017c 01a1 017d  s ...|.j...|...}
-000010a0: 027c 006a 00a0 027c 01a1 017d 037c 027c  .|.j...|...}.|.|
-000010b0: 0366 0253 0072 5300 0000 2903 7254 0000  .f.S.rS...).rT..
-000010c0: 005a 0d70 7265 6469 6374 5f70 726f 6261  .Z.predict_proba
-000010d0: 7246 0000 0029 0472 2100 0000 721f 0000  rF...).r!...r...
-000010e0: 00da 1070 7265 6469 6374 6564 5f70 726f  ...predicted_pro
-000010f0: 6261 73da 1170 7265 6469 6374 6564 5f63  bas..predicted_c
-00001100: 6c61 7373 6573 7218 0000 0072 1800 0000  lassesr....r....
-00001110: 7219 0000 0072 4600 0000 6800 0000 7306  r....rF...h...s.
-00001120: 0000 000c 010c 0108 017a 1343 7573 746f  .........z.Custo
-00001130: 6d4d 6f64 656c 2e70 7265 6469 6374 290c  mModel.predict).
-00001140: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00001150: 5500 0000 7229 0000 0072 3100 0000 722a  U...r)...r1...r*
-00001160: 0000 0072 5a00 0000 7203 0000 0072 0e00  ...rZ...r....r..
-00001170: 0000 720d 0000 0072 4600 0000 7218 0000  ..r....rF...r...
-00001180: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001190: 7252 0000 005a 0000 0073 1c00 0000 0800  rR...Z...s......
-000011a0: 0801 0203 0402 02fe 0403 02fd 0404 02fc  ................
-000011b0: 0405 02fb 0206 0afa 200a 7252 0000 0063  ........ .rR...c
-000011c0: 0000 0000 0000 0000 0000 0000 0d00 0000  ................
-000011d0: 0a00 0000 4300 0000 73b4 0200 0074 0083  ....C...s....t..
-000011e0: 007d 0074 0183 007d 0164 017c 015f 0264  .}.t...}.d.|._.d
-000011f0: 027c 015f 0364 037c 015f 0447 0064 0464  .|._.d.|._.G.d.d
-00001200: 0584 0064 0574 0583 037d 027c 0283 007d  ...d.t...}.|...}
-00001210: 0374 0664 0664 077c 007c 017c 0364 088d  .t.d.d.|.|.|.d..
-00001220: 057d 0474 07a0 0864 0964 0a84 0074 0964  .}.t...d.d...t.d
-00001230: 0183 0144 0083 0164 0b64 0a84 0074 0964  ...D...d.d...t.d
-00001240: 0183 0144 0083 0164 0c64 0a84 0074 0964  ...D...d.d...t.d
-00001250: 0183 0144 0083 0164 0d64 0a84 0074 0964  ...D...d.d...t.d
-00001260: 0183 0144 0083 0164 0e64 0a84 0074 0964  ...D...d.d...t.d
-00001270: 0183 0144 0083 0164 0f64 0a84 0074 0964  ...D...d.d...t.d
-00001280: 0183 0144 0083 0164 109c 06a1 017d 0574  ...D...d.....}.t
-00001290: 07a0 0a67 0064 11a2 01a1 017d 0674 07a0  ...g.d.....}.t..
-000012a0: 0864 1264 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-000012b0: 0164 1364 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-000012c0: 0164 1464 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-000012d0: 0164 1564 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-000012e0: 0164 1664 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-000012f0: 0164 1764 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-00001300: 0164 109c 06a1 017d 077c 067c 0564 073c  .d.....}.|.|.d.<
-00001310: 007c 04a0 0b7c 0564 07a1 0201 007c 04a0  .|...|.d.....|..
-00001320: 0c7c 07a1 015c 027d 087d 0974 0d6a 0e7d  .|...\.}.}.t.j.}
-00001330: 0a74 0f7c 087c 0a83 027d 0b7c 0b73 f864  .t.|.|...}.|.s.d
-00001340: 1864 1974 10a0 11a1 0076 0073 bd74 12a0  .d.t.....v.s.t..
-00001350: 1374 0fa1 0172 c274 12a0 1474 0fa1 016e  .t...r.t...t...n
-00001360: 0164 1964 1a74 10a0 11a1 0076 0073 ce74  .d.d.t.....v.s.t
-00001370: 12a0 137c 08a1 0172 d374 12a0 147c 08a1  ...|...r.t...|..
-00001380: 016e 0164 1a64 1b74 10a0 11a1 0076 0073  .n.d.d.t.....v.s
-00001390: df74 12a0 1374 0da1 0172 e474 12a0 1474  .t...t...r.t...t
-000013a0: 0da1 016e 0164 1b74 12a0 147c 0aa1 0174  ...n.d.t...|...t
-000013b0: 12a0 147c 0ba1 0164 1c9c 0516 007d 0c74  ...|...d.....}.t
-000013c0: 1574 12a0 167c 0ca1 0183 0182 0164 0004  .t...|.......d..
-000013d0: 007d 0a7d 0b74 0d6a 0e7d 0a74 0f7c 097c  .}.}.t.j.}.t.|.|
-000013e0: 0a83 027d 0b7c 0b90 0173 5464 1864 1974  ...}.|...sTd.d.t
-000013f0: 10a0 11a1 0076 0090 0173 1574 12a0 1374  .....v...s.t...t
-00001400: 0fa1 0190 0172 1a74 12a0 1474 0fa1 016e  .....r.t...t...n
-00001410: 0164 1964 1d74 10a0 11a1 0076 0090 0173  .d.d.t.....v...s
-00001420: 2874 12a0 137c 09a1 0190 0172 2d74 12a0  (t...|.....r-t..
-00001430: 147c 09a1 016e 0164 1d64 1b74 10a0 11a1  .|...n.d.d.t....
-00001440: 0076 0090 0173 3b74 12a0 1374 0da1 0190  .v...s;t...t....
-00001450: 0172 4074 12a0 1474 0da1 016e 0164 1b74  .r@t...t...n.d.t
-00001460: 12a0 147c 0aa1 0174 12a0 147c 0ba1 0164  ...|...t...|...d
-00001470: 1c9c 0516 007d 0c74 1574 12a0 167c 0ca1  .....}.t.t...|..
-00001480: 0183 0182 0164 0004 007d 0a7d 0b64 0053  .....d...}.}.d.S
-00001490: 0029 1e4e 721e 0000 0054 e902 0000 0063  .).Nr....T.....c
-000014a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000014b0: 0c00 0000 0000 0000 7386 0000 0065 005a  ........s....e.Z
-000014c0: 0164 005a 0264 0f64 0265 0366 0287 0066  .d.Z.d.d.e.f...f
-000014d0: 0164 0364 0484 0d5a 0464 0565 056a 0664  .d.d...Z.d.e.j.d
-000014e0: 0665 056a 0764 0765 0865 056a 0665 0965  .e.j.d.e.e.j.e.e
-000014f0: 056a 0719 0066 0219 0066 0664 0864 0984  .j...f...f.d.d..
-00001500: 045a 0a09 0a09 0b64 1064 0565 056a 0664  .Z.....d.d.e.j.d
-00001510: 0665 0965 056a 0719 0064 0c65 0b64 0765  .e.e.j...d.e.d.e
-00001520: 0865 056a 0665 0965 056a 0719 0066 0219  .e.j.e.e.j...f..
-00001530: 0066 0864 0d64 0e84 055a 0c87 0004 005a  .f.d.d...Z.....Z
-00001540: 0d53 0029 117a 3674 6573 745f 626c 7565  .S.).z6test_blue
-00001550: 6361 7374 5f77 6974 685f 6375 7374 6f6d  cast_with_custom
-00001560: 5f6d 6f64 656c 2e3c 6c6f 6361 6c73 3e2e  _model.<locals>.
-00001570: 5246 4543 5653 656c 6563 746f 7272 0100  RFECVSelectorr..
-00001580: 0000 7214 0000 0063 0200 0000 0000 0000  ..r....c........
-00001590: 0000 0000 0200 0000 0800 0000 1300 0000  ................
-000015a0: 7342 0000 0074 0083 00a0 01a1 0001 0064  sB...t.........d
-000015b0: 007c 005f 027c 017c 005f 0374 0474 05a0  .|._.|.|._.t.t..
-000015c0: 06a1 0064 0174 0764 027c 0164 0364 048d  ...d.t.d.|.d.d..
-000015d0: 0364 0174 0874 0983 0164 0264 058d 067c  .d.t.t...d.d...|
-000015e0: 005f 0a64 0053 0029 064e 721b 0000 0072  ._.d.S.).Nr....r
-000015f0: 5d00 0000 5429 0272 1400 0000 da07 7368  ]...T).r......sh
-00001600: 7566 666c 6529 06da 0965 7374 696d 6174  uffle)...estimat
-00001610: 6f72 da04 7374 6570 da02 6376 5a16 6d69  or..step..cvZ.mi
-00001620: 6e5f 6665 6174 7572 6573 5f74 6f5f 7365  n_features_to_se
-00001630: 6c65 6374 5a07 7363 6f72 696e 67da 066e  lectZ.scoring..n
-00001640: 5f6a 6f62 7329 0bda 0573 7570 6572 7255  _jobs)...superrU
-00001650: 0000 00da 1173 656c 6563 7465 645f 6665  .....selected_fe
-00001660: 6174 7572 6573 7214 0000 0072 0500 0000  aturesr....r....
-00001670: da03 7867 625a 0d58 4742 436c 6173 7369  ..xgbZ.XGBClassi
-00001680: 6669 6572 7208 0000 0072 0600 0000 7207  fierr....r....r.
-00001690: 0000 00da 1273 656c 6563 7469 6f6e 5f73  .....selection_s
-000016a0: 7472 6174 6567 7929 0272 2100 0000 7214  trategy).r!...r.
-000016b0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
-000016c0: 7218 0000 0072 1900 0000 7255 0000 0078  r....r....rU...x
-000016d0: 0000 0073 1600 0000 0a01 0601 0601 0201  ...s............
-000016e0: 0601 0201 0c01 0201 0601 0201 0cfa 7a3f  ..............z?
-000016f0: 7465 7374 5f62 6c75 6563 6173 745f 7769  test_bluecast_wi
-00001700: 7468 5f63 7573 746f 6d5f 6d6f 6465 6c2e  th_custom_model.
-00001710: 3c6c 6f63 616c 733e 2e52 4645 4356 5365  <locals>.RFECVSe
-00001720: 6c65 6374 6f72 2e5f 5f69 6e69 745f 5f72  lector.__init__r
-00001730: 1f00 0000 7223 0000 0072 1200 0000 6303  ....r#...r....c.
-00001740: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00001750: 0000 0053 0000 0073 3400 0000 7c00 6a00  ...S...s4...|.j.
-00001760: a001 7c01 7c02 a102 0100 7c00 6a00 6a02  ..|.|.....|.j.j.
-00001770: 7c00 5f03 7c01 6a04 6400 6400 8502 7c00  |._.|.j.d.d...|.
-00001780: 6a03 6602 1900 7d01 7c01 7c02 6602 5300  j.f...}.|.|.f.S.
-00001790: 7253 0000 0029 0572 6600 0000 725a 0000  rS...).rf...rZ..
-000017a0: 005a 0873 7570 706f 7274 5f72 6400 0000  .Z.support_rd...
-000017b0: da03 6c6f 6372 2500 0000 7218 0000 0072  ..locr%...r....r
-000017c0: 1800 0000 7219 0000 0072 2600 0000 8500  ....r....r&.....
-000017d0: 0000 7308 0000 000e 030a 0114 0108 017a  ..s............z
-000017e0: 4474 6573 745f 626c 7565 6361 7374 5f77  Dtest_bluecast_w
-000017f0: 6974 685f 6375 7374 6f6d 5f6d 6f64 656c  ith_custom_model
-00001800: 2e3c 6c6f 6361 6c73 3e2e 5246 4543 5653  .<locals>.RFECVS
-00001810: 656c 6563 746f 722e 6669 745f 7472 616e  elector.fit_tran
-00001820: 7366 6f72 6d4e 4672 2700 0000 6304 0000  sformNFr'...c...
-00001830: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-00001840: 0053 0000 0073 1c00 0000 7c01 6a00 6400  .S...s....|.j.d.
-00001850: 6400 8502 7c00 6a01 6602 1900 7d01 7c01  d...|.j.f...}.|.
-00001860: 7c02 6602 5300 7253 0000 0029 0272 6900  |.f.S.rS...).ri.
-00001870: 0000 7264 0000 0072 2b00 0000 7218 0000  ..rd...r+...r...
-00001880: 0072 1800 0000 7219 0000 0072 2c00 0000  .r....r....r,...
-00001890: 8d00 0000 7304 0000 0014 0608 017a 4074  ....s........z@t
-000018a0: 6573 745f 626c 7565 6361 7374 5f77 6974  est_bluecast_wit
-000018b0: 685f 6375 7374 6f6d 5f6d 6f64 656c 2e3c  h_custom_model.<
-000018c0: 6c6f 6361 6c73 3e2e 5246 4543 5653 656c  locals>.RFECVSel
-000018d0: 6563 746f 722e 7472 616e 7366 6f72 6d29  ector.transform)
-000018e0: 0172 0100 0000 722d 0000 0029 0e72 2e00  .r....r-...).r..
-000018f0: 0000 722f 0000 0072 3000 0000 da03 696e  ..r/...r0.....in
-00001900: 7472 5500 0000 7229 0000 0072 3100 0000  trU...r)...r1...
-00001910: 722a 0000 0072 0300 0000 7202 0000 0072  r*...r....r....r
-00001920: 2600 0000 7232 0000 0072 2c00 0000 da0d  &...r2...r,.....
-00001930: 5f5f 636c 6173 7363 656c 6c5f 5f72 1800  __classcell__r..
-00001940: 0000 7218 0000 0072 6700 0000 7219 0000  ..r....rg...r...
-00001950: 00da 0d52 4645 4356 5365 6c65 6374 6f72  ...RFECVSelector
-00001960: 7700 0000 7328 0000 0008 0014 0102 0d04  w...s(..........
-00001970: 0102 ff04 0102 ff12 020a fe02 0b02 0104  ................
-00001980: fc04 0202 fe08 0302 fd02 0402 fc12 0512  ................
-00001990: fb72 6c00 0000 7234 0000 0072 2300 0000  .rl...r4...r#...
-000019a0: 2905 7235 0000 0072 3600 0000 5a08 6d6c  ).r5...r6...Z.ml
-000019b0: 5f6d 6f64 656c 7237 0000 00da 1763 7573  _modelr7.....cus
-000019c0: 746f 6d5f 6665 6174 7572 655f 7365 6c65  tom_feature_sele
-000019d0: 6374 6f72 6301 0000 0000 0000 0000 0000  ctorc...........
-000019e0: 0002 0000 0003 0000 0053 0000 00f3 1000  .........S......
-000019f0: 0000 6700 7c00 5d04 7d01 7c01 9102 7102  ..g.|.].}.|...q.
-00001a00: 5300 7218 0000 0072 1800 0000 a902 da02  S.r....r........
-00001a10: 2e30 da01 6972 1800 0000 7218 0000 0072  .0..ir....r....r
-00001a20: 1900 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-00001a30: a400 0000 f302 0000 0010 007a 3374 6573  ...........z3tes
-00001a40: 745f 626c 7565 6361 7374 5f77 6974 685f  t_bluecast_with_
-00001a50: 6375 7374 6f6d 5f6d 6f64 656c 2e3c 6c6f  custom_model.<lo
-00001a60: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00001a70: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001a80: 0003 0000 0053 0000 0072 6e00 0000 7218  .....S...rn...r.
-00001a90: 0000 0072 1800 0000 726f 0000 0072 1800  ...r....ro...r..
-00001aa0: 0000 7218 0000 0072 1900 0000 7272 0000  ..r....r....rr..
-00001ab0: 00a5 0000 0072 7300 0000 6301 0000 0000  .....rs...c.....
-00001ac0: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00001ad0: 0000 0072 6e00 0000 7218 0000 0072 1800  ...rn...r....r..
-00001ae0: 0000 726f 0000 0072 1800 0000 7218 0000  ..ro...r....r...
-00001af0: 0072 1900 0000 7272 0000 00a6 0000 0072  .r....rr.......r
-00001b00: 7300 0000 6301 0000 0000 0000 0000 0000  s...c...........
-00001b10: 0002 0000 0003 0000 0053 0000 0072 6e00  .........S...rn.
-00001b20: 0000 7218 0000 0072 1800 0000 726f 0000  ..r....r....ro..
-00001b30: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001b40: 7272 0000 00a7 0000 0072 7300 0000 6301  rr.......rs...c.
-00001b50: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001b60: 0000 0053 0000 0072 6e00 0000 7218 0000  ...S...rn...r...
-00001b70: 0072 1800 0000 726f 0000 0072 1800 0000  .r....ro...r....
-00001b80: 7218 0000 0072 1900 0000 7272 0000 00a8  r....r....rr....
-00001b90: 0000 0072 7300 0000 6301 0000 0000 0000  ...rs...c.......
-00001ba0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00001bb0: 0072 6e00 0000 7218 0000 0072 1800 0000  .rn...r....r....
-00001bc0: 726f 0000 0072 1800 0000 7218 0000 0072  ro...r....r....r
-00001bd0: 1900 0000 7272 0000 00a9 0000 0072 7300  ....rr.......rs.
-00001be0: 0000 2906 5a08 6665 6174 7572 6531 5a08  ..).Z.feature1Z.
-00001bf0: 6665 6174 7572 6532 5a08 6665 6174 7572  feature2Z.featur
-00001c00: 6533 5a08 6665 6174 7572 6534 5a08 6665  e3Z.feature4Z.fe
-00001c10: 6174 7572 6535 5a08 6665 6174 7572 6536  ature5Z.feature6
-00001c20: 290a 7201 0000 0072 1b00 0000 7201 0000  ).r....r....r...
-00001c30: 0072 1b00 0000 7201 0000 0072 1b00 0000  .r....r....r....
-00001c40: 7201 0000 0072 1b00 0000 7201 0000 0072  r....r....r....r
-00001c50: 1b00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00001c60: 0002 0000 0003 0000 0053 0000 0072 6e00  .........S...rn.
-00001c70: 0000 7218 0000 0072 1800 0000 726f 0000  ..r....r....ro..
-00001c80: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001c90: 7272 0000 00af 0000 0072 7300 0000 6301  rr.......rs...c.
-00001ca0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001cb0: 0000 0053 0000 0072 6e00 0000 7218 0000  ...S...rn...r...
-00001cc0: 0072 1800 0000 726f 0000 0072 1800 0000  .r....ro...r....
-00001cd0: 7218 0000 0072 1900 0000 7272 0000 00b0  r....r....rr....
-00001ce0: 0000 0072 7300 0000 6301 0000 0000 0000  ...rs...c.......
-00001cf0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00001d00: 0072 6e00 0000 7218 0000 0072 1800 0000  .rn...r....r....
-00001d10: 726f 0000 0072 1800 0000 7218 0000 0072  ro...r....r....r
-00001d20: 1900 0000 7272 0000 00b1 0000 0072 7300  ....rr.......rs.
-00001d30: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001d40: 0000 0003 0000 0053 0000 0072 6e00 0000  .......S...rn...
-00001d50: 7218 0000 0072 1800 0000 726f 0000 0072  r....r....ro...r
-00001d60: 1800 0000 7218 0000 0072 1900 0000 7272  ....r....r....rr
-00001d70: 0000 00b2 0000 0072 7300 0000 6301 0000  .......rs...c...
-00001d80: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00001d90: 0053 0000 0072 6e00 0000 7218 0000 0072  .S...rn...r....r
-00001da0: 1800 0000 726f 0000 0072 1800 0000 7218  ....ro...r....r.
-00001db0: 0000 0072 1900 0000 7272 0000 00b3 0000  ...r....rr......
-00001dc0: 0072 7300 0000 6301 0000 0000 0000 0000  .rs...c.........
-00001dd0: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
-00001de0: 6e00 0000 7218 0000 0072 1800 0000 726f  n...r....r....ro
-00001df0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00001e00: 0000 7272 0000 00b4 0000 0072 7300 0000  ..rr.......rs...
-00001e10: 7a52 6173 7365 7274 2025 2870 7936 2973  zRassert %(py6)s
-00001e20: 0a7b 2528 7079 3629 7320 3d20 2528 7079  .{%(py6)s = %(py
-00001e30: 3029 7328 2528 7079 3129 732c 2025 2870  0)s(%(py1)s, %(p
-00001e40: 7934 2973 0a7b 2528 7079 3429 7320 3d20  y4)s.{%(py4)s = 
-00001e50: 2528 7079 3229 732e 6e64 6172 7261 790a  %(py2)s.ndarray.
-00001e60: 7d29 0a7d 7228 0000 0072 5b00 0000 da02  }).}r(...r[.....
-00001e70: 6e70 2905 723d 0000 0072 3e00 0000 5a03  np).r=...r>...Z.
-00001e80: 7079 325a 0370 7934 723f 0000 0072 5c00  py2Z.py4r?...r\.
-00001e90: 0000 2917 7252 0000 0072 0a00 0000 7241  ..).rR...r....rA
-00001ea0: 0000 0072 4200 0000 7243 0000 0072 0f00  ...rB...rC...r..
-00001eb0: 0000 7209 0000 0072 2900 0000 7231 0000  ..r....r)...r1..
-00001ec0: 00da 0572 616e 6765 722a 0000 0072 5a00  ...ranger*...rZ.
-00001ed0: 0000 7246 0000 0072 7400 0000 da07 6e64  ..rF...rt.....nd
-00001ee0: 6172 7261 7972 2800 0000 724a 0000 0072  arrayr(...rJ...r
-00001ef0: 4b00 0000 7248 0000 0072 4c00 0000 724d  K...rH...rL...rM
-00001f00: 0000 0072 4e00 0000 724f 0000 0029 0d5a  ...rN...rO...).Z
-00001f10: 0c63 7573 746f 6d5f 6d6f 6465 6c72 5000  .custom_modelrP.
-00001f20: 0000 726c 0000 0072 6d00 0000 da08 626c  ..rl...rm.....bl
-00001f30: 7565 6361 7374 7256 0000 0072 5800 0000  uecastrV...rX...
-00001f40: 7257 0000 0072 5b00 0000 725c 0000 005a  rW...r[...r\...Z
-00001f50: 0b40 7079 5f61 7373 6572 7433 5a0b 4070  .@py_assert3Z.@p
-00001f60: 795f 6173 7365 7274 355a 0b40 7079 5f66  y_assert5Z.@py_f
-00001f70: 6f72 6d61 7437 7218 0000 0072 1800 0000  ormat7r....r....
-00001f80: 7219 0000 00da 1f74 6573 745f 626c 7565  r......test_blue
-00001f90: 6361 7374 5f77 6974 685f 6375 7374 6f6d  cast_with_custom
-00001fa0: 5f6d 6f64 656c 6e00 0000 734c 0000 0006  _modeln...sL....
-00001fb0: 0206 0106 0106 0106 0110 0306 1f02 0302  ................
-00001fc0: 0102 0102 0102 0102 0106 fb04 0910 0210  ................
-00001fd0: 0110 0110 0110 0110 0104 fa04 ff0e 0a04  ................
-00001fe0: 0110 0210 0110 0110 0110 0110 0104 fa04  ................
-00001ff0: ff08 0b0c 030e 03aa 03bc 0172 7800 0000  ...........rx...
-00002000: 292c da08 6275 696c 7469 6e73 724a 0000  ),..builtinsrJ..
-00002010: 00da 195f 7079 7465 7374 2e61 7373 6572  ..._pytest.asser
-00002020: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
-00002030: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
-00002040: 7248 0000 00da 0674 7970 696e 6772 0200  rH.....typingr..
-00002050: 0000 7203 0000 00da 056e 756d 7079 7274  ..r......numpyrt
-00002060: 0000 00da 0670 616e 6461 7372 2900 0000  .....pandasr)...
-00002070: da06 7079 7465 7374 5a07 7867 626f 6f73  ..pytestZ.xgboos
-00002080: 7472 6500 0000 5a10 736b 6c65 6172 6e2e  tre...Z.sklearn.
-00002090: 656e 7365 6d62 6c65 7204 0000 005a 1973  ensembler....Z.s
-000020a0: 6b6c 6561 726e 2e66 6561 7475 7265 5f73  klearn.feature_s
-000020b0: 656c 6563 7469 6f6e 7205 0000 005a 0f73  electionr....Z.s
-000020c0: 6b6c 6561 726e 2e6d 6574 7269 6373 7206  klearn.metricsr.
-000020d0: 0000 0072 0700 0000 5a17 736b 6c65 6172  ...r....Z.sklear
-000020e0: 6e2e 6d6f 6465 6c5f 7365 6c65 6374 696f  n.model_selectio
-000020f0: 6e72 0800 0000 5a18 626c 7565 6361 7374  nr....Z.bluecast
-00002100: 2e62 6c75 6570 7269 6e74 732e 6361 7374  .blueprints.cast
-00002110: 7209 0000 005a 1f62 6c75 6563 6173 742e  r....Z.bluecast.
-00002120: 636f 6e66 6967 2e74 7261 696e 696e 675f  config.training_
-00002130: 636f 6e66 6967 720a 0000 0072 0b00 0000  configr....r....
-00002140: 5a22 626c 7565 6361 7374 2e6d 6c5f 6d6f  Z"bluecast.ml_mo
-00002150: 6465 6c6c 696e 672e 6261 7365 5f63 6c61  delling.base_cla
-00002160: 7373 6573 720c 0000 0072 0d00 0000 720e  ssesr....r....r.
-00002170: 0000 005a 1d62 6c75 6563 6173 742e 7072  ...Z.bluecast.pr
-00002180: 6570 726f 6365 7373 696e 672e 6375 7374  eprocessing.cust
-00002190: 6f6d 720f 0000 00da 2462 6c75 6563 6173  omr.....$bluecas
-000021a0: 742e 7465 7374 732e 6d61 6b65 5f64 6174  t.tests.make_dat
-000021b0: 612e 6372 6561 7465 5f64 6174 6172 1100  a.create_datar..
-000021c0: 0000 da07 6669 7874 7572 6572 3100 0000  ....fixturer1...
-000021d0: 721a 0000 0072 5100 0000 7252 0000 0072  r....rQ...rR...r
-000021e0: 7800 0000 7218 0000 0072 1800 0000 7218  x...r....r....r.
-000021f0: 0000 0072 1900 0000 da08 3c6d 6f64 756c  ...r......<modul
-00002200: 653e 0100 0000 7326 0000 002a 0008 0208  e>....s&...*....
-00002210: 0108 0108 010c 010c 0110 010c 010c 0210  ................
-00002220: 0114 010c 050c 0104 031c 0108 0610 3c0c  ..............<.
-00002230: 14                                       .
+00000380: 047c 035f 0247 0064 0564 0684 0064 0674  .|._.G.d.d...d.t
+00000390: 0383 037d 047c 0483 007d 0574 0464 0764  ...}.|...}.t.d.d
+000003a0: 087c 037c 0564 098d 047d 067c 066a 057c  .|.|.d...}.|.j.|
+000003b0: 017c 016a 0664 0864 0264 0a8d 027c 0164  .|.j.d.d.d...|.d
+000003c0: 0819 0064 0864 0b8d 0401 0074 0764 0c83  ...d.d.....t.d..
+000003d0: 0101 007c 06a0 087c 026a 0664 0864 0264  ...|...|.j.d.d.d
+000003e0: 0a8d 02a1 015c 027d 077d 0874 0764 0d83  .....\.}.}.t.d..
+000003f0: 0101 0074 097c 0783 017d 097c 026a 0a7d  ...t.|...}.|.j.}
+00000400: 0a74 097c 0a83 017d 0b7c 097c 0b6b 027d  .t.|...}.|.|.k.}
+00000410: 0c7c 0c73 c474 0ba0 0c64 0e7c 0c66 0164  .|.s.t...d.|.f.d
+00000420: 0f7c 097c 0b66 02a1 0464 1074 0da0 0ea1  .|.|.f...d.t....
+00000430: 0076 0073 6e74 0ba0 0f74 09a1 0172 7374  .v.snt...t...rst
+00000440: 0ba0 1074 09a1 016e 0164 1064 1174 0da0  ...t...n.d.d.t..
+00000450: 0ea1 0076 0073 7f74 0ba0 0f7c 07a1 0172  ...v.s.t...|...r
+00000460: 8474 0ba0 107c 07a1 016e 0164 1174 0ba0  .t...|...n.d.t..
+00000470: 107c 09a1 0164 1074 0da0 0ea1 0076 0073  .|...d.t.....v.s
+00000480: 9474 0ba0 0f74 09a1 0172 9974 0ba0 1074  .t...t...r.t...t
+00000490: 09a1 016e 0164 1064 1274 0da0 0ea1 0076  ...n.d.d.t.....v
+000004a0: 0073 a574 0ba0 0f7c 02a1 0172 aa74 0ba0  .s.t...|...r.t..
+000004b0: 107c 02a1 016e 0164 1274 0ba0 107c 0aa1  .|...n.d.t...|..
+000004c0: 0174 0ba0 107c 0ba1 0164 139c 0716 007d  .t...|...d.....}
+000004d0: 0d64 1464 157c 0d69 0116 007d 0e74 1174  .d.d.|.i...}.t.t
+000004e0: 0ba0 127c 0ea1 0183 0182 0164 1604 007d  ...|.......d...}
+000004f0: 0904 007d 0c04 007d 0a7d 0b74 097c 0883  ...}...}.}.t.|..
+00000500: 017d 097c 026a 0a7d 0a74 097c 0a83 017d  .}.|.j.}.t.|...}
+00000510: 0b7c 097c 0b6b 027d 0c7c 0c90 0173 4f74  .|.|.k.}.|...sOt
+00000520: 0ba0 0c64 0e7c 0c66 0164 0f7c 097c 0b66  ...d.|.f.d.|.|.f
+00000530: 02a1 0464 1074 0da0 0ea1 0076 0073 f374  ...d.t.....v.s.t
+00000540: 0ba0 0f74 09a1 0172 f874 0ba0 1074 09a1  ...t...r.t...t..
+00000550: 016e 0164 1064 1774 0da0 0ea1 0076 0090  .n.d.d.t.....v..
+00000560: 0173 0674 0ba0 0f7c 08a1 0190 0172 0b74  .s.t...|.....r.t
+00000570: 0ba0 107c 08a1 016e 0164 1774 0ba0 107c  ...|...n.d.t...|
+00000580: 09a1 0164 1074 0da0 0ea1 0076 0090 0173  ...d.t.....v...s
+00000590: 1d74 0ba0 0f74 09a1 0190 0172 2274 0ba0  .t...t.....r"t..
+000005a0: 1074 09a1 016e 0164 1064 1274 0da0 0ea1  .t...n.d.d.t....
+000005b0: 0076 0090 0173 3074 0ba0 0f7c 02a1 0190  .v...s0t...|....
+000005c0: 0172 3574 0ba0 107c 02a1 016e 0164 1274  .r5t...|...n.d.t
+000005d0: 0ba0 107c 0aa1 0174 0ba0 107c 0ba1 0164  ...|...t...|...d
+000005e0: 139c 0716 007d 0d64 1464 157c 0d69 0116  .....}.d.d.|.i..
+000005f0: 007d 0e74 1174 0ba0 127c 0ea1 0183 0182  .}.t.t...|......
+00000600: 0164 1604 007d 0904 007d 0c04 007d 0a7d  .d...}...}...}.}
+00000610: 0b64 1653 0029 187a 2254 6573 7420 7468  .d.S.).z"Test th
+00000620: 6174 2074 6573 7473 2074 6865 2042 6c75  at tests the Blu
+00000630: 6543 6173 7420 636c 6173 7372 0100 0000  eCast classr....
+00000640: e901 0000 00e9 6400 0000 e910 0000 0063  ......d........c
+00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000660: 0c00 0000 4000 0000 7380 0000 0065 005a  ....@...s....e.Z
+00000670: 0164 005a 0264 0165 036a 0464 0265 036a  .d.Z.d.e.j.d.e.j
+00000680: 0466 0464 0364 0484 045a 0564 0165 036a  .f.d.d...Z.d.e.j
+00000690: 0464 0565 036a 0664 0265 0765 036a 0465  .d.e.j.d.e.e.j.e
+000006a0: 036a 0666 0219 0066 0664 0664 0784 045a  .j.f...f.d.d...Z
+000006b0: 0809 0809 0964 0d64 0165 036a 0464 0565  .....d.d.e.j.d.e
+000006c0: 0965 036a 0619 0064 0a65 0a64 0265 0765  .e.j...d.e.d.e.e
+000006d0: 036a 0465 0965 036a 0619 0066 0219 0066  .j.e.e.j...f...f
+000006e0: 0864 0b64 0c84 055a 0b64 0853 0029 0e7a  .d.d...Z.d.S.).z
+000006f0: 3d74 6573 745f 626c 7565 7072 696e 745f  =test_blueprint_
+00000700: 7867 626f 6f73 742e 3c6c 6f63 616c 733e  xgboost.<locals>
+00000710: 2e4d 7943 7573 746f 6d4c 6173 744d 696c  .MyCustomLastMil
+00000720: 6550 7265 7072 6f63 6573 7369 6e67 da02  ePreprocessing..
+00000730: 6466 7212 0000 0063 0200 0000 0000 0000  dfr....c........
+00000740: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00000750: 730c 0000 0064 017c 0164 023c 007c 0153  s....d.|.d.<.|.S
+00000760: 0029 034e e905 0000 005a 0a63 7573 746f  .).N.....Z.custo
+00000770: 6d5f 636f 6c72 1800 0000 2902 da04 7365  m_colr....)...se
+00000780: 6c66 721e 0000 0072 1800 0000 7218 0000  lfr....r....r...
+00000790: 0072 1900 0000 da0f 6375 7374 6f6d 5f66  .r......custom_f
+000007a0: 756e 6374 696f 6e28 0000 0073 0400 0000  unction(...s....
+000007b0: 0801 0401 7a4d 7465 7374 5f62 6c75 6570  ....zMtest_bluep
+000007c0: 7269 6e74 5f78 6762 6f6f 7374 2e3c 6c6f  rint_xgboost.<lo
+000007d0: 6361 6c73 3e2e 4d79 4375 7374 6f6d 4c61  cals>.MyCustomLa
+000007e0: 7374 4d69 6c65 5072 6570 726f 6365 7373  stMilePreprocess
+000007f0: 696e 672e 6375 7374 6f6d 5f66 756e 6374  ing.custom_funct
+00000800: 696f 6eda 0674 6172 6765 7463 0300 0000  ion..targetc....
+00000810: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000820: 5300 0000 7326 0000 007c 00a0 007c 01a1  S...s&...|...|..
+00000830: 017d 017c 01a0 0164 01a1 017d 017c 02a0  .}.|...d...}.|..
+00000840: 0164 01a1 017d 027c 017c 0266 0253 0029  .d...}.|.|.f.S.)
+00000850: 024e 69e8 0300 0029 0272 2100 0000 da04  .Ni....).r!.....
+00000860: 6865 6164 a903 7220 0000 0072 1e00 0000  head..r ...r....
+00000870: 7222 0000 0072 1800 0000 7218 0000 0072  r"...r....r....r
+00000880: 1900 0000 da0d 6669 745f 7472 616e 7366  ......fit_transf
+00000890: 6f72 6d2c 0000 0073 0800 0000 0a03 0a01  orm,...s........
+000008a0: 0a01 0801 7a4b 7465 7374 5f62 6c75 6570  ....zKtest_bluep
+000008b0: 7269 6e74 5f78 6762 6f6f 7374 2e3c 6c6f  rint_xgboost.<lo
+000008c0: 6361 6c73 3e2e 4d79 4375 7374 6f6d 4c61  cals>.MyCustomLa
+000008d0: 7374 4d69 6c65 5072 6570 726f 6365 7373  stMilePreprocess
+000008e0: 696e 672e 6669 745f 7472 616e 7366 6f72  ing.fit_transfor
+000008f0: 6d4e 46da 0e70 7265 6469 6374 6f6e 5f6d  mNF..predicton_m
+00000900: 6f64 6563 0400 0000 0000 0000 0000 0000  odec............
+00000910: 0400 0000 0300 0000 5300 0000 7336 0000  ........S...s6..
+00000920: 007c 00a0 007c 01a1 017d 017c 0373 1774  .|...|...}.|.s.t
+00000930: 017c 0274 026a 0383 0272 177c 01a0 0464  .|.t.j...r.|...d
+00000940: 01a1 017d 017c 02a0 0464 01a1 017d 027c  ...}.|...d...}.|
+00000950: 017c 0266 0253 0029 024e 721c 0000 0029  .|.f.S.).Nr....)
+00000960: 0572 2100 0000 da0a 6973 696e 7374 616e  .r!.....isinstan
+00000970: 6365 da02 7064 da06 5365 7269 6573 7223  ce..pd..Seriesr#
+00000980: 0000 00a9 0472 2000 0000 721e 0000 0072  .....r ...r....r
+00000990: 2200 0000 7226 0000 0072 1800 0000 7218  "...r&...r....r.
+000009a0: 0000 0072 1900 0000 da09 7472 616e 7366  ...r......transf
+000009b0: 6f72 6d34 0000 0073 0a00 0000 0a06 1001  orm4...s........
+000009c0: 0a01 0a01 0801 7a47 7465 7374 5f62 6c75  ......zGtest_blu
+000009d0: 6570 7269 6e74 5f78 6762 6f6f 7374 2e3c  eprint_xgboost.<
+000009e0: 6c6f 6361 6c73 3e2e 4d79 4375 7374 6f6d  locals>.MyCustom
+000009f0: 4c61 7374 4d69 6c65 5072 6570 726f 6365  LastMilePreproce
+00000a00: 7373 696e 672e 7472 616e 7366 6f72 6da9  ssing.transform.
+00000a10: 024e 4629 0cda 085f 5f6e 616d 655f 5fda  .NF)...__name__.
+00000a20: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000a30: 7561 6c6e 616d 655f 5f72 2800 0000 da09  ualname__r(.....
+00000a40: 4461 7461 4672 616d 6572 2100 0000 7229  DataFramer!...r)
+00000a50: 0000 0072 0300 0000 7225 0000 0072 0200  ...r....r%...r..
+00000a60: 0000 da04 626f 6f6c 722b 0000 0072 1800  ....boolr+...r..
+00000a70: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000a80: 00da 1d4d 7943 7573 746f 6d4c 6173 744d  ...MyCustomLastM
+00000a90: 696c 6550 7265 7072 6f63 6573 7369 6e67  ilePreprocessing
+00000aa0: 2700 0000 7328 0000 0008 0016 0102 0404  '...s(..........
+00000ab0: 0102 ff04 0102 ff0e 020a fe02 0b02 0104  ................
+00000ac0: fc04 0202 fe08 0302 fd02 0402 fc12 050e  ................
+00000ad0: fb72 3200 0000 da06 6269 6e61 7279 7222  .r2.....binaryr"
+00000ae0: 0000 0029 04da 0d63 6c61 7373 5f70 726f  ...)...class_pro
+00000af0: 626c 656d da0d 7461 7267 6574 5f63 6f6c  blem..target_col
+00000b00: 756d 6e5a 0c63 6f6e 665f 7867 626f 6f73  umnZ.conf_xgboos
+00000b10: 74da 1c63 7573 746f 6d5f 6c61 7374 5f6d  t..custom_last_m
+00000b20: 696c 655f 636f 6d70 7574 6174 696f 6e29  ile_computation)
+00000b30: 01da 0461 7869 7329 015a 0a74 6172 6765  ...axis).Z.targe
+00000b40: 745f 636f 6c7a 1641 7574 6f74 756e 696e  t_colz.Autotunin
+00000b50: 6720 7375 6363 6573 7366 756c 2e7a 1650  g successful.z.P
+00000b60: 7265 6469 6374 696e 6720 7375 6363 6573  redicting succes
+00000b70: 7366 756c 2e29 01fa 023d 3d29 017a 6b25  sful.)...==).zk%
+00000b80: 2870 7933 2973 0a7b 2528 7079 3329 7320  (py3)s.{%(py3)s 
+00000b90: 3d20 2528 7079 3029 7328 2528 7079 3129  = %(py0)s(%(py1)
+00000ba0: 7329 0a7d 203d 3d20 2528 7079 3130 2973  s).} == %(py10)s
+00000bb0: 0a7b 2528 7079 3130 2973 203d 2025 2870  .{%(py10)s = %(p
+00000bc0: 7935 2973 2825 2870 7938 2973 0a7b 2528  y5)s(%(py8)s.{%(
+00000bd0: 7079 3829 7320 3d20 2528 7079 3629 732e  py8)s = %(py6)s.
+00000be0: 696e 6465 780a 7d29 0a7d da03 6c65 6eda  index.}).}..len.
+00000bf0: 0779 5f70 726f 6273 7217 0000 0029 07da  .y_probsr....)..
+00000c00: 0370 7930 da03 7079 315a 0370 7933 5a03  .py0..py1Z.py3Z.
+00000c10: 7079 35da 0370 7936 5a03 7079 385a 0470  py5..py6Z.py8Z.p
+00000c20: 7931 307a 0f61 7373 6572 7420 2528 7079  y10z.assert %(py
+00000c30: 3132 2973 5a04 7079 3132 4eda 0979 5f63  12)sZ.py12N..y_c
+00000c40: 6c61 7373 6573 2913 720b 0000 005a 0973  lasses).r....Z.s
+00000c50: 7465 7073 5f6d 6178 5a0e 6e75 6d5f 6c65  teps_maxZ.num_le
+00000c60: 6176 6573 5f6d 6178 720f 0000 0072 0900  aves_maxr....r..
+00000c70: 0000 5a08 6669 745f 6576 616c da04 6472  ..Z.fit_eval..dr
+00000c80: 6f70 da05 7072 696e 74da 0770 7265 6469  op..print..predi
+00000c90: 6374 7239 0000 00da 0569 6e64 6578 da0a  ctr9.....index..
+00000ca0: 4070 7974 6573 745f 6172 da11 5f63 616c  @pytest_ar.._cal
+00000cb0: 6c5f 7265 7072 636f 6d70 6172 65da 0c40  l_reprcompare..@
+00000cc0: 7079 5f62 7569 6c74 696e 73da 066c 6f63  py_builtins..loc
+00000cd0: 616c 73da 185f 7368 6f75 6c64 5f72 6570  als.._should_rep
+00000ce0: 725f 676c 6f62 616c 5f6e 616d 65da 095f  r_global_name.._
+00000cf0: 7361 6665 7265 7072 da0e 4173 7365 7274  saferepr..Assert
+00000d00: 696f 6e45 7272 6f72 da13 5f66 6f72 6d61  ionError.._forma
+00000d10: 745f 6578 706c 616e 6174 696f 6e29 0f72  t_explanation).r
+00000d20: 1a00 0000 7216 0000 0072 1700 0000 5a14  ....r....r....Z.
+00000d30: 7867 626f 6f73 745f 7061 7261 6d5f 636f  xgboost_param_co
+00000d40: 6e66 6967 7232 0000 0072 3600 0000 5a06  nfigr2...r6...Z.
+00000d50: 6175 746f 6d6c 723a 0000 0072 3e00 0000  automlr:...r>...
+00000d60: 5a0b 4070 795f 6173 7365 7274 325a 0b40  Z.@py_assert2Z.@
+00000d70: 7079 5f61 7373 6572 7437 5a0b 4070 795f  py_assert7Z.@py_
+00000d80: 6173 7365 7274 395a 0b40 7079 5f61 7373  assert9Z.@py_ass
+00000d90: 6572 7434 5a0c 4070 795f 666f 726d 6174  ert4Z.@py_format
+00000da0: 3131 5a0c 4070 795f 666f 726d 6174 3133  11Z.@py_format13
+00000db0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+00000dc0: 1674 6573 745f 626c 7565 7072 696e 745f  .test_blueprint_
+00000dd0: 7867 626f 6f73 741e 0000 0073 3400 0000  xgboost....s4...
+00000de0: 0802 0801 0601 0601 0601 1003 0619 0202  ................
+00000df0: 0201 0201 0201 0201 06fc 0406 0201 0c01  ................
+00000e00: 0601 0201 06fc 0806 1801 0801 fe01 0a00  ................
+00000e10: fe01 1c00 724b 0000 0063 0000 0000 0000  ....rK...c......
+00000e20: 0000 0000 0000 0000 0000 0a00 0000 4000  ..............@.
+00000e30: 0000 7356 0000 0065 005a 0164 005a 0264  ..sV...e.Z.d.Z.d
+00000e40: 0164 0284 005a 0364 0365 046a 0564 0465  .d...Z.d.e.j.d.e
+00000e50: 046a 0564 0565 046a 0664 0665 046a 0664  .j.d.e.j.d.e.j.d
+00000e60: 0764 0866 0a64 0964 0a84 045a 0764 0b65  .d.f.d.d...Z.d.e
+00000e70: 046a 0564 0765 0865 0965 0a66 0219 0066  .j.d.e.e.e.f...f
+00000e80: 0464 0c64 0d84 045a 0b64 0853 0029 0eda  .d.d...Z.d.S.)..
+00000e90: 0b43 7573 746f 6d4d 6f64 656c 6301 0000  .CustomModelc...
+00000ea0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000eb0: 0043 0000 0073 0a00 0000 6400 7c00 5f00  .C...s....d.|._.
+00000ec0: 6400 5300 a901 4e29 01da 056d 6f64 656c  d.S...N)...model
+00000ed0: 2901 7220 0000 0072 1800 0000 7218 0000  ).r ...r....r...
+00000ee0: 0072 1900 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
+00000ef0: 5600 0000 7302 0000 000a 017a 1443 7573  V...s......z.Cus
+00000f00: 746f 6d4d 6f64 656c 2e5f 5f69 6e69 745f  tomModel.__init_
+00000f10: 5fda 0778 5f74 7261 696e da06 785f 7465  _..x_train..x_te
+00000f20: 7374 da07 795f 7472 6169 6eda 0679 5f74  st..y_train..y_t
+00000f30: 6573 7472 1200 0000 4e63 0500 0000 0000  estr....Nc......
+00000f40: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
+00000f50: 0000 731a 0000 0074 0083 007c 005f 017c  ..s....t...|._.|
+00000f60: 006a 01a0 027c 017c 03a1 0201 0064 0053  .j...|.|.....d.S
+00000f70: 0072 4d00 0000 2903 7204 0000 0072 4e00  .rM...).r....rN.
+00000f80: 0000 da03 6669 7429 0572 2000 0000 7250  ....fit).r ...rP
+00000f90: 0000 0072 5100 0000 7252 0000 0072 5300  ...rQ...rR...rS.
+00000fa0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000fb0: 0072 5400 0000 5900 0000 7304 0000 0008  .rT...Y...s.....
+00000fc0: 0712 017a 0f43 7573 746f 6d4d 6f64 656c  ...z.CustomModel
+00000fd0: 2e66 6974 721e 0000 0063 0200 0000 0000  .fitr....c......
+00000fe0: 0000 0000 0000 0400 0000 0300 0000 4300  ..............C.
+00000ff0: 0000 7320 0000 007c 006a 00a0 017c 01a1  ..s ...|.j...|..
+00001000: 017d 027c 006a 00a0 027c 01a1 017d 037c  .}.|.j...|...}.|
+00001010: 027c 0366 0253 0072 4d00 0000 2903 724e  .|.f.S.rM...).rN
+00001020: 0000 005a 0d70 7265 6469 6374 5f70 726f  ...Z.predict_pro
+00001030: 6261 7241 0000 0029 0472 2000 0000 721e  barA...).r ...r.
+00001040: 0000 00da 1070 7265 6469 6374 6564 5f70  .....predicted_p
+00001050: 726f 6261 73da 1170 7265 6469 6374 6564  robas..predicted
+00001060: 5f63 6c61 7373 6573 7218 0000 0072 1800  _classesr....r..
+00001070: 0000 7219 0000 0072 4100 0000 6300 0000  ..r....rA...c...
+00001080: 7306 0000 000c 010c 0108 017a 1343 7573  s..........z.Cus
+00001090: 746f 6d4d 6f64 656c 2e70 7265 6469 6374  tomModel.predict
+000010a0: 290c 722d 0000 0072 2e00 0000 722f 0000  ).r-...r....r/..
+000010b0: 0072 4f00 0000 7228 0000 0072 3000 0000  .rO...r(...r0...
+000010c0: 7229 0000 0072 5400 0000 7203 0000 0072  r)...rT...r....r
+000010d0: 0e00 0000 720d 0000 0072 4100 0000 7218  ....r....rA...r.
+000010e0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+000010f0: 0000 724c 0000 0055 0000 0073 1c00 0000  ..rL...U...s....
+00001100: 0800 0801 0203 0402 02fe 0403 02fd 0404  ................
+00001110: 02fc 0405 02fb 0206 0afa 200a 724c 0000  .......... .rL..
+00001120: 0063 0000 0000 0000 0000 0000 0000 0f00  .c..............
+00001130: 0000 0a00 0000 4300 0000 73ce 0200 0074  ......C...s....t
+00001140: 0083 007d 0074 0183 007d 0164 017c 015f  ...}.t...}.d.|._
+00001150: 0264 027c 015f 0364 037c 015f 0447 0064  .d.|._.d.|._.G.d
+00001160: 0464 0584 0064 0574 0583 037d 0247 0064  .d...d.t...}.G.d
+00001170: 0664 0784 0064 0774 0583 037d 037c 0283  .d...d.t...}.|..
+00001180: 007d 047c 0383 007d 0574 0664 0864 097c  .}.|...}.t.d.d.|
+00001190: 007c 017c 047c 0564 0a8d 067d 0674 07a0  .|.|.|.d...}.t..
+000011a0: 0864 0b64 0c84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000011b0: 0164 0d64 0c84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000011c0: 0164 0e64 0c84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000011d0: 0164 0f64 0c84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000011e0: 0164 1064 0c84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000011f0: 0164 1164 0c84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+00001200: 0164 129c 06a1 017d 0774 07a0 0a67 0064  .d.....}.t...g.d
+00001210: 13a2 01a1 017d 0874 07a0 0864 1464 0c84  .....}.t...d.d..
+00001220: 0074 0964 0183 0144 0083 0164 1564 0c84  .t.d...D...d.d..
+00001230: 0074 0964 0183 0144 0083 0164 1664 0c84  .t.d...D...d.d..
+00001240: 0074 0964 0183 0144 0083 0164 1764 0c84  .t.d...D...d.d..
+00001250: 0074 0964 0183 0144 0083 0164 1864 0c84  .t.d...D...d.d..
+00001260: 0074 0964 0183 0144 0083 0164 1964 0c84  .t.d...D...d.d..
+00001270: 0074 0964 0183 0144 0083 0164 129c 06a1  .t.d...D...d....
+00001280: 017d 097c 087c 0764 093c 007c 06a0 0b7c  .}.|.|.d.<.|...|
+00001290: 0764 09a1 0201 007c 06a0 0c7c 09a1 015c  .d.....|...|...\
+000012a0: 027d 0a7d 0b74 0d6a 0e7d 0c74 0f7c 0a7c  .}.}.t.j.}.t.|.|
+000012b0: 0c83 027d 0d7c 0d90 0173 0564 1a64 1b74  ...}.|...s.d.d.t
+000012c0: 10a0 11a1 0076 0073 ca74 12a0 1374 0fa1  .....v.s.t...t..
+000012d0: 0172 cf74 12a0 1474 0fa1 016e 0164 1b64  .r.t...t...n.d.d
+000012e0: 1c74 10a0 11a1 0076 0073 db74 12a0 137c  .t.....v.s.t...|
+000012f0: 0aa1 0172 e074 12a0 147c 0aa1 016e 0164  ...r.t...|...n.d
+00001300: 1c64 1d74 10a0 11a1 0076 0073 ec74 12a0  .d.t.....v.s.t..
+00001310: 1374 0da1 0172 f174 12a0 1474 0da1 016e  .t...r.t...t...n
+00001320: 0164 1d74 12a0 147c 0ca1 0174 12a0 147c  .d.t...|...t...|
+00001330: 0da1 0164 1e9c 0516 007d 0e74 1574 12a0  ...d.....}.t.t..
+00001340: 167c 0ea1 0183 0182 0164 0004 007d 0c7d  .|.......d...}.}
+00001350: 0d74 0d6a 0e7d 0c74 0f7c 0b7c 0c83 027d  .t.j.}.t.|.|...}
+00001360: 0d7c 0d90 0173 6164 1a64 1b74 10a0 11a1  .|...sad.d.t....
+00001370: 0076 0090 0173 2274 12a0 1374 0fa1 0190  .v...s"t...t....
+00001380: 0172 2774 12a0 1474 0fa1 016e 0164 1b64  .r't...t...n.d.d
+00001390: 1f74 10a0 11a1 0076 0090 0173 3574 12a0  .t.....v...s5t..
+000013a0: 137c 0ba1 0190 0172 3a74 12a0 147c 0ba1  .|.....r:t...|..
+000013b0: 016e 0164 1f64 1d74 10a0 11a1 0076 0090  .n.d.d.t.....v..
+000013c0: 0173 4874 12a0 1374 0da1 0190 0172 4d74  .sHt...t.....rMt
+000013d0: 12a0 1474 0da1 016e 0164 1d74 12a0 147c  ...t...n.d.t...|
+000013e0: 0ca1 0174 12a0 147c 0da1 0164 1e9c 0516  ...t...|...d....
+000013f0: 007d 0e74 1574 12a0 167c 0ea1 0183 0182  .}.t.t...|......
+00001400: 0164 0004 007d 0c7d 0d64 0053 0029 204e  .d...}.}.d.S.) N
+00001410: e90a 0000 0054 e902 0000 0063 0000 0000  .....T.....c....
+00001420: 0000 0000 0000 0000 0000 0000 0c00 0000  ................
+00001430: 0000 0000 f386 0000 0065 005a 0164 005a  .........e.Z.d.Z
+00001440: 0264 0f64 0265 0366 0287 0066 0164 0364  .d.d.e.f...f.d.d
+00001450: 0484 0d5a 0464 0565 056a 0664 0665 056a  ...Z.d.e.j.d.e.j
+00001460: 0764 0765 0865 056a 0665 0965 056a 0719  .d.e.e.j.e.e.j..
+00001470: 0066 0219 0066 0664 0864 0984 045a 0a09  .f...f.d.d...Z..
+00001480: 0a09 0b64 1064 0565 056a 0664 0665 0965  ...d.d.e.j.d.e.e
+00001490: 056a 0719 0064 0c65 0b64 0765 0865 056a  .j...d.e.d.e.e.j
+000014a0: 0665 0965 056a 0719 0066 0219 0066 0864  .e.e.j...f...f.d
+000014b0: 0d64 0e84 055a 0c87 0004 005a 0d53 0029  .d...Z.....Z.S.)
+000014c0: 117a 3674 6573 745f 626c 7565 6361 7374  .z6test_bluecast
+000014d0: 5f77 6974 685f 6375 7374 6f6d 5f6d 6f64  _with_custom_mod
+000014e0: 656c 2e3c 6c6f 6361 6c73 3e2e 5246 4543  el.<locals>.RFEC
+000014f0: 5653 656c 6563 746f 7272 0100 0000 7214  VSelectorr....r.
+00001500: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00001510: 0200 0000 0800 0000 1300 0000 f342 0000  .............B..
+00001520: 0074 0083 00a0 01a1 0001 0064 007c 005f  .t.........d.|._
+00001530: 027c 017c 005f 0374 0474 05a0 06a1 0064  .|.|._.t.t.....d
+00001540: 0174 0764 027c 0164 0364 048d 0364 0174  .t.d.|.d.d...d.t
+00001550: 0874 0983 0164 0264 058d 067c 005f 0a64  .t...d.d...|._.d
+00001560: 0053 00a9 064e 721b 0000 0072 5800 0000  .S...Nr....rX...
+00001570: 5429 0272 1400 0000 da07 7368 7566 666c  T).r......shuffl
+00001580: 6529 06da 0965 7374 696d 6174 6f72 da04  e)...estimator..
+00001590: 7374 6570 da02 6376 5a16 6d69 6e5f 6665  step..cvZ.min_fe
+000015a0: 6174 7572 6573 5f74 6f5f 7365 6c65 6374  atures_to_select
+000015b0: 5a07 7363 6f72 696e 67da 066e 5f6a 6f62  Z.scoring..n_job
+000015c0: 73a9 0bda 0573 7570 6572 724f 0000 00da  s....superrO....
+000015d0: 1173 656c 6563 7465 645f 6665 6174 7572  .selected_featur
+000015e0: 6573 7214 0000 0072 0500 0000 da03 7867  esr....r......xg
+000015f0: 625a 0d58 4742 436c 6173 7369 6669 6572  bZ.XGBClassifier
+00001600: 7208 0000 0072 0600 0000 7207 0000 00da  r....r....r.....
+00001610: 1273 656c 6563 7469 6f6e 5f73 7472 6174  .selection_strat
+00001620: 6567 79a9 0272 2000 0000 7214 0000 00a9  egy..r ...r.....
+00001630: 01da 095f 5f63 6c61 7373 5f5f 7218 0000  ...__class__r...
+00001640: 0072 1900 0000 724f 0000 0073 0000 00f3  .r....rO...s....
+00001650: 1600 0000 0a01 0601 0601 0201 0601 0201  ................
+00001660: 0c01 0201 0601 0201 0cfa 7a3f 7465 7374  ..........z?test
+00001670: 5f62 6c75 6563 6173 745f 7769 7468 5f63  _bluecast_with_c
+00001680: 7573 746f 6d5f 6d6f 6465 6c2e 3c6c 6f63  ustom_model.<loc
+00001690: 616c 733e 2e52 4645 4356 5365 6c65 6374  als>.RFECVSelect
+000016a0: 6f72 2e5f 5f69 6e69 745f 5f72 1e00 0000  or.__init__r....
+000016b0: 7222 0000 0072 1200 0000 6303 0000 0000  r"...r....c.....
+000016c0: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
+000016d0: 0000 0073 3400 0000 7c00 6a00 a001 7c01  ...s4...|.j...|.
+000016e0: 7c02 a102 0100 7c00 6a00 6a02 7c00 5f03  |.....|.j.j.|._.
+000016f0: 7c01 6a04 6400 6400 8502 7c00 6a03 6602  |.j.d.d...|.j.f.
+00001700: 1900 7d01 7c01 7c02 6602 5300 724d 0000  ..}.|.|.f.S.rM..
+00001710: 0029 0572 6500 0000 7254 0000 005a 0873  .).re...rT...Z.s
+00001720: 7570 706f 7274 5f72 6300 0000 da03 6c6f  upport_rc.....lo
+00001730: 6372 2400 0000 7218 0000 0072 1800 0000  cr$...r....r....
+00001740: 7219 0000 0072 2500 0000 8000 0000 7308  r....r%.......s.
+00001750: 0000 000e 030a 0114 0108 017a 4474 6573  ...........zDtes
+00001760: 745f 626c 7565 6361 7374 5f77 6974 685f  t_bluecast_with_
+00001770: 6375 7374 6f6d 5f6d 6f64 656c 2e3c 6c6f  custom_model.<lo
+00001780: 6361 6c73 3e2e 5246 4543 5653 656c 6563  cals>.RFECVSelec
+00001790: 746f 722e 6669 745f 7472 616e 7366 6f72  tor.fit_transfor
+000017a0: 6d4e 4672 2600 0000 6304 0000 0000 0000  mNFr&...c.......
+000017b0: 0000 0000 0004 0000 0003 0000 0053 0000  .............S..
+000017c0: 0073 1c00 0000 7c01 6a00 6400 6400 8502  .s....|.j.d.d...
+000017d0: 7c00 6a01 6602 1900 7d01 7c01 7c02 6602  |.j.f...}.|.|.f.
+000017e0: 5300 724d 0000 0029 0272 6a00 0000 7263  S.rM...).rj...rc
+000017f0: 0000 0072 2a00 0000 7218 0000 0072 1800  ...r*...r....r..
+00001800: 0000 7219 0000 0072 2b00 0000 8800 0000  ..r....r+.......
+00001810: 7304 0000 0014 0608 017a 4074 6573 745f  s........z@test_
+00001820: 626c 7565 6361 7374 5f77 6974 685f 6375  bluecast_with_cu
+00001830: 7374 6f6d 5f6d 6f64 656c 2e3c 6c6f 6361  stom_model.<loca
+00001840: 6c73 3e2e 5246 4543 5653 656c 6563 746f  ls>.RFECVSelecto
+00001850: 722e 7472 616e 7366 6f72 6da9 0172 0100  r.transform..r..
+00001860: 0000 722c 0000 00a9 0e72 2d00 0000 722e  ..r,.....r-...r.
+00001870: 0000 0072 2f00 0000 da03 696e 7472 4f00  ...r/.....intrO.
+00001880: 0000 7228 0000 0072 3000 0000 7229 0000  ..r(...r0...r)..
+00001890: 0072 0300 0000 7202 0000 0072 2500 0000  .r....r....r%...
+000018a0: 7231 0000 0072 2b00 0000 da0d 5f5f 636c  r1...r+.....__cl
+000018b0: 6173 7363 656c 6c5f 5f72 1800 0000 7218  asscell__r....r.
+000018c0: 0000 0072 6700 0000 7219 0000 00da 0d52  ...rg...r......R
+000018d0: 4645 4356 5365 6c65 6374 6f72 7200 0000  FECVSelectorr...
+000018e0: 7328 0000 0008 0014 0102 0d04 0102 ff04  s(..............
+000018f0: 0102 ff12 020a fe02 0b02 0104 fc04 0202  ................
+00001900: fe08 0302 fd02 0402 fc12 0512 fb72 6f00  .............ro.
+00001910: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001920: 0000 000c 0000 0000 0000 0072 5900 0000  ...........rY...
+00001930: 2911 7a3d 7465 7374 5f62 6c75 6563 6173  ).z=test_bluecas
+00001940: 745f 7769 7468 5f63 7573 746f 6d5f 6d6f  t_with_custom_mo
+00001950: 6465 6c2e 3c6c 6f63 616c 733e 2e4d 7943  del.<locals>.MyC
+00001960: 7573 746f 6d50 7265 7072 6f63 6573 736f  ustomPreprocesso
+00001970: 7272 0100 0000 7214 0000 0063 0200 0000  rr....r....c....
+00001980: 0000 0000 0000 0000 0200 0000 0800 0000  ................
+00001990: 1300 0000 725a 0000 0072 5b00 0000 7261  ....rZ...r[...ra
+000019a0: 0000 0072 6600 0000 7267 0000 0072 1800  ...rf...rg...r..
+000019b0: 0000 7219 0000 0072 4f00 0000 9200 0000  ..r....rO.......
+000019c0: 7269 0000 007a 4674 6573 745f 626c 7565  ri...zFtest_blue
+000019d0: 6361 7374 5f77 6974 685f 6375 7374 6f6d  cast_with_custom
+000019e0: 5f6d 6f64 656c 2e3c 6c6f 6361 6c73 3e2e  _model.<locals>.
+000019f0: 4d79 4375 7374 6f6d 5072 6570 726f 6365  MyCustomPreproce
+00001a00: 7373 6f72 2e5f 5f69 6e69 745f 5f72 1e00  ssor.__init__r..
+00001a10: 0000 7222 0000 0072 1200 0000 6303 0000  ..r"...r....c...
+00001a20: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+00001a30: 0053 0000 00f3 0800 0000 7c01 7c02 6602  .S........|.|.f.
+00001a40: 5300 724d 0000 0072 1800 0000 7224 0000  S.rM...r....r$..
+00001a50: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001a60: 7225 0000 009f 0000 0073 0200 0000 0803  r%.......s......
+00001a70: 7a4b 7465 7374 5f62 6c75 6563 6173 745f  zKtest_bluecast_
+00001a80: 7769 7468 5f63 7573 746f 6d5f 6d6f 6465  with_custom_mode
+00001a90: 6c2e 3c6c 6f63 616c 733e 2e4d 7943 7573  l.<locals>.MyCus
+00001aa0: 746f 6d50 7265 7072 6f63 6573 736f 722e  tomPreprocessor.
+00001ab0: 6669 745f 7472 616e 7366 6f72 6d4e 4672  fit_transformNFr
+00001ac0: 2600 0000 6304 0000 0000 0000 0000 0000  &...c...........
+00001ad0: 0004 0000 0002 0000 0053 0000 0072 7000  .........S...rp.
+00001ae0: 0000 724d 0000 0072 1800 0000 722a 0000  ..rM...r....r*..
+00001af0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001b00: 722b 0000 00a4 0000 0073 0200 0000 0806  r+.......s......
+00001b10: 7a47 7465 7374 5f62 6c75 6563 6173 745f  zGtest_bluecast_
+00001b20: 7769 7468 5f63 7573 746f 6d5f 6d6f 6465  with_custom_mode
+00001b30: 6c2e 3c6c 6f63 616c 733e 2e4d 7943 7573  l.<locals>.MyCus
+00001b40: 746f 6d50 7265 7072 6f63 6573 736f 722e  tomPreprocessor.
+00001b50: 7472 616e 7366 6f72 6d72 6b00 0000 722c  transformrk...r,
+00001b60: 0000 0072 6c00 0000 7218 0000 0072 1800  ...rl...r....r..
+00001b70: 0000 7267 0000 0072 1900 0000 da14 4d79  ..rg...r......My
+00001b80: 4375 7374 6f6d 5072 6570 726f 6365 7373  CustomPreprocess
+00001b90: 6f72 9100 0000 7328 0000 0008 0014 0102  or....s(........
+00001ba0: 0d04 0102 ff04 0102 ff12 020a fe02 0802  ................
+00001bb0: 0104 fc04 0202 fe08 0302 fd02 0402 fc12  ................
+00001bc0: 0512 fb72 7100 0000 7233 0000 0072 2200  ...rq...r3...r".
+00001bd0: 0000 2906 7234 0000 0072 3500 0000 5a08  ..).r4...r5...Z.
+00001be0: 6d6c 5f6d 6f64 656c 5a0d 636f 6e66 5f74  ml_modelZ.conf_t
+00001bf0: 7261 696e 696e 67da 1763 7573 746f 6d5f  raining..custom_
+00001c00: 6665 6174 7572 655f 7365 6c65 6374 6f72  feature_selector
+00001c10: 5a13 6375 7374 6f6d 5f70 7265 7072 6f63  Z.custom_preproc
+00001c20: 6573 736f 7263 0100 0000 0000 0000 0000  essorc..........
+00001c30: 0000 0200 0000 0300 0000 5300 0000 f310  ..........S.....
+00001c40: 0000 0067 007c 005d 047d 017c 0191 0271  ...g.|.].}.|...q
+00001c50: 0253 0072 1800 0000 7218 0000 00a9 02da  .S.r....r.......
+00001c60: 022e 30da 0169 7218 0000 0072 1800 0000  ..0..ir....r....
+00001c70: 7219 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+00001c80: 3ebc 0000 00f3 0200 0000 1000 7a33 7465  >...........z3te
+00001c90: 7374 5f62 6c75 6563 6173 745f 7769 7468  st_bluecast_with
+00001ca0: 5f63 7573 746f 6d5f 6d6f 6465 6c2e 3c6c  _custom_model.<l
+00001cb0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00001cc0: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
+00001cd0: 0000 0300 0000 5300 0000 7273 0000 0072  ......S...rs...r
+00001ce0: 1800 0000 7218 0000 0072 7400 0000 7218  ....r....rt...r.
+00001cf0: 0000 0072 1800 0000 7219 0000 0072 7700  ...r....r....rw.
+00001d00: 0000 bd00 0000 7278 0000 0063 0100 0000  ......rx...c....
+00001d10: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001d20: 5300 0000 7273 0000 0072 1800 0000 7218  S...rs...r....r.
+00001d30: 0000 0072 7400 0000 7218 0000 0072 1800  ...rt...r....r..
+00001d40: 0000 7219 0000 0072 7700 0000 be00 0000  ..r....rw.......
+00001d50: 7278 0000 0063 0100 0000 0000 0000 0000  rx...c..........
+00001d60: 0000 0200 0000 0300 0000 5300 0000 7273  ..........S...rs
+00001d70: 0000 0072 1800 0000 7218 0000 0072 7400  ...r....r....rt.
+00001d80: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00001d90: 0072 7700 0000 bf00 0000 7278 0000 0063  .rw.......rx...c
+00001da0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001db0: 0300 0000 5300 0000 7273 0000 0072 1800  ....S...rs...r..
+00001dc0: 0000 7218 0000 0072 7400 0000 7218 0000  ..r....rt...r...
+00001dd0: 0072 1800 0000 7219 0000 0072 7700 0000  .r....r....rw...
+00001de0: c000 0000 7278 0000 0063 0100 0000 0000  ....rx...c......
+00001df0: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
+00001e00: 0000 7273 0000 0072 1800 0000 7218 0000  ..rs...r....r...
+00001e10: 0072 7400 0000 7218 0000 0072 1800 0000  .rt...r....r....
+00001e20: 7219 0000 0072 7700 0000 c100 0000 7278  r....rw.......rx
+00001e30: 0000 0029 065a 0866 6561 7475 7265 315a  ...).Z.feature1Z
+00001e40: 0866 6561 7475 7265 325a 0866 6561 7475  .feature2Z.featu
+00001e50: 7265 335a 0866 6561 7475 7265 345a 0866  re3Z.feature4Z.f
+00001e60: 6561 7475 7265 355a 0866 6561 7475 7265  eature5Z.feature
+00001e70: 3629 0a72 0100 0000 721b 0000 0072 0100  6).r....r....r..
+00001e80: 0000 721b 0000 0072 0100 0000 721b 0000  ..r....r....r...
+00001e90: 0072 0100 0000 721b 0000 0072 0100 0000  .r....r....r....
+00001ea0: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001eb0: 0000 0200 0000 0300 0000 5300 0000 7273  ..........S...rs
+00001ec0: 0000 0072 1800 0000 7218 0000 0072 7400  ...r....r....rt.
+00001ed0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00001ee0: 0072 7700 0000 c700 0000 7278 0000 0063  .rw.......rx...c
+00001ef0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001f00: 0300 0000 5300 0000 7273 0000 0072 1800  ....S...rs...r..
+00001f10: 0000 7218 0000 0072 7400 0000 7218 0000  ..r....rt...r...
+00001f20: 0072 1800 0000 7219 0000 0072 7700 0000  .r....r....rw...
+00001f30: c800 0000 7278 0000 0063 0100 0000 0000  ....rx...c......
+00001f40: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
+00001f50: 0000 7273 0000 0072 1800 0000 7218 0000  ..rs...r....r...
+00001f60: 0072 7400 0000 7218 0000 0072 1800 0000  .rt...r....r....
+00001f70: 7219 0000 0072 7700 0000 c900 0000 7278  r....rw.......rx
+00001f80: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001f90: 0200 0000 0300 0000 5300 0000 7273 0000  ........S...rs..
+00001fa0: 0072 1800 0000 7218 0000 0072 7400 0000  .r....r....rt...
+00001fb0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00001fc0: 7700 0000 ca00 0000 7278 0000 0063 0100  w.......rx...c..
+00001fd0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001fe0: 0000 5300 0000 7273 0000 0072 1800 0000  ..S...rs...r....
+00001ff0: 7218 0000 0072 7400 0000 7218 0000 0072  r....rt...r....r
+00002000: 1800 0000 7219 0000 0072 7700 0000 cb00  ....r....rw.....
+00002010: 0000 7278 0000 0063 0100 0000 0000 0000  ..rx...c........
+00002020: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00002030: 7273 0000 0072 1800 0000 7218 0000 0072  rs...r....r....r
+00002040: 7400 0000 7218 0000 0072 1800 0000 7219  t...r....r....r.
+00002050: 0000 0072 7700 0000 cc00 0000 7278 0000  ...rw.......rx..
+00002060: 007a 5261 7373 6572 7420 2528 7079 3629  .zRassert %(py6)
+00002070: 730a 7b25 2870 7936 2973 203d 2025 2870  s.{%(py6)s = %(p
+00002080: 7930 2973 2825 2870 7931 2973 2c20 2528  y0)s(%(py1)s, %(
+00002090: 7079 3429 730a 7b25 2870 7934 2973 203d  py4)s.{%(py4)s =
+000020a0: 2025 2870 7932 2973 2e6e 6461 7272 6179   %(py2)s.ndarray
+000020b0: 0a7d 290a 7d72 2700 0000 7255 0000 00da  .}).}r'...rU....
+000020c0: 026e 7029 0572 3b00 0000 723c 0000 005a  .np).r;...r<...Z
+000020d0: 0370 7932 5a03 7079 3472 3d00 0000 7256  .py2Z.py4r=...rV
+000020e0: 0000 0029 1772 4c00 0000 720a 0000 005a  ...).rL...r....Z
+000020f0: 1c68 7970 6572 7061 7261 6d65 7465 725f  .hyperparameter_
+00002100: 7475 6e69 6e67 5f72 6f75 6e64 735a 1865  tuning_roundsZ.e
+00002110: 6e61 626c 655f 6665 6174 7572 655f 7365  nable_feature_se
+00002120: 6c65 6374 696f 6e5a 1468 7970 6572 7475  lectionZ.hypertu
+00002130: 6e69 6e67 5f63 765f 666f 6c64 7372 0f00  ning_cv_foldsr..
+00002140: 0000 7209 0000 0072 2800 0000 7230 0000  ..r....r(...r0..
+00002150: 00da 0572 616e 6765 7229 0000 0072 5400  ...ranger)...rT.
+00002160: 0000 7241 0000 0072 7900 0000 da07 6e64  ..rA...ry.....nd
+00002170: 6172 7261 7972 2700 0000 7245 0000 0072  arrayr'...rE...r
+00002180: 4600 0000 7243 0000 0072 4700 0000 7248  F...rC...rG...rH
+00002190: 0000 0072 4900 0000 724a 0000 0029 0f5a  ...rI...rJ...).Z
+000021a0: 0c63 7573 746f 6d5f 6d6f 6465 6c5a 0c74  .custom_modelZ.t
+000021b0: 7261 696e 5f63 6f6e 6669 6772 6f00 0000  rain_configro...
+000021c0: 7271 0000 0072 7200 0000 5a0e 6375 7374  rq...rr...Z.cust
+000021d0: 756d 5f70 7265 7072 6f63 da08 626c 7565  um_preproc..blue
+000021e0: 6361 7374 7250 0000 0072 5200 0000 7251  castrP...rR...rQ
+000021f0: 0000 0072 5500 0000 7256 0000 005a 0b40  ...rU...rV...Z.@
+00002200: 7079 5f61 7373 6572 7433 5a0b 4070 795f  py_assert3Z.@py_
+00002210: 6173 7365 7274 355a 0b40 7079 5f66 6f72  assert5Z.@py_for
+00002220: 6d61 7437 7218 0000 0072 1800 0000 7219  mat7r....r....r.
+00002230: 0000 00da 1f74 6573 745f 626c 7565 6361  .....test_blueca
+00002240: 7374 5f77 6974 685f 6375 7374 6f6d 5f6d  st_with_custom_m
+00002250: 6f64 656c 6900 0000 7352 0000 0006 0206  odeli...sR......
+00002260: 0106 0106 0106 0110 0310 1f06 1b06 0102  ................
+00002270: 0302 0102 0102 0102 0102 0102 0106 fa04  ................
+00002280: 0a10 0210 0110 0110 0110 0110 0104 fa04  ................
+00002290: ff0e 0a04 0110 0210 0110 0110 0110 0110  ................
+000022a0: 0104 fa04 ff08 0b0c 030e 03ac 03bc 0172  ...............r
+000022b0: 7d00 0000 292c da08 6275 696c 7469 6e73  }...),..builtins
+000022c0: 7245 0000 00da 195f 7079 7465 7374 2e61  rE....._pytest.a
+000022d0: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
+000022e0: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
+000022f0: 7269 7465 7243 0000 00da 0674 7970 696e  riterC.....typin
+00002300: 6772 0200 0000 7203 0000 00da 056e 756d  gr....r......num
+00002310: 7079 7279 0000 00da 0670 616e 6461 7372  pyry.....pandasr
+00002320: 2800 0000 da06 7079 7465 7374 5a07 7867  (.....pytestZ.xg
+00002330: 626f 6f73 7472 6400 0000 5a10 736b 6c65  boostrd...Z.skle
+00002340: 6172 6e2e 656e 7365 6d62 6c65 7204 0000  arn.ensembler...
+00002350: 005a 1973 6b6c 6561 726e 2e66 6561 7475  .Z.sklearn.featu
+00002360: 7265 5f73 656c 6563 7469 6f6e 7205 0000  re_selectionr...
+00002370: 005a 0f73 6b6c 6561 726e 2e6d 6574 7269  .Z.sklearn.metri
+00002380: 6373 7206 0000 0072 0700 0000 5a17 736b  csr....r....Z.sk
+00002390: 6c65 6172 6e2e 6d6f 6465 6c5f 7365 6c65  learn.model_sele
+000023a0: 6374 696f 6e72 0800 0000 5a18 626c 7565  ctionr....Z.blue
+000023b0: 6361 7374 2e62 6c75 6570 7269 6e74 732e  cast.blueprints.
+000023c0: 6361 7374 7209 0000 005a 1f62 6c75 6563  castr....Z.bluec
+000023d0: 6173 742e 636f 6e66 6967 2e74 7261 696e  ast.config.train
+000023e0: 696e 675f 636f 6e66 6967 720a 0000 0072  ing_configr....r
+000023f0: 0b00 0000 5a22 626c 7565 6361 7374 2e6d  ....Z"bluecast.m
+00002400: 6c5f 6d6f 6465 6c6c 696e 672e 6261 7365  l_modelling.base
+00002410: 5f63 6c61 7373 6573 720c 0000 0072 0d00  _classesr....r..
+00002420: 0000 720e 0000 005a 1d62 6c75 6563 6173  ..r....Z.bluecas
+00002430: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
+00002440: 6375 7374 6f6d 720f 0000 00da 2462 6c75  customr.....$blu
+00002450: 6563 6173 742e 7465 7374 732e 6d61 6b65  ecast.tests.make
+00002460: 5f64 6174 612e 6372 6561 7465 5f64 6174  _data.create_dat
+00002470: 6172 1100 0000 da07 6669 7874 7572 6572  ar......fixturer
+00002480: 3000 0000 721a 0000 0072 4b00 0000 724c  0...r....rK...rL
+00002490: 0000 0072 7d00 0000 7218 0000 0072 1800  ...r}...r....r..
+000024a0: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
+000024b0: 6f64 756c 653e 0100 0000 7326 0000 002a  odule>....s&...*
+000024c0: 0008 0208 0108 0108 010c 010c 0110 010c  ................
+000024d0: 010c 0210 0114 010c 050c 0104 031c 0108  ................
+000024e0: 0610 370c 14                             ..7..
```

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.9/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc` & `bluecast-0.9/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/make_data/create_data.py` & `bluecast-0.9/bluecast/tests/make_data/create_data.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_cast.py` & `bluecast-0.9/bluecast/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_cast_cv.py` & `bluecast-0.9/bluecast/tests/test_cast_cv.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_check_gpu_support.py` & `bluecast-0.9/bluecast/tests/test_check_gpu_support.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_custom_processing_base_class.py` & `bluecast-0.9/bluecast/tests/test_custom_processing_base_class.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_datetime_features.py` & `bluecast-0.9/bluecast/tests/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_encode_target_labels.py` & `bluecast-0.9/bluecast/tests/test_encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_feature_type_detector.py` & `bluecast-0.9/bluecast/tests/test_feature_type_detector.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_load_for_production.py` & `bluecast-0.9/bluecast/tests/test_load_for_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_nulls_and_infs.py` & `bluecast-0.9/bluecast/tests/test_nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_save_to_production.py` & `bluecast-0.9/bluecast/tests/test_save_to_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_schema_checks.py` & `bluecast-0.9/bluecast/tests/test_schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_shap_explanations.py` & `bluecast-0.9/bluecast/tests/test_shap_explanations.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_target_encoding_binary.py` & `bluecast-0.9/bluecast/tests/test_target_encoding_binary.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_target_encoding_multiclass.py` & `bluecast-0.9/bluecast/tests/test_target_encoding_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/bluecast/tests/test_train_test_split.py` & `bluecast-0.9/bluecast/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.8/pyproject.toml` & `bluecast-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluecast"
-version = "0.8"
+version = "0.9"
 description = "A lightweight and fast automl framework"
 authors = ["Thomas Meißner <meissnercorporation@gmx.de>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `bluecast-0.8/PKG-INFO` & `bluecast-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecast
-Version: 0.8
+Version: 0.9
 Summary: A lightweight and fast automl framework
 Home-page: https://github.com/ThomasMeissnerDS/BlueCast
 License: GPL-3.0-only
 Author: Thomas Meißner
 Author-email: meissnercorporation@gmx.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -160,14 +160,24 @@
             :, feat_type_detector.num_columns])
 
 # show correlation to target
 correlation_to_target(train_data.loc[
             :, feat_type_detector.num_columns
         ],
         "EC1",)
+
+# show feature space after principal component analysis
+plot_pca(train_data.loc[
+            :, feat_type_detector.num_columns
+        ], "target")
+
+# show feature space after t-SNE
+plot_tsne(train_data.loc[
+            :, feat_type_detector.num_columns
+        ], "target", perplexity=30, random_state=0)
 ```
 
 #### Enable cross-validation
 
 While the default behaviour of BlueCast is to use a simple
 train-test-split, cross-validation can be enabled easily:
```


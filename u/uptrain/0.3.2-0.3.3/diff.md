# Comparing `tmp/uptrain-0.3.2.tar.gz` & `tmp/uptrain-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptrain-0.3.2.tar", last modified: Thu Jul  6 12:17:42 2023, max compression
+gzip compressed data, was "uptrain-0.3.3.tar", last modified: Fri Jul  7 06:55:33 2023, max compression
```

## Comparing `uptrain-0.3.2.tar` & `uptrain-0.3.3.tar`

### file list

```diff
@@ -1,185 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.195446 uptrain-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 12:17:32.000000 uptrain-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-06 12:17:42.195446 uptrain-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-07-06 12:17:32.000000 uptrain-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.175445 uptrain-0.3.2/regression_testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/regression_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-07-06 12:17:32.000000 uptrain-0.3.2/regression_testing/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:17:42.195446 uptrain-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-06 12:17:32.000000 uptrain-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.175445 uptrain-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-06 12:17:32.000000 uptrain-0.3.2/tests/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.175445 uptrain-0.3.2/uptrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.175445 uptrain-0.3.2/uptrain/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/dashboard/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/dashboard/st_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/dashboard/st_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/dashboard/st_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.179445 uptrain-0.3.2/uptrain/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/framework/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/framework/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/framework/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/framework/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.179445 uptrain-0.3.2/uptrain/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.179445 uptrain-0.3.2/uptrain/operators/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.179445 uptrain-0.3.2/uptrain/operators/code/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/code/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/code/sql/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/code/sql/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/drift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/embs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.179445 uptrain-0.3.2/uptrain/operators/io/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/io/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.183446 uptrain-0.3.2/uptrain/operators/language/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/model_grade.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/openai_evals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/rouge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/language/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/operators/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.183446 uptrain-0.3.2/uptrain/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/utilities/sql_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/utilities/sqlglot_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.183446 uptrain-0.3.2/uptrain/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.183446 uptrain-0.3.2/uptrain/v0/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.183446 uptrain-0.3.2/uptrain/v0/core/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.183446 uptrain-0.3.2/uptrain/v0/core/classes/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/algorithms/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/algorithms/popularity_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.183446 uptrain-0.3.2/uptrain/v0/core/classes/distances/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/distances/abstract_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/distances/cosine_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/distances/distance_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/distances/hamming_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/distances/l2_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/distances/norm_ratio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.183446 uptrain-0.3.2/uptrain/v0/core/classes/finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/finetuning/AbstractFinetune.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/finetuning/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.187445 uptrain-0.3.2/uptrain/v0/core/classes/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/helpers/annotation_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/helpers/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/helpers/dataset_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/helpers/model_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.187445 uptrain-0.3.2/uptrain/v0/core/classes/io/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/io/runtime_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.187445 uptrain-0.3.2/uptrain/v0/core/classes/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/logging/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/logging/log_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/logging/log_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/logging/new_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/logging/new_st_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/logging/new_st_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/logging/st_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.187445 uptrain-0.3.2/uptrain/v0/core/classes/managers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/managers/check_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.187445 uptrain-0.3.2/uptrain/v0/core/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/abstract_measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/feature_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/input_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/measurable_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/output_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/measurables/scalar_from_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/core/classes/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/abstract_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/abstract_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/custom_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/data_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/edge_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/feature_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/model_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/monitors/output_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/core/classes/signals/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/signals/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/signals/signal_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/core/classes/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/statistics/abstract_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/statistics/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/statistics/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/statistics/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/statistics/norm_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/statistics/old_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/core/classes/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/visuals/abstract_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/visuals/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/visuals/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/visuals/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/classes/visuals/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/core/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/encoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/lib/datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/lib/helper_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/core/lib/model_signal_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/ee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/ee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/ee/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/ee/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/ee/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/ee/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/ee/classes/measurables/llm_measurables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/uptrain/v0/ee/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/ee/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/ee/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/ee/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-06 12:17:32.000000 uptrain-0.3.2/uptrain/v0/ee/lib/ops_agg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.175445 uptrain-0.3.2/uptrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-06 12:17:42.000000 uptrain-0.3.2/uptrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-06 12:17:42.000000 uptrain-0.3.2/uptrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:17:42.000000 uptrain-0.3.2/uptrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-06 12:17:42.000000 uptrain-0.3.2/uptrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 12:17:42.000000 uptrain-0.3.2/uptrain.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:17:42.191445 uptrain-0.3.2/validation_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 12:17:32.000000 uptrain-0.3.2/validation_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 12:17:32.000000 uptrain-0.3.2/validation_wrapper/validation_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 06:55:23.000000 uptrain-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 06:55:33.855613 uptrain-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-07 06:55:23.000000 uptrain-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-07 06:55:23.000000 uptrain-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:55:33.855613 uptrain-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-07-07 06:55:23.000000 uptrain-0.3.3/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/dashboard/st_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/dashboard/st_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/dashboard/st_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/operators/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/code/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/embs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/operators/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/io/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/operators/language/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/model_grade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.831613 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/completion_fns/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/elsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/openai_evals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/utilities/sql_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/utilities/sqlglot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/v0/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/v0/core/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/v0/core/classes/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/algorithms/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/algorithms/popularity_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/abstract_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/cosine_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/distance_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/hamming_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/l2_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/norm_ratio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/finetuning/AbstractFinetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/finetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/finetuning/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/annotation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/dataset_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/model_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/io/runtime_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/log_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/log_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/new_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/new_st_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/new_st_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/st_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.847613 uptrain-0.3.3/uptrain/v0/core/classes/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/managers/check_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.847613 uptrain-0.3.3/uptrain/v0/core/classes/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/abstract_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/feature_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/input_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/measurable_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/output_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/scalar_from_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.847613 uptrain-0.3.3/uptrain/v0/core/classes/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/abstract_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/abstract_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/custom_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/edge_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/feature_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/model_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/output_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/classes/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/signals/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/signals/signal_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/classes/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/abstract_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/norm_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/old_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/classes/visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/abstract_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/encoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/model_signal_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/ee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/ee/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/ee/classes/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/classes/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/classes/measurables/llm_measurables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/uptrain/v0/ee/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/lib/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/lib/ops_agg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/uptrain/v0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_a-b_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_concept_drift_custom_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_data_integrity_zscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_edge_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/uptrain/v0/tests/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/get_data_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/model_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/model_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/pushup_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_monitors_concept_drift_adwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_monitors_concept_drift_ddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_recommender_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_visuals_dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_visuals_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_visuals_shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/uptrain/validation_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/validation_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/validation_wrapper/validation_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/top_level.txt
```

### Comparing `uptrain-0.3.2/LICENSE` & `uptrain-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/PKG-INFO` & `uptrain-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: uptrain
-Version: 0.3.2
+Version: 0.3.3
 Summary: UpTrain - ML Observability and Retraining Framework
-Home-page: https://github.com/uptrain-ai/uptrain
-Maintainer: UpTrain AI Team
-Maintainer-email: uptrain.ai@gmail.com
-License: Apache License 2.0
-Keywords: uptrain ai retraining ML observability
+Maintainer-email: UpTrain AI Team <uptrain.ai@gmail.com>
+License: Apache-2.0
+Project-URL: Homepage, https://uptrain.ai
+Project-URL: Repository, https://github.com/uptrain-ai/uptrain
+Keywords: uptrain,ai,retraining,ML,observability
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
-Provides-Extra: v0
-Provides-Extra: full
+Provides-Extra: test
 License-File: LICENSE
 
 <h4 align="center">
   <a href="https://uptrain.ai">
     <img width="300" src="https://user-images.githubusercontent.com/108270398/214240695-4f958b76-c993-4ddd-8de6-8668f4d0da84.png" alt="uptrain">
   </a>
 </h4>
@@ -105,14 +104,19 @@
 To run it on your machine, checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/quickstart):
 
 ### Install the package through pip:
 ```bash
 pip install uptrain
 ```
 
+Note: Uptrain uses commonly used python libraries like openai-evals and sentence-transformers. To make sure, all the functionalities work, use the `uptrain-add` command to install the full version of the package.
+```bash
+uptrain-add --feature full
+```
+
 ### How to define checks:
 Say we want to check whether our model's responses contain any grammatical mistakes or not.
 
 ```python
 # Define your checkset - list of simple checks, dataset file, 
 # and api_keys
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.3.2 Summary: UpTrain - ML
-Observability and Retraining Framework Home-page: https://github.com/uptrain-
-ai/uptrain Maintainer: UpTrain AI Team Maintainer-email: uptrain.ai@gmail.com
-License: Apache License 2.0 Keywords: uptrain ai retraining ML observability
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-Provides-Extra: v0 Provides-Extra: full License-File: LICENSE
+Metadata-Version: 2.1 Name: uptrain Version: 0.3.3 Summary: UpTrain - ML
+Observability and Retraining Framework Maintainer-email: UpTrain AI Team
+ai@gmail.com> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
+Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
+uptrain,ai,retraining,ML,observability Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
+:: Software Development :: Build Tools Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown Provides-Extra: test License-File:
+LICENSE
                                *** [uptrain] ***
 ***** An open-source framework to evaluate, test and monitor LLM applications
 *****
             Docs  - Slack_Community - Bug_Report - Feature_Request
    *** [https://img.shields.io/github/contributors/uptrain-ai/uptrain] [PRs
                   Welcome] [Docs] [Community] [Website]  ***
   **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM
@@ -40,22 +41,25 @@
 for hallucinations. - **[Toxic Keywords Checks]()** - Make sure your model
 outputs are not biased or contain toxic keywords. - **[Feature Slicing]()** -
 Built-in pivoting functionalities for data dice and slice to pinpoint low-
 performing cohorts. - **[Realtime Dashboards]()** - Monitor your model's
 performance in realtime. # Get started ð  To run it on your machine,
 checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/
 quickstart): ### Install the package through pip: ```bash pip install uptrain
-``` ### How to define checks: Say we want to check whether our model's
-responses contain any grammatical mistakes or not. ```python # Define your
-checkset - list of simple checks, dataset file, # and api_keys checkset =
-CheckSet( checks = Check( name = "grammar_score", operators = [ GrammarScore
-( col_in_text = "model_response", col_out = "grammar_score" ), ], plots =
-PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader(fpath =
-'...') ) settings = Settings(openai_api_key = '...') checkset.setup(settings)
-checkset.run() ```
+``` Note: Uptrain uses commonly used python libraries like openai-evals and
+sentence-transformers. To make sure, all the functionalities work, use the
+`uptrain-add` command to install the full version of the package. ```bash
+uptrain-add --feature full ``` ### How to define checks: Say we want to check
+whether our model's responses contain any grammatical mistakes or not.
+```python # Define your checkset - list of simple checks, dataset file, # and
+api_keys checkset = CheckSet( checks = Check( name = "grammar_score", operators
+= [ GrammarScore( col_in_text = "model_response", col_out = "grammar_score" ),
+], plots = PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader
+(fpath = '...') ) settings = Settings(openai_api_key = '...') checkset.setup
+(settings) checkset.run() ```
 # Integrations | Eval Frameworks | LLM Providers | LLM Packages | Serving
 frameworks | | ------------- | ------------- | ------------- | ------------- |
 | OpenAI Evals â | GPT-3.5-turbo â | Langchain ð | HuggingFace ð | |
 EleutherAI LM Eval ð | GPT-4 â | Llama Index ð | Replicate ð | |
 BIG-Bench ð | Claude ð | AutoGPT ð | | | Cohere ð | # UpTrain in
 Action ## Experimentation You can use the UpTrain framework to run and compare
 LLM responses for different prompts, models, LLM chains, etc. Check out the
```

### Comparing `uptrain-0.3.2/README.md` & `uptrain-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,19 @@
 To run it on your machine, checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/quickstart):
 
 ### Install the package through pip:
 ```bash
 pip install uptrain
 ```
 
+Note: Uptrain uses commonly used python libraries like openai-evals and sentence-transformers. To make sure, all the functionalities work, use the `uptrain-add` command to install the full version of the package.
+```bash
+uptrain-add --feature full
+```
+
 ### How to define checks:
 Say we want to check whether our model's responses contain any grammatical mistakes or not.
 
 ```python
 # Define your checkset - list of simple checks, dataset file, 
 # and api_keys
```

#### html2text {}

```diff
@@ -29,22 +29,25 @@
 for hallucinations. - **[Toxic Keywords Checks]()** - Make sure your model
 outputs are not biased or contain toxic keywords. - **[Feature Slicing]()** -
 Built-in pivoting functionalities for data dice and slice to pinpoint low-
 performing cohorts. - **[Realtime Dashboards]()** - Monitor your model's
 performance in realtime. # Get started ð  To run it on your machine,
 checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/
 quickstart): ### Install the package through pip: ```bash pip install uptrain
-``` ### How to define checks: Say we want to check whether our model's
-responses contain any grammatical mistakes or not. ```python # Define your
-checkset - list of simple checks, dataset file, # and api_keys checkset =
-CheckSet( checks = Check( name = "grammar_score", operators = [ GrammarScore
-( col_in_text = "model_response", col_out = "grammar_score" ), ], plots =
-PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader(fpath =
-'...') ) settings = Settings(openai_api_key = '...') checkset.setup(settings)
-checkset.run() ```
+``` Note: Uptrain uses commonly used python libraries like openai-evals and
+sentence-transformers. To make sure, all the functionalities work, use the
+`uptrain-add` command to install the full version of the package. ```bash
+uptrain-add --feature full ``` ### How to define checks: Say we want to check
+whether our model's responses contain any grammatical mistakes or not.
+```python # Define your checkset - list of simple checks, dataset file, # and
+api_keys checkset = CheckSet( checks = Check( name = "grammar_score", operators
+= [ GrammarScore( col_in_text = "model_response", col_out = "grammar_score" ),
+], plots = PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader
+(fpath = '...') ) settings = Settings(openai_api_key = '...') checkset.setup
+(settings) checkset.run() ```
 # Integrations | Eval Frameworks | LLM Providers | LLM Packages | Serving
 frameworks | | ------------- | ------------- | ------------- | ------------- |
 | OpenAI Evals â | GPT-3.5-turbo â | Langchain ð | HuggingFace ð | |
 EleutherAI LM Eval ð | GPT-4 â | Llama Index ð | Replicate ð | |
 BIG-Bench ð | Claude ð | AutoGPT ð | | | Cohere ð | # UpTrain in
 Action ## Experimentation You can use the UpTrain framework to run and compare
 LLM responses for different prompts, models, LLM chains, etc. Check out the
```

### Comparing `uptrain-0.3.2/tests/test_operators.py` & `uptrain-0.3.3/tests/test_operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 SELF_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 # uptrain.operators.drift
 def test_concept_drift():
     import polars as pl
     from uptrain.operators import ParamsDDM, ConceptDrift
-    from uptrain.operators.io import CsvReader
+    from uptrain.operators import CsvReader
 
     # Create an instance of the ParamsDDM class with the parameters
     params_ddm = ParamsDDM(warm_start=500, warning_threshold=2.0, drift_threshold=3.0)
 
     # Create an instance of the ConceptDrift operator
     op = ConceptDrift(algorithm="DDM", params=params_ddm, col_in_measure="prediction")
 
@@ -29,15 +29,15 @@
     if output["alert_info"] is not None:
         print("Counter:", output["alert_info"]["counter"])
 
 
 # uptrain.operators.language.embedding
 def test_embedding():
     import polars as pl
-    from uptrain.operators.language import Embedding
+    from uptrain.operators import Embedding
 
     # Create a DataFrame
     df = pl.DataFrame(
         {"text": ["This is the first sentence.", "Here is another sentence."]}
     )
 
     # Create an instance of the Embedding class
@@ -50,15 +50,15 @@
     print(embeddings)
 
 
 # uptrain.operators.embs
 def test_embs_cosine_distribution():
     import polars as pl
     from uptrain.operators import Distribution
-    from uptrain.operators.io import JsonReader
+    from uptrain.operators import JsonReader
 
     # Create an instance of the Distribution operator
     op = Distribution(
         kind="cosine_similarity",
         col_in_embs=["context_embeddings", "response_embeddings"],
         col_in_groupby=["question_idx", "experiment_id"],
         col_out=["similarity-context", "similarity-response"],
@@ -76,15 +76,15 @@
     print(output)
 
 
 # uptrain.operators.embs
 def test_embs_rouge_score():
     import polars as pl
     from uptrain.operators import Distribution
-    from uptrain.operators.io import JsonReader
+    from uptrain.operators import JsonReader
 
     # Create an instance of the Distribution operator
     op = Distribution(
         kind="rouge",
         col_in_embs=["document_text"],
         col_in_groupby=["question_idx", "experiment_id"],
         col_out=["rogue_f1"],
@@ -101,15 +101,15 @@
     print(output)
 
 
 # uptrain.operators.embs
 def test_embs_umap_operator():
     import polars as pl
     from uptrain.operators import UMAP
-    from uptrain.operators.io import JsonReader
+    from uptrain.operators import JsonReader
 
     # Create an instance of the UMAP operator
     op = UMAP(col_in_embs_1="context_embeddings", col_in_embs_2="response_embeddings")
 
     # Run the operator on the input data
     input_data = (
         JsonReader(fpath=os.path.join(SELF_DIR, "data/qna_on_docs_samples.jsonl"))
@@ -148,15 +148,15 @@
     # Print the similarity scores
     print(similarity_scores)
 
 
 # uptrain.operators.metrics
 def test_accuracy_operator():
     from uptrain.operators import Accuracy
-    from uptrain.operators.io import CsvReader
+    from uptrain.operators import CsvReader
 
     # Create an instance of the Accuracy operator
     op = Accuracy(
         kind="NOT_EQUAL",
         col_in_prediction="prediction",
         col_in_ground_truth="ground_truth",
     )
@@ -205,53 +205,53 @@
     # Create a line chart using the PlotlyChart class
     line_chart = PlotlyChart.Line(props={"x": "x", "y": "y"}, title="Line Chart")
 
     # Generate the line chart
     line_chart = line_chart.run(df)["extra"]["chart"]
 
     # Show the chart
-    line_chart.show()
+    # line_chart.show()
 
     # SCATTER CHART
     # Create a scatter chart using the PlotlyChart class
     scatter_chart = PlotlyChart.Scatter(
         props={"x": "x", "y": "y"}, title="Scatter Chart"
     )
 
     # Generate the scatter chart
     scatter_chart = scatter_chart.run(df)["extra"]["chart"]
 
     # Show the chart
-    scatter_chart.show()
+    # scatter_chart.show()
 
     # BAR CHART
     # Create a bar chart using the PlotlyChart class
     bar_chart = PlotlyChart.Bar(props={"x": "x", "y": "y"}, title="Bar Chart")
 
     # Generate the bar chart
     bar_chart = bar_chart.run(df)["extra"]["chart"]
 
     # Show the chart
-    bar_chart.show()
+    # bar_chart.show()
 
     # HISTOGRAM
     # Create a histogram using the PlotlyChart class
     histogram = PlotlyChart.Histogram(props={"x": "x"}, title="Histogram")
 
     # Generate the histogram
     histogram = histogram.run(df)["extra"]["chart"]
 
     # Show the chart
-    histogram.show()
+    # histogram.show()
 
 
 # uptrain.operators.language.rouge
 def test_rouge_operator():
     import polars as pl
-    from uptrain.operators.language import RougeScore
+    from uptrain.operators import RougeScore
 
     # Create a DataFrame
     df = pl.DataFrame(
         {
             "text_generated": [
                 "This is the generated text.",
                 "Another generated sentence.",
@@ -272,15 +272,15 @@
     # Print the Rouge-L scores
     print(scores)
 
 
 # uptrain.operators.language.text
 def test_docs_link_version_operator():
     import polars as pl
-    from uptrain.operators.language import DocsLinkVersion
+    from uptrain.operators import DocsLinkVersion
 
     # Create a DataFrame
     df = pl.DataFrame(
         {
             "text": [
                 "https://docs.streamlit.io/1.9.0/library/api-reference/charts/st.plotly_chart#stplotly_chart",
                 "No version here",
@@ -297,15 +297,15 @@
     # Print the extracted version numbers
     print(versions)
 
 
 # uptrain.operators.language.text
 def test_text_length_operator():
     import polars as pl
-    from uptrain.operators.language import TextLength
+    from uptrain.operators import TextLength
 
     # Create a DataFrame
     df = pl.DataFrame(
         {
             "text": [
                 "This is a sample text.",
                 "Another example sentence.",
@@ -323,15 +323,15 @@
     # Print the text lengths
     print(lengths)
 
 
 # uptrain.operators.language.text
 def test_text_comparison_operator():
     import polars as pl
-    from uptrain.operators.language import TextComparison
+    from uptrain.operators import TextComparison
 
     # Create a DataFrame
     df = pl.DataFrame(
         {
             "text": [
                 "This is a sample text.",
                 "Another example sentence.",
```

### Comparing `uptrain-0.3.2/uptrain/dashboard/st_helpers.py` & `uptrain-0.3.3/uptrain/dashboard/st_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             format_func=lambda x: checks[x].name,
         )  # streamlit is being weird with classes, so iterate over their indices
     check = checks[select_check_index]  # type: ignore
     return check
 
 
 def load_data_for_check_local(settings: "Settings", check: "Check"):
-    from uptrain.operators.io import DeltaWriter, JsonWriter
+    from uptrain.operators import DeltaWriter, JsonWriter
 
     sink = CheckSet._get_sink_for_check(settings, check)
     if isinstance(sink, (DeltaWriter, JsonWriter)):
         source = sink.to_reader()
         source.setup(settings)
     else:
         raise NotImplementedError(f"{type(sink)} is not supported for now.")
```

### Comparing `uptrain-0.3.2/uptrain/dashboard/st_run.py` & `uptrain-0.3.3/uptrain/dashboard/st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/dashboard/st_setup.py` & `uptrain-0.3.3/uptrain/dashboard/st_setup.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/framework/base.py` & `uptrain-0.3.3/uptrain/framework/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/framework/checks.py` & `uptrain-0.3.3/uptrain/framework/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,26 +101,25 @@
         preprocessors (list[TableOp]): A list of operators to run on the input data before running the checks.
         checks (list[Check]): The set of checks to run on the input data.
     """
 
     source: Operator
     checks: list[Check]
     preprocessors: list[TransformOp]
-    _consolidated_check: None
 
     def __init__(
         self,
         source: Operator,
         checks: list[t.Any],
         preprocessors: list[TransformOp] | None = None,
     ):
         self._consolidated_check = Check(
             name="Consolidated Results",
             operators=[],
-            plots=[PlotlyChart.Table(title="Consolidated Results")]
+            plots=[PlotlyChart.Table(title="Consolidated Results")],
         )
 
         self.source = source
         self.checks = checks
         self.preprocessors = preprocessors if preprocessors is not None else []
 
         # verify all checks have different names
@@ -150,15 +149,15 @@
         for check in self.checks:
             check.setup(self._settings)
         self._consolidated_check.setup(self._settings)
         return self
 
     def run(self):
         """Run all checks in this set."""
-        from uptrain.operators.io import JsonWriter
+        from uptrain.operators.io.writers import JsonWriter
 
         source_output = self.source.run()["output"]
         assert source_output is not None, "Output of source is None"
 
         if len(self.preprocessors) > 0:
             for preprocessor in self.preprocessors:
                 source_output = preprocessor.run(source_output)["output"]
@@ -174,25 +173,32 @@
         consolidated_outputs = source_output
         for check in self.checks:
             check_output = check.run(source_output)
             assert check_output is not None, f"Output of check {check.name} is None"
             self._get_sink_for_check(self._settings, check).run(check_output)
 
             if all(isinstance(operator, ColumnOp) for operator in check.operators):
-                consolidated_outputs = consolidated_outputs.with_columns([
-                    check_output[col_name] for col_name in list(set(check_output.columns) - set(consolidated_outputs.columns))
-                ])
-
-        self._get_sink_for_check(self._settings, self._consolidated_check).run(self._consolidated_check.run(consolidated_outputs))
+                consolidated_outputs = consolidated_outputs.with_columns(
+                    [
+                        check_output[col_name]
+                        for col_name in list(
+                            set(check_output.columns)
+                            - set(consolidated_outputs.columns)
+                        )
+                    ]
+                )
 
+        self._get_sink_for_check(self._settings, self._consolidated_check).run(
+            self._consolidated_check.run(consolidated_outputs)
+        )
 
     @staticmethod
     def _get_sink_for_check(settings: Settings, check: Check):
         """Get the sink operator for this check."""
-        from uptrain.operators.io import JsonWriter
+        from uptrain.operators.io.writers import JsonWriter
 
         return JsonWriter(
             fpath=os.path.join(settings.logs_folder, f"{check.name}.jsonl")
         )
 
     @classmethod
     def from_dict(cls, data: dict) -> "CheckSet":
@@ -204,15 +210,15 @@
             checks=[deserialize_operator(check) for check in data.get("checks", [])],
         )
 
     def dict(self) -> dict:
         return {
             "source": to_py_types(self.source),
             "preprocessors": [to_py_types(op) for op in self.preprocessors],
-            "checks": [to_py_types(check) for check in self.checks]
+            "checks": [to_py_types(check) for check in self.checks],
         }
 
     @classmethod
     def deserialize(cls, fpath: str) -> "CheckSet":
         with open(fpath, "r") as f:
             return cls.from_dict(jsonload(f))
```

### Comparing `uptrain-0.3.2/uptrain/framework/remote.py` & `uptrain-0.3.3/uptrain/framework/remote.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/framework/signal.py` & `uptrain-0.3.3/uptrain/framework/signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/base.py` & `uptrain-0.3.3/uptrain/operators/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/code/sql/sql.py` & `uptrain-0.3.3/uptrain/operators/code/sql.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/drift.py` & `uptrain-0.3.3/uptrain/operators/drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/embs.py` & `uptrain-0.3.3/uptrain/operators/embs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/io/readers.py` & `uptrain-0.3.3/uptrain/operators/io/readers.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/io/writers.py` & `uptrain-0.3.3/uptrain/operators/io/writers.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,29 +29,29 @@
         if self.columns is None:
             self.columns = list(data.columns)
         assert set(self.columns) == set(data.columns)
         data.write_delta(self.fpath, mode="append")
         return {"output": None}
 
     def to_reader(self):
-        from uptrain.operators.io import DeltaReader
+        from uptrain.operators.io.readers import DeltaReader
 
         return DeltaReader(fpath=self.fpath)  # type: ignore
 
 
 @register_op
 class JsonWriter(OpBaseModel):
     fpath: str
     columns: t.Optional[list[str]] = None
 
     def setup(self, settings: Settings):
         return self
 
     def to_reader(self):
-        from uptrain.operators.io import JsonReader
+        from uptrain.operators.io.readers import JsonReader
 
         return JsonReader(fpath=self.fpath)  # type: ignore
 
     def run(self, data: pl.DataFrame) -> TYPE_TABLE_OUTPUT:
         if self.columns is None:
             self.columns = list(data.columns)
         assert set(self.columns) == set(data.columns)
```

### Comparing `uptrain-0.3.2/uptrain/operators/language/embedding.py` & `uptrain-0.3.3/uptrain/operators/language/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     Returns:
         TYPE_TABLE_OUTPUT: A dictionary containing the generated embeddings.
 
     Example:
         ```
         import polars as pl
-        from uptrain.operators.language import Embedding
+        from uptrain.operators import Embedding
 
         # Create a DataFrame
         df = pl.DataFrame({
             "text": ["This is the first sentence.", "Here is another sentence."]
         })
 
         # Create an instance of the Embedding class
```

### Comparing `uptrain-0.3.2/uptrain/operators/language/generation.py` & `uptrain-0.3.3/uptrain/operators/language/generation.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/language/grammar.py` & `uptrain-0.3.3/uptrain/operators/language/grammar.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/language/llm.py` & `uptrain-0.3.3/uptrain/operators/language/llm.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/language/model_grade.py` & `uptrain-0.3.3/uptrain/operators/language/model_grade.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/language/openai_evals.py` & `uptrain-0.3.3/uptrain/operators/language/openai_evals.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/language/rouge.py` & `uptrain-0.3.3/uptrain/operators/language/rouge.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     Returns:
         dict: A dictionary containing the Rouge scores for each pair of generated and source text.
 
     Example:
         ```
         import polars as pl
-        from uptrain.operators.language import RougeScore
+        from uptrain.operators import RougeScore
 
         # Create a DataFrame
         df = pl.DataFrame({
             "text_generated": ["This is the generated text.", "Another generated sentence."],
             "text_source": ["This is the original source text.", "This is a different source text."]
         })
```

### Comparing `uptrain-0.3.2/uptrain/operators/language/text.py` & `uptrain-0.3.3/uptrain/operators/language/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     Returns:
         dict: A dictionary containing the extracted version numbers.
 
     Example:
         ```
         import polars as pl
-        from uptrain.operators.language import DocsLinkVersion
+        from uptrain.operators import DocsLinkVersion
 
         # Create a DataFrame
         df = pl.DataFrame({
             "text": ["https://docs.streamlit.io/1.9.0/library/api-reference/charts/st.plotly_chart#stplotly_chart", "No version here"]
         })
 
         # Create an instance of the DocsLinkVersion class
@@ -97,15 +97,15 @@
 
     Returns:
         dict: A dictionary containing the calculated text lengths.
 
     Example:
         ```
         import polars as pl
-        from uptrain.operators.language import TextLength
+        from uptrain.operators import TextLength
 
         # Create a DataFrame
         df = pl.DataFrame({
             "text": ["This is a sample text.", "Another example sentence.", "Yet another sentence."]
         })
 
         # Create an instance of the TextLength class
@@ -154,15 +154,15 @@
 
     Returns:
         dict: A dictionary containing the comparison results (1 if equal, 0 otherwise).
 
     Example:
         ```
         import polars as pl
-        from uptrain.operators.language import TextComparison
+        from uptrain.operators import TextComparison
 
         # Create a DataFrame
         df = pl.DataFrame({
             "text": ["This is a sample text.", "Another example sentence.", "Yet another sentence."]
         })
 
         # Set the reference text for comparison
```

### Comparing `uptrain-0.3.2/uptrain/operators/metrics.py` & `uptrain-0.3.3/uptrain/operators/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         col_in_prediction (str): The name of the column containing the predicted values.
         col_in_ground_truth (str): The name of the column containing the ground truth values.
         col_out (str): The name of the output column containing the accuracy scores.
 
     Example:
         ```
         from uptrain.operators import Accuracy
-        from uptrain.operators.io import CsvReader
+        from uptrain.operators import CsvReader
 
         # Create an instance of the Accuracy operator
         op = Accuracy(
                 kind="NOT_EQUAL",
                 col_in_prediction="prediction",
                 col_in_ground_truth="ground_truth"
             )
```

### Comparing `uptrain-0.3.2/uptrain/operators/similarity.py` & `uptrain-0.3.3/uptrain/operators/similarity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/table.py` & `uptrain-0.3.3/uptrain/operators/table.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/operators/vis.py` & `uptrain-0.3.3/uptrain/operators/vis.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/utilities/__init__.py` & `uptrain-0.3.3/uptrain/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/utilities/sql_utils.py` & `uptrain-0.3.3/uptrain/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/utilities/sql_utils_test.py` & `uptrain-0.3.3/uptrain/utilities/sql_utils_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/utilities/sqlglot_test.py` & `uptrain-0.3.3/uptrain/utilities/sqlglot_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/constants.py` & `uptrain-0.3.3/uptrain/v0/constants.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/algorithms/clustering.py` & `uptrain-0.3.3/uptrain/v0/core/classes/algorithms/clustering.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/algorithms/popularity_bias.py` & `uptrain-0.3.3/uptrain/v0/core/classes/algorithms/popularity_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/distances/cosine_distance.py` & `uptrain-0.3.3/uptrain/v0/core/classes/distances/cosine_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/distances/distance_resolver.py` & `uptrain-0.3.3/uptrain/v0/core/classes/distances/distance_resolver.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/distances/hamming_distance.py` & `uptrain-0.3.3/uptrain/v0/core/classes/distances/hamming_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/distances/l2_distance.py` & `uptrain-0.3.3/uptrain/v0/core/classes/distances/l2_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/distances/norm_ratio.py` & `uptrain-0.3.3/uptrain/v0/core/classes/distances/norm_ratio.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/finetuning/finetuning.py` & `uptrain-0.3.3/uptrain/v0/core/classes/finetuning/finetuning.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/framework.py` & `uptrain-0.3.3/uptrain/v0/core/classes/framework.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/helpers/annotation_helper.py` & `uptrain-0.3.3/uptrain/v0/core/classes/helpers/annotation_helper.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/helpers/config_handler.py` & `uptrain-0.3.3/uptrain/v0/core/classes/helpers/config_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/helpers/dataset_handler.py` & `uptrain-0.3.3/uptrain/v0/core/classes/helpers/dataset_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/helpers/model_handler.py` & `uptrain-0.3.3/uptrain/v0/core/classes/helpers/model_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/io/runtime_manager.py` & `uptrain-0.3.3/uptrain/v0/core/classes/io/runtime_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/logging/log_handler.py` & `uptrain-0.3.3/uptrain/v0/core/classes/logging/log_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/logging/log_postgres.py` & `uptrain-0.3.3/uptrain/v0/core/classes/logging/log_postgres.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/logging/log_streamlit.py` & `uptrain-0.3.3/uptrain/v0/core/classes/logging/log_streamlit.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/logging/new_log_handler.py` & `uptrain-0.3.3/uptrain/v0/core/classes/logging/new_log_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/logging/new_st_run.py` & `uptrain-0.3.3/uptrain/v0/core/classes/logging/new_st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/logging/new_st_setup.py` & `uptrain-0.3.3/uptrain/v0/core/classes/logging/new_st_setup.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/logging/st_run.py` & `uptrain-0.3.3/uptrain/v0/core/classes/logging/st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/managers/check_manager.py` & `uptrain-0.3.3/uptrain/v0/core/classes/managers/check_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/__init__.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/abstract_measurable.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/abstract_measurable.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/accuracy.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/accuracy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/condition.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/condition.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/custom.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/custom.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/distance.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/feature.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/feature_concat.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/feature_concat.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/input_feature.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/input_feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/measurable.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/measurable.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/measurable_resolver.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/measurable_resolver.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/output_feature.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/output_feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/measurables/scalar_from_embedding.py` & `uptrain-0.3.3/uptrain/v0/core/classes/measurables/scalar_from_embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/abstract_check.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/abstract_check.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/abstract_monitor.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/abstract_monitor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/accuracy.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/accuracy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/concept_drift.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/concept_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/custom_monitor.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/custom_monitor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/data_drift.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/data_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/data_integrity.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/data_integrity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/edge_case.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/edge_case.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/feature_drift.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/feature_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/model_bias.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/model_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/monitors/output_comparison.py` & `uptrain-0.3.3/uptrain/v0/core/classes/monitors/output_comparison.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/signals/signal.py` & `uptrain-0.3.3/uptrain/v0/core/classes/signals/signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/signals/signal_manager.py` & `uptrain-0.3.3/uptrain/v0/core/classes/signals/signal_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/statistics/convergence.py` & `uptrain-0.3.3/uptrain/v0/core/classes/statistics/convergence.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/statistics/distance.py` & `uptrain-0.3.3/uptrain/v0/core/classes/statistics/distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/statistics/distribution.py` & `uptrain-0.3.3/uptrain/v0/core/classes/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/statistics/norm_embedding.py` & `uptrain-0.3.3/uptrain/v0/core/classes/statistics/norm_embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/statistics/old_distribution.py` & `uptrain-0.3.3/uptrain/v0/core/classes/statistics/old_distribution.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/visuals/clustering.py` & `uptrain-0.3.3/uptrain/v0/core/classes/visuals/clustering.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/visuals/dimensionality_reduction.py` & `uptrain-0.3.3/uptrain/v0/core/classes/visuals/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/visuals/plot.py` & `uptrain-0.3.3/uptrain/v0/core/classes/visuals/plot.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/classes/visuals/shap.py` & `uptrain-0.3.3/uptrain/v0/core/classes/visuals/shap.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/encoders/__init__.py` & `uptrain-0.3.3/uptrain/v0/core/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/lib/algorithms.py` & `uptrain-0.3.3/uptrain/v0/core/lib/algorithms.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/lib/cache.py` & `uptrain-0.3.3/uptrain/v0/core/lib/cache.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/lib/datastores.py` & `uptrain-0.3.3/uptrain/v0/core/lib/datastores.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/lib/helper_funcs.py` & `uptrain-0.3.3/uptrain/v0/core/lib/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/core/lib/model_signal_funcs.py` & `uptrain-0.3.3/uptrain/v0/core/lib/model_signal_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/ee/classes/measurables/llm_measurables.py` & `uptrain-0.3.3/uptrain/v0/ee/classes/measurables/llm_measurables.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/ee/lib/algorithms.py` & `uptrain-0.3.3/uptrain/v0/ee/lib/algorithms.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/ee/lib/cache.py` & `uptrain-0.3.3/uptrain/v0/ee/lib/cache.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain/v0/ee/lib/ops_agg.py` & `uptrain-0.3.3/uptrain/v0/ee/lib/ops_agg.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.2/uptrain.egg-info/PKG-INFO` & `uptrain-0.3.3/uptrain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: uptrain
-Version: 0.3.2
+Version: 0.3.3
 Summary: UpTrain - ML Observability and Retraining Framework
-Home-page: https://github.com/uptrain-ai/uptrain
-Maintainer: UpTrain AI Team
-Maintainer-email: uptrain.ai@gmail.com
-License: Apache License 2.0
-Keywords: uptrain ai retraining ML observability
+Maintainer-email: UpTrain AI Team <uptrain.ai@gmail.com>
+License: Apache-2.0
+Project-URL: Homepage, https://uptrain.ai
+Project-URL: Repository, https://github.com/uptrain-ai/uptrain
+Keywords: uptrain,ai,retraining,ML,observability
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
-Provides-Extra: v0
-Provides-Extra: full
+Provides-Extra: test
 License-File: LICENSE
 
 <h4 align="center">
   <a href="https://uptrain.ai">
     <img width="300" src="https://user-images.githubusercontent.com/108270398/214240695-4f958b76-c993-4ddd-8de6-8668f4d0da84.png" alt="uptrain">
   </a>
 </h4>
@@ -105,14 +104,19 @@
 To run it on your machine, checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/quickstart):
 
 ### Install the package through pip:
 ```bash
 pip install uptrain
 ```
 
+Note: Uptrain uses commonly used python libraries like openai-evals and sentence-transformers. To make sure, all the functionalities work, use the `uptrain-add` command to install the full version of the package.
+```bash
+uptrain-add --feature full
+```
+
 ### How to define checks:
 Say we want to check whether our model's responses contain any grammatical mistakes or not.
 
 ```python
 # Define your checkset - list of simple checks, dataset file, 
 # and api_keys
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.3.2 Summary: UpTrain - ML
-Observability and Retraining Framework Home-page: https://github.com/uptrain-
-ai/uptrain Maintainer: UpTrain AI Team Maintainer-email: uptrain.ai@gmail.com
-License: Apache License 2.0 Keywords: uptrain ai retraining ML observability
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-Provides-Extra: v0 Provides-Extra: full License-File: LICENSE
+Metadata-Version: 2.1 Name: uptrain Version: 0.3.3 Summary: UpTrain - ML
+Observability and Retraining Framework Maintainer-email: UpTrain AI Team
+ai@gmail.com> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
+Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
+uptrain,ai,retraining,ML,observability Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
+:: Software Development :: Build Tools Classifier: License :: OSI Approved ::
+Apache Software License Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown Provides-Extra: test License-File:
+LICENSE
                                *** [uptrain] ***
 ***** An open-source framework to evaluate, test and monitor LLM applications
 *****
             Docs  - Slack_Community - Bug_Report - Feature_Request
    *** [https://img.shields.io/github/contributors/uptrain-ai/uptrain] [PRs
                   Welcome] [Docs] [Community] [Website]  ***
   **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM
@@ -40,22 +41,25 @@
 for hallucinations. - **[Toxic Keywords Checks]()** - Make sure your model
 outputs are not biased or contain toxic keywords. - **[Feature Slicing]()** -
 Built-in pivoting functionalities for data dice and slice to pinpoint low-
 performing cohorts. - **[Realtime Dashboards]()** - Monitor your model's
 performance in realtime. # Get started ð  To run it on your machine,
 checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/
 quickstart): ### Install the package through pip: ```bash pip install uptrain
-``` ### How to define checks: Say we want to check whether our model's
-responses contain any grammatical mistakes or not. ```python # Define your
-checkset - list of simple checks, dataset file, # and api_keys checkset =
-CheckSet( checks = Check( name = "grammar_score", operators = [ GrammarScore
-( col_in_text = "model_response", col_out = "grammar_score" ), ], plots =
-PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader(fpath =
-'...') ) settings = Settings(openai_api_key = '...') checkset.setup(settings)
-checkset.run() ```
+``` Note: Uptrain uses commonly used python libraries like openai-evals and
+sentence-transformers. To make sure, all the functionalities work, use the
+`uptrain-add` command to install the full version of the package. ```bash
+uptrain-add --feature full ``` ### How to define checks: Say we want to check
+whether our model's responses contain any grammatical mistakes or not.
+```python # Define your checkset - list of simple checks, dataset file, # and
+api_keys checkset = CheckSet( checks = Check( name = "grammar_score", operators
+= [ GrammarScore( col_in_text = "model_response", col_out = "grammar_score" ),
+], plots = PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader
+(fpath = '...') ) settings = Settings(openai_api_key = '...') checkset.setup
+(settings) checkset.run() ```
 # Integrations | Eval Frameworks | LLM Providers | LLM Packages | Serving
 frameworks | | ------------- | ------------- | ------------- | ------------- |
 | OpenAI Evals â | GPT-3.5-turbo â | Langchain ð | HuggingFace ð | |
 EleutherAI LM Eval ð | GPT-4 â | Llama Index ð | Replicate ð | |
 BIG-Bench ð | Claude ð | AutoGPT ð | | | Cohere ð | # UpTrain in
 Action ## Experimentation You can use the UpTrain framework to run and compare
 LLM responses for different prompts, models, LLM chains, etc. Check out the
```

### Comparing `uptrain-0.3.2/uptrain.egg-info/SOURCES.txt` & `uptrain-0.3.3/uptrain.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 LICENSE
 README.md
-setup.py
-regression_testing/__init__.py
-regression_testing/experiment.py
+pyproject.toml
 tests/test_operators.py
 uptrain/__init__.py
+uptrain/cli.py
 uptrain.egg-info/PKG-INFO
 uptrain.egg-info/SOURCES.txt
 uptrain.egg-info/dependency_links.txt
+uptrain.egg-info/entry_points.txt
 uptrain.egg-info/requires.txt
 uptrain.egg-info/top_level.txt
 uptrain/dashboard/__init__.py
-uptrain/dashboard/__init__.pyi
 uptrain/dashboard/st_helpers.py
 uptrain/dashboard/st_run.py
 uptrain/dashboard/st_setup.py
 uptrain/framework/__init__.py
-uptrain/framework/__init__.pyi
 uptrain/framework/base.py
 uptrain/framework/checks.py
 uptrain/framework/remote.py
 uptrain/framework/signal.py
 uptrain/operators/__init__.py
-uptrain/operators/__init__.pyi
 uptrain/operators/base.py
 uptrain/operators/drift.py
 uptrain/operators/embs.py
 uptrain/operators/metrics.py
 uptrain/operators/similarity.py
 uptrain/operators/table.py
 uptrain/operators/vis.py
 uptrain/operators/code/__init__.py
-uptrain/operators/code/sql/__init__.py
-uptrain/operators/code/sql/__init__.pyi
-uptrain/operators/code/sql/sql.py
+uptrain/operators/code/sql.py
 uptrain/operators/io/__init__.py
-uptrain/operators/io/__init__.pyi
 uptrain/operators/io/readers.py
 uptrain/operators/io/writers.py
 uptrain/operators/language/__init__.py
-uptrain/operators/language/__init__.pyi
 uptrain/operators/language/embedding.py
 uptrain/operators/language/generation.py
 uptrain/operators/language/grammar.py
 uptrain/operators/language/llm.py
 uptrain/operators/language/model_grade.py
 uptrain/operators/language/openai_evals.py
 uptrain/operators/language/rouge.py
 uptrain/operators/language/text.py
+uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
+uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
 uptrain/utilities/__init__.py
 uptrain/utilities/sql_utils.py
 uptrain/utilities/sql_utils_test.py
 uptrain/utilities/sqlglot_test.py
 uptrain/v0/__init__.py
 uptrain/v0/constants.py
 uptrain/v0/core/__init__.py
@@ -140,9 +135,30 @@
 uptrain/v0/ee/classes/__init__.py
 uptrain/v0/ee/classes/measurables/__init__.py
 uptrain/v0/ee/classes/measurables/llm_measurables.py
 uptrain/v0/ee/lib/__init__.py
 uptrain/v0/ee/lib/algorithms.py
 uptrain/v0/ee/lib/cache.py
 uptrain/v0/ee/lib/ops_agg.py
-validation_wrapper/__init__.py
-validation_wrapper/validation_manager.py
+uptrain/v0/tests/test_a-b_testing.py
+uptrain/v0/tests/test_concept_drift_custom_monitor.py
+uptrain/v0/tests/test_dashboard.py
+uptrain/v0/tests/test_data_drift.py
+uptrain/v0/tests/test_data_integrity.py
+uptrain/v0/tests/test_data_integrity_zscore.py
+uptrain/v0/tests/test_datastores.py
+uptrain/v0/tests/test_edge_cases.py
+uptrain/v0/tests/test_monitors_concept_drift_adwin.py
+uptrain/v0/tests/test_monitors_concept_drift_ddm.py
+uptrain/v0/tests/test_recommender_bias.py
+uptrain/v0/tests/test_visuals_dimensionality_reduction.py
+uptrain/v0/tests/test_visuals_plot.py
+uptrain/v0/tests/test_visuals_shap.py
+uptrain/v0/tests/test_helpers/__init__.py
+uptrain/v0/tests/test_helpers/dataset.py
+uptrain/v0/tests/test_helpers/get_data_from_remote.py
+uptrain/v0/tests/test_helpers/helper_funcs.py
+uptrain/v0/tests/test_helpers/model_tensorflow.py
+uptrain/v0/tests/test_helpers/model_torch.py
+uptrain/v0/tests/test_helpers/pushup_signal.py
+uptrain/validation_wrapper/__init__.py
+uptrain/validation_wrapper/validation_manager.py
```

### Comparing `uptrain-0.3.2/validation_wrapper/validation_manager.py` & `uptrain-0.3.3/uptrain/validation_wrapper/validation_manager.py`

 * *Files identical despite different names*


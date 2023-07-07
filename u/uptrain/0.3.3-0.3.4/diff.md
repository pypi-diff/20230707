# Comparing `tmp/uptrain-0.3.3.tar.gz` & `tmp/uptrain-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptrain-0.3.3.tar", last modified: Fri Jul  7 06:55:33 2023, max compression
+gzip compressed data, was "uptrain-0.3.4.tar", last modified: Fri Jul  7 09:32:53 2023, max compression
```

## Comparing `uptrain-0.3.3.tar` & `uptrain-0.3.4.tar`

### file list

```diff
@@ -1,204 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 06:55:23.000000 uptrain-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 06:55:33.855613 uptrain-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-07 06:55:23.000000 uptrain-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-07 06:55:23.000000 uptrain-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:55:33.855613 uptrain-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-07-07 06:55:23.000000 uptrain-0.3.3/tests/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/dashboard/st_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/dashboard/st_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/dashboard/st_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/framework/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/operators/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/code/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/drift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/embs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain/operators/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/io/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/operators/language/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/model_grade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.831613 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/completion_fns/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/elsuite/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/openai_evals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/rouge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/language/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/operators/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/utilities/sql_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/utilities/sqlglot_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/v0/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/v0/core/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.839613 uptrain-0.3.3/uptrain/v0/core/classes/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/algorithms/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/algorithms/popularity_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/distances/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/abstract_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/cosine_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/distance_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/hamming_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/l2_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/distances/norm_ratio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/finetuning/AbstractFinetune.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/finetuning/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/annotation_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/dataset_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/helpers/model_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/io/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/io/runtime_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.843613 uptrain-0.3.3/uptrain/v0/core/classes/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/log_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/log_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/new_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/new_st_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/new_st_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/logging/st_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.847613 uptrain-0.3.3/uptrain/v0/core/classes/managers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/managers/check_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.847613 uptrain-0.3.3/uptrain/v0/core/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/abstract_measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/feature_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/input_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/measurable_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/output_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/measurables/scalar_from_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.847613 uptrain-0.3.3/uptrain/v0/core/classes/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/abstract_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/abstract_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/custom_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/data_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/edge_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/feature_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/model_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/monitors/output_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/classes/signals/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/signals/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/signals/signal_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/classes/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/abstract_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/norm_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/statistics/old_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/classes/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/abstract_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/classes/visuals/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/encoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/helper_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/core/lib/model_signal_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/ee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/ee/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.851613 uptrain-0.3.3/uptrain/v0/ee/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/classes/measurables/llm_measurables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/uptrain/v0/ee/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/ee/lib/ops_agg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/uptrain/v0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_a-b_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_concept_drift_custom_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_data_integrity_zscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_edge_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/uptrain/v0/tests/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/get_data_from_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/helper_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/model_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/model_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_helpers/pushup_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_monitors_concept_drift_adwin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_monitors_concept_drift_ddm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_recommender_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_visuals_dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_visuals_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/v0/tests/test_visuals_shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.855613 uptrain-0.3.3/uptrain/validation_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/validation_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-07 06:55:23.000000 uptrain-0.3.3/uptrain/validation_wrapper/validation_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:55:33.835613 uptrain-0.3.3/uptrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 06:55:33.000000 uptrain-0.3.3/uptrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.894305 uptrain-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 09:32:44.000000 uptrain-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 09:32:53.894305 uptrain-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-07 09:32:44.000000 uptrain-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-07 09:32:44.000000 uptrain-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:32:53.894305 uptrain-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-07-07 09:32:44.000000 uptrain-0.3.4/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/uptrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/uptrain/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/st_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/st_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/dashboard/st_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/uptrain/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/framework/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/code/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/embs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/io/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/language/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/model_grade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.866305 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/completion_fns/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/elsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/openai_evals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/language/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/operators/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/utilities/sql_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/utilities/sqlglot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/v0/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.874305 uptrain-0.3.4/uptrain/v0/core/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/algorithms/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/algorithms/popularity_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/abstract_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/cosine_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/distance_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/hamming_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/l2_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/distances/norm_ratio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/finetuning/AbstractFinetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/finetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/finetuning/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/annotation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/dataset_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/helpers/model_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/io/runtime_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.878305 uptrain-0.3.4/uptrain/v0/core/classes/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/log_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/log_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/new_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/new_st_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/new_st_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/logging/st_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.882305 uptrain-0.3.4/uptrain/v0/core/classes/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/managers/check_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.882305 uptrain-0.3.4/uptrain/v0/core/classes/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/abstract_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/feature_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/input_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/measurable_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/output_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/measurables/scalar_from_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/classes/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/abstract_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/abstract_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/custom_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/edge_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/feature_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/model_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/monitors/output_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/classes/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/signals/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/signals/signal_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/classes/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/abstract_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/norm_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/statistics/old_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/classes/visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/abstract_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/classes/visuals/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/encoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/core/lib/model_signal_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/ee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.886305 uptrain-0.3.4/uptrain/v0/ee/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.890305 uptrain-0.3.4/uptrain/v0/ee/classes/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/classes/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/classes/measurables/llm_measurables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.890305 uptrain-0.3.4/uptrain/v0/ee/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/lib/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/ee/lib/ops_agg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.890305 uptrain-0.3.4/uptrain/v0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_a-b_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_concept_drift_custom_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_data_integrity_zscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_edge_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.894305 uptrain-0.3.4/uptrain/v0/tests/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/get_data_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/model_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/model_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_helpers/pushup_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_monitors_concept_drift_adwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_monitors_concept_drift_ddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_recommender_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_visuals_dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_visuals_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/v0/tests/test_visuals_shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.894305 uptrain-0.3.4/uptrain/validation_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/validation_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-07 09:32:44.000000 uptrain-0.3.4/uptrain/validation_wrapper/validation_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:32:53.870305 uptrain-0.3.4/uptrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 09:32:53.000000 uptrain-0.3.4/uptrain.egg-info/top_level.txt
```

### Comparing `uptrain-0.3.3/LICENSE` & `uptrain-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/PKG-INFO` & `uptrain-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptrain
-Version: 0.3.3
+Version: 0.3.4
 Summary: UpTrain - ML Observability and Retraining Framework
 Maintainer-email: UpTrain AI Team <uptrain.ai@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain
 Keywords: uptrain,ai,retraining,ML,observability
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.3.3 Summary: UpTrain - ML
+Metadata-Version: 2.1 Name: uptrain Version: 0.3.4 Summary: UpTrain - ML
 Observability and Retraining Framework Maintainer-email: UpTrain AI Team
 ai@gmail.com> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
 uptrain,ai,retraining,ML,observability Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.8
```

### Comparing `uptrain-0.3.3/README.md` & `uptrain-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/pyproject.toml` & `uptrain-0.3.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "uptrain"
-version = "0.3.3"
+version = "0.3.4"
 description = "UpTrain - ML Observability and Retraining Framework"
 readme = "README.md"
 maintainers = [{ name = "UpTrain AI Team", email = "uptrain.ai@gmail.com" }]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -46,7 +46,11 @@
 # Optional dependencies are installed using the uptrain-cli
 test = [
     "pytest>=7.0"
 ]
 
 [tools.setuptools]
 packages = ["uptrain"]
+include-package-data = true
+
+[tool.setuptools.package-data]
+"*" = ["*.pyi"]
```

### Comparing `uptrain-0.3.3/tests/test_operators.py` & `uptrain-0.3.4/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/cli.py` & `uptrain-0.3.4/uptrain/cli.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/dashboard/st_helpers.py` & `uptrain-0.3.4/uptrain/dashboard/st_helpers.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/dashboard/st_run.py` & `uptrain-0.3.4/uptrain/dashboard/st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/dashboard/st_setup.py` & `uptrain-0.3.4/uptrain/dashboard/st_setup.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/framework/base.py` & `uptrain-0.3.4/uptrain/framework/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/framework/checks.py` & `uptrain-0.3.4/uptrain/framework/checks.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/framework/remote.py` & `uptrain-0.3.4/uptrain/framework/remote.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/framework/signal.py` & `uptrain-0.3.4/uptrain/framework/signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/base.py` & `uptrain-0.3.4/uptrain/operators/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/code/sql.py` & `uptrain-0.3.4/uptrain/operators/code/sql.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/drift.py` & `uptrain-0.3.4/uptrain/operators/drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/embs.py` & `uptrain-0.3.4/uptrain/operators/embs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/io/readers.py` & `uptrain-0.3.4/uptrain/operators/io/readers.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/io/writers.py` & `uptrain-0.3.4/uptrain/operators/io/writers.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/embedding.py` & `uptrain-0.3.4/uptrain/operators/language/embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/generation.py` & `uptrain-0.3.4/uptrain/operators/language/generation.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/grammar.py` & `uptrain-0.3.4/uptrain/operators/language/grammar.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/llm.py` & `uptrain-0.3.4/uptrain/operators/language/llm.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/model_grade.py` & `uptrain-0.3.4/uptrain/operators/language/model_grade.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py` & `uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py` & `uptrain-0.3.4/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/openai_evals.py` & `uptrain-0.3.4/uptrain/operators/language/openai_evals.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/rouge.py` & `uptrain-0.3.4/uptrain/operators/language/rouge.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/language/text.py` & `uptrain-0.3.4/uptrain/operators/language/text.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/metrics.py` & `uptrain-0.3.4/uptrain/operators/metrics.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/similarity.py` & `uptrain-0.3.4/uptrain/operators/similarity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/table.py` & `uptrain-0.3.4/uptrain/operators/table.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/operators/vis.py` & `uptrain-0.3.4/uptrain/operators/vis.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/utilities/__init__.py` & `uptrain-0.3.4/uptrain/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/utilities/sql_utils.py` & `uptrain-0.3.4/uptrain/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/utilities/sql_utils_test.py` & `uptrain-0.3.4/uptrain/utilities/sql_utils_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/utilities/sqlglot_test.py` & `uptrain-0.3.4/uptrain/utilities/sqlglot_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/constants.py` & `uptrain-0.3.4/uptrain/v0/constants.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/algorithms/clustering.py` & `uptrain-0.3.4/uptrain/v0/core/classes/algorithms/clustering.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/algorithms/popularity_bias.py` & `uptrain-0.3.4/uptrain/v0/core/classes/algorithms/popularity_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/distances/cosine_distance.py` & `uptrain-0.3.4/uptrain/v0/core/classes/distances/cosine_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/distances/distance_resolver.py` & `uptrain-0.3.4/uptrain/v0/core/classes/distances/distance_resolver.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/distances/hamming_distance.py` & `uptrain-0.3.4/uptrain/v0/core/classes/distances/hamming_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/distances/l2_distance.py` & `uptrain-0.3.4/uptrain/v0/core/classes/distances/l2_distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/distances/norm_ratio.py` & `uptrain-0.3.4/uptrain/v0/core/classes/distances/norm_ratio.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/finetuning/finetuning.py` & `uptrain-0.3.4/uptrain/v0/core/classes/finetuning/finetuning.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/framework.py` & `uptrain-0.3.4/uptrain/v0/core/classes/framework.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/helpers/annotation_helper.py` & `uptrain-0.3.4/uptrain/v0/core/classes/helpers/annotation_helper.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/helpers/config_handler.py` & `uptrain-0.3.4/uptrain/v0/core/classes/helpers/config_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/helpers/dataset_handler.py` & `uptrain-0.3.4/uptrain/v0/core/classes/helpers/dataset_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/helpers/model_handler.py` & `uptrain-0.3.4/uptrain/v0/core/classes/helpers/model_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/io/runtime_manager.py` & `uptrain-0.3.4/uptrain/v0/core/classes/io/runtime_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/logging/log_handler.py` & `uptrain-0.3.4/uptrain/v0/core/classes/logging/log_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/logging/log_postgres.py` & `uptrain-0.3.4/uptrain/v0/core/classes/logging/log_postgres.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/logging/log_streamlit.py` & `uptrain-0.3.4/uptrain/v0/core/classes/logging/log_streamlit.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/logging/new_log_handler.py` & `uptrain-0.3.4/uptrain/v0/core/classes/logging/new_log_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/logging/new_st_run.py` & `uptrain-0.3.4/uptrain/v0/core/classes/logging/new_st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/logging/new_st_setup.py` & `uptrain-0.3.4/uptrain/v0/core/classes/logging/new_st_setup.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/logging/st_run.py` & `uptrain-0.3.4/uptrain/v0/core/classes/logging/st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/managers/check_manager.py` & `uptrain-0.3.4/uptrain/v0/core/classes/managers/check_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/__init__.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/abstract_measurable.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/abstract_measurable.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/accuracy.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/accuracy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/condition.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/condition.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/custom.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/custom.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/distance.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/feature.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/feature_concat.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/feature_concat.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/input_feature.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/input_feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/measurable.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/measurable.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/measurable_resolver.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/measurable_resolver.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/output_feature.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/output_feature.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/measurables/scalar_from_embedding.py` & `uptrain-0.3.4/uptrain/v0/core/classes/measurables/scalar_from_embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/abstract_check.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/abstract_check.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/abstract_monitor.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/abstract_monitor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/accuracy.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/accuracy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/concept_drift.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/concept_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/custom_monitor.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/custom_monitor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/data_drift.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/data_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/data_integrity.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/data_integrity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/edge_case.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/edge_case.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/feature_drift.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/feature_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/model_bias.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/model_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/monitors/output_comparison.py` & `uptrain-0.3.4/uptrain/v0/core/classes/monitors/output_comparison.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/signals/signal.py` & `uptrain-0.3.4/uptrain/v0/core/classes/signals/signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/signals/signal_manager.py` & `uptrain-0.3.4/uptrain/v0/core/classes/signals/signal_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/statistics/convergence.py` & `uptrain-0.3.4/uptrain/v0/core/classes/statistics/convergence.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/statistics/distance.py` & `uptrain-0.3.4/uptrain/v0/core/classes/statistics/distance.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/statistics/distribution.py` & `uptrain-0.3.4/uptrain/v0/core/classes/statistics/distribution.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/statistics/norm_embedding.py` & `uptrain-0.3.4/uptrain/v0/core/classes/statistics/norm_embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/statistics/old_distribution.py` & `uptrain-0.3.4/uptrain/v0/core/classes/statistics/old_distribution.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/visuals/clustering.py` & `uptrain-0.3.4/uptrain/v0/core/classes/visuals/clustering.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/visuals/dimensionality_reduction.py` & `uptrain-0.3.4/uptrain/v0/core/classes/visuals/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/visuals/plot.py` & `uptrain-0.3.4/uptrain/v0/core/classes/visuals/plot.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/classes/visuals/shap.py` & `uptrain-0.3.4/uptrain/v0/core/classes/visuals/shap.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/encoders/__init__.py` & `uptrain-0.3.4/uptrain/v0/core/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/lib/algorithms.py` & `uptrain-0.3.4/uptrain/v0/core/lib/algorithms.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/lib/cache.py` & `uptrain-0.3.4/uptrain/v0/core/lib/cache.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/lib/datastores.py` & `uptrain-0.3.4/uptrain/v0/core/lib/datastores.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/lib/helper_funcs.py` & `uptrain-0.3.4/uptrain/v0/core/lib/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/core/lib/model_signal_funcs.py` & `uptrain-0.3.4/uptrain/v0/core/lib/model_signal_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/ee/classes/measurables/llm_measurables.py` & `uptrain-0.3.4/uptrain/v0/ee/classes/measurables/llm_measurables.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/ee/lib/algorithms.py` & `uptrain-0.3.4/uptrain/v0/ee/lib/algorithms.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/ee/lib/cache.py` & `uptrain-0.3.4/uptrain/v0/ee/lib/cache.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/ee/lib/ops_agg.py` & `uptrain-0.3.4/uptrain/v0/ee/lib/ops_agg.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_a-b_testing.py` & `uptrain-0.3.4/uptrain/v0/tests/test_a-b_testing.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_concept_drift_custom_monitor.py` & `uptrain-0.3.4/uptrain/v0/tests/test_concept_drift_custom_monitor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_dashboard.py` & `uptrain-0.3.4/uptrain/v0/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_data_drift.py` & `uptrain-0.3.4/uptrain/v0/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_data_integrity.py` & `uptrain-0.3.4/uptrain/v0/tests/test_data_integrity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_data_integrity_zscore.py` & `uptrain-0.3.4/uptrain/v0/tests/test_data_integrity_zscore.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_datastores.py` & `uptrain-0.3.4/uptrain/v0/tests/test_datastores.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_edge_cases.py` & `uptrain-0.3.4/uptrain/v0/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_helpers/dataset.py` & `uptrain-0.3.4/uptrain/v0/tests/test_helpers/dataset.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_helpers/get_data_from_remote.py` & `uptrain-0.3.4/uptrain/v0/tests/test_helpers/get_data_from_remote.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_helpers/helper_funcs.py` & `uptrain-0.3.4/uptrain/v0/tests/test_helpers/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_helpers/model_tensorflow.py` & `uptrain-0.3.4/uptrain/v0/tests/test_helpers/model_tensorflow.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_helpers/model_torch.py` & `uptrain-0.3.4/uptrain/v0/tests/test_helpers/model_torch.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_helpers/pushup_signal.py` & `uptrain-0.3.4/uptrain/v0/tests/test_helpers/pushup_signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_monitors_concept_drift_adwin.py` & `uptrain-0.3.4/uptrain/v0/tests/test_monitors_concept_drift_adwin.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_monitors_concept_drift_ddm.py` & `uptrain-0.3.4/uptrain/v0/tests/test_monitors_concept_drift_ddm.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_recommender_bias.py` & `uptrain-0.3.4/uptrain/v0/tests/test_recommender_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_visuals_dimensionality_reduction.py` & `uptrain-0.3.4/uptrain/v0/tests/test_visuals_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_visuals_plot.py` & `uptrain-0.3.4/uptrain/v0/tests/test_visuals_plot.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/v0/tests/test_visuals_shap.py` & `uptrain-0.3.4/uptrain/v0/tests/test_visuals_shap.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain/validation_wrapper/validation_manager.py` & `uptrain-0.3.4/uptrain/validation_wrapper/validation_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.3.3/uptrain.egg-info/PKG-INFO` & `uptrain-0.3.4/uptrain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptrain
-Version: 0.3.3
+Version: 0.3.4
 Summary: UpTrain - ML Observability and Retraining Framework
 Maintainer-email: UpTrain AI Team <uptrain.ai@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain
 Keywords: uptrain,ai,retraining,ML,observability
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.3.3 Summary: UpTrain - ML
+Metadata-Version: 2.1 Name: uptrain Version: 0.3.4 Summary: UpTrain - ML
 Observability and Retraining Framework Maintainer-email: UpTrain AI Team
 ai@gmail.com> License: Apache-2.0 Project-URL: Homepage, https://uptrain.ai
 Project-URL: Repository, https://github.com/uptrain-ai/uptrain Keywords:
 uptrain,ai,retraining,ML,observability Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.8
```

### Comparing `uptrain-0.3.3/uptrain.egg-info/SOURCES.txt` & `uptrain-0.3.4/uptrain.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 uptrain.egg-info/PKG-INFO
 uptrain.egg-info/SOURCES.txt
 uptrain.egg-info/dependency_links.txt
 uptrain.egg-info/entry_points.txt
 uptrain.egg-info/requires.txt
 uptrain.egg-info/top_level.txt
 uptrain/dashboard/__init__.py
+uptrain/dashboard/__init__.pyi
 uptrain/dashboard/st_helpers.py
 uptrain/dashboard/st_run.py
 uptrain/dashboard/st_setup.py
 uptrain/framework/__init__.py
+uptrain/framework/__init__.pyi
 uptrain/framework/base.py
 uptrain/framework/checks.py
 uptrain/framework/remote.py
 uptrain/framework/signal.py
 uptrain/operators/__init__.py
+uptrain/operators/__init__.pyi
 uptrain/operators/base.py
 uptrain/operators/drift.py
 uptrain/operators/embs.py
 uptrain/operators/metrics.py
 uptrain/operators/similarity.py
 uptrain/operators/table.py
 uptrain/operators/vis.py
```


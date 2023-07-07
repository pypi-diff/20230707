# Comparing `tmp/kensu-2.5.5.tar.gz` & `tmp/kensu-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kensu-2.5.5.tar", last modified: Fri Feb  3 16:42:10 2023, max compression
+gzip compressed data, was "kensu-2.6.2.tar", last modified: Fri Jul  7 08:30:54 2023, max compression
```

## Comparing `kensu-2.5.5.tar` & `kensu-2.6.2.tar`

### file list

```diff
@@ -1,228 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.924961 kensu-2.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-03 16:42:01.000000 kensu-2.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-02-03 16:42:10.924961 kensu-2.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-02-03 16:42:01.000000 kensu-2.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.900961 kensu-2.5.5/kensu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/kensu_airflow_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/operators/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/operators/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/airflow/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/airflow/providers/google/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/providers/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/airflow/providers/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/providers/google/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/airflow/providers/google/cloud/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/providers/google/cloud/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/providers/google/cloud/operators/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/airflow/providers/google/cloud/transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/providers/google/cloud/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/airflow/providers/google/cloud/transfers/gcs_to_gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/boto3/
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/boto3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/botocore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/botocore/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24194 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu/client/apis/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68944 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/apis/kensu_entities_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.912961 kensu-2.5.5/kensu/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_code_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_entity_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_entity_report_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_lineage_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_model_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_model_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_physical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_process_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_process_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_process_run_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_schema_field_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/batch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/code_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/code_base_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/code_base_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/code_version_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/code_version_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/data_source_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/data_source_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/data_stats_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/field_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/lineage_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/lineage_run_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/lineage_run_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/logical_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/model_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/model_metrics_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/model_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/model_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/model_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/model_training_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/model_training_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/physical_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/physical_location_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/physical_location_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_lineage_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_lineage_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_run_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_run_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_run_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/process_run_stats_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/project_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/project_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/schema_lineage_dependency_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/schema_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/schema_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/user_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/models/user_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.912961 kensu-2.5.5/kensu/exp/
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/exp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/gluonts/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/evaluation/backtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/gluonts/ksu_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/ksu_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/ksu_utils/dataset_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/gluonts/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/model/deepar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/model/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/model/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/mx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/gluonts/mx/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/mx/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/gluonts/mx/model/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/google/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/google/cloud/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/google/cloud/bigquery/job/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/job/bigquery_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/job/bq_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/job/offline_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/job/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/google/cloud/bigquery/job/remote_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/matplotlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/matplotlib/axes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/matplotlib/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/matplotlib/axes/_subplots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/matplotlib/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/matplotlib/pyplot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.916961 kensu-2.5.5/kensu/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/numpy/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65628 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pandas/data_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pandas/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/pandas_gbq/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pandas_gbq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pandas_gbq/pandas_gbq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/psycopg2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/psycopg2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/psycopg2/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/psycopg2/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/psycopg2/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/psycopg2/pghelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/pysftp/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pysftp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/pyspark/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46776 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/pyspark/spark_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/requests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sklearn/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sklearn/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sklearn/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/sklearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sklearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sklearn/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.920961 kensu-2.5.5/kensu/sklearn/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sklearn/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/sklearn/sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.924961 kensu-2.5.5/kensu/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.924961 kensu-2.5.5/kensu/utils/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/add_deps_builder_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/ended_builder_element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.924961 kensu-2.5.5/kensu/utils/dsl/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/extractors/external_lineage_dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/extractors/generic_datasource_info_support.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/lineage_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/mapping_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/process_lineage_deps_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/dsl/with_output_builder_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/injection.py
--rw-r--r--   0 runner    (1001) docker     (123)    42781 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/kensu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/kensu_class_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/kensu_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/rule_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/simple_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-02-03 16:42:01.000000 kensu-2.5.5/kensu/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:42:10.904961 kensu-2.5.5/kensu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-02-03 16:42:10.000000 kensu-2.5.5/kensu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-02-03 16:42:10.000000 kensu-2.5.5/kensu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 16:42:10.000000 kensu-2.5.5/kensu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-03 16:42:10.000000 kensu-2.5.5/kensu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-03 16:42:10.000000 kensu-2.5.5/kensu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-03 16:42:01.000000 kensu-2.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-03 16:42:10.924961 kensu-2.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-02-03 16:42:01.000000 kensu-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.881592 kensu-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 08:30:41.000000 kensu-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-07 08:30:54.881592 kensu-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-07 08:30:41.000000 kensu-2.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.853592 kensu-2.6.2/kensu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.853592 kensu-2.6.2/kensu/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/kensu_airflow_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.853592 kensu-2.6.2/kensu/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/operators/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/operators/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.853592 kensu-2.6.2/kensu/airflow/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.853592 kensu-2.6.2/kensu/airflow/providers/google/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/providers/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.857592 kensu-2.6.2/kensu/airflow/providers/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/providers/google/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.857592 kensu-2.6.2/kensu/airflow/providers/google/cloud/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/providers/google/cloud/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/providers/google/cloud/operators/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.857592 kensu-2.6.2/kensu/airflow/providers/google/cloud/transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/providers/google/cloud/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/airflow/providers/google/cloud/transfers/gcs_to_gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.857592 kensu-2.6.2/kensu/boto3/
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/boto3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.857592 kensu-2.6.2/kensu/botocore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/botocore/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.857592 kensu-2.6.2/kensu/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24194 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.857592 kensu-2.6.2/kensu/client/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68944 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/apis/kensu_entities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.865592 kensu-2.6.2/kensu/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_code_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_entity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_entity_report_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_lineage_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_model_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_model_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_physical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_process_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_process_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_process_run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_schema_field_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/batch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/code_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/code_base_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/code_base_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/code_version_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/code_version_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/data_source_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/data_source_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/data_stats_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/field_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/lineage_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/lineage_run_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/lineage_run_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/logical_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/model_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/model_metrics_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/model_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/model_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/model_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/model_training_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/model_training_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/physical_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/physical_location_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/physical_location_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_lineage_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_lineage_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_run_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_run_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/process_run_stats_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/project_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/project_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/schema_lineage_dependency_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/schema_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/schema_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/user_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/models/user_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.865592 kensu-2.6.2/kensu/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/exp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.865592 kensu-2.6.2/kensu/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/gluonts/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/evaluation/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/gluonts/ksu_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/ksu_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/ksu_utils/dataset_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/gluonts/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/model/deepar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/model/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/model/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/mx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/gluonts/mx/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/mx/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/gluonts/mx/model/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/google/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/google/cloud/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.869592 kensu-2.6.2/kensu/google/cloud/bigquery/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/job/bigquery_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/job/bq_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/job/offline_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/job/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/google/cloud/bigquery/job/remote_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/matplotlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/matplotlib/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/matplotlib/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/matplotlib/axes/_subplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/matplotlib/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/matplotlib/pyplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/numpy/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65628 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pandas/data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pandas/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/pandas_gbq/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pandas_gbq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pandas_gbq/pandas_gbq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/psycopg2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/psycopg2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.873592 kensu-2.6.2/kensu/psycopg2/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/psycopg2/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/psycopg2/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/psycopg2/pghelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.877592 kensu-2.6.2/kensu/pysftp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pysftp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.877592 kensu-2.6.2/kensu/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54879 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/pyspark/spark_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.877592 kensu-2.6.2/kensu/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/requests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.877592 kensu-2.6.2/kensu/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.877592 kensu-2.6.2/kensu/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sklearn/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sklearn/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sklearn/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.877592 kensu-2.6.2/kensu/sklearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sklearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sklearn/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.877592 kensu-2.6.2/kensu/sklearn/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sklearn/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/sklearn/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.881592 kensu-2.6.2/kensu/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.881592 kensu-2.6.2/kensu/utils/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/add_deps_builder_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/ended_builder_element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.881592 kensu-2.6.2/kensu/utils/dsl/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/extractors/external_lineage_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/extractors/generic_datasource_info_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/lineage_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/mapping_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/process_lineage_deps_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/dsl/with_output_builder_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42882 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/kensu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/kensu_class_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/kensu_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.881592 kensu-2.6.2/kensu/utils/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/remote/circuit_breakers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/rule_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/simple_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-07 08:30:41.000000 kensu-2.6.2/kensu/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:30:54.853592 kensu-2.6.2/kensu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-07 08:30:54.000000 kensu-2.6.2/kensu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-07 08:30:54.000000 kensu-2.6.2/kensu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:30:54.000000 kensu-2.6.2/kensu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-07 08:30:54.000000 kensu-2.6.2/kensu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 08:30:54.000000 kensu-2.6.2/kensu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 08:30:41.000000 kensu-2.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 08:30:54.885592 kensu-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-07 08:30:41.000000 kensu-2.6.2/setup.py
```

### Comparing `kensu-2.5.5/LICENSE` & `kensu-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/PKG-INFO` & `kensu-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: kensu
-Version: 2.5.5
+Version: 2.6.2
 Home-page: 
 Author-email: 
 Keywords: DODD,Data Observability Driven Development,Data Observability,Analytics Observability
 Platform: Posix; MacOS X; Windows
 Provides-Extra: pysftp
 Provides-Extra: pandas
 Provides-Extra: sklearn
 Provides-Extra: numpy
 Provides-Extra: scikit-learn
-Provides-Extra: gluonts
 Provides-Extra: gluon
+Provides-Extra: gluonts
 Provides-Extra: boto
 Provides-Extra: boto3
-Provides-Extra: pg
 Provides-Extra: psycopg2-binary
+Provides-Extra: pg
 Provides-Extra: pglast
-Provides-Extra: gbq
 Provides-Extra: google-cloud-bigquery
+Provides-Extra: gbq
 Provides-Extra: sqlparse 
-Provides-Extra: airflow
 Provides-Extra: airflow-google
 Provides-Extra: apache-airflow[google]
+Provides-Extra: airflow
 Provides-Extra: twine
 Provides-Extra: gcsfs
 Provides-Extra: fsspec
-Provides-Extra: packaging
 Provides-Extra: sdk
+Provides-Extra: packaging
 Provides-Extra: kafka
 Provides-Extra: confluent-kafka
-Provides-Extra: GitPython
 Provides-Extra: git
+Provides-Extra: GitPython
 Provides-Extra: pytest-sftpserver
 Provides-Extra: test
 Provides-Extra: pytest
 Provides-Extra: pytest-mock
 Provides-Extra: pytest-vcr
 Provides-Extra: all
 Provides-Extra: all-but-test
```

### Comparing `kensu-2.5.5/README.md` & `kensu-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/airflow/kensu_airflow_collector.py` & `kensu-2.6.2/kensu/airflow/kensu_airflow_collector.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/airflow/operators/bash.py` & `kensu-2.6.2/kensu/airflow/operators/bash.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/airflow/operators/python.py` & `kensu-2.6.2/kensu/airflow/operators/python.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/airflow/providers/google/cloud/operators/bigquery.py` & `kensu-2.6.2/kensu/airflow/providers/google/cloud/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/airflow/providers/google/cloud/transfers/gcs_to_gcs.py` & `kensu-2.6.2/kensu/airflow/providers/google/cloud/transfers/gcs_to_gcs.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/boto3/__init__.py` & `kensu-2.6.2/kensu/boto3/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/__init__.py` & `kensu-2.6.2/kensu/client/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/api_client.py` & `kensu-2.6.2/kensu/client/api_client.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/apis/kensu_entities_api.py` & `kensu-2.6.2/kensu/client/apis/kensu_entities_api.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/configuration.py` & `kensu-2.6.2/kensu/client/configuration.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/__init__.py` & `kensu-2.6.2/kensu/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_code_base.py` & `kensu-2.6.2/kensu/client/models/batch_code_base.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_code_version.py` & `kensu-2.6.2/kensu/client/models/batch_code_version.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_data_source.py` & `kensu-2.6.2/kensu/client/models/batch_data_source.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_data_stats.py` & `kensu-2.6.2/kensu/client/models/batch_data_stats.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_entity_report.py` & `kensu-2.6.2/kensu/client/models/batch_entity_report.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_entity_report_result.py` & `kensu-2.6.2/kensu/client/models/batch_entity_report_result.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_error_message.py` & `kensu-2.6.2/kensu/client/models/batch_error_message.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_lineage_run.py` & `kensu-2.6.2/kensu/client/models/batch_lineage_run.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_model.py` & `kensu-2.6.2/kensu/client/models/batch_model.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_model_metrics.py` & `kensu-2.6.2/kensu/client/models/batch_model_metrics.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_model_training.py` & `kensu-2.6.2/kensu/client/models/batch_model_training.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_physical_location.py` & `kensu-2.6.2/kensu/client/models/batch_physical_location.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_process.py` & `kensu-2.6.2/kensu/client/models/batch_process.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_process_lineage.py` & `kensu-2.6.2/kensu/client/models/batch_process_lineage.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_process_run.py` & `kensu-2.6.2/kensu/client/models/batch_process_run.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_process_run_stats.py` & `kensu-2.6.2/kensu/client/models/batch_process_run_stats.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_project.py` & `kensu-2.6.2/kensu/client/models/batch_project.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_schema.py` & `kensu-2.6.2/kensu/client/models/batch_schema.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_schema_field_tag.py` & `kensu-2.6.2/kensu/client/models/batch_schema_field_tag.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/batch_user.py` & `kensu-2.6.2/kensu/client/models/batch_user.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/code_base.py` & `kensu-2.6.2/kensu/client/models/code_base.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/code_base_pk.py` & `kensu-2.6.2/kensu/client/models/code_base_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/code_base_ref.py` & `kensu-2.6.2/kensu/client/models/code_base_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/code_version.py` & `kensu-2.6.2/kensu/client/models/code_version.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/code_version_pk.py` & `kensu-2.6.2/kensu/client/models/code_version_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/code_version_ref.py` & `kensu-2.6.2/kensu/client/models/code_version_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/data_source.py` & `kensu-2.6.2/kensu/client/models/data_source.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/data_source_pk.py` & `kensu-2.6.2/kensu/client/models/data_source_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/data_source_ref.py` & `kensu-2.6.2/kensu/client/models/data_source_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/data_stats.py` & `kensu-2.6.2/kensu/client/models/data_stats.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/data_stats_pk.py` & `kensu-2.6.2/kensu/client/models/data_stats_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/field_def.py` & `kensu-2.6.2/kensu/client/models/field_def.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/lineage_run.py` & `kensu-2.6.2/kensu/client/models/lineage_run.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/lineage_run_pk.py` & `kensu-2.6.2/kensu/client/models/lineage_run_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/lineage_run_ref.py` & `kensu-2.6.2/kensu/client/models/lineage_run_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/logical_data_source.py` & `kensu-2.6.2/kensu/client/models/logical_data_source.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/model.py` & `kensu-2.6.2/kensu/client/models/model.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/model_metrics.py` & `kensu-2.6.2/kensu/client/models/model_metrics.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/model_metrics_pk.py` & `kensu-2.6.2/kensu/client/models/model_metrics_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/model_pk.py` & `kensu-2.6.2/kensu/client/models/model_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/model_ref.py` & `kensu-2.6.2/kensu/client/models/model_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/model_training.py` & `kensu-2.6.2/kensu/client/models/model_training.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/model_training_pk.py` & `kensu-2.6.2/kensu/client/models/model_training_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/model_training_ref.py` & `kensu-2.6.2/kensu/client/models/model_training_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/physical_location.py` & `kensu-2.6.2/kensu/client/models/physical_location.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/physical_location_pk.py` & `kensu-2.6.2/kensu/client/models/physical_location_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/physical_location_ref.py` & `kensu-2.6.2/kensu/client/models/physical_location_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process.py` & `kensu-2.6.2/kensu/client/models/process.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_lineage.py` & `kensu-2.6.2/kensu/client/models/process_lineage.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_lineage_pk.py` & `kensu-2.6.2/kensu/client/models/process_lineage_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_lineage_ref.py` & `kensu-2.6.2/kensu/client/models/process_lineage_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_pk.py` & `kensu-2.6.2/kensu/client/models/process_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_ref.py` & `kensu-2.6.2/kensu/client/models/process_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_run.py` & `kensu-2.6.2/kensu/client/models/process_run.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_run_pk.py` & `kensu-2.6.2/kensu/client/models/process_run_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_run_ref.py` & `kensu-2.6.2/kensu/client/models/process_run_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_run_stats.py` & `kensu-2.6.2/kensu/client/models/process_run_stats.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/process_run_stats_pk.py` & `kensu-2.6.2/kensu/client/models/process_run_stats_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/project.py` & `kensu-2.6.2/kensu/client/models/project.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/project_pk.py` & `kensu-2.6.2/kensu/client/models/project_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/project_ref.py` & `kensu-2.6.2/kensu/client/models/project_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/schema.py` & `kensu-2.6.2/kensu/client/models/schema.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/schema_lineage_dependency_def.py` & `kensu-2.6.2/kensu/client/models/schema_lineage_dependency_def.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/schema_pk.py` & `kensu-2.6.2/kensu/client/models/schema_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/schema_ref.py` & `kensu-2.6.2/kensu/client/models/schema_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/user.py` & `kensu-2.6.2/kensu/client/models/user.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/user_pk.py` & `kensu-2.6.2/kensu/client/models/user_pk.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/models/user_ref.py` & `kensu-2.6.2/kensu/client/models/user_ref.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/client/rest.py` & `kensu-2.6.2/kensu/client/rest.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/exp/__init__.py` & `kensu-2.6.2/kensu/exp/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/gluonts/evaluation/backtest.py` & `kensu-2.6.2/kensu/gluonts/evaluation/backtest.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/gluonts/ksu_utils/dataset_helpers.py` & `kensu-2.6.2/kensu/gluonts/ksu_utils/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/gluonts/model/deepar.py` & `kensu-2.6.2/kensu/gluonts/model/deepar.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/gluonts/model/forecast.py` & `kensu-2.6.2/kensu/gluonts/model/forecast.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/gluonts/mx/model/predictor.py` & `kensu-2.6.2/kensu/gluonts/mx/model/predictor.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/google/cloud/bigquery/client.py` & `kensu-2.6.2/kensu/google/cloud/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/google/cloud/bigquery/extractor.py` & `kensu-2.6.2/kensu/google/cloud/bigquery/extractor.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/google/cloud/bigquery/job/bigquery_stats.py` & `kensu-2.6.2/kensu/google/cloud/bigquery/job/bigquery_stats.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/google/cloud/bigquery/job/bq_helpers.py` & `kensu-2.6.2/kensu/google/cloud/bigquery/job/bq_helpers.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/google/cloud/bigquery/job/offline_parser.py` & `kensu-2.6.2/kensu/google/cloud/bigquery/job/offline_parser.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/google/cloud/bigquery/job/query.py` & `kensu-2.6.2/kensu/google/cloud/bigquery/job/query.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/google/cloud/bigquery/job/remote_parser.py` & `kensu-2.6.2/kensu/google/cloud/bigquery/job/remote_parser.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/itertools.py` & `kensu-2.6.2/kensu/itertools.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/json/__init__.py` & `kensu-2.6.2/kensu/json/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/matplotlib/axes/_subplots.py` & `kensu-2.6.2/kensu/matplotlib/axes/_subplots.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/matplotlib/extractor.py` & `kensu-2.6.2/kensu/matplotlib/extractor.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/matplotlib/pyplot.py` & `kensu-2.6.2/kensu/matplotlib/pyplot.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/numpy/__init__.py` & `kensu-2.6.2/kensu/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/numpy/extractor.py` & `kensu-2.6.2/kensu/numpy/extractor.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/pandas/__init__.py` & `kensu-2.6.2/kensu/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/pandas/data_frame.py` & `kensu-2.6.2/kensu/pandas/data_frame.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/pandas/extractor.py` & `kensu-2.6.2/kensu/pandas/extractor.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/pandas_gbq/pandas_gbq.py` & `kensu-2.6.2/kensu/pandas_gbq/pandas_gbq.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/pickle/pickle.py` & `kensu-2.6.2/kensu/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/psycopg2/extras/__init__.py` & `kensu-2.6.2/kensu/psycopg2/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/psycopg2/parser.py` & `kensu-2.6.2/kensu/psycopg2/parser.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/psycopg2/pghelpers.py` & `kensu-2.6.2/kensu/psycopg2/pghelpers.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/pysftp/__init__.py` & `kensu-2.6.2/kensu/pysftp/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/pyspark/spark_connector.py` & `kensu-2.6.2/kensu/pyspark/spark_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,38 +264,35 @@
             import traceback
             logging.warning("KENSU: unexpected issue: {}".format(traceback.format_exc()))
         return self
     return report_as_kpi
 
 
 def patch_kensu_df_helpers():
-    try:
-        logging.info('KENSU: Adding DataFrame.report_as_kensu_datasource')
-        from pyspark.sql import DataFrame
-        DataFrame.report_as_kensu_datasource = report_df_as_kensu_datasource()
-        logging.info('KENSU: done adding DataFrame.report_as_kensu_datasource')
-    except:
-        import traceback
-        logging.warning("KENSU: unexpected issue when patching DataFrame.report_as_kensu_datasource: {}".format(traceback.format_exc()))
-    try:
-        logging.info('KENSU: Adding DataFrame.report_as_kensu_jdbc_datasource')
-        from pyspark.sql import DataFrame
-        DataFrame.report_as_kensu_jdbc_datasource = report_df_as_kensu_jdbc_datasource()
-        logging.info('KENSU: done adding DataFrame.report_as_kensu_jdbc_datasource')
-    except:
-        import traceback
-        logging.warning("KENSU: unexpected issue when patching DataFrame.report_as_kensu_jdbc_datasource: {}".format(traceback.format_exc()))
-    try:
-        logging.info('KENSU: Adding DataFrame.report_as_kpi')
-        from pyspark.sql import DataFrame
-        DataFrame.report_as_kpi = report_df_as_kpi()
-        logging.info('KENSU: done adding DataFrame.report_as_kpi')
-    except:
-        import traceback
-        logging.warning("KENSU: unexpected issue when patching DataFrame.report_as_kpi: {}".format(traceback.format_exc()))
+    fns_to_patch = list(map(lambda fn: [fn.__name__, fn], [
+        addOutputObservations,
+        addCustomObservationsToOutput,
+        reportCustomKafkaInputSchema,
+        reportCustomEventhubInputSchema
+    ])) + [
+        ['report_as_kensu_datasource', report_df_as_kensu_datasource()],
+        ['report_as_kensu_jdbc_datasource', report_df_as_kensu_jdbc_datasource()],
+        ['report_as_kpi', report_df_as_kpi()]
+    ]
+    for fn_name, wrapper_builder in fns_to_patch:
+        try:
+            logging.info(f'KENSU: Patching DataFrame.{fn_name}')
+            from pyspark.sql import DataFrame
+            # can setattr behave differently than .somename = somevalue?
+            setattr(DataFrame, fn_name, wrapper_builder)
+            logging.info(f'KENSU: done patching DataFrame.{fn_name}')
+        except:
+            import traceback
+            log_and_print(logging.warning,
+                          f"KENSU: unexpected issue when patching DataFrame.{fn_name}: {traceback.format_exc()}")
 
 
 def join_paths(maybe_directory, # type: str
                file # type: str
                ):
     if maybe_directory is not None and maybe_directory.strip():
         import os
@@ -523,14 +520,20 @@
         project_name=None,
         h2o_support=None,
         h2o_create_virtual_training_datasource=None,
         patch_pandas_conversions=False,
         pandas_to_spark_df_via_tmp_file=None,
         pandas_to_spark_tmp_dir=None,
         use_api_client=None,
+        remote_conf_enabled=True,
+        remote_conf_timeout_secs=None,
+        remote_circuit_breaker_enabled=True,
+        remote_circuit_breaker_precheck_delay_secs=None,
+        datastats_send_timeout_secs=None,
+        conf_file_path=None,
         **kwargs
 ):
     import os
     is_tracking_disabled = (os.environ.get("KSU_DISABLE_TRACKING", 'False') == 'True') or disable_tracking
 
     if not is_tracking_disabled:
         logging.info("Initializing Kensu tracking...")
@@ -684,14 +687,16 @@
                 if value is not None:
                     properties.add(t2(name, value))
 
             properties.add(provider_class_name)
             properties.add(repository)
             properties.add(version)
             properties.add(user)
+            if kensu_ingestion_url:
+                properties.add(t2("kensu_ingestion_url", kensu_ingestion_url))
             if kensu_ingestion_token:
                 properties.add(t2("kensu_ingestion_token", kensu_ingestion_token))
             if report_to_file is not None:
                 properties.add(t2("report_to_file", report_to_file))
             if logs_dir_path:
                 properties.add(t2("offline_report_dir_path", logs_dir_path))
             if offline_file_name:
@@ -722,14 +727,28 @@
             add_prop("output_stats_compute_quantiles", output_stats_compute_quantiles)
             add_prop("output_stats_compute_simple_num", output_stats_compute_simple_num)
             add_prop("output_stats_compute_std_dev", output_stats_compute_std_dev)
             add_prop("output_stats_cache_by_path", output_stats_cache_by_path)
             add_prop("output_stats_coalesce_enabled", output_stats_coalesce_enabled)
             add_prop("output_stats_coalesce_workers", output_stats_coalesce_workers)
 
+            def extract_prop(name, tpe, value):
+                return name, extract_config_property(key=name, default=None, arg=value, kw=kwargs, conf=kensu_conf, tpe=tpe)
+
+            properties_by_name = [
+                extract_prop('remote_conf_enabled', tpe=bool, value=remote_conf_enabled),
+                extract_prop('remote_conf_timeout_secs', tpe=int, value=remote_conf_timeout_secs),
+                extract_prop('remote_circuit_breaker_enabled', tpe=bool, value=remote_circuit_breaker_enabled),
+                extract_prop('remote_circuit_breaker_precheck_delay_secs', tpe=int, value=remote_circuit_breaker_precheck_delay_secs),
+                extract_prop('datastats_send_timeout_secs', tpe=int, value=datastats_send_timeout_secs),
+            ]
+            for prop_name, prop_value in properties_by_name:
+                if prop_value is not None:
+                    add_prop(prop_name, prop_value)
+
             if shutdown_timeout_sec is not None:
                 properties.add(t2("shutdown_timeout_sec", shutdown_timeout_sec))
             if enable_collector_log_file:
                 debug_level = collector_log_level or "INFO"
                 if process_name is not None:
                     kensu_debug_filename = join_paths(logs_dir_path, process_name + ".kensu-collector.log")
                 else:
@@ -778,16 +797,22 @@
             if maybe_fake_timestamp is not None:
                 set_fake_timestamp(spark_session, maybe_fake_timestamp)
             maybe_ds_path_sanitizer_search = os.environ.get('KSU_DS_PATH_SANITIZER_SEARCH')
             maybe_ds_path_sanitizer_replace = os.environ.get('KSU_DS_PATH_SANITIZER_REPLACE')
             if (maybe_ds_path_sanitizer_search is not None) and (maybe_ds_path_sanitizer_replace is not None):
                 add_ds_path_sanitizer(spark_session, maybe_ds_path_sanitizer_search, maybe_ds_path_sanitizer_replace)
 
-            w = jvm.io.kensu.sparkcollector.KensuSparkCollector.KensuSparkSession(spark_session._jsparkSession)
-            w.track(ingestion_url, jvm.scala.Option.empty(), properties.toSeq())
+            if is_databricks():
+                print('Detected Databricks Notebook - initializing Kensu via DatabricksCollector.track()')
+                w = ref_scala_object(jvm, 'io.kensu.sparkcollector.environments.DatabricksCollector')
+                # FIXME: DON'T WE OVERRIDE SOME UNNEEDED CONF KEYS!?
+                w.track(spark_session._jsparkSession, conf_file_path or get_conf_path(), properties.toSeq())
+            else:
+                w = jvm.io.kensu.sparkcollector.KensuSparkCollector.KensuSparkSession(spark_session._jsparkSession)
+                w.track(ingestion_url, jvm.scala.Option.empty(), properties.toSeq())
 
             if (shutdown_timeout_sec is not None) and (shutdown_timeout_sec > 0):
                 logging.info('KENSU: patching spark.stop to wait for Kensu Spark-Collector reporting to finish')
                 from pyspark.sql import SparkSession
                 SparkSession.stop = patched_spark_stop(SparkSession.stop, shutdown_timeout_sec)
                 logging.info('KENSU: patching spark.stop done')
 
@@ -867,8 +892,159 @@
                                   debug_stdout_enabled=True,
                                   create_virtual_training_datasource=h2o_create_virtual_training_datasource)
 
         except Exception as e:
             import traceback
             logging.warning("Error when initializing Kensu tracking: " + traceback.format_exc())
     else:
-        logging.info("Tracking by Kensu is disabled")
+        logging.info("Tracking by Kensu is disabled")
+
+
+def check_spark_circuit_breakers_and_stop_if_broken(
+        spark,
+        stop_spark=True):
+    cls = ref_scala_object(spark.sparkContext._jvm, "io.kensu.sparkcollector.KensuSparkCollector")
+    breakers_failed = cls.checkIfCircuitBreakersFailedAndPrepShutdown(spark._jsparkSession)
+    if breakers_failed:
+        logging.warning("Some kensu circuit breaker has failed (there are active unresolved tickets in a rule "
+                        "marked as a circuit breaker), so the app will shutdown now")
+        if stop_spark:
+            logging.warning("Shutting down Spark context now...")
+            spark.stop()
+        else:
+            logging.warning("Not shutting down Spark context as it was not requested.")
+    return breakers_failed
+
+
+def is_databricks():
+    import os
+    return "DATABRICKS_RUNTIME_VERSION" in os.environ
+
+
+def log_and_print(log_fn, msg):
+    log_fn(msg)
+    # in Databricks print to stdout too, so output is visible in the same notebook
+    # (default logging loglevel is WARNING, so logging.info would be lost)
+    if is_databricks():
+        print(msg)
+
+
+def with_catch_errors(fn_name, default_result, fn_result_lambda):
+    # TODO: check configurable decorators too https://stackoverflow.com/a/27446895 ?
+    result = default_result
+    try:
+        logging.info(f'KENSU: in {fn_name}')
+        result = fn_result_lambda(default_result)
+        logging.info(f'KENSU: {fn_name} done')
+    except:
+        import traceback
+        log_and_print(logging.warning, f"KENSU: unexpected issue in {fn_name}: {traceback.format_exc()}")
+    return result
+
+
+def catch_errors_with_default_self(func):
+    def new_func(*args, **kwargs):
+        default_self = args[0]
+        return with_catch_errors(
+            fn_name=func.__name__,
+            default_result=default_self,
+            fn_result_lambda=lambda default_result: func(*args, **kwargs))
+    new_func.__doc__ = func.__doc__
+    new_func.__name__ = func.__name__
+    try:
+        import inspect
+        new_func.__signature__ = inspect.signature(func)
+    except:
+        pass
+    return new_func
+
+
+@catch_errors_with_default_self
+def addOutputObservations(df,  # type: DataFrame
+                          compute_count_distinct=False  # not recommended due to likely performance impact
+                          ):
+    # FIXME: looks like we have a repeating pyspark DF -> JVM DF -> pyspark DF pattern here
+    spark = df.sql_ctx.sparkSession
+    jvm = spark.sparkContext._jvm
+    cls = ref_scala_object(jvm, "org.apache.spark.sql.kensu.KensuObserveMetrics")
+    #   def addOutputObservations(df: DataFrame, computeCountDistinct: Boolean = false): DataFrame
+    jdf = cls.addOutputObservations(df._jdf, compute_count_distinct)
+    # finally convert Java DataFrame back to python DataFrame
+    from pyspark.sql.dataframe import DataFrame
+    return DataFrame(jdf, spark)
+
+
+# a global var, used in addCustomObservationsToOutput
+next_observation_num = 0
+
+
+@catch_errors_with_default_self
+def addCustomObservationsToOutput(df,  # type: DataFrame
+                                  *exprs  # type: pyspark.sql.column.Column
+                                 ):
+    """
+    custom observations/metrics can be added at any stage of the stream DataFrame - and currently uses same semantics as
+     pyspark's own DataFrame.observe(), so can pass any Spark aggregation expressions.
+
+    just make sure that each expression:
+    - return a double datatype .cast("double")
+    - has a unique and meaningful alias within the whole stream DataFrame
+      because that will become metrics name in Kensu, e.g. expr.alias("someColumn.max_before_filtering")
+
+    see https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.DataFrame.observe.html
+    """
+    global next_observation_num
+    next_observation_num = next_observation_num + 1
+    return df.observe(
+        # observation ID must be unique and start with ksu_metrics_output_
+        f"ksu_metrics_output_custom_gen{next_observation_num}",
+       *exprs
+    )
+
+
+def pyspark_datatype_to_jvm(jvm, pyspark_datatype):
+    return ref_scala_object(jvm, "org.apache.spark.sql.types.DataType")\
+        .fromJson(pyspark_datatype.json())
+
+
+@catch_errors_with_default_self
+def reportCustomKafkaInputSchema(df,  # type: DataFrame
+                                 custom_schema=None,  # StructType, if None, will use current DataFrame schema
+                                 fieldNamePrefix="value.",
+                                 schemaDesc="after Kafka event value parsing"
+                                ):
+    """
+    this reports a custom schema for a Kafka read operations in Spark Streaming.
+    it works by finding all/any such source URIs in the provided `SparkStreaming DataFrame`,
+    and for each (if any), reporting the provided custom schema
+
+    P.S. custom schema may appear in Kensu a few minutes later if the source was not yet ingested before (ingestion delay)
+    """
+    jvm = get_jvm_from_df(df)
+    cls = ref_scala_object(jvm, "org.apache.spark.sql.kensu.KafkaStreamCustomSchema")
+    jvm_datatype = pyspark_datatype_to_jvm(jvm, custom_schema or df.schema())
+    #   def reportCustomSchema(df: DataFrame, custom_schema: StructType, fieldNamePrefix: String, schemaDesc: String): DataFrame
+    res = cls.reportCustomSchema(df._jdf, jvm_datatype, fieldNamePrefix, schemaDesc)
+    log_and_print(logging.info, f'Tried reporting custom Kafka schema: {res}')
+    return df
+
+
+@catch_errors_with_default_self
+def reportCustomEventhubInputSchema(df,  # type: DataFrame
+                                 custom_schema=None,  # StructType, if None, will use current DataFrame schema
+                                 fieldNamePrefix="body.",
+                                 schemaDesc="after EventHub event value parsing"
+                                 ):
+    """
+    this reports a custom schema for a EventHub read operations in Spark Streaming.
+    it works by finding all/any such source URIs in the provided `SparkStreaming DataFrame`,
+    and for each (if any), reporting the provided custom schema
+
+    P.S. custom schema may appear in Kensu a few minutes later if the source was not yet ingested before (ingestion delay)
+    """
+    jvm = get_jvm_from_df(df)
+    cls = ref_scala_object(jvm, "org.apache.spark.sql.kensu.EventHubsCustomSchema")
+    jvm_datatype = pyspark_datatype_to_jvm(jvm, custom_schema or df.schema())
+    #   def reportCustomSchema(df: DataFrame, custom_schema: StructType, fieldNamePrefix: String, schemaDesc: String): DataFrame
+    res = cls.reportCustomSchema(df._jdf, jvm_datatype, fieldNamePrefix, schemaDesc)
+    log_and_print(logging.info, f'Tried reporting custom EventHub schema: {res}')
+    return df
```

### Comparing `kensu-2.5.5/kensu/requests/api.py` & `kensu-2.6.2/kensu/requests/api.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/requests/models.py` & `kensu-2.6.2/kensu/requests/models.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/sdk/__init__.py` & `kensu-2.6.2/kensu/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/sklearn/extractor.py` & `kensu-2.6.2/kensu/sklearn/extractor.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/sklearn/linear_model.py` & `kensu-2.6.2/kensu/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/sklearn/model_selection/__init__.py` & `kensu-2.6.2/kensu/sklearn/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/sklearn/neighbors.py` & `kensu-2.6.2/kensu/sklearn/neighbors.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/sklearn/preprocessing/__init__.py` & `kensu-2.6.2/kensu/sklearn/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/add_deps_builder_element.py` & `kensu-2.6.2/kensu/utils/dsl/add_deps_builder_element.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/ended_builder_element.py` & `kensu-2.6.2/kensu/utils/dsl/ended_builder_element.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/extractors/__init__.py` & `kensu-2.6.2/kensu/utils/dsl/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/extractors/external_lineage_dtos.py` & `kensu-2.6.2/kensu/utils/dsl/extractors/external_lineage_dtos.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/extractors/generic_datasource_info_support.py` & `kensu-2.6.2/kensu/utils/dsl/extractors/generic_datasource_info_support.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/lineage_builder.py` & `kensu-2.6.2/kensu/utils/dsl/lineage_builder.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/mapping_strategies.py` & `kensu-2.6.2/kensu/utils/dsl/mapping_strategies.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/process_lineage_deps_builder.py` & `kensu-2.6.2/kensu/utils/dsl/process_lineage_deps_builder.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/dsl/with_output_builder_element.py` & `kensu-2.6.2/kensu/utils/dsl/with_output_builder_element.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/exceptions.py` & `kensu-2.6.2/kensu/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/helpers.py` & `kensu-2.6.2/kensu/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/injection.py` & `kensu-2.6.2/kensu/utils/injection.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/kensu.py` & `kensu-2.6.2/kensu/utils/kensu.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,14 +268,16 @@
             self.project_refs = []
         else:
             project = Project(pk=ProjectPK(name=project_name))
             self.projects.append(project)
             self.project_refs = [project.to_ref()]
 
         process_run_name = process_name + "@" + datetime.datetime.now().isoformat()
+        if timestamp is not None:
+            process_run_name = process_name + "@" + str(timestamp)
         self.process_run = ProcessRun(
             pk=ProcessRunPK(process_ref=self.process.to_ref(), qualified_name=process_run_name)
             , launched_by_user_ref=self.user.to_ref()
             , executed_code_version_ref=self.code_version.to_ref()
             , projects_refs=self.project_refs
             , environment = environment
         )
```

### Comparing `kensu-2.5.5/kensu/utils/kensu_class_handlers.py` & `kensu-2.6.2/kensu/utils/kensu_class_handlers.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/kensu_provider.py` & `kensu-2.6.2/kensu/utils/kensu_provider.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/reporters.py` & `kensu-2.6.2/kensu/utils/reporters.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/rule_engine.py` & `kensu-2.6.2/kensu/utils/rule_engine.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu/utils/wrappers.py` & `kensu-2.6.2/kensu/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `kensu-2.5.5/kensu.egg-info/PKG-INFO` & `kensu-2.6.2/kensu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: kensu
-Version: 2.5.5
+Version: 2.6.2
 Home-page: 
 Author-email: 
 Keywords: DODD,Data Observability Driven Development,Data Observability,Analytics Observability
 Platform: Posix; MacOS X; Windows
 Provides-Extra: pysftp
 Provides-Extra: pandas
 Provides-Extra: sklearn
 Provides-Extra: numpy
 Provides-Extra: scikit-learn
-Provides-Extra: gluonts
 Provides-Extra: gluon
+Provides-Extra: gluonts
 Provides-Extra: boto
 Provides-Extra: boto3
-Provides-Extra: pg
 Provides-Extra: psycopg2-binary
+Provides-Extra: pg
 Provides-Extra: pglast
-Provides-Extra: gbq
 Provides-Extra: google-cloud-bigquery
+Provides-Extra: gbq
 Provides-Extra: sqlparse 
-Provides-Extra: airflow
 Provides-Extra: airflow-google
 Provides-Extra: apache-airflow[google]
+Provides-Extra: airflow
 Provides-Extra: twine
 Provides-Extra: gcsfs
 Provides-Extra: fsspec
-Provides-Extra: packaging
 Provides-Extra: sdk
+Provides-Extra: packaging
 Provides-Extra: kafka
 Provides-Extra: confluent-kafka
-Provides-Extra: GitPython
 Provides-Extra: git
+Provides-Extra: GitPython
 Provides-Extra: pytest-sftpserver
 Provides-Extra: test
 Provides-Extra: pytest
 Provides-Extra: pytest-mock
 Provides-Extra: pytest-vcr
 Provides-Extra: all
 Provides-Extra: all-but-test
```

### Comparing `kensu-2.5.5/kensu.egg-info/SOURCES.txt` & `kensu-2.6.2/kensu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -175,8 +175,9 @@
 kensu/utils/dsl/ended_builder_element.py
 kensu/utils/dsl/lineage_builder.py
 kensu/utils/dsl/mapping_strategies.py
 kensu/utils/dsl/process_lineage_deps_builder.py
 kensu/utils/dsl/with_output_builder_element.py
 kensu/utils/dsl/extractors/__init__.py
 kensu/utils/dsl/extractors/external_lineage_dtos.py
-kensu/utils/dsl/extractors/generic_datasource_info_support.py
+kensu/utils/dsl/extractors/generic_datasource_info_support.py
+kensu/utils/remote/circuit_breakers.py
```

### Comparing `kensu-2.5.5/kensu.egg-info/requires.txt` & `kensu-2.6.2/kensu.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -15,64 +15,64 @@
 [GitPython]
 GitPython
 
 [airflow]
 apache-airflow[google]==2.2.3
 
 [airflow-google]
-twine<=3.8.0
-gcsfs
 fsspec
 apache-airflow[google]==2.2.3
+gcsfs
+twine<=3.8.0
 
 [all]
-pglast==v3.4
+fsspec
+pytest-sftpserver
 pytest>=6.2.4
-numpy>=1.19.5
+apache-airflow[google]==2.2.3
 pysftp>=0.2.9
-sqlparse>=0.4.2
+pytest-vcr
 scikit-learn>=0.24.2
-gcsfs
-boto3
-fsspec
-pandas>=1.2.4
-confluent-kafka
-google-cloud-bigquery>=2.26.0
-apache-airflow[google]==2.2.3
 psycopg2-binary==2.9.3
+twine<=3.8.0
+gluonts==0.6.5
+gcsfs
 packaging
+pglast==v3.4
 pytest-mock
 GitPython
-pytest-vcr
-gluonts==0.6.5
-twine<=3.8.0
-pytest-sftpserver
+confluent-kafka
+pandas>=1.2.4
+sqlparse>=0.4.2
+numpy>=1.19.5
+google-cloud-bigquery>=2.26.0
+boto3
 
 [all-but-test]
-pglast==v3.4
+fsspec
+pytest-sftpserver
 pytest>=6.2.4
-numpy>=1.19.5
+apache-airflow[google]==2.2.3
 pysftp>=0.2.9
-sqlparse>=0.4.2
+pytest-vcr
 scikit-learn>=0.24.2
-gcsfs
-boto3
-fsspec
-pandas>=1.2.4
-confluent-kafka
-google-cloud-bigquery>=2.26.0
-apache-airflow[google]==2.2.3
 psycopg2-binary==2.9.3
+twine<=3.8.0
+gluonts==0.6.5
+gcsfs
 packaging
+pglast==v3.4
 pytest-mock
 GitPython
-pytest-vcr
-gluonts==0.6.5
-twine<=3.8.0
-pytest-sftpserver
+confluent-kafka
+pandas>=1.2.4
+sqlparse>=0.4.2
+numpy>=1.19.5
+google-cloud-bigquery>=2.26.0
+boto3
 
 [apache-airflow[google]]
 apache-airflow[google]==2.2.3
 
 [boto]
 boto3
 
@@ -117,16 +117,16 @@
 
 [pandas]
 numpy>=1.19.5
 pandas>=1.2.4
 
 [pg]
 psycopg2-binary==2.9.3
-pglast==v3.4
 sqlparse>=0.4.2
+pglast==v3.4
 
 [pglast]
 pglast==v3.4
 
 [psycopg2-binary]
 psycopg2-binary==2.9.3
 
@@ -148,21 +148,21 @@
 [scikit-learn]
 scikit-learn>=0.24.2
 
 [sdk]
 packaging
 
 [sklearn]
-scikit-learn>=0.24.2
 numpy>=1.19.5
+scikit-learn>=0.24.2
 
 [sqlparse ]
 sqlparse>=0.4.2
 
 [test]
-pytest>=6.2.4
 pytest-sftpserver
 pytest-vcr
+pytest>=6.2.4
 pytest-mock
 
 [twine]
 twine<=3.8.0
```

### Comparing `kensu-2.5.5/setup.py` & `kensu-2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 NAME = "kensu"
 
 
 BUILD_FLAVOR = os.environ["BUILD_FLAVOR"] if "BUILD_FLAVOR" in os.environ else ""
 BUILD_NUMBER = os.environ["BUILD_NUMBER"] if "BUILD_NUMBER" in os.environ else ""
 # https://semver.org/
-VERSION = "2.5.5" + BUILD_FLAVOR + BUILD_NUMBER
+VERSION = "2.6.2" + BUILD_FLAVOR + BUILD_NUMBER
+
 
 
 
 # To install the library, run the following
 #
 # python setup.py install
 #
```


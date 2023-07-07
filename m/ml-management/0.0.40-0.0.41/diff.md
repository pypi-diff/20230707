# Comparing `tmp/ml-management-0.0.40.tar.gz` & `tmp/ml-management-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.40.tar", last modified: Thu Jun 29 11:20:50 2023, max compression
+gzip compressed data, was "ml-management-0.0.41.tar", last modified: Fri Jul  7 06:26:59 2023, max compression
```

## Comparing `ml-management-0.0.40.tar` & `ml-management-0.0.41.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/
--rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-05-30 08:20:16.000000 ml-management-0.0.40/MANIFEST.in
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.502761 ml-management-0.0.40/ML_management/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-08 12:48:25.000000 ml-management-0.0.40/ML_management/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.502761 ml-management-0.0.40/ML_management/collectors/
--rw-rw-r--   0 denis     (1000) denis     (1000)      120 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1092 2023-06-05 06:12:04.000000 ml-management-0.0.40/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      456 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1318 2023-06-08 08:02:27.000000 ml-management-0.0.40/ML_management/collectors/collectors.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.502761 ml-management-0.0.40/ML_management/collectors/dummy/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      463 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.502761 ml-management-0.0.40/ML_management/collectors/s3/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    10609 2023-06-21 07:06:27.000000 ml-management-0.0.40/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/collectors/topic_markers/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)   331440 2023-06-05 06:12:04.000000 ml-management-0.0.40/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3167 2023-06-05 06:12:04.000000 ml-management-0.0.40/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/dataset_loader_template/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2407 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/executor_template/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/executor_template/default_executors/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      895 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      843 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      869 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4566 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      402 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      334 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/mlmanagement/
--rw-rw-r--   0 denis     (1000) denis     (1000)      737 2023-06-29 10:47:21.000000 ml-management-0.0.40/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3392 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5054 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    14229 2023-06-29 10:47:21.000000 ml-management-0.0.40/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    10260 2023-06-26 13:36:25.000000 ml-management-0.0.40/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      201 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5001 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      316 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/models/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      949 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/models/patterns/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4202 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      561 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      445 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/registry/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/registry/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2566 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/registry/exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     7556 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/tests/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/tests/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3361 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     9275 2023-06-21 07:06:27.000000 ml-management-0.0.40/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/uploader_data/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1694 2023-06-21 07:06:27.000000 ml-management-0.0.40/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      394 2023-06-29 11:20:50.506761 ml-management-0.0.40/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)       56 2023-05-30 08:20:16.000000 ml-management-0.0.40/README.md
--rw-rw-r--   0 denis     (1000) denis     (1000)        7 2023-06-29 11:15:02.000000 ml-management-0.0.40/VERSION
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ml_management.egg-info/
--rw-rw-r--   0 denis     (1000) denis     (1000)      394 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)     2449 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)      153 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/requires.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       14 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-06-29 11:20:50.506761 ml-management-0.0.40/setup.cfg
--rw-rw-r--   0 denis     (1000) denis     (1000)     1052 2023-06-26 13:36:25.000000 ml-management-0.0.40/setup.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       18 2023-07-05 09:14:25.000000 ml-management-0.0.41/MANIFEST.in
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/__init__.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/collectors/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      120 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1092 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      456 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1318 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/collectors.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/collectors/dummy/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      463 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/collectors/s3/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     9711 2023-07-06 08:06:30.000000 ml-management-0.0.41/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.949116 ml-management-0.0.41/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)   331440 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3167 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.953116 ml-management-0.0.41/ML_management/dataset_loader_template/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2407 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      457 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.953116 ml-management-0.0.41/ML_management/executor_template/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.953116 ml-management-0.0.41/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      895 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      843 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      869 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     4566 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      402 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      334 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/mlmanagement/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      737 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3392 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     5054 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    14229 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    10260 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      201 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     5001 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      316 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/models/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      949 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/models/patterns/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     4202 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      561 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      445 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      457 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/registry/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/registry/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2566 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/registry/exceptions.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     7556 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/tests/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/tests/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3361 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     9858 2023-07-05 16:21:11.000000 ml-management-0.0.41/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ML_management/uploader_data/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-07-05 09:14:25.000000 ml-management-0.0.41/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1914 2023-07-05 16:21:11.000000 ml-management-0.0.41/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1430 2023-07-05 16:21:11.000000 ml-management-0.0.41/ML_management/uploader_data/utils.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      312 2023-07-07 06:26:59.957116 ml-management-0.0.41/PKG-INFO
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       56 2023-07-05 09:14:25.000000 ml-management-0.0.41/README.md
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        6 2023-07-07 06:25:31.000000 ml-management-0.0.41/VERSION
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-07-07 06:26:59.957116 ml-management-0.0.41/ml_management.egg-info/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      312 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2486 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        1 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      166 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       14 2023-07-07 06:26:59.000000 ml-management-0.0.41/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       38 2023-07-07 06:26:59.957116 ml-management-0.0.41/setup.cfg
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1076 2023-07-05 16:21:11.000000 ml-management-0.0.41/setup.py
```

### Comparing `ml-management-0.0.40/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.41/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/collectors/collectors.py` & `ml-management-0.0.41/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.41/ML_management/collectors/s3/s3collector.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import posixpath
 from typing import List, Optional, Union
 
 from boto3 import client
 from botocore.exceptions import ClientError
 from ML_management.collectors.collector_pattern import CollectorPattern
+from tqdm import tqdm
 
 
 class S3FolderNotFound(Exception):
     """Define Version Not Found Exception."""
 
     def __init__(self, path: str, bucket: str):
         self.path = path
@@ -81,79 +82,30 @@
                 "aws_secret_access_key": {"type": "string"},
                 "aws_session_token": {"type": "string"},
             },
             "required": ["bucket"],
             "additionalProperties": False,
         }
 
-    def _download_file(self, bucket: str, service_client, remote_file_path: str, local_path: str):
-        dirpath = posixpath.dirname(remote_file_path)
-        local_dir_path = os.path.join(local_path, dirpath)
-        local_file_path = os.path.join(local_path, remote_file_path)
-        if not os.path.exists(local_dir_path):
-            os.makedirs(local_dir_path, exist_ok=True)
-        try:
-            with open(local_file_path, "wb") as _file:
-                service_client.download_fileobj(bucket, remote_file_path, _file)
-        except ClientError as err:
-            if err.response["Error"]["Code"] == "404":
-                # maybe user forgot to add trailing slash? Try to download as folder
-                try:
-                    remote_folder_path = remote_file_path + "/"
-                    self._download_folder(bucket, service_client, remote_folder_path, local_path)
-                except S3FolderNotFound:
-                    try:
-                        # maybe, bad bucket?
-                        service_client.head_bucket(Bucket=bucket)
-                    except ClientError as err:
-                        if err.response["Error"]["Code"] == "404":
-                            # bad bucket it is.
-                            raise S3BucketNotFound(bucket=bucket)
-                        else:
-                            raise err
-                    # bucket is ok, it is a bad object
-                    raise S3ObjectNotFound(path=remote_file_path, bucket=bucket)  # attempt of search as a folder failed
-            else:
-                raise err
-        return local_file_path
-
-    def _download_folder(self, bucket, service_client, folder_path, local_path):
-        paginator = service_client.get_paginator("list_objects_v2")
-        # TODO prevent infinite loop, sometimes the dir is recursively included ???
-        try:
-            page_iterator = paginator.paginate(Bucket=bucket, Prefix=folder_path)
-            for page in page_iterator:
-                if page["KeyCount"] == 0:
-                    # folder not found or is empty?
-                    raise S3FolderNotFound(path=folder_path, bucket=bucket)
-                # Objects listed directly will be files
-                for obj in page.get("Contents", []):
-                    file_path = obj.get("Key")
-                    self._download_file(bucket, service_client, file_path, local_path)
-        except ClientError as err:
-            if err.response["Error"]["Code"] == "NoSuchBucket":
-                raise S3BucketNotFound(bucket=bucket)
-            else:
-                raise err
-
     def set_data(
         self,
         *,
-        local_path: str = "/s3_data/",
+        local_path: str = "s3_data",
         bucket: str,  # TODO do we pass bucket or not? is it always possible to parse?
         remote_paths: Optional[List[str]] = None,
         service_name: str = "s3",
         region_name: Optional[str] = None,
         api_version: Optional[str] = None,
         use_ssl: bool = True,
         verify: Optional[Union[bool, str]] = None,
         endpoint_url: Optional[str] = None,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
+        verbose: bool = True,
     ) -> str:
         """
         Set data.
 
         :type local_path: string
         :param local_path: Local path to save data to.  Defaults to /s3_data/.
 
@@ -213,32 +165,81 @@
         :type aws_secret_access_key: string
         :param aws_secret_access_key: The secret key to use when creating
             the client.  Same semantics as aws_access_key_id above.
 
         :type aws_session_token: string
         :param aws_session_token: The session token to use when creating
             the client.  Same semantics as aws_access_key_id above.
+
+        :type verbose: bool
+        :param verbose: Whether to disable the entire progressbar wrapper.
         """
         service_client = client(
             service_name=service_name,
             region_name=region_name,
             api_version=api_version,
             use_ssl=use_ssl,
             verify=verify,
             endpoint_url=endpoint_url if endpoint_url else self.default_url,
             aws_access_key_id=aws_access_key_id if aws_access_key_id else self.default_access_key_id,
             aws_secret_access_key=aws_secret_access_key if aws_secret_access_key else self.default_secret_access_key,
             aws_session_token=aws_session_token,
         )
-        if remote_paths is not None:
-            for path in remote_paths:
-                if path.endswith("/"):
-                    # it is a folder
-                    # list all files in a folder in one go and download them all!
-                    self._download_folder(bucket, service_client, path, local_path)
-                else:
-                    # it is a file
-                    self._download_file(bucket, service_client, path, local_path)
-        else:
-            for key in service_client.list_objects(Bucket=bucket)["Contents"]:
-                self._download_file(bucket, service_client, key["Key"], local_path)
+
+        def compute_space(paginator, remote_path: str = ""):
+            space_size = 0
+
+            page_iterator = paginator.paginate(
+                Bucket=bucket,
+                Prefix=remote_path,
+            )
+            for page in page_iterator:
+                if page["KeyCount"] == 0:
+                    raise S3ObjectNotFound(path=remote_path, bucket=bucket)
+                for obj in page.get("Contents", []):
+                    space_size += obj["Size"]
+
+            return space_size
+
+        remote_paths = remote_paths if remote_paths else [""]
+        data_size = 0
+
+        try:
+            paginator = service_client.get_paginator("list_objects_v2")
+            for remote_path in remote_paths:
+                data_size += compute_space(paginator, remote_path)
+        except ClientError as err:
+            if err.response["Error"]["Code"] == "NoSuchBucket":
+                raise S3BucketNotFound(bucket=bucket)
+            else:
+                raise err
+
+        with tqdm(
+            total=data_size,
+            unit="B",
+            unit_scale=True,
+            unit_divisor=1024,
+            disable=not verbose,
+        ) as pbar:
+            for remote_path in remote_paths:
+                page_iterator = paginator.paginate(
+                    Bucket=bucket,
+                    Prefix=remote_path,
+                )
+                for page in page_iterator:
+                    for obj in page.get("Contents", []):
+                        file_path = obj.get("Key")
+
+                        local_dir_path = os.path.join(local_path, posixpath.dirname(file_path))
+                        local_file_path = os.path.join(local_path, file_path)
+                        if not os.path.exists(local_dir_path):
+                            os.makedirs(local_dir_path, exist_ok=True)
+
+                        with open(local_file_path, "wb") as _file:
+                            service_client.download_fileobj(
+                                Bucket=bucket,
+                                Key=file_path,
+                                Fileobj=_file,
+                                Callback=pbar.update,
+                            )
+
         return local_path
```

### Comparing `ml-management-0.0.40/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.41/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.41/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.41/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.41/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.41/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.41/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.41/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.41/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.41/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.41/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.41/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.41/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.41/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.41/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.41/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.41/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/registry/exceptions.py` & `ml-management-0.0.41/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/registry/registry_manager.py` & `ml-management-0.0.41/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.41/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.40/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.41/ML_management/tests/test_s3_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,38 +9,52 @@
 from ML_management.collectors import COLLECTORS
 from ML_management.collectors.s3.s3collector import S3BucketNotFound, S3FolderNotFound, S3ObjectNotFound
 
 
 def mock_client_download_successful(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
+    class mock_paginator:
+        def paginate(self, *args, **kwargs):
+            return [
+                {
+                    "KeyCount": 3,
+                    "Contents": [
+                        {"Key": "sample_data/1.txt", "Size": 0},
+                        {"Key": "sample_data/2.txt", "Size": 0},
+                        {"Key": "sample_data/sample_folder/3.txt", "Size": 0},
+                    ],
+                }
+            ]
+
     def mock_download_file(Bucket, Key, Fileobj, ExtraArgs=None, Callback=None, Config=None):
         files_content_map = {
             "sample_data/1.txt": "one\n",
             "sample_data/2.txt": "two\n",
             "sample_data/sample_folder/3.txt": "three\n",
         }
         Fileobj.write(files_content_map[Key].encode("utf-8"))
 
     client.download_fileobj = Mock(side_effect=mock_download_file)
+    client.get_paginator = Mock(return_value=mock_paginator())
     return client
 
 
 def mock_client_download_folder_successful(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
     class mock_paginator:
         def paginate(self, *args, **kwargs):
             return [
                 {
                     "KeyCount": 3,
                     "Contents": [
-                        {"Key": "sample_data/1.txt"},
-                        {"Key": "sample_data/2.txt"},
-                        {"Key": "sample_data/sample_folder/3.txt"},
+                        {"Key": "sample_data/1.txt", "Size": 0},
+                        {"Key": "sample_data/2.txt", "Size": 0},
+                        {"Key": "sample_data/sample_folder/3.txt", "Size": 0},
                     ],
                 }
             ]
 
     def mock_download_file(Bucket, Key, Fileobj, ExtraArgs=None, Callback=None, Config=None):
         files_content_map = {
             "sample_data/1.txt": "one\n",
@@ -70,15 +84,14 @@
 
     class mock_paginator:
         def paginate(self, *args, **kwargs):
             return [{"KeyCount": 0}]
 
     client.download_fileobj = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_fileobj"))
     client.get_paginator = Mock(return_value=mock_paginator())
-    client.head_bucket = Mock()
     return client
 
 
 def mock_client_bad_bucket_folder(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
     class mock_paginator:
@@ -95,15 +108,14 @@
 
     class mock_paginator:
         def paginate(self, *args, **kwargs):
             return [{"KeyCount": 0}]
 
     client.download_fileobj = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_fileobj"))
     client.get_paginator = Mock(return_value=mock_paginator())
-    client.head_bucket = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_fileobj"))
     return client
 
 
 class TestS3Dataset(unittest.TestCase):
     """
     Mock S3 structure:
 
@@ -129,14 +141,15 @@
                 "sample_data/1.txt",
                 "sample_data/2.txt",
                 "sample_data/sample_folder/3.txt",
             ],
             endpoint_url=endpoint_url,
             aws_access_key_id="some_mock_key",
             aws_secret_access_key="some_mock_key",
+            verbose=False,
         )
 
         with open(os.path.join(local_path, "sample_data/1.txt"), "r") as f:
             text_one = f.read()
             self.assertEqual(text_one, "one\n")
         with open(os.path.join(local_path, "sample_data/2.txt"), "r") as f:
             text_one = f.read()
@@ -159,14 +172,15 @@
         local_path = s3_dataset.set_data(
             local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
             bucket="test-data",
             remote_paths=["sample_data/"],
             endpoint_url=endpoint_url,
             aws_access_key_id="some_mock_key",
             aws_secret_access_key="some_mock_key",
+            verbose=False,
         )
 
         with open(os.path.join(local_path, "sample_data/1.txt"), "r") as f:
             text_one = f.read()
             self.assertEqual(text_one, "one\n")
         with open(os.path.join(local_path, "sample_data/2.txt"), "r") as f:
             text_one = f.read()
@@ -190,33 +204,35 @@
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="test-data",
                 remote_paths=["sample_data/nosuchfile.txt"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
+                verbose=False,
             )
 
     @patch(
         "ML_management.collectors.s3.s3collector.client",
         new=mock_client_bad_folder,
     )
     def test_download_bad_folder(self):
         s3_dataset = COLLECTORS["s3"]()
         assert mock_client_bad_folder is ML_management.collectors.s3.s3collector.client
         endpoint_url = "some_mock_url"
 
-        with self.assertRaises(S3FolderNotFound):
+        with self.assertRaises(S3ObjectNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="test-data",
                 remote_paths=["sample_data/nosuchfolder/"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
+                verbose=False,
             )
 
     @patch(
         "ML_management.collectors.s3.s3collector.client",
         new=mock_client_bad_bucket_folder,
     )
     def test_download_bad_bucket_folder(self):
@@ -228,31 +244,33 @@
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="nosuchbucket",
                 remote_paths=["sample_data/"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
+                verbose=False,
             )
 
     @patch(
         "ML_management.collectors.s3.s3collector.client",
         new=mock_client_bad_bucket_object,
     )
     def test_download_bad_bucket_object(self):
         s3_dataset = COLLECTORS["s3"]()
         assert mock_client_bad_bucket_object is ML_management.collectors.s3.s3collector.client
         endpoint_url = "some_mock_url"
 
-        with self.assertRaises(S3BucketNotFound):
+        with self.assertRaises(S3ObjectNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="nosuchbucket",
                 remote_paths=["sample_data/1.txt"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
+                verbose=False,
             )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ml-management-0.0.40/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.41/ML_management/uploader_data/s3_uploader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Define S3Uploader class."""
 import os
 
 from boto3 import client
+from ML_management.uploader_data.utils import get_space_size, get_upload_paths
+from tqdm import tqdm
 
 
 class S3Uploader:
     """S3 uploader files class."""
 
     def __init__(self):
         """Init creds."""
         self.default_url = os.environ.get("MLFLOW_S3_ENDPOINT_URL", "http://minio-mlmanagement.ru/")
         self.default_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID", "minioadmin")
         self.default_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY", "minioadmin")
 
-    def upload(self, local_path: str, bucket: str):
+    def upload(self, local_path: str, bucket: str, verbose: bool = True):
         """Upload."""
         local_path = os.path.normpath(local_path)
         if not os.path.exists(local_path):
             raise FileExistsError(f"Path: {local_path} does not exist")
 
         service_client = client(
             service_name="s3",
@@ -27,16 +29,25 @@
             aws_access_key_id=self.default_access_key_id,
             aws_secret_access_key=self.default_secret_access_key,
         )
         buckets = [item["Name"] for item in service_client.list_buckets()["Buckets"]]
         if bucket not in buckets:
             service_client.create_bucket(Bucket=bucket)
 
-        if os.path.isfile(local_path):
-            with open(local_path, "rb") as _file:
-                service_client.upload_fileobj(_file, bucket)
-        else:
-            for root, _, files in os.walk(local_path):
-                for file in files:
-                    filename = file if root == local_path else os.path.join(os.path.relpath(root, start=local_path), file)
-                    with open(os.path.join(root, file), "rb") as _file:
-                        service_client.upload_fileobj(_file, bucket, filename)
+        space_size = get_space_size(local_path)
+        upload_paths = get_upload_paths(local_path)
+
+        with tqdm(
+            total=space_size,
+            disable=not verbose,
+            unit="B",
+            unit_scale=True,
+            unit_divisor=1024,
+        ) as pbar:
+            for path in upload_paths:
+                with open(path.local_path, "rb") as _file:
+                    service_client.upload_fileobj(
+                        Fileobj=_file,
+                        Bucket=bucket,
+                        Key=path.storage_path,
+                        Callback=pbar.update,
+                    )
```

### Comparing `ml-management-0.0.40/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.41/ml_management.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -44,12 +44,13 @@
 ML_management/registry/exceptions.py
 ML_management/registry/registry_manager.py
 ML_management/tests/__init__.py
 ML_management/tests/test_jsonschema_inference.py
 ML_management/tests/test_s3_dataset.py
 ML_management/uploader_data/__init__.py
 ML_management/uploader_data/s3_uploader.py
+ML_management/uploader_data/utils.py
 ml_management.egg-info/PKG-INFO
 ml_management.egg-info/SOURCES.txt
 ml_management.egg-info/dependency_links.txt
 ml_management.egg-info/requires.txt
 ml_management.egg-info/top_level.txt
```

### Comparing `ml-management-0.0.40/setup.py` & `ml-management-0.0.41/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,11 +24,12 @@
         "mlflow==2.4.0",
         "pandas>=0.20.1,<=1.5.2",
         "numpy>=1.8.1,<=1.23.5",
         "jsonschema==2.6.0",
         "requests_toolbelt>=0.9.1,<=0.10.1",
         "boto3==1.21.21",
         "protobuf<4.0.0",
+        "tqdm==4.65.0",
     ],
     data_files=[("", ["VERSION"])],
     python_requires=">=3.8",
 )
```


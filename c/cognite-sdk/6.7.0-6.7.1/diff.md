# Comparing `tmp/cognite_sdk-6.7.0.tar.gz` & `tmp/cognite_sdk-6.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.7.0.tar", max compression
+gzip compressed data, was "cognite_sdk-6.7.1.tar", max compression
```

## Comparing `cognite_sdk-6.7.0.tar` & `cognite_sdk-6.7.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0    11349 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/LICENSE
--rw-r--r--   0        0        0     3945 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/README.md
--rw-r--r--   0        0        0      574 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     7558 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49210 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1317 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     8056 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     9702 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0     3088 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/graphql.py
--rw-r--r--   0        0        0    42810 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6620 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     8221 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11115 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87544 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21384 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17504 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41590 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45636 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    50175 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9619 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6088 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24756 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22919 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    38200 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7936 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    28258 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19276 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    22021 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     5083 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4691 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9705 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1881 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38337 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api_client.py
--rw-r--r--   0        0        0     9688 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/beta.py
--rw-r--r--   0        0        0     5675 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/config.py
--rw-r--r--   0        0        0    22326 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     4207 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0     5154 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/aggregations.py
--rw-r--r--   0        0        0    11348 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7670 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4710 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0      693 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/graphql.py
--rw-r--r--   0        0        0     6968 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    31559 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0    13178 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/query.py
--rw-r--r--   0        0        0     2944 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    15109 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6349 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9968 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/py.typed
--rw-r--r--   0        0        0     9163 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7559 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7748 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2222 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/pyproject.toml
--rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/LICENSE
+-rw-r--r--   0        0        0     3945 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/README.md
+-rw-r--r--   0        0        0      574 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     7558 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49210 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1317 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     8056 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     9702 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0     3088 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/data_modeling/graphql.py
+-rw-r--r--   0        0        0    43356 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6620 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     8845 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11115 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87544 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21384 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17504 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41590 2023-07-07 14:35:56.387971 cognite_sdk-6.7.1/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45636 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    50175 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9619 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6088 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24756 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22919 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    38200 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7936 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    28258 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19276 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    22021 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5083 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4691 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9705 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1881 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38337 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     9688 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/beta.py
+-rw-r--r--   0        0        0     5675 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/config.py
+-rw-r--r--   0        0        0    22326 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     4207 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0     5154 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/aggregations.py
+-rw-r--r--   0        0        0    11348 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7670 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4710 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0      693 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/graphql.py
+-rw-r--r--   0        0        0     6968 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    31559 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0    13178 2023-07-07 14:35:56.391971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/query.py
+-rw-r--r--   0        0        0     2944 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14889 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6349 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9968 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/py.typed
+-rw-r--r--   0        0        0     9163 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7559 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7748 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-07-07 14:35:56.395971 cognite_sdk-6.7.1/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2222 2023-07-07 14:35:56.399971 cognite_sdk-6.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.7.1/PKG-INFO
```

### Comparing `cognite_sdk-6.7.0/LICENSE` & `cognite_sdk-6.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/README.md` & `cognite_sdk-6.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/__init__.py` & `cognite_sdk-6.7.1/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/annotations.py` & `cognite_sdk-6.7.1/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/assets.py` & `cognite_sdk-6.7.1/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.7.1/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.7.1/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.7.1/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/graphql.py` & `cognite_sdk-6.7.1/cognite/client/_api/data_modeling/graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.7.1/cognite/client/_api/data_modeling/instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,21 +292,23 @@
         )
 
     def _load_node_and_edge_ids(
         self,
         nodes: NodeId | Sequence[NodeId] | tuple[str, str] | Sequence[tuple[str, str]] | None,
         edges: EdgeId | Sequence[EdgeId] | tuple[str, str] | Sequence[tuple[str, str]] | None,
     ) -> DataModelingIdentifierSequence:
+        nodes_seq: Sequence[NodeId | tuple[str, str]]
         if isinstance(nodes, NodeId) or (isinstance(nodes, tuple) and isinstance(nodes[0], str)):
-            nodes_seq: Sequence[NodeId | tuple[str, str]] = [nodes]  # type: ignore[list-item]
+            nodes_seq = [nodes]  # type: ignore[list-item]
         else:
             nodes_seq = nodes  # type: ignore[assignment]
 
+        edges_seq: Sequence[EdgeId | tuple[str, str]]
         if isinstance(edges, EdgeId) or (isinstance(edges, tuple) and isinstance(edges[0], str)):
-            edges_seq: Sequence[EdgeId | tuple[str, str]] = [edges]  # type: ignore[list-item]
+            edges_seq = [edges]  # type: ignore[list-item]
         else:
             edges_seq = edges  # type: ignore[assignment]
 
         identifiers = []
         if nodes_seq:
             node_ids = _load_identifier(nodes_seq, "node")
             identifiers.extend(node_ids._identifiers)
@@ -332,22 +334,31 @@
 
         Examples:
 
             Delete instances by id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
-                >>> c.data_modeling.instances.delete(nodes=("myNode", "mySpace"))
+                >>> c.data_modeling.instances.delete(nodes=("mySpace", "myNode"))
 
             Delete nodes and edges using the built in data class
 
                 >>> from cognite.client import CogniteClient
                 >>> from cognite.client.data_classes.data_modeling import NodeId, EdgeId
                 >>> c = CogniteClient()
                 >>> c.data_modeling.instances.delete(NodeId('mySpace', 'myNode'), EdgeId('mySpace', 'myEdge'))
+
+            Delete all nodes from a NodeList
+
+                >>> from cognite.client import CogniteClient
+                >>> from cognite.client.data_classes.data_modeling import NodeId, EdgeId
+                >>> c = CogniteClient()
+                >>> my_view = c.data_modeling.views.retrieve('mySpace', 'myView')
+                >>> my_nodes = c.data_modeling.instances.list(instance_type='node', sources=my_view, limit=None)
+                >>> c.data_modeling.instances.delete(nodes=my_nodes.as_ids())
         """
         identifiers = self._load_node_and_edge_ids(nodes, edges)
         deleted_instances = cast(List, self._delete_multiple(identifiers, wrap_ids=True, returns_items=True))
         node_ids = [NodeId.load(item) for item in deleted_instances if item["instanceType"] == "node"]
         edge_ids = [EdgeId.load(item) for item in deleted_instances if item["instanceType"] == "edge"]
         return InstancesDeleteResult(node_ids, edge_ids)
```

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.7.1/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.7.1/cognite/client/_api/data_modeling/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from collections import defaultdict
 from typing import Iterator, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.ids import (
     ViewId,
     ViewIdentifier,
@@ -78,44 +79,56 @@
         """Iterate over views
 
         Fetches views as they are iterated over, so you keep a limited number of views in memory.
 
         Yields:
             View: yields Views one by one.
         """
-        return cast(Iterator[View], self())
+        return self()
+
+    def _get_latest_views(self, views: ViewList) -> ViewList:
+        views_by_space_and_xid = defaultdict(list)
+        for view in views:
+            views_by_space_and_xid[(view.space, view.external_id)].append(view)
+        return ViewList([max(views, key=lambda view: view.created_time) for views in views_by_space_and_xid.values()])
 
     def retrieve(
         self,
         ids: ViewIdentifier | Sequence[ViewIdentifier],
         include_inherited_properties: bool = True,
+        all_versions: bool = True,
     ) -> ViewList:
         """`Retrieve a single view by id. <https://developer.cognite.com/api#tag/Views/operation/byExternalIdsViews>`_
 
         Args:
-            ids (ViewId | Sequence[ViewId]): View dentifier(s)
+            ids (ViewId | Sequence[ViewId]): View identifier(s)
             include_inherited_properties (bool): Whether to include properties inherited from views this view implements.
+            all_versions (bool): Whether to return all versions. If false, only the newest version is returned,
 
         Returns:
             Optional[View]: Requested view or None if it does not exist.
 
         Examples:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.views.retrieve(('mySpace', 'myView', 'v1'))
 
         """
         identifier = _load_identifier(ids, "view")
-        return self._retrieve_multiple(
+        views = self._retrieve_multiple(
             list_cls=ViewList,
             resource_cls=View,
             identifiers=identifier,
             params={"includeInheritedProperties": include_inherited_properties},
         )
+        if all_versions is True:
+            return views
+        else:
+            return self._get_latest_views(views)
 
     def delete(self, ids: ViewIdentifier | Sequence[ViewIdentifier]) -> list[ViewId]:
         """`Delete one or more views <https://developer.cognite.com/api#tag/Views/operation/deleteViews>`_
 
         Args:
             ids (ViewId | Sequence[ViewId]): View dentifier(s)
         Returns:
```

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/data_sets.py` & `cognite_sdk-6.7.1/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.7.1/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/datapoints.py` & `cognite_sdk-6.7.1/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/diagrams.py` & `cognite_sdk-6.7.1/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.7.1/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/events.py` & `cognite_sdk-6.7.1/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.7.1/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/files.py` & `cognite_sdk-6.7.1/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/functions.py` & `cognite_sdk-6.7.1/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/geospatial.py` & `cognite_sdk-6.7.1/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/iam.py` & `cognite_sdk-6.7.1/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/labels.py` & `cognite_sdk-6.7.1/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/raw.py` & `cognite_sdk-6.7.1/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/relationships.py` & `cognite_sdk-6.7.1/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/sequences.py` & `cognite_sdk-6.7.1/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.7.1/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/templates.py` & `cognite_sdk-6.7.1/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/three_d.py` & `cognite_sdk-6.7.1/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/time_series.py` & `cognite_sdk-6.7.1/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.7.1/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.7.1/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.7.1/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.7.1/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.7.1/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api/vision.py` & `cognite_sdk-6.7.1/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_api_client.py` & `cognite_sdk-6.7.1/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_cognite_client.py` & `cognite_sdk-6.7.1/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_http_client.py` & `cognite_sdk-6.7.1/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.7.1/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.7.1/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.7.1/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.7.1/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.7.1/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.7.1/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.7.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.7.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.7.1/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.7.1/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/config.py` & `cognite_sdk-6.7.1/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/credentials.py` & `cognite_sdk-6.7.1/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/_base.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/assets.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/aggregations.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/aggregations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/graphql.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/query.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/query.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_modeling/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,22 +200,14 @@
             description=self.description,
             name=self.name,
             filter=self.filter,
             implements=self.implements,
             properties=properties,
         )
 
-    def as_id(self) -> ViewId:
-        """Convert to a view id.
-
-        Returns:
-            ViewId: The view id.
-        """
-        return ViewId(space=self.space, external_id=self.external_id, version=self.version)
-
 
 class ViewList(CogniteResourceList[View]):
     _RESOURCE = View
 
     def to_view_apply(self) -> ViewApplyList:
         """Convert to a view an apply list.
```

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/events.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/files.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/functions.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/iam.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/labels.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/raw.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/shared.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/templates.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.7.1/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/exceptions.py` & `cognite_sdk-6.7.1/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/testing.py` & `cognite_sdk-6.7.1/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/__init__.py` & `cognite_sdk-6.7.1/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.7.1/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.7.1/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_graph.py` & `cognite_sdk-6.7.1/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_identifier.py` & `cognite_sdk-6.7.1/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_logging.py` & `cognite_sdk-6.7.1/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.7.1/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.7.1/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.7.1/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_text.py` & `cognite_sdk-6.7.1/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_time.py` & `cognite_sdk-6.7.1/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_validation.py` & `cognite_sdk-6.7.1/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.7.1/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.7.0/pyproject.toml` & `cognite_sdk-6.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.7.0"
+version = "6.7.1"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.7.0/PKG-INFO` & `cognite_sdk-6.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.7.0
+Version: 6.7.1
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.7.0 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.7.1 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```


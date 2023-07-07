# Comparing `tmp/cognite_sdk-6.6.1.tar.gz` & `tmp/cognite_sdk-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.6.1.tar", max compression
+gzip compressed data, was "cognite_sdk-6.7.0.tar", max compression
```

## Comparing `cognite_sdk-6.6.1.tar` & `cognite_sdk-6.7.0.tar`

### file list

```diff
@@ -1,116 +1,118 @@
--rw-r--r--   0        0        0    11349 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/LICENSE
--rw-r--r--   0        0        0     3945 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/README.md
--rw-r--r--   0        0        0      574 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     7558 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49210 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     8056 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     9702 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    42810 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6620 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     8221 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11115 2023-07-07 13:16:37.673561 cognite_sdk-6.6.1/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87544 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21384 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17504 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41590 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45636 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    50175 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9619 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6088 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24756 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22919 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    38200 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7936 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    28258 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19276 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    22021 2023-07-07 13:16:37.677561 cognite_sdk-6.6.1/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     5083 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4691 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9705 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1881 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38337 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_api_client.py
--rw-r--r--   0        0        0     9688 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/beta.py
--rw-r--r--   0        0        0     5675 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/config.py
--rw-r--r--   0        0        0    22326 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     4207 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0     5154 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/aggregations.py
--rw-r--r--   0        0        0    11348 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7670 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4710 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     6968 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    31559 2023-07-07 13:16:37.681561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0    13178 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/query.py
--rw-r--r--   0        0        0     2944 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    15109 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6349 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7559 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7748 2023-07-07 13:16:37.685561 cognite_sdk-6.6.1/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2222 2023-07-07 13:16:37.689561 cognite_sdk-6.6.1/pyproject.toml
--rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/LICENSE
+-rw-r--r--   0        0        0     3945 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/README.md
+-rw-r--r--   0        0        0      574 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     7558 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49210 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1317 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     8056 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     9702 2023-07-07 14:31:14.097038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0     3088 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/graphql.py
+-rw-r--r--   0        0        0    42810 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6620 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     8221 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11115 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87544 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21384 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17504 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41590 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45636 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    50175 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9619 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6088 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24756 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22919 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    38200 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7936 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    28258 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19276 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    22021 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5083 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4691 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9705 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1881 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38337 2023-07-07 14:31:14.101038 cognite_sdk-6.7.0/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     9688 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/beta.py
+-rw-r--r--   0        0        0     5675 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/config.py
+-rw-r--r--   0        0        0    22326 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     4207 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0     5154 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/aggregations.py
+-rw-r--r--   0        0        0    11348 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7670 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4710 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0      693 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/graphql.py
+-rw-r--r--   0        0        0     6968 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    31559 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0    13178 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/query.py
+-rw-r--r--   0        0        0     2944 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    15109 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6349 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-07-07 14:31:14.105038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9968 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/py.typed
+-rw-r--r--   0        0        0     9163 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7559 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7748 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2222 2023-07-07 14:31:14.109038 cognite_sdk-6.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.7.0/PKG-INFO
```

### Comparing `cognite_sdk-6.6.1/LICENSE` & `cognite_sdk-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/README.md` & `cognite_sdk-6.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/__init__.py` & `cognite_sdk-6.7.0/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/annotations.py` & `cognite_sdk-6.7.0/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/assets.py` & `cognite_sdk-6.7.0/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
 from cognite.client._api.data_modeling.containers import ContainersAPI
 from cognite.client._api.data_modeling.data_models import DataModelsAPI
+from cognite.client._api.data_modeling.graphql import DataModelingGraphQLAPI
 from cognite.client._api.data_modeling.instances import InstancesAPI
 from cognite.client._api.data_modeling.spaces import SpacesAPI
 from cognite.client._api.data_modeling.views import ViewsAPI
 from cognite.client._api_client import APIClient
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
@@ -18,7 +19,8 @@
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self.containers = ContainersAPI(config, api_version, cognite_client)
         self.data_models = DataModelsAPI(config, api_version, cognite_client)
         self.spaces = SpacesAPI(config, api_version, cognite_client)
         self.views = ViewsAPI(config, api_version, cognite_client)
         self.instances = InstancesAPI(config, api_version, cognite_client)
+        self.graphql = DataModelingGraphQLAPI(config, api_version, cognite_client)
```

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.7.0/cognite/client/_api/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/data_sets.py` & `cognite_sdk-6.7.0/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.7.0/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/datapoints.py` & `cognite_sdk-6.7.0/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/diagrams.py` & `cognite_sdk-6.7.0/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.7.0/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/events.py` & `cognite_sdk-6.7.0/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.7.0/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/files.py` & `cognite_sdk-6.7.0/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/functions.py` & `cognite_sdk-6.7.0/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/geospatial.py` & `cognite_sdk-6.7.0/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/iam.py` & `cognite_sdk-6.7.0/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/labels.py` & `cognite_sdk-6.7.0/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/raw.py` & `cognite_sdk-6.7.0/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/relationships.py` & `cognite_sdk-6.7.0/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/sequences.py` & `cognite_sdk-6.7.0/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.7.0/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/templates.py` & `cognite_sdk-6.7.0/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/three_d.py` & `cognite_sdk-6.7.0/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/time_series.py` & `cognite_sdk-6.7.0/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.7.0/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.7.0/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.7.0/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.7.0/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.7.0/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api/vision.py` & `cognite_sdk-6.7.0/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_api_client.py` & `cognite_sdk-6.7.0/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_cognite_client.py` & `cognite_sdk-6.7.0/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_http_client.py` & `cognite_sdk-6.7.0/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.7.0/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.7.0/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.7.0/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.7.0/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.7.0/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/config.py` & `cognite_sdk-6.7.0/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/credentials.py` & `cognite_sdk-6.7.0/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/_base.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/assets.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/aggregations.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/aggregations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/query.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/query.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/events.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/files.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/functions.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/iam.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/labels.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/raw.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/shared.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/templates.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.7.0/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/exceptions.py` & `cognite_sdk-6.7.0/cognite/client/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 from __future__ import annotations
 
 import json
 import reprlib
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Sequence
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Sequence
 
 if TYPE_CHECKING:
     from cognite.client.data_classes import AssetHierarchy
 
 
 class CogniteException(Exception):
     pass
 
 
+@dataclass
+class GraphQLErrorSpec:
+    message: str
+    locations: Optional[list[dict[str, int]]]
+
+    def __repr__(self) -> str:
+        return f"GraphQLErrorSpec(message={self.message}, locations={self.locations}"
+
+    @classmethod
+    def load(cls, data: Dict[str, Any]) -> GraphQLErrorSpec:
+        return cls(
+            message=data["message"],
+            locations=data.get("locations"),
+        )
+
+
+class CogniteGraphQLError(CogniteException):
+    def __init__(self, errors: list[GraphQLErrorSpec]):
+        self.errors = errors
+
+
 class CogniteConnectionError(CogniteException):
     pass
 
 
 class CogniteConnectionRefused(CogniteConnectionError):
     def __str__(self) -> str:
         return "Cognite API connection refused. Please try again later."
```

### Comparing `cognite_sdk-6.6.1/cognite/client/testing.py` & `cognite_sdk-6.7.0/cognite/client/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from cognite.client import CogniteClient
 from cognite.client._api.annotations import AnnotationsAPI
 from cognite.client._api.assets import AssetsAPI
 from cognite.client._api.data_modeling import DataModelingAPI
 from cognite.client._api.data_modeling.containers import ContainersAPI
 from cognite.client._api.data_modeling.data_models import DataModelsAPI
+from cognite.client._api.data_modeling.graphql import DataModelingGraphQLAPI
 from cognite.client._api.data_modeling.instances import InstancesAPI
 from cognite.client._api.data_modeling.spaces import SpacesAPI
 from cognite.client._api.data_modeling.views import ViewsAPI
 from cognite.client._api.data_sets import DataSetsAPI
 from cognite.client._api.datapoints import DatapointsAPI
 from cognite.client._api.diagrams import DiagramsAPI
 from cognite.client._api.entity_matching import EntityMatchingAPI
@@ -79,14 +80,15 @@
 
         self.data_modeling = MagicMock(spec=DataModelingAPI)
         self.data_modeling.containers = MagicMock(spec_set=ContainersAPI)
         self.data_modeling.data_models = MagicMock(spec_set=DataModelsAPI)
         self.data_modeling.spaces = MagicMock(spec_set=SpacesAPI)
         self.data_modeling.views = MagicMock(spec_set=ViewsAPI)
         self.data_modeling.instances = MagicMock(spec_set=InstancesAPI)
+        self.data_modeling.graphql = MagicMock(spec_set=DataModelingGraphQLAPI)
 
         self.data_sets = MagicMock(spec_set=DataSetsAPI)
 
         self.diagrams = MagicMock(spec_set=DiagramsAPI)
         self.entity_matching = MagicMock(spec_set=EntityMatchingAPI)
         self.events = MagicMock(spec_set=EventsAPI)
```

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/__init__.py` & `cognite_sdk-6.7.0/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.7.0/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.7.0/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_graph.py` & `cognite_sdk-6.7.0/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_identifier.py` & `cognite_sdk-6.7.0/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_logging.py` & `cognite_sdk-6.7.0/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.7.0/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.7.0/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.7.0/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_text.py` & `cognite_sdk-6.7.0/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_time.py` & `cognite_sdk-6.7.0/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_validation.py` & `cognite_sdk-6.7.0/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.7.0/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.6.1/pyproject.toml` & `cognite_sdk-6.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.6.1"
+version = "6.7.0"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.6.1/PKG-INFO` & `cognite_sdk-6.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.6.1
+Version: 6.7.0
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
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.6.1 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.7.0 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```


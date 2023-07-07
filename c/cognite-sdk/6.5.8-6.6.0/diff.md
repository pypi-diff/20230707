# Comparing `tmp/cognite_sdk-6.5.8.tar.gz` & `tmp/cognite_sdk-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.5.8.tar", max compression
+gzip compressed data, was "cognite_sdk-6.6.0.tar", max compression
```

## Comparing `cognite_sdk-6.5.8.tar` & `cognite_sdk-6.6.0.tar`

### file list

```diff
@@ -1,115 +1,116 @@
--rw-r--r--   0        0        0    11349 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/README.md
--rw-r--r--   0        0        0      574 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     7558 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49210 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     8056 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     9702 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    37850 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6620 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     8221 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11115 2023-06-30 10:47:20.239304 cognite_sdk-6.5.8/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87544 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21384 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17504 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41590 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45636 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    50175 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9619 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6088 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24756 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22919 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    38200 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7936 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    28258 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19276 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    22021 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     5083 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4691 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9705 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1881 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38337 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/beta.py
--rw-r--r--   0        0        0     4631 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-06-30 10:47:20.243304 cognite_sdk-6.5.8/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     4087 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0     5154 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/aggregations.py
--rw-r--r--   0        0        0    11348 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7670 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4710 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     6968 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    30913 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0     2944 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    15109 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6349 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7559 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7748 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-30 10:47:20.247304 cognite_sdk-6.5.8/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-30 10:47:20.251304 cognite_sdk-6.5.8/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/LICENSE
+-rw-r--r--   0        0        0     3945 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/README.md
+-rw-r--r--   0        0        0      574 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     7558 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49210 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     8056 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     9702 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    42810 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6620 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     8221 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11115 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87544 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21384 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17504 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41590 2023-07-06 15:18:32.421450 cognite_sdk-6.6.0/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45636 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    50175 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9619 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6088 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24756 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22919 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    38200 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7936 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    28258 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19276 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    22021 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5083 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4691 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9705 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1881 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38337 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/beta.py
+-rw-r--r--   0        0        0     4631 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     4207 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0     5154 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/aggregations.py
+-rw-r--r--   0        0        0    11348 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7670 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4710 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     6968 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    31559 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0    13178 2023-07-06 15:18:32.425450 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/query.py
+-rw-r--r--   0        0        0     2944 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    15109 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6349 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7559 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7748 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-07-06 15:18:32.429451 cognite_sdk-6.6.0/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2222 2023-07-06 15:18:32.433451 cognite_sdk-6.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.6.0/PKG-INFO
```

### Comparing `cognite_sdk-6.5.8/LICENSE` & `cognite_sdk-6.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/README.md` & `cognite_sdk-6.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/__init__.py` & `cognite_sdk-6.6.0/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/annotations.py` & `cognite_sdk-6.6.0/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/assets.py` & `cognite_sdk-6.6.0/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.6.0/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.6.0/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.6.0/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.6.0/cognite/client/_api/data_modeling/instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     InstancesResult,
     Node,
     NodeApply,
     NodeApplyResult,
     NodeApplyResultList,
     NodeList,
 )
+from cognite.client.data_classes.data_modeling.query import (
+    Query,
+    QueryResult,
+)
 from cognite.client.data_classes.data_modeling.views import View
 from cognite.client.utils._identifier import DataModelingIdentifierSequence
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
 
 
@@ -729,14 +733,105 @@
 
         res = self._post(url_path=self._RESOURCE_PATH + "/aggregate", json=body)
         if is_singleton:
             return HistogramValue.load(res.json()["items"][0]["aggregates"][0])
         else:
             return [HistogramValue.load(item["aggregates"][0]) for item in res.json()["items"]]
 
+    def query(self, query: Query) -> QueryResult:
+        """`Advanced query interface for nodes/edges. <https://developer.cognite.com/api/v1/#tag/Instances/operation/queryContent>`_
+
+        The Data Modelling API exposes an advanced query interface. The query interface supports parameterization,
+        recursive edge traversal, chaining of result sets, and granular property selection.
+
+        Args:
+            query: Query.
+
+        Returns:
+            QueryResult: The resulting nodes and/or edges from the query.
+
+        Examples:
+
+            Find actors in movies released before 2000 sorted by actor name:
+
+                >>> from cognite.client import CogniteClient
+                >>> from cognite.client.data_classes.data_modeling.query import Query, Select, NodeResultSetExpression, EdgeResultSetExpression, SourceSelector
+                >>> from cognite.client.data_classes.data_modeling.filters import Range, Equals
+                >>> from cognite.client.data_classes.data_modeling.ids import ViewId
+                >>> c = CogniteClient()
+                >>> movie_id = ViewId("mySpace", "MovieView", "v1")
+                >>> actor_id = ViewId("mySpace", "ActorView", "v1")
+                >>> query = Query(
+                ...         with_ = {
+                ...             "movies": NodeResultSetExpression(filter=Range(movie_id.as_property_ref("releaseYear"), lt=2000)),
+                ...             "actors_in_movie": EdgeResultSetExpression(from_="movies", filter=Equals(["edge", "type"], {"space": movie_id.space, "externalId": "Movie.actors"})),
+                ...             "actors": NodeResultSetExpression(from_="actors_in_movie"),
+                ...         },
+                ...         select = {
+                ...             "actors": Select(
+                ...                            [SourceSelector(actor_id, ["name"])], sort=[actor_id.as_property_ref("name")]),
+                ...         },
+                ... )
+                >>> res = c.data_modeling.instances.query(query)
+        """
+        return self._query_or_sync(query, "query")
+
+    def sync(self, query: Query) -> QueryResult:
+        """`Subscription to changes for nodes/edges. <https://developer.cognite.com/api/v1/#tag/Instances/operation/syncContent>`_
+
+        Subscribe to changes for nodes and edges in a project, matching a supplied filter.
+
+        Args:
+            query: Query.
+
+        Returns:
+            QueryResult: The resulting nodes and/or edges from the query.
+
+        Examples:
+
+            Find actors in movies released before 2000 sorted by actor name:
+
+                >>> from cognite.client import CogniteClient
+                >>> from cognite.client.data_classes.data_modeling.query import Query, Select, NodeResultSetExpression, EdgeResultSetExpression, SourceSelector
+                >>> from cognite.client.data_classes.data_modeling.filters import Range, Equals
+                >>> from cognite.client.data_classes.data_modeling.ids import ViewId
+                >>> c = CogniteClient()
+                >>> movie_id = ViewId("mySpace", "MovieView", "v1")
+                >>> actor_id = ViewId("mySpace", "ActorView", "v1")
+                >>> query = Query(
+                ...         with_ = {
+                ...             "movies": NodeResultSetExpression(filter=Range(movie_id.as_property_ref("releaseYear"), lt=2000)),
+                ...             "actors_in_movie": EdgeResultSetExpression(from_="movies", filter=Equals(["edge", "type"], {"space": movie_id.space, "externalId": "Movie.actors"})),
+                ...             "actors": NodeResultSetExpression(from_="actors_in_movie"),
+                ...         },
+                ...         select = {
+                ...             "actors": Select(
+                ...                            [SourceSelector(actor_id, ["name"])], sort=[actor_id.as_property_ref("name")]),
+                ...         },
+                ... )
+                >>> res = c.data_modeling.instances.sync(query)
+                >>> # Added a new movie with actors released before 2000
+                >>> query.cursors = res.cursors
+                >>> res_new = c.data_modeling.instances.sync(query)
+
+            In the last example, the res_new will only contain the actors that have been added with the new movie.
+        """
+        return self._query_or_sync(query, "sync")
+
+    def _query_or_sync(self, query: Query, endpoint: Literal["query", "sync"]) -> QueryResult:
+        body = query.dump(camel_case=True)
+
+        result = self._post(url_path=self._RESOURCE_PATH + f"/{endpoint}", json=body)
+
+        json_payload = result.json()
+        default_by_reference = query.instance_type_by_result_expression()
+        results = QueryResult.load(json_payload["items"], default_by_reference, json_payload["nextCursor"])
+
+        return results
+
     @overload
     def list(
         self,
         instance_type: Literal["node"] = "node",
         include_typing: bool = False,
         sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
```

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.6.0/cognite/client/_api/data_modeling/spaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         self,
         limit: int = LIST_LIMIT_DEFAULT,
         include_global: bool = False,
     ) -> SpaceList:
         """`List spaces <https://developer.cognite.com/api#tag/Spaces/operation/listSpacesV3>`_
 
         Args:
-            limit (int, optional): Maximum number of spaces to return. Defaults to 25. Set to -1, float("inf") or None
+            limit (int, optional): Maximum number of spaces to return. Defaults to 10. Set to -1, float("inf") or None
                 to return all items.
             include_global (bool, optional): Whether to include global spaces. Defaults to False.
 
         Returns:
             SpaceList: List of requested spaces
 
         Examples:
```

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.6.0/cognite/client/_api/data_modeling/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         include_inherited_properties: bool = True,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> ViewList:
         """`List views <https://developer.cognite.com/api#tag/Views/operation/listViews>`_
 
         Args:
-            limit (int, optional): Maximum number of views to return. Defaults to 25. Set to -1, float("inf") or None
+            limit (int, optional): Maximum number of views to return. Defaults to 10. Set to -1, float("inf") or None
                 to return all items.
             space: (str | None): The space to query.
             include_inherited_properties (bool): Whether to include properties inherited from views this view implements.
             all_versions (bool): Whether to return all versions. If false, only the newest version is returned,
                                  which is determined based on the 'createdTime' field.
             include_global (bool): Whether to include global views.
```

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/data_sets.py` & `cognite_sdk-6.6.0/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.6.0/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/datapoints.py` & `cognite_sdk-6.6.0/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/diagrams.py` & `cognite_sdk-6.6.0/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.6.0/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/events.py` & `cognite_sdk-6.6.0/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.6.0/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/files.py` & `cognite_sdk-6.6.0/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/functions.py` & `cognite_sdk-6.6.0/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/geospatial.py` & `cognite_sdk-6.6.0/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/iam.py` & `cognite_sdk-6.6.0/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/labels.py` & `cognite_sdk-6.6.0/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/raw.py` & `cognite_sdk-6.6.0/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/relationships.py` & `cognite_sdk-6.6.0/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/sequences.py` & `cognite_sdk-6.6.0/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.6.0/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/templates.py` & `cognite_sdk-6.6.0/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/three_d.py` & `cognite_sdk-6.6.0/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/time_series.py` & `cognite_sdk-6.6.0/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.6.0/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.6.0/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.6.0/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.6.0/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.6.0/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api/vision.py` & `cognite_sdk-6.6.0/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_api_client.py` & `cognite_sdk-6.6.0/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_cognite_client.py` & `cognite_sdk-6.6.0/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_http_client.py` & `cognite_sdk-6.6.0/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.6.0/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.6.0/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.6.0/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.6.0/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.6.0/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.6.0/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.6.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.6.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.6.0/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.6.0/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/config.py` & `cognite_sdk-6.6.0/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/credentials.py` & `cognite_sdk-6.6.0/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/_base.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/assets.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cognite.client.data_classes.data_modeling import aggregations, filters
+from cognite.client.data_classes.data_modeling import aggregations, filters, query
 from cognite.client.data_classes.data_modeling.aggregations import AggregatedValue, Aggregation
 from cognite.client.data_classes.data_modeling.containers import (
     Constraint,
     Container,
     ContainerApply,
     ContainerApplyList,
     ContainerFilter,
@@ -54,24 +54,26 @@
 )
 from cognite.client.data_classes.data_modeling.instances import (
     Edge,
     EdgeApply,
     EdgeApplyResult,
     EdgeApplyResultList,
     EdgeList,
+    EdgeListWithCursor,
     InstanceApply,
     InstancesApplyResult,
     InstancesDeleteResult,
     InstanceSort,
     InstancesResult,
     Node,
     NodeApply,
     NodeApplyResult,
     NodeApplyResultList,
     NodeList,
+    NodeListWithCursor,
     NodeOrEdgeData,
 )
 from cognite.client.data_classes.data_modeling.spaces import Space, SpaceApply, SpaceApplyList, SpaceList
 from cognite.client.data_classes.data_modeling.views import (
     ConnectionDefinition,
     MappedProperty,
     MappedPropertyApply,
@@ -152,24 +154,27 @@
     "Json",
     "TimeSeriesReference",
     "FileReference",
     "SequenceReference",
     "PropertyType",
     "Node",
     "NodeList",
+    "NodeListWithCursor",
     "NodeApply",
     "NodeApplyResult",
     "NodeApplyResultList",
     "Edge",
     "EdgeList",
+    "EdgeListWithCursor",
     "EdgeApply",
     "EdgeApplyResult",
     "EdgeApplyResultList",
     "InstanceSort",
     "NodeOrEdgeData",
     "NodeId",
     "EdgeId",
     "InstancesApplyResult",
     "InstancesDeleteResult",
     "InstancesResult",
     "InstanceApply",
+    "query",
 ]
```

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/aggregations.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/aggregations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import json
 from abc import abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import (
+    TYPE_CHECKING,
     Any,
+    Collection,
     Dict,
     ItemsView,
     Iterator,
     KeysView,
     List,
     Literal,
     Mapping,
@@ -40,14 +42,16 @@
     EdgeId,
     NodeId,
     ViewId,
     ViewIdentifier,
 )
 from cognite.client.utils._text import convert_all_keys_to_snake_case
 
+if TYPE_CHECKING:
+    from cognite.client import CogniteClient
 PropertyValue = Union[str, int, float, bool, dict, List[str], List[int], List[float], List[bool], List[dict]]
 Space = str
 PropertyIdentifier = str
 
 
 @dataclass
 class NodeOrEdgeData:
@@ -685,28 +689,40 @@
 class NodeList(CogniteResourceList[Node]):
     _RESOURCE = Node
 
     def as_ids(self) -> list[NodeId]:
         return [node.as_id() for node in self]
 
 
+class NodeListWithCursor(NodeList):
+    def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
+        super().__init__(resources, cognite_client)
+        self.cursor: str | None = None
+
+
 class EdgeApplyResultList(CogniteResourceList[EdgeApplyResult]):
     _RESOURCE = EdgeApplyResult
 
     def as_ids(self) -> list[EdgeId]:
         return [edge.as_id() for edge in self]
 
 
 class EdgeList(CogniteResourceList[Edge]):
     _RESOURCE = Edge
 
     def as_ids(self) -> list[EdgeId]:
         return [edge.as_id() for edge in self]
 
 
+class EdgeListWithCursor(EdgeList):
+    def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
+        super().__init__(resources, cognite_client)
+        self.cursor: str | None = None
+
+
 class InstanceSort(CogniteFilter):
     def __init__(
         self,
         property: list[str] | tuple[str, ...],
         direction: Literal["ascending", "descending"] = "ascending",
         nulls_first: bool = False,
     ):
@@ -724,14 +740,18 @@
         edges (EdgeList): A list of edges.
 
     """
 
     nodes: NodeList
     edges: EdgeList
 
+    @classmethod
+    def load(cls, data: str | dict) -> InstancesResult:
+        raise NotImplementedError()
+
 
 @dataclass
 class InstancesApplyResult:
     """This represents the write result of an instance query
 
     Args:
         nodes (NodeApplyResultList): A list of nodes.
```

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/events.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/files.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/functions.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/iam.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/labels.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/raw.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/shared.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/templates.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.6.0/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/exceptions.py` & `cognite_sdk-6.6.0/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/testing.py` & `cognite_sdk-6.6.0/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/__init__.py` & `cognite_sdk-6.6.0/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.6.0/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.6.0/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_graph.py` & `cognite_sdk-6.6.0/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_identifier.py` & `cognite_sdk-6.6.0/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_logging.py` & `cognite_sdk-6.6.0/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.6.0/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.6.0/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.6.0/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_text.py` & `cognite_sdk-6.6.0/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_time.py` & `cognite_sdk-6.6.0/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_validation.py` & `cognite_sdk-6.6.0/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.6.0/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.8/pyproject.toml` & `cognite_sdk-6.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.5.8"
+version = "6.6.0"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
 
@@ -33,23 +33,25 @@
 backports-zoneinfo = { version = ">=0.2.1",  python = "<3.9", extras = ["tzdata"], optional = true}
 # Windows does not have a ANSI database and need tzdata
 tzdata = {version = ">=2023.3", markers = "sys_platform == 'win32'", optional = true }
 geopandas = { version = ">=0.10.0", optional = true }
 shapely = { version = ">=1.7.0", optional = true }
 pyodide-http = {version = "^0.2.0", optional = true }
 graphlib-backport = {version = "^1.0.0", python = "<3.9"}
+PyYAML = {version = "^6.0", optional = true}
 
 [tool.poetry.extras]
 pandas = ["pandas", "backports-zoneinfo"]
 numpy = ["numpy"]
 geo = ["geopandas", "shapely"]
 sympy = ["sympy"]
 functions = ["pip"]
+yaml = ["PyYAML"]
 pyodide = ["pyodide-http"]  # keep pyodide related dependencies outside of 'all'
-all = ["pandas", "geopandas", "shapely", "sympy", "pip", "backports-zoneinfo"]
+all = ["pandas", "geopandas", "shapely", "sympy", "pip", "backports-zoneinfo", "yaml"]
 
 [tool.poetry.group.dev.dependencies]
 docutils = "==0.15.2"
 sphinx = "^5.0.1"
 sphinx-rtd-theme = ">=1.0.0"
 pytest = ">=7"
 pytest-cov = ">=3"
```

### Comparing `cognite_sdk-6.5.8/PKG-INFO` & `cognite_sdk-6.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.5.8
+Version: 6.6.0
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,16 @@
 Provides-Extra: all
 Provides-Extra: functions
 Provides-Extra: geo
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: pyodide
 Provides-Extra: sympy
+Provides-Extra: yaml
+Requires-Dist: PyYAML (>=6.0,<7.0) ; extra == "yaml"
 Requires-Dist: backports-zoneinfo[tzdata] (>=0.2.1) ; (python_version < "3.9") and (extra == "pandas" or extra == "all")
 Requires-Dist: geopandas (>=0.10.0) ; extra == "geo" or extra == "all"
 Requires-Dist: graphlib-backport (>=1.0.0,<2.0.0) ; python_version < "3.9"
 Requires-Dist: msal (>=1,<2)
 Requires-Dist: numpy (>=1.20,<2.0) ; extra == "numpy"
 Requires-Dist: pandas (>=1.4) ; extra == "pandas" or extra == "all"
 Requires-Dist: pip (>=20.0.0) ; extra == "functions" or extra == "all"
```

#### html2text {}

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.5.8 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.6.0 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
-Provides-Extra: pandas Provides-Extra: pyodide Provides-Extra: sympy Requires-
-Dist: backports-zoneinfo[tzdata] (>=0.2.1) ; (python_version < "3.9") and
-(extra == "pandas" or extra == "all") Requires-Dist: geopandas (>=0.10.0) ;
-extra == "geo" or extra == "all" Requires-Dist: graphlib-backport
-(>=1.0.0,<2.0.0) ; python_version < "3.9" Requires-Dist: msal (>=1,<2)
-Requires-Dist: numpy (>=1.20,<2.0) ; extra == "numpy" Requires-Dist: pandas
-(>=1.4) ; extra == "pandas" or extra == "all" Requires-Dist: pip (>=20.0.0) ;
-extra == "functions" or extra == "all" Requires-Dist: protobuf (>=3.16.0)
-Requires-Dist: pyodide-http (>=0.2.0,<0.3.0) ; extra == "pyodide" Requires-
-Dist: requests (>=2,<3) Requires-Dist: requests_oauthlib (>=1,<2) Requires-
-Dist: shapely (>=1.7.0) ; extra == "geo" or extra == "all" Requires-Dist:
-sortedcontainers (>=2.2,<3.0) Requires-Dist: sympy ; extra == "sympy" or extra
-== "all" Requires-Dist: tzdata (>=2023.3) ; sys_platform == "win32" Project-
-URL: Documentation, https://cognite-sdk-python.readthedocs-hosted.com
-Description-Content-Type: text/markdown [Cognite_logo] Cognite Python SDK
-========================== [![build](https://github.com/cognitedata/cognite-
-sdk-python/workflows/release/badge.svg)](https://github.com/cognitedata/
-cognite-sdk-python/actions?query=workflow:release) [![Downloads](https://
-img.shields.io/pypi/dm/cognite-sdk)](https://pypistats.org/packages/cognite-
-sdk) [![GitHub](https://img.shields.io/github/license/cognitedata/cognite-sdk-
-python)](https://github.com/cognitedata/cognite-sdk-python/blob/master/LICENSE)
-[![codecov](https://codecov.io/gh/cognitedata/cognite-sdk-python/branch/master/
-graph/badge.svg)](https://codecov.io/gh/cognitedata/cognite-sdk-python) [!
+Provides-Extra: pandas Provides-Extra: pyodide Provides-Extra: sympy Provides-
+Extra: yaml Requires-Dist: PyYAML (>=6.0,<7.0) ; extra == "yaml" Requires-Dist:
+backports-zoneinfo[tzdata] (>=0.2.1) ; (python_version < "3.9") and (extra ==
+"pandas" or extra == "all") Requires-Dist: geopandas (>=0.10.0) ; extra ==
+"geo" or extra == "all" Requires-Dist: graphlib-backport (>=1.0.0,<2.0.0) ;
+python_version < "3.9" Requires-Dist: msal (>=1,<2) Requires-Dist: numpy
+(>=1.20,<2.0) ; extra == "numpy" Requires-Dist: pandas (>=1.4) ; extra ==
+"pandas" or extra == "all" Requires-Dist: pip (>=20.0.0) ; extra == "functions"
+or extra == "all" Requires-Dist: protobuf (>=3.16.0) Requires-Dist: pyodide-
+http (>=0.2.0,<0.3.0) ; extra == "pyodide" Requires-Dist: requests (>=2,<3)
+Requires-Dist: requests_oauthlib (>=1,<2) Requires-Dist: shapely (>=1.7.0) ;
+extra == "geo" or extra == "all" Requires-Dist: sortedcontainers (>=2.2,<3.0)
+Requires-Dist: sympy ; extra == "sympy" or extra == "all" Requires-Dist: tzdata
+(>=2023.3) ; sys_platform == "win32" Project-URL: Documentation, https://
+cognite-sdk-python.readthedocs-hosted.com Description-Content-Type: text/
+markdown [Cognite_logo] Cognite Python SDK ========================== [![build]
+(https://github.com/cognitedata/cognite-sdk-python/workflows/release/
+badge.svg)](https://github.com/cognitedata/cognite-sdk-python/
+actions?query=workflow:release) [![Downloads](https://img.shields.io/pypi/dm/
+cognite-sdk)](https://pypistats.org/packages/cognite-sdk) [![GitHub](https://
+img.shields.io/github/license/cognitedata/cognite-sdk-python)](https://
+github.com/cognitedata/cognite-sdk-python/blob/master/LICENSE) [![codecov]
+(https://codecov.io/gh/cognitedata/cognite-sdk-python/branch/master/graph/
+badge.svg)](https://codecov.io/gh/cognitedata/cognite-sdk-python) [!
 [Documentation Status](https://readthedocs.com/projects/cognite-sdk-python/
 badge/?version=latest)](https://cognite-sdk-python.readthedocs-hosted.com/en/
 latest/) [![PyPI version](https://badge.fury.io/py/cognite-sdk.svg)](https://
 pypi.org/project/cognite-sdk/) [![mypy](http://www.mypy-lang.org/static/
 mypy_badge.svg)](http://mypy-lang.org) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/
 black) This is the Cognite Python SDK for developers and data scientists
```


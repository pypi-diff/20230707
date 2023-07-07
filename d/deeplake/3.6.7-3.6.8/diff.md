# Comparing `tmp/deeplake-3.6.7.tar.gz` & `tmp/deeplake-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.6.7.tar", last modified: Wed Jun 28 11:38:45 2023, max compression
+gzip compressed data, was "deeplake-3.6.8.tar", last modified: Fri Jul  7 15:36:44 2023, max compression
```

## Comparing `deeplake-3.6.7.tar` & `deeplake-3.6.8.tar`

### file list

```diff
@@ -1,398 +1,399 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.737727 deeplake-3.6.7/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-06-28 11:36:15.000000 deeplake-3.6.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-28 11:36:15.000000 deeplake-3.6.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    26013 2023-06-28 11:38:45.737727 deeplake-3.6.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25284 2023-06-28 11:36:15.000000 deeplake-3.6.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.707727 deeplake-3.6.7/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.707727 deeplake-3.6.7/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100616 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    89755 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     7900 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    18861 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    25050 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7499 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     7081 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    13490 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19099 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     7420 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   118018 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   177242 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    15775 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11965 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5265 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    20369 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    16043 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.717727 deeplake-3.6.7/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    20658 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13833 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/azure.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25799 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    50495 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7485 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    12917 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52842 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29645 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5970 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26286 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)    38384 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15388 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    11402 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4510 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6949 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     5040 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)    12156 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25912 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22454 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9862 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7317 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.727727 deeplake-3.6.7/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2554 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    16369 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.737727 deeplake-3.6.7/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3151 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    35113 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.737727 deeplake-3.6.7/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3220 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4137 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4204 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8767 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.737727 deeplake-3.6.7/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25277 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.737727 deeplake-3.6.7/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-06-28 11:36:15.000000 deeplake-3.6.7/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 11:38:45.707727 deeplake-3.6.7/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    26013 2023-06-28 11:38:45.000000 deeplake-3.6.7/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12677 2023-06-28 11:38:45.000000 deeplake-3.6.7/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 11:38:45.000000 deeplake-3.6.7/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-28 11:38:45.000000 deeplake-3.6.7/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 11:38:45.000000 deeplake-3.6.7/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-28 11:38:45.000000 deeplake-3.6.7/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-28 11:38:45.000000 deeplake-3.6.7/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-28 11:38:45.737727 deeplake-3.6.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3357 2023-06-28 11:36:15.000000 deeplake-3.6.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-07-07 15:35:13.000000 deeplake-3.6.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-07 15:35:13.000000 deeplake-3.6.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    26013 2023-07-07 15:36:44.987345 deeplake-3.6.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25284 2023-07-07 15:35:13.000000 deeplake-3.6.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   100629 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    89755 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    18861 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    25990 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     7081 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    13490 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19099 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   118602 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   181668 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    15791 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    20369 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    16043 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    20658 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13833 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25799 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    50495 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    12917 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52842 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29645 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5970 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      682 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26865 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)    38773 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15186 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11509 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6949 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     5040 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25912 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22454 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9862 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7317 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    16369 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3151 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    35113 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7549 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_keys.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25277 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26013 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12710 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-07 15:36:44.987345 deeplake-3.6.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-07-07 15:35:13.000000 deeplake-3.6.8/setup.py
```

### Comparing `deeplake-3.6.7/LICENSE` & `deeplake-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/PKG-INFO` & `deeplake-3.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.7
+Version: 3.6.8
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.7 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.8 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.7/README.md` & `deeplake-3.6.8/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/__init__.py` & `deeplake-3.6.8/deeplake/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,23 +75,21 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.6.7"
+__version__ = "3.6.8"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
-deeplake_reporter.system_report(publish=True)
-deeplake_reporter.setup_excepthook(publish=True)
 
 event_queue: Queue = Queue()
 
 
 def send_event():
     while True:
         try:
```

### Comparing `deeplake-3.6.7/deeplake/api/dataset.py` & `deeplake-3.6.8/deeplake/api/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
             "storage": cache_chain,
             "read_only": storage.read_only,
             "public": public,
             "token": token,
             "org_id": org_id,
             "verbose": verbose,
         }
-        ret = dataset._load(dataset_kwargs)
+        ret = dataset._load(dataset_kwargs, create=True)
         return ret
 
     @staticmethod
     @spinner
     def load(
         path: Union[str, pathlib.Path],
         read_only: Optional[bool] = None,
```

### Comparing `deeplake-3.6.7/deeplake/api/info.py` & `deeplake-3.6.8/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/link.py` & `deeplake-3.6.8/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/link_tiled.py` & `deeplake-3.6.8/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/read.py` & `deeplake-3.6.8/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_access_method.py` & `deeplake-3.6.8/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_agreement.py` & `deeplake-3.6.8/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_api.py` & `deeplake-3.6.8/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.6.8/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.6.8/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.6.8/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.6.8/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_dataset.py` & `deeplake-3.6.8/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_dicom.py` & `deeplake-3.6.8/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_downsample.py` & `deeplake-3.6.8/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_events.py` & `deeplake-3.6.8/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_grayscale.py` & `deeplake-3.6.8/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_info.py` & `deeplake-3.6.8/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.6.8/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_json.py` & `deeplake-3.6.8/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_link.py` & `deeplake-3.6.8/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.6.8/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_linking.py` & `deeplake-3.6.8/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_mesh.py` & `deeplake-3.6.8/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_meta.py` & `deeplake-3.6.8/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_nifti.py` & `deeplake-3.6.8/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_none.py` & `deeplake-3.6.8/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.6.8/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_pickle.py` & `deeplake-3.6.8/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.6.8/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_polygons.py` & `deeplake-3.6.8/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_pop.py` & `deeplake-3.6.8/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_readonly.py` & `deeplake-3.6.8/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_rechunk.py` & `deeplake-3.6.8/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_reset.py` & `deeplake-3.6.8/deeplake/api/tests/test_reset.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,7 +320,28 @@
 
     del ds.storage["version_control_info.json"]
     ds.storage.flush()
 
     ds = deeplake.load(local_path)
 
     np.testing.assert_array_equal(ds.abc.numpy(), [[1]])
+
+
+def test_load_corrupt_dataset_no_meta(local_path):
+    ds = deeplake.empty(local_path, overwrite=True)
+
+    with ds:
+        ds.create_tensor("abc")
+        ds.abc.append(1)
+        a = ds.commit()
+
+        ds.abc.append(2)
+        b = ds.commit()
+
+        del ds.storage["dataset_meta.json"]
+
+    ds = deeplake.load(local_path)
+    assert ds.commit_id == b
+    np.testing.assert_array_equal(ds.abc.numpy(), [[1], [2]])
+
+    with pytest.raises(CheckoutError):
+        ds.checkout(a)
```

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_sample_info.py` & `deeplake-3.6.8/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_text.py` & `deeplake-3.6.8/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_update_samples.py` & `deeplake-3.6.8/deeplake/api/tests/test_update_samples.py`

 * *Files 5% similar despite different names*

```diff
@@ -711,7 +711,44 @@
 
     assert ds[3:].images1.shape == (3, 900, 900, 3)
     assert ds[3:].images2.shape == (3, 323, 480, 3)
 
     ds[3:].update({"images1": [dog] * 3, "images2": [cat] * 3})
     assert ds.images1.shape == (6, 323, 480, 3)
     assert ds.images2.shape == (6, 900, 900, 3)
+
+
+def test_update_bug(local_path):
+    with deeplake.empty(local_path, overwrite=True) as ds:
+        ds.create_tensor("abc")
+        ds.abc.extend([1, 2, 3, 4, 5])
+
+    with pytest.raises(SampleUpdateError):
+        ds.abc[4] = "abcd"
+
+    ds.abc[4] = 1
+
+    np.testing.assert_array_equal(ds.abc.numpy(), [[1], [2], [3], [4], [1]])
+
+    ds = deeplake.load(local_path)
+
+    np.testing.assert_array_equal(ds.abc.numpy(), [[1], [2], [3], [4], [1]])
+
+
+def test_update_vc_bug(local_path):
+    with deeplake.empty(local_path, overwrite=True) as ds:
+        ds.create_tensor("abc")
+        ds.abc.extend([1, 2, 3, 4, 5])
+
+    ds.commit()
+
+    with pytest.raises(SampleUpdateError):
+        ds.abc[4] = "abcd"
+
+    ds.abc[4] = 1
+
+    np.testing.assert_array_equal(ds.abc.numpy(), [[1], [2], [3], [4], [1]])
+
+    ds = deeplake.load(local_path)
+
+    print(ds.abc.numpy())
+    np.testing.assert_array_equal(ds.abc.numpy(), [[1], [2], [3], [4], [1]])
```

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_video.py` & `deeplake-3.6.8/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tests/test_views.py` & `deeplake-3.6.8/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/api/tiled.py` & `deeplake-3.6.8/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/structured/base.py` & `deeplake-3.6.8/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/structured/dataframe.py` & `deeplake-3.6.8/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.6.8/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.6.8/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.6.8/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.6.8/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/base.py` & `deeplake-3.6.8/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.6.8/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.6.8/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.6.8/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.6.8/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.6.8/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.6.8/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/util.py` & `deeplake-3.6.8/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.6.8/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.6.8/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/cli/auth.py` & `deeplake-3.6.8/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/cli/test_cli.py` & `deeplake-3.6.8/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/client/client.py` & `deeplake-3.6.8/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/client/config.py` & `deeplake-3.6.8/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/client/log.py` & `deeplake-3.6.8/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/client/test_client.py` & `deeplake-3.6.8/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/client/utils.py` & `deeplake-3.6.8/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/compression.py` & `deeplake-3.6.8/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/constants.py` & `deeplake-3.6.8/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/chunk/base_chunk.py` & `deeplake-3.6.8/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.6.8/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.6.8/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.6.8/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.6.8/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.6.8/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.6.8/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/chunk_engine.py` & `deeplake-3.6.8/deeplake/core/chunk_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1293,23 +1293,32 @@
         self,
         index: Index,
         samples: Union[np.ndarray, Sequence[InputSample], InputSample],
         operator: Optional[str] = None,
         link_callback: Optional[Callable] = None,
     ):
         """Update data at `index` with `samples`."""
+
+        cmap = self.commit_chunk_map
+        if cmap is not None:
+            cmap = CommitChunkMap.frombuffer(cmap.tobytes())
         try:
             self.check_link_ready()
             (self._sequence_update if self.is_sequence else self._update)(  # type: ignore
                 index,
                 samples,
                 operator,
                 link_callback=link_callback,
             )
         except Exception as e:
+            if cmap is not None:
+                key = get_tensor_commit_chunk_map_key(self.key, self.commit_id)
+                self.meta_cache[key] = cmap
+                self._commit_chunk_map = cmap
+                self.meta_cache.register_deeplake_object(key, cmap)
             raise SampleUpdateError(self.name) from e
 
     def _get_samples_to_move(self, chunk) -> List[Sample]:
         decompress = isinstance(chunk, ChunkCompressedChunk) or self.is_text_like
         samples_to_move: List[Sample] = []
         sum_bytes = 0
 
@@ -1549,56 +1558,57 @@
         link_callback: Optional[Callable] = None,
     ):
         """Update data at `index` with `samples`."""
         self._write_initialization()
         self.cached_data = None
         initial_autoflush = self.cache.autoflush
         self.cache.autoflush = False
+        try:
+            if operator is not None:
+                return self._update_with_operator(index, samples, operator)
 
-        if operator is not None:
-            return self._update_with_operator(index, samples, operator)
-
-        enc = self.chunk_id_encoder
-        index_length = index.length(self.num_samples)
-        samples = make_sequence(samples, index_length)
-        verified_samples = self.check_each_sample(samples)
-        if self.tensor_meta.htype == "class_label":
-            samples = self._convert_class_labels(samples)
-        if self.tensor_meta.htype == "polygon":
-            samples = [Polygons(sample, self.tensor_meta.dtype) for sample in samples]  # type: ignore
-        nbytes_after_updates: List[int] = []
-        global_sample_indices = tuple(index.values[0].indices(self.num_samples))
-        is_sequence = self.is_sequence
-        for i, sample in enumerate(samples):  # type: ignore
-            sample = None if is_empty_list(sample) else sample
-            global_sample_index = global_sample_indices[i]  # TODO!
-            if self._is_tiled_sample(global_sample_index):
-                self._update_tiled_sample(
-                    global_sample_index, index, sample, nbytes_after_updates
-                )
-            else:
-                self._update_non_tiled_sample(
-                    global_sample_index, index, sample, nbytes_after_updates
-                )
-            self.update_creds(global_sample_index, sample)
-            if update_commit_diff:
-                self.commit_diff.update_data(global_sample_index)
-            chunk_min, chunk_max = self.min_chunk_size, self.max_chunk_size
-            check_suboptimal_chunks(nbytes_after_updates, chunk_min, chunk_max)
-
-            if link_callback:
-                new_sample = verified_samples[i] if verified_samples else sample
-                link_callback(
-                    global_sample_index,
-                    sub_index=Index(index.values[1:]),
-                    new_sample=new_sample,
-                    flat=True if is_sequence else None,
-                )
-        self.cache.autoflush = initial_autoflush
-        self.cache.maybe_flush()
+            enc = self.chunk_id_encoder
+            index_length = index.length(self.num_samples)
+            samples = make_sequence(samples, index_length)
+            verified_samples = self.check_each_sample(samples)
+            if self.tensor_meta.htype == "class_label":
+                samples = self._convert_class_labels(samples)
+            if self.tensor_meta.htype == "polygon":
+                samples = [Polygons(sample, self.tensor_meta.dtype) for sample in samples]  # type: ignore
+            nbytes_after_updates: List[int] = []
+            global_sample_indices = tuple(index.values[0].indices(self.num_samples))
+            is_sequence = self.is_sequence
+            for i, sample in enumerate(samples):  # type: ignore
+                sample = None if is_empty_list(sample) else sample
+                global_sample_index = global_sample_indices[i]  # TODO!
+                if self._is_tiled_sample(global_sample_index):
+                    self._update_tiled_sample(
+                        global_sample_index, index, sample, nbytes_after_updates
+                    )
+                else:
+                    self._update_non_tiled_sample(
+                        global_sample_index, index, sample, nbytes_after_updates
+                    )
+                self.update_creds(global_sample_index, sample)
+                if update_commit_diff:
+                    self.commit_diff.update_data(global_sample_index)
+                chunk_min, chunk_max = self.min_chunk_size, self.max_chunk_size
+                check_suboptimal_chunks(nbytes_after_updates, chunk_min, chunk_max)
+
+                if link_callback:
+                    new_sample = verified_samples[i] if verified_samples else sample
+                    link_callback(
+                        global_sample_index,
+                        sub_index=Index(index.values[1:]),
+                        new_sample=new_sample,
+                        flat=True if is_sequence else None,
+                    )
+        finally:
+            self.cache.autoflush = initial_autoflush
+            self.cache.maybe_flush()
         return verified_samples
 
     def _update_with_operator(
         self,
         index: Index,
         samples: Union[np.ndarray, Sequence[InputSample], InputSample],
         operator: str,
```

### Comparing `deeplake-3.6.7/deeplake/core/compression.py` & `deeplake-3.6.8/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/compute/process.py` & `deeplake-3.6.8/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/compute/provider.py` & `deeplake-3.6.8/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/compute/ray.py` & `deeplake-3.6.8/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/compute/serial.py` & `deeplake-3.6.8/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/compute/thread.py` & `deeplake-3.6.8/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/dataset/__init__.py` & `deeplake-3.6.8/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/dataset/dataset.py` & `deeplake-3.6.8/deeplake/core/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1302,14 +1302,26 @@
     def __iter__(self):
         dataset_read(self)
         for i in range(len(self)):
             yield self.__getitem__(
                 i, is_iteration=not isinstance(self.index.values[0], list)
             )
 
+    def _get_commit_id_for_address(self, address, version_state):
+        if address in version_state["branch_commit_map"]:
+            branch = address
+            commit_id = version_state["branch_commit_map"][branch]
+        elif address in version_state["commit_node_map"]:
+            commit_id = address
+        else:
+            raise CheckoutError(
+                f"Address {address} not found. Ensure the commit id / branch name is correct."
+            )
+        return commit_id
+
     def _load_version_info(self, address=None):
         """Loads data from version_control_file otherwise assume it doesn't exist and load all empty"""
         if self.version_state:
             return
 
         if address is None:
             address = "main"
@@ -1321,23 +1333,15 @@
             except Exception as e:
                 version_info = rebuild_version_info(self.storage)
                 if version_info is None:
                     raise e
             version_state["branch_commit_map"] = version_info["branch_commit_map"]
             version_state["commit_node_map"] = version_info["commit_node_map"]
 
-            if address in version_state["branch_commit_map"]:
-                branch = address
-                commit_id = version_state["branch_commit_map"][branch]
-            elif address in version_state["commit_node_map"]:
-                commit_id = address
-            else:
-                raise CheckoutError(
-                    f"Address {address} not found. Ensure the commit id / branch name is correct."
-                )
+            commit_id = self._get_commit_id_for_address(address, version_state)
 
             version_state["commit_id"] = commit_id
             version_state["commit_node"] = version_state["commit_node_map"][commit_id]
             version_state["branch"] = version_state["commit_node"].branch
         except Exception as e:
             if isinstance(e, CheckoutError):
                 raise e from None
@@ -1753,17 +1757,22 @@
             changes["dataset"] = dataset_changes_1, dataset_changes_2
             changes["tensor"] = tensor_changes_1, tensor_changes_2
             return changes
         all_changes = get_all_changes_string(*res)
         print(all_changes)
         return None
 
-    def _populate_meta(self, verbose=True):
+    def _populate_meta(self, address: Optional[str] = None, verbose=True):
         """Populates the meta information for the dataset."""
-        if dataset_exists(self.storage):
+        if address is None:
+            commit_id = self._get_commit_id_for_address("main", self.version_state)
+        else:
+            commit_id = self._get_commit_id_for_address(address, self.version_state)
+
+        if dataset_exists(self.storage, commit_id):
             load_meta(self)
 
         elif not self.storage.empty():
             # dataset does not exist, but the path was not empty
             raise PathNotEmptyException
 
         else:
@@ -2243,15 +2252,17 @@
         if self.is_first_load:
             self.storage.autoflush = True
             self._load_version_info(address)
             self._load_link_creds()
             self._set_read_only(
                 self._read_only, err=self._read_only_error
             )  # TODO: weird fix for dataset unpickling
-            self._populate_meta(verbose)  # TODO: use the same scheme as `load_info`
+            self._populate_meta(
+                address, verbose
+            )  # TODO: use the same scheme as `load_info`
             if self.index.is_trivial():
                 self.index = Index.from_json(self.meta.default_index)
         elif not self._read_only:
             self._lock(verbose=verbose)  # for ref counting
 
         if not self.is_first_load and not self.group_index:
             self._reload_version_state()
@@ -2812,51 +2823,25 @@
 
     def __args__(self):
         return None
 
     def __bool__(self):
         return True
 
-    def extend(self, samples: Dict[str, Any], skip_ok: bool = False):
-        """Appends multiple rows of samples to mutliple tensors at once. This method expects all tensors being updated to be of the same length.
-
-        Args:
-            samples (Dict[str, Any]): Dictionary with tensor names as keys and samples as values.
-            skip_ok (bool): Skip tensors not in ``samples`` if set to True.
-
-        Raises:
-            KeyError: If any tensor in the dataset is not a key in ``samples`` and ``skip_ok`` is ``False``.
-            TensorDoesNotExistError: If tensor in ``samples`` does not exist.
-            ValueError: If all tensors being updated are not of the same length.
-            NotImplementedError: If an error occurs while writing tiles.
-            Exception: Error while attempting to rollback appends.
-        """
-        if isinstance(samples, Dataset):
-            samples = samples.tensors
-        if not samples:
-            return
-        n = len(samples[next(iter(samples.keys()))])
-        for v in samples.values():
-            if len(v) != n:
-                sizes = {k: len(v) for (k, v) in samples.items()}
-                raise ValueError(
-                    f"Incoming samples are not of equal lengths. Incoming sample sizes: {sizes}"
-                )
-        [f() for f in list(self._update_hooks.values())]
-        with self:
-            for i in range(n):
-                self.append({k: v[i] for k, v in samples.items()}, skip_ok=skip_ok)
-
-    @invalid_view_op
-    def append(
-        self, sample: Dict[str, Any], skip_ok: bool = False, append_empty: bool = False
+    def _append_or_extend(
+        self,
+        sample: Dict[str, Any],
+        extend: bool = False,
+        skip_ok: bool = False,
+        append_empty: bool = False,
     ):
-        """Append samples to mutliple tensors at once. This method expects all tensors being updated to be of the same length.
+        """Append or extend samples to mutliple tensors at once. This method expects all tensors being updated to be of the same length.
 
         Args:
+            extend (bool): Extends if True. Appends if False.
             sample (dict): Dictionary with tensor names as keys and samples as values.
             skip_ok (bool): Skip tensors not in ``sample`` if set to ``True``.
             append_empty (bool): Append empty samples to tensors not specified in ``sample`` if set to ``True``. If True, ``skip_ok`` is ignored.
 
         Raises:
             KeyError: If any tensor in the dataset is not a key in ``sample`` and ``skip_ok`` is ``False``.
             TensorDoesNotExistError: If tensor in ``sample`` does not exist.
@@ -2888,34 +2873,58 @@
             )
         for k in sample:
             if k not in tensors:
                 raise TensorDoesNotExistError(k)
         tensors_to_check_length = tensors if append_empty else sample
         if len(set(map(len, (tensors[k] for k in tensors_to_check_length)))) != 1:
             raise ValueError(
-                "When appending using Dataset.append, all tensors being updated are expected to have the same length."
+                "When appending using Dataset.append or Dataset.extend, all tensors being updated are expected to have the same length."
             )
+        if extend:
+            sample_lens = set(map(len, sample.values()))
+            if sample_lens == {0}:
+                return
+            if len(sample_lens) > 1 and not append_empty:
+                raise ValueError(
+                    "All tensors have to be extended to the same length. Specify `append_empty=True` to pad tensors receiving fewer samples."
+                )
+            max_len = max(sample_lens)
         [f() for f in list(self._update_hooks.values())]
         tensors_appended = []
         with self:
             for k in tensors:
+                extend_extra_nones = 0
                 if k in sample:
                     v = sample[k]
+                    if extend:
+                        extend_extra_nones = max(max_len - len(v), 0)
                 else:
                     if skip_ok:
                         continue
                     else:
-                        v = None
+                        if extend:
+                            v = [None] * max_len
+                        else:
+                            v = None
                 try:
                     tensor = tensors[k]
                     enc = tensor.chunk_engine.chunk_id_encoder
                     num_chunks = enc.num_chunks
-                    tensor.append(v)
+                    if extend:
+                        tensor.extend(v)
+                        if extend_extra_nones:
+                            tensor.extend([None] * extend_extra_nones)
+                    else:
+                        tensor.append(v)
                     tensors_appended.append(k)
                 except Exception as e:
+                    if extend:
+                        raise NotImplementedError(
+                            "Unable to recover from error while extending multiple tensors with numpy arrays."
+                        )
                     new_num_chunks = enc.num_chunks
                     num_chunks_added = new_num_chunks - num_chunks
                     if num_chunks_added > 1:
                         # This is unlikely to happen, i.e the sample passed the validation
                         # steps and tiling but some error occured while writing tiles to chunks
                         raise NotImplementedError(
                             "Unable to recover from error while writing tiles."
@@ -2927,14 +2936,107 @@
                             self[k].pop()
                         except Exception as e2:
                             raise Exception(
                                 "Error while attempting to rollback appends"
                             ) from e2
                     raise e
 
+    def extend(
+        self,
+        samples: Dict[str, Any],
+        skip_ok: bool = False,
+        append_empty: bool = False,
+        ignore_errors: bool = False,
+    ):
+        """Appends multiple rows of samples to mutliple tensors at once. This method expects all tensors being updated to be of the same length.
+
+        Args:
+            samples (Dict[str, Any]): Dictionary with tensor names as keys and samples as values.
+            skip_ok (bool): Skip tensors not in ``samples`` if set to True.
+            append_empty (bool): Append empty samples to tensors not specified in ``sample`` if set to ``True``. If True, ``skip_ok`` is ignored.
+            ignore_errors (bool): Skip samples that cause errors while extending, if set to ``True``.
+
+        Raises:
+            KeyError: If any tensor in the dataset is not a key in ``samples`` and ``skip_ok`` is ``False``.
+            TensorDoesNotExistError: If tensor in ``samples`` does not exist.
+            ValueError: If all tensors being updated are not of the same length.
+            NotImplementedError: If an error occurs while writing tiles.
+            Exception: Error while attempting to rollback appends.
+        """
+        extend = False
+        if isinstance(samples, Dataset):
+            samples = samples.tensors
+            extend = True
+        elif set(map(type, samples.values())) == {np.ndarray}:
+            extend = True
+        if not samples:
+            return
+        n = len(samples[next(iter(samples.keys()))])
+        for v in samples.values():
+            if len(v) != n:
+                sizes = {k: len(v) for (k, v) in samples.items()}
+                raise ValueError(
+                    f"Incoming samples are not of equal lengths. Incoming sample sizes: {sizes}"
+                )
+        [f() for f in list(self._update_hooks.values())]
+        if extend:
+            if ignore_errors:
+                warnings.warn(
+                    "`ignore_errors` argument will be ignored while extending with numpy arrays or tensors."
+                )
+            return self._append_or_extend(
+                samples, extend=True, skip_ok=skip_ok, append_empty=append_empty
+            )
+        with self:
+            for i in range(n):
+                try:
+                    self.append(
+                        {k: v[i] for k, v in samples.items()},
+                        skip_ok=skip_ok,
+                        append_empty=append_empty,
+                    )
+                except Exception as e:
+                    if ignore_errors:
+                        continue
+                    else:
+                        raise e
+
+    @invalid_view_op
+    def append(
+        self, sample: Dict[str, Any], skip_ok: bool = False, append_empty: bool = False
+    ):
+        """Append samples to mutliple tensors at once. This method expects all tensors being updated to be of the same length.
+
+        Args:
+            sample (dict): Dictionary with tensor names as keys and samples as values.
+            skip_ok (bool): Skip tensors not in ``sample`` if set to ``True``.
+            append_empty (bool): Append empty samples to tensors not specified in ``sample`` if set to ``True``. If True, ``skip_ok`` is ignored.
+
+        Raises:
+            KeyError: If any tensor in the dataset is not a key in ``sample`` and ``skip_ok`` is ``False``.
+            TensorDoesNotExistError: If tensor in ``sample`` does not exist.
+            ValueError: If all tensors being updated are not of the same length.
+            NotImplementedError: If an error occurs while writing tiles.
+            Exception: Error while attempting to rollback appends.
+            SampleAppendingError: Error that occurs when someone tries to append a tensor value directly to the dataset without specifying tensor name.
+
+        Examples:
+
+            >>> ds = deeplake.empty("../test/test_ds")
+            >>> ds.create_tensor('data')
+            Tensor(key='data')
+            >>> ds.create_tensor('labels')
+            Tensor(key='labels')
+            >>> ds.append({"data": [1, 2, 3, 4], "labels":[0, 1, 2, 3]})
+
+        """
+        self._append_or_extend(
+            sample, extend=False, skip_ok=skip_ok, append_empty=append_empty
+        )
+
     def update(self, sample: Dict[str, Any]):
         """Update existing samples in the dataset with new values.
 
         Examples:
 
             >>> ds[0].update({"images": deeplake.read("new_image.png"), "labels": 1})
```

### Comparing `deeplake-3.6.7/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.6.8/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 from warnings import warn
 import time
 import deeplake
 
 
 class DeepLakeCloudDataset(Dataset):
-    """Subclass of :class:`Dataset`. Deep Lake cloud datasets are those datasets which are stored on Activeloop servers, their paths look like:
+    """Subclass of :class:`Dataset`. Deep Lake cloud datasets are those datasets which are stored in or connected to Activeloop servers, their paths look like:
     ``hub://username/dataset_name``."""
 
     def _first_load_init(self, verbose=True):
         self._set_org_and_name()
         if self.is_first_load:
             if self.is_actually_cloud:
                 if self.verbose and verbose:
```

### Comparing `deeplake-3.6.7/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.6.8/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.6.8/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/dataset/invalid_view.py` & `deeplake-3.6.8/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/dataset/view_entry.py` & `deeplake-3.6.8/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/fast_forwarding.py` & `deeplake-3.6.8/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/index/index.py` & `deeplake-3.6.8/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/io.py` & `deeplake-3.6.8/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/ipc.py` & `deeplake-3.6.8/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/link_creds.py` & `deeplake-3.6.8/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/linked_chunk_engine.py` & `deeplake-3.6.8/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/linked_sample.py` & `deeplake-3.6.8/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/linked_tiled_sample.py` & `deeplake-3.6.8/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/lock.py` & `deeplake-3.6.8/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/dataset_meta.py` & `deeplake-3.6.8/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.6.8/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.6.8/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.6.8/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/creds.py` & `deeplake-3.6.8/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/pad.py` & `deeplake-3.6.8/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/sequence.py` & `deeplake-3.6.8/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/shape.py` & `deeplake-3.6.8/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/encode/tile.py` & `deeplake-3.6.8/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/meta/tensor_meta.py` & `deeplake-3.6.8/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/partial_reader.py` & `deeplake-3.6.8/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/partial_sample.py` & `deeplake-3.6.8/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/polygon.py` & `deeplake-3.6.8/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/query/autocomplete.py` & `deeplake-3.6.8/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/query/filter.py` & `deeplake-3.6.8/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/query/query.py` & `deeplake-3.6.8/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/sample.py` & `deeplake-3.6.8/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/serialize.py` & `deeplake-3.6.8/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/azure.py` & `deeplake-3.6.8/deeplake/core/storage/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.6.8/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/gcs.py` & `deeplake-3.6.8/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/google_drive.py` & `deeplake-3.6.8/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/local.py` & `deeplake-3.6.8/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/lru_cache.py` & `deeplake-3.6.8/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/memory.py` & `deeplake-3.6.8/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/provider.py` & `deeplake-3.6.8/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/storage/s3.py` & `deeplake-3.6.8/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tensor.py` & `deeplake-3.6.8/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tensor_link.py` & `deeplake-3.6.8/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/test_serialize.py` & `deeplake-3.6.8/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tests/test_compression.py` & `deeplake-3.6.8/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tests/test_compute.py` & `deeplake-3.6.8/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.6.8/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tests/test_io.py` & `deeplake-3.6.8/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tests/test_locking.py` & `deeplake-3.6.8/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tests/test_readonly.py` & `deeplake-3.6.8/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tests/test_serialize.py` & `deeplake-3.6.8/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tiling/deserialize.py` & `deeplake-3.6.8/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tiling/optimizer.py` & `deeplake-3.6.8/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.6.8/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tiling/serialize.py` & `deeplake-3.6.8/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.6.8/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/tiling/test_serialize.py` & `deeplake-3.6.8/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/transform/test_transform.py` & `deeplake-3.6.8/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/transform/transform.py` & `deeplake-3.6.8/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/transform/transform_dataset.py` & `deeplake-3.6.8/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/transform/transform_tensor.py` & `deeplake-3.6.8/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/__init__.py` & `deeplake-3.6.8/deeplake/core/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.6.8/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self,
         path: Union[str, pathlib.Path],
         tensor_params: List[Dict[str, object]] = DEFAULT_VECTORSTORE_TENSORS,
         embedding_function: Optional[Callable] = None,
         read_only: Optional[bool] = False,
         ingestion_batch_size: int = 1000,
         num_workers: int = 0,
-        exec_option: str = "python",
+        exec_option: str = "auto",
         token: Optional[str] = None,
         overwrite: bool = False,
         verbose: bool = True,
         runtime: Optional[Dict] = None,
         **kwargs: Any,
     ) -> None:
         """Creates an empty VectorStore or loads an existing one if it exists at the specified ``path``.
@@ -75,16 +75,16 @@
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
             tensor_params (List[Dict[str, dict]], optional): List of dictionaries that contains information about tensors that user wants to create. See ``create_tensor`` in Deep Lake API docs for more information. Defaults to ``DEFAULT_VECTORSTORE_TENSORS``.
             embedding_function (Optional[callable], optional): Function that converts the embeddable data into embeddings. Defaults to None.
             read_only (bool, optional):  Opens dataset in read-only mode if True. Defaults to False.
             num_workers (int): Number of workers to use for parallel ingestion.
             ingestion_batch_size (int): Batch size to use for parallel ingestion.
-            exec_option (str): Default method for search execution. It could be either It could be either ``"python"``, ``"compute_engine"`` or ``"tensor_db"``. Defaults to ``"python"``.
-
+            exec_option (str): Default method for search execution. It could be either It could be either ``"auto"``, ``"python"``, ``"compute_engine"`` or ``"tensor_db"``. Defaults to ``"auto"``.
+                - ``auto``- Selects the best execution method based on the storage location of the Vector Store. It is the default option.
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
                 - ``tensor_db`` - Performant and fully-hosted Managed Tensor Database that is responsible for storage and query execution. Only available for data stored in the Deep Lake Managed Database. Store datasets in this database by specifying runtime = {"tensor_db": True} during dataset creation.
             token (str, optional): Activeloop token, used for fetching user credentials. This is Optional, tokens are normally autogenerated. Defaults to None.
             overwrite (bool): If set to True this overwrites the Vector Store if it already exists. Defaults to False.
             verbose (bool): Whether to print summary of the dataset created. Defaults to True.
             runtime (Dict, optional): Parameters for creating the Vector Store in Deep Lake's Managed Tensor Database. Not applicable when loading an existing Vector Store. To create a Vector Store in the Managed Tensor Database, set `runtime = {"tensor_db": True}`.
@@ -130,15 +130,17 @@
             exec_option,
             embedding_function,
             overwrite,
             runtime,
             **kwargs,
         )
         self.embedding_function = embedding_function
-        self.exec_option = exec_option
+        self.exec_option = utils.parse_exec_option(
+            self.dataset, exec_option, _INDRA_INSTALLED
+        )
         self.verbose = verbose
         self.tensor_params = tensor_params
 
     def add(
         self,
         embedding_function: Optional[Union[Callable, List[Callable]]] = None,
         embedding_data: Optional[Union[List, List[List]]] = None,
@@ -291,15 +293,15 @@
         embedding_data=None,
         embedding_function: Optional[Callable] = None,
         embedding: Optional[Union[List[float], np.ndarray]] = None,
         k: int = 4,
         distance_metric: str = "COS",
         query: Optional[str] = None,
         filter: Optional[Union[Dict, Callable]] = None,
-        exec_option: Optional[str] = "python",
+        exec_option: Optional[str] = None,
         embedding_tensor: str = "embedding",
         return_tensors: Optional[List[str]] = None,
         return_view: bool = False,
     ) -> Union[Dict, deeplake.core.dataset.Dataset]:
         """VectorStore search method that combines embedding search, metadata search, and custom TQL search.
 
         Examples:
@@ -337,22 +339,22 @@
             distance_metric (str): Type of distance metric to use for sorting the data. Avaliable options are: ``"L1", "L2", "COS", "MAX"``. Defaults to ``"COS"``.
             query (Optional[str]):  TQL Query string for direct evaluation, without application of additional filters or vector search.
             filter (Union[Dict, Callable], optional): Additional filter evaluated prior to the embedding search.
 
                 - ``Dict`` - Key-value search on tensors of htype json, evaluated on an AND basis (a sample must satisfy all key-value filters to be True) Dict = {"tensor_name_1": {"key": value}, "tensor_name_2": {"key": value}}
                 - ``Function`` - Any function that is compatible with :meth:`Dataset.filter <deeplake.core.dataset.Dataset.filter>`.
 
-            exec_option (Optional[str]): Method for search execution. It could be either ``"python"``, ``"compute_engine"`` or ``"tensor_db"``. Defaults to ``"python"``.
+            exec_option (Optional[str]): Method for search execution. It could be either ``"python"``, ``"compute_engine"`` or ``"tensor_db"``. Defaults to ``None``, which inherits the option from the Vector Store initialization.
 
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
                 - ``tensor_db`` - Performant and fully-hosted Managed Tensor Database that is responsible for storage and query execution. Only available for data stored in the Deep Lake Managed Database. Store datasets in this database by specifying runtime = {"tensor_db": True} during dataset creation.
             embedding_tensor (str): Name of tensor with embeddings. Defaults to "embedding".
-            return_tensors (Optional[List[str]]): List of tensors to return data for. Defaults to None. If None, all tensors are returned.
-            return_view (bool): Return a Deep Lake dataset view that satisfied the search parameters, instead of a dictinary with data. Defaults to False.
+            return_tensors (Optional[List[str]]): List of tensors to return data for. Defaults to None, which returns data for all tensors except the embedding tensor (in order to minimize payload). To return data for all tensors, specify return_tensors = "*".
+            return_view (bool): Return a Deep Lake dataset view that satisfied the search parameters, instead of a dictionary with data. Defaults to False. If ``True`` return_tensors is set to "*" beucase data is lazy-loaded and there is no cost to including all tensors in the view.
 
         ..
             # noqa: DAR101
 
         Raises:
             ValueError: When invalid parameters are specified.
 
@@ -389,31 +391,30 @@
             query=query,
             filter=filter,
             exec_option=exec_option,
             embedding_tensor=embedding_tensor,
             return_tensors=return_tensors,
         )
 
+        return_tensors = utils.parse_return_tensors(
+            self.dataset, return_tensors, embedding_tensor, return_view
+        )
+
         query_emb: Optional[Union[List[float], np.ndarray[Any, Any]]] = None
         if query is None:
             query_emb = dataset_utils.get_embedding(
                 embedding,
                 embedding_data,
                 embedding_function=embedding_function or self.embedding_function,
             )
             if isinstance(query_emb, np.ndarray):
                 assert (
                     query_emb.ndim == 1 or query_emb.shape[0] == 1
                 ), "Query embedding must be 1-dimensional. Please consider using another embedding function for converting query string to embedding."
 
-        if not return_tensors:
-            return_tensors = [
-                tensor for tensor in self.dataset.tensors if tensor != embedding_tensor
-            ]
-
         return vector_search.search(
             query=query,
             logger=logger,
             filter=filter,
             query_embedding=query_emb,
             k=k,
             distance_metric=distance_metric,
@@ -426,15 +427,15 @@
 
     def delete(
         self,
         row_ids: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
         filter: Optional[Union[Dict, Callable]] = None,
         query: Optional[str] = None,
-        exec_option: Optional[str] = "python",
+        exec_option: Optional[str] = None,
         delete_all: Optional[bool] = None,
     ) -> bool:
         """Delete the data in the Vector Store. Does not delete the tensor definitions. To delete the vector store completely, first run :meth:`VectorStore.delete_by_path()`.
 
         Examples:
             >>> # Delete using ids:
             >>> data = vector_store.delete(ids)
@@ -454,15 +455,15 @@
             ids (Optional[List[str]]): List of unique ids. Defaults to None.
             row_ids (Optional[List[str]]): List of absolute row indices from the dataset. Defaults to None.
             filter (Union[Dict, Callable], optional): Filter for finding samples for deletion.
 
                 - ``Dict`` - Key-value search on tensors of htype json, evaluated on an AND basis (a sample must satisfy all key-value filters to be True) Dict = {"tensor_name_1": {"key": value}, "tensor_name_2": {"key": value}}
                 - ``Function`` - Any function that is compatible with `deeplake.filter`.
             query (Optional[str]):  TQL Query string for direct evaluation for finding samples for deletion, without application of additional filters.
-            exec_option (str, optional): Method for search execution for finding samples for deletion. It could be either ``"python"`` or ``"compute_engine"``. Defaults to ``"python"``.
+            exec_option (str, optional): Method for search execution for finding samples for deletion. It could be either ``"python"`` or ``"compute_engine"``. Defaults to ``None``, which inherits the option from the Vector Store initialization.
 
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - Performant C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local datasets.
             delete_all (Optional[bool]): Whether to delete all the samples and version history of the dataset. Defaults to None.
 
         ..
             # noqa: DAR101
@@ -481,17 +482,17 @@
                 "query": query[0:100] if query is not None else False,
                 "filter": True if filter is not None else False,
                 "exec_option": exec_option,
                 "delete_all": delete_all,
             },
         )
 
-        dataset_utils.check_delete_arguments(
-            ids, filter, query, delete_all, row_ids, exec_option
-        )
+        exec_option = exec_option or self.exec_option
+
+        dataset_utils.check_delete_arguments(ids, filter, query, delete_all, row_ids)
 
         (
             self.dataset,
             dataset_deleted,
         ) = dataset_utils.delete_all_samples_if_specified(
             self.dataset,
             delete_all,
```

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.6.8/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,18 @@
     VectorStore,
 )
 from deeplake.core.vectorstore import utils
 from deeplake.tests.common import requires_libdeeplake
 from deeplake.constants import (
     DEFAULT_VECTORSTORE_TENSORS,
 )
-from deeplake.util.exceptions import IncorrectEmbeddingShapeError
+from deeplake.util.exceptions import (
+    IncorrectEmbeddingShapeError,
+    TensorDoesNotExistError,
+)
 
 from math import isclose
 import uuid
 import os
 
 EMBEDDING_DIM = 100
 NUMBER_OF_DATA = 10
@@ -145,14 +148,17 @@
     """Test basic search features"""
     # Initialize vector store object and add data
     vector_store = DeepLakeVectorStore(
         path=local_path,
         overwrite=True,
         token=hub_cloud_dev_token,
     )
+
+    assert vector_store.exec_option == "python"
+
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
 
     with pytest.raises(ValueError):
         vector_store.add(
             embedding_function=embedding_fn2,
             embedding_data=texts,
             text=texts,
@@ -162,15 +168,14 @@
     data_default = vector_store.search(
         embedding=query_embedding,
     )
     assert (len(data_default.keys())) > 0
     # Use python implementation to search the data
     data_p = vector_store.search(
         embedding=query_embedding,
-        exec_option="python",
         k=2,
         return_tensors=["id", "text"],
         filter={"metadata": {"abc": 1}},
     )
 
     assert len(data_p["text"]) == 1
     assert (
@@ -180,54 +185,53 @@
 
     # Load a vector store object from the cloud for indra testing
     vector_store_cloud = DeepLakeVectorStore(
         path="hub://testingacc2/vectorstore_test",
         read_only=True,
         token=hub_cloud_dev_token,
     )
+    assert vector_store_cloud.exec_option == "compute_engine"
+
     # Use indra implementation to search the data
     data_ce = vector_store_cloud.search(
         embedding=query_embedding,
-        exec_option="compute_engine",
         k=2,
-        return_tensors=["ids", "text"],
+        return_tensors=["id", "text"],
     )
     assert len(data_ce["text"]) == 2
     assert (
         sum([tensor in data_ce.keys() for tensor in vector_store_cloud.dataset.tensors])
         == 2
     )  # One for each return_tensors
     assert len(data_ce.keys()) == 3  # One for each return_tensors + score
 
     with pytest.raises(ValueError):
         data_ce = vector_store_cloud.search(
-            query=f"SELECT * WHERE id=='{vector_store_cloud.dataset.ids[0].numpy()[0]}'",
+            query=f"SELECT * WHERE id=='{vector_store_cloud.dataset.id[0].numpy()[0]}'",
             embedding=query_embedding,
-            exec_option="compute_engine",
             k=2,
-            return_tensors=["ids", "text"],
+            return_tensors=["id", "text"],
         )
 
     # Run a full custom query
     test_text = vector_store_cloud.dataset.text[0].data()["value"]
     data_q = vector_store_cloud.search(
-        query=f"select * where text == '{test_text}'", exec_option="compute_engine"
+        query=f"select * where text == '{test_text}'",
     )
 
     assert len(data_q["text"]) == 1
     assert data_q["text"][0] == test_text
     assert sum(
         [tensor in data_q.keys() for tensor in vector_store_cloud.dataset.tensors]
     ) == len(
         vector_store_cloud.dataset.tensors
     )  # One for each tensor - embedding + score
 
     # Run a filter query using a json
     data_e_j = vector_store.search(
-        exec_option="python",
         k=2,
         return_tensors=["id", "text"],
         filter={"metadata": {"abc": 1}},
     )
     assert len(data_e_j["text"]) == 1
     assert (
         sum([tensor in data_e_j.keys() for tensor in vector_store.dataset.tensors]) == 2
@@ -235,131 +239,131 @@
     assert len(data_e_j.keys()) == 2
 
     # Run the same filter as above using a function
     def filter_fn(x):
         return x["metadata"].data()["value"]["abc"] == 1
 
     data_e_f = vector_store.search(
-        exec_option="python",
         k=2,
         return_tensors=["id", "text"],
         filter=filter_fn,
     )
     assert len(data_e_f["text"]) == 1
     assert (
         sum([tensor in data_e_f.keys() for tensor in vector_store.dataset.tensors]) == 2
     )  # One for each return_tensors
     assert len(data_e_f.keys()) == 2
 
     # Check returning views
     data_p_v = vector_store.search(
         embedding=query_embedding,
-        exec_option="python",
         k=2,
         filter={"metadata": {"abc": 1}},
         return_view=True,
     )
     assert len(data_p_v) == 1
     assert isinstance(data_p_v.text[0].data()["value"], str)
     assert data_p_v.embedding[0].numpy().size > 0
 
+    # Check that specifying exec option during search works, by specifying an invalid option
+    with pytest.raises(ValueError):
+        vector_store.search(
+            embedding=query_embedding,
+            exec_option="tensor_db",
+            k=2,
+            filter={"metadata": {"abc": 1}},
+            return_view=True,
+        )
+
     data_ce_v = vector_store_cloud.search(
-        embedding=query_embedding, exec_option="compute_engine", k=2, return_view=True
+        embedding=query_embedding, k=2, return_view=True
     )
     assert len(data_ce_v) == 2
     assert isinstance(data_ce_v.text[0].data()["value"], str)
     assert data_ce_v.embedding[0].numpy().size > 0
 
     # Check exceptions
+    # Invalid exec option
     with pytest.raises(ValueError):
         vector_store.search(embedding=query_embedding, exec_option="remote_tensor_db")
+    # Search without parameters
     with pytest.raises(ValueError):
         vector_store.search()
+    # Query with python exec_option
     with pytest.raises(ValueError):
         vector_store.search(query="dummy", exec_option="python")
-    with pytest.raises(ValueError):
+    # Returning a tensor that does not exist
+    with pytest.raises(TensorDoesNotExistError):
         vector_store.search(
-            query="dummy",
+            embedding=query_embedding,
             return_tensors=["non_existant_tensor"],
-            exec_option="compute_engine",
         )
+    # Specifying return tensors is not valid when also specifying a query
     with pytest.raises(ValueError):
-        vector_store.search(query="dummy", return_tensors=["ids"], exec_option="python")
+        vector_store_cloud.search(query="dummy", return_tensors=["id"])
+    # Specifying a filter function is not valid when also specifying a query
     with pytest.raises(ValueError):
-        vector_store.search(
-            query="dummy", filter=filter_fn, exec_option="compute_engine"
+        vector_store_cloud.search(query="dummy", filter=filter_fn)
+    # Specifying a filter function is not valid when exec_option is "compute_engine"
+    with pytest.raises(ValueError):
+        vector_store_cloud.search(
+            embedding=query_embedding, filter=filter_fn, exec_option="compute_engine"
         )
+    # Not specifying a query or data that should be embedded
     with pytest.raises(ValueError):
         vector_store.search(
             embedding_function=embedding_fn,
         )
-
+    # Empty dataset cannot be queried
     with pytest.raises(ValueError):
-        vector_store = DeepLakeVectorStore(path="mem://xyz")
-
-        vector_store.search(
+        vector_store_empty = DeepLakeVectorStore(path="mem://xyz")
+        vector_store_empty.search(
             embedding=query_embedding,
-            exec_option="python",
             k=2,
             filter={"metadata": {"abc": 1}},
             return_view=True,
         )
 
     vector_store = DeepLakeVectorStore(path="mem://xyz")
+    assert vector_store.exec_option == "python"
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
 
     data = vector_store.search(
-        exec_option="python",
         embedding_function=embedding_fn3,
         embedding_data=["dummy"],
         return_view=True,
         k=2,
     )
     assert len(data) == 2
     assert isinstance(data.text[0].data()["value"], str)
     assert data.embedding[0].numpy().size > 0
 
     data = vector_store.search(
-        exec_option="python",
         filter={"metadata": {"abcdefh": 1}},
         embedding=None,
         return_view=True,
         k=2,
     )
     assert len(data) == 0
 
     data = vector_store.search(
-        exec_option="python",
         filter={"metadata": {"abcdefh": 1}},
         embedding=query_embedding,
         k=2,
     )
     assert len(data) == 4
     assert len(data["id"]) == 0
     assert len(data["metadata"]) == 0
     assert len(data["text"]) == 0
     assert len(data["score"]) == 0
 
-    with pytest.raises(ValueError):
-        data = vector_store.search(
-            exec_option="compute_engine",
-            filter=filter_fn,
-            k=2,
-        )
-
-    with pytest.raises(ValueError):
-        data = vector_store.search(
-            exec_option="compute_engine",
-            query="select * where metadata == {'abcdefg': 28}",
-            return_tensors=["metadata", "id"],
-        )
-
     vector_store = DeepLakeVectorStore(
         path="mem://xyz", embedding_function=embedding_fn
     )
+    assert vector_store.exec_option == "python"
     vector_store.add(embedding=embeddings, text=texts, metadata=metadatas)
     result = vector_store.search(embedding=np.zeros((1, EMBEDDING_DIM)))
     assert len(result) == 4
 
 
 @requires_libdeeplake
 @pytest.mark.parametrize("distance_metric", ["L1", "L2", "COS", "MAX"])
@@ -394,41 +398,44 @@
                 * (abs(data_p["score"][i]) + abs(data_ce["score"][i]))
                 / 2,
             )
             for i in range(len(data_p["score"]))
         ]
     )
     assert data_p["text"] == data_ce["text"]
-    assert data_p["ids"] == data_ce["ids"]
+    assert data_p["id"] == data_ce["id"]
     assert data_p["metadata"] == data_ce["metadata"]
 
     # use indra implementation to search the data
     data_ce = vector_store.search(
         embedding=None,
         exec_option="compute_engine",
         distance_metric=distance_metric,
-        filter={"metadata": {"abcdefg": 28}},
+        filter={"metadata": {"abc": 100}},
     )
 
-    assert data_ce["ids"] == "0"
+    # All medatata are the same to this should return k (k) results
+    assert len(data_ce["id"]) == 4
 
     with pytest.raises(ValueError):
         # use indra implementation to search the data
         data_ce = vector_store.search(
             query="select * where metadata == {'abcdefg': 28}",
             exec_option="compute_engine",
             distance_metric=distance_metric,
             filter={"metadata": {"abcdefg": 28}},
         )
 
+    test_id = vector_store.dataset.id[0].data()["value"]
+
     data_ce = vector_store.search(
-        query="select * where ids == '0'",
+        query=f"select * where id == '{test_id}'",
         exec_option="compute_engine",
     )
-    assert data_ce["ids"] == ["0"]
+    assert data_ce["id"][0] == test_id
 
 
 @requires_libdeeplake
 def test_search_managed(hub_cloud_dev_token):
     """Test whether managed TQL and client-side TQL return the same results"""
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
@@ -458,15 +465,15 @@
                 * (abs(data_ce["score"][i]) + abs(data_db["score"][i]))
                 / 2,
             )
             for i in range(len(data_ce["score"]))
         ]
     )
     assert data_ce["text"] == data_db["text"]
-    assert data_ce["ids"] == data_db["ids"]
+    assert data_ce["id"] == data_db["id"]
 
 
 def test_delete(local_path, capsys):
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
         path=local_path,
         overwrite=True,
@@ -509,54 +516,51 @@
     assert vector_store.dataset.tensors.keys() == tensors_before_delete.keys()
 
     vector_store.delete_by_path(local_path)
     dirs = os.listdir("./")
     assert local_path not in dirs
 
     # backwards compatibility test:
-    vector_store = DeepLakeVectorStore(
+    vector_store_b = DeepLakeVectorStore(
         path=local_path,
         overwrite=True,
         tensor_params=[
             {
                 "name": "ids",
                 "htype": "text",
             },
             {
                 "name": "docs",
                 "htype": "text",
             },
         ],
     )
     # add data to the dataset:
-    vector_store.add(ids=ids, docs=texts)
+    vector_store_b.add(ids=ids, docs=texts)
 
     # delete the data in the dataset by id:
-    vector_store.delete(row_ids=[0])
-    assert len(vector_store.dataset) == NUMBER_OF_DATA - 1
+    vector_store_b.delete(row_ids=[0])
+    assert len(vector_store_b.dataset) == NUMBER_OF_DATA - 1
 
     ds = deeplake.empty(local_path, overwrite=True)
-    ds.create_tensor("ids", htype="text")
+    ds.create_tensor("id", htype="text")
     ds.create_tensor("embedding", htype="embedding")
     ds.extend(
         {
-            "ids": ids,
+            "id": ids,
             "embedding": embeddings,
         }
     )
 
     vector_store = DeepLakeVectorStore(
         path=local_path,
     )
     vector_store.delete(ids=ids[:3])
     assert len(vector_store) == NUMBER_OF_DATA - 3
 
-    with pytest.raises(ValueError):
-        vector_store.delete(ids=ids[5:7], exec_option="remote_tensor_db")
-
 
 def test_ingestion(local_path, capsys):
     # create data
     number_of_data = 1000
     texts, embeddings, ids, metadatas, _ = utils.create_data(
         number_of_data=number_of_data, embedding_dim=EMBEDDING_DIM
     )
```

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,22 +457,18 @@
 
         delete_view = dataset.filter(lambda x: x[id_tensor].data()["value"] in ids)
 
     row_ids = list(delete_view.sample_indices)
     return row_ids
 
 
-def check_delete_arguments(ids, filter, query, delete_all, row_ids, exec_option):
+def check_delete_arguments(ids, filter, query, delete_all, row_ids):
     if (
         ids is None
         and filter is None
         and query is None
         and delete_all is None
         and row_ids is None
     ):
         raise ValueError(
             "Either ids, row_ids, filter, query, or delete_all must be specified."
         )
-    if exec_option not in ("python", "compute_engine", "tensor_db"):
-        raise ValueError(
-            "Invalid `exec_option` it should be either `python`, `compute_engine`."
-        )
```

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         "embedding_ctx_length": None,
         "chunk_size": None,
         "max_retries": None,
     }
 
     dataset = dataset_utils.create_or_load_dataset(
         tensor_params=DEFAULT_VECTORSTORE_TENSORS,
-        dataset_path="hub://testingacc2/vectorstore_dbengine",
+        dataset_path="hub://testingacc2/vectorstore_test_create_dbengine",
         token=hub_cloud_dev_token,
         creds={},
         logger=logger,
         read_only=False,
         exec_option="tensor_db",
         runtime={"tensor_db": True},
         overwrite=True,
@@ -80,18 +80,19 @@
         "max_retries": None,
     }
     assert (
         "s3://activeloopai-db-engine"
         in dataset.storage.__dict__["next_storage"].__dict__["root"]
     )
 
+    # Test whether not specifiying runtime with exec_option tensor_db raises error
     with pytest.raises(ValueError):
         dataset = dataset_utils.create_or_load_dataset(
             tensor_params=DEFAULT_VECTORSTORE_TENSORS,
-            dataset_path="hub://testingacc2/vectorstore_dbengine",
+            dataset_path="hub://testingacc2/vectorstore_test_create_dbengine",
             token=hub_cloud_dev_token,
             creds={},
             logger=logger,
             read_only=False,
             exec_option="tensor_db",
             runtime=None,
             overwrite=True,
```

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         str: TQL representation of the query string.
     """
 
     order = tql_distance_metrics.get_order_type_for_distance_metric(distance_metric)
     tql_distrance_metric = tql_distance_metrics.get_tql_distance_metric(
         distance_metric, embedding_tensor, query_embedding
     )
+
     query = create_query_string(
         tql_distrance_metric, tql_filter, limit, order, tensor_list
     )
     return query
 
 
 def convert_tensor_to_str(query_embedding: np.ndarray):
```

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from deeplake.constants import MB
 from deeplake.enterprise.util import raise_indra_installation_error
 from deeplake.util.warnings import always_warn
 
+from deeplake.core.dataset import DeepLakeCloudDataset
+
 import numpy as np
 
 import random
 import string
 from typing import Optional, List, Dict, Callable
 
 EXEC_OPTION_TO_RUNTIME: Dict[str, Optional[Dict]] = {
@@ -15,14 +17,44 @@
 }
 
 
 def parse_tensor_return(tensor):
     return tensor.data(aslist=True)["value"]
 
 
+def parse_exec_option(dataset, exec_option, indra_installed):
+    """Select the best available exec_option for the given dataset and environment"""
+    if exec_option == "auto":
+        if isinstance(dataset, DeepLakeCloudDataset):
+            if "vector_db/" in dataset.base_storage.path:
+                return "tensor_db"
+            elif indra_installed:
+                return "compute_engine"
+            else:
+                return "python"
+        else:
+            return "python"
+    else:
+        return exec_option
+
+
+def parse_return_tensors(dataset, return_tensors, embedding_tensor, return_view):
+    """Select the best selection of data and tensors to be returned"""
+    if return_view:
+        return_tensors = "*"
+
+    if not return_tensors or return_tensors == "*":
+        return_tensors = [
+            tensor
+            for tensor in dataset.tensors
+            if (tensor != embedding_tensor or return_tensors == "*")
+        ]
+    return return_tensors
+
+
 def check_indra_installation(exec_option, indra_installed):
     if exec_option == "compute_engine" and not indra_installed:
         raise raise_indra_installation_error(
             indra_import_error=False
         )  # pragma: no cover
```

### Comparing `deeplake-3.6.7/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.6.8/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/version_control/commit_diff.py` & `deeplake-3.6.8/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/version_control/commit_node.py` & `deeplake-3.6.8/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.6.8/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/version_control/test_merge.py` & `deeplake-3.6.8/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/core/version_control/test_version_control.py` & `deeplake-3.6.8/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.6.8/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/enterprise/dataloader.py` & `deeplake-3.6.8/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.6.8/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.6.8/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/enterprise/test_pytorch.py` & `deeplake-3.6.8/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/enterprise/test_query.py` & `deeplake-3.6.8/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.6.8/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/enterprise/util.py` & `deeplake-3.6.8/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/hooks.py` & `deeplake-3.6.8/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/htype.py` & `deeplake-3.6.8/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.6.8/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/pytorch/common.py` & `deeplake-3.6.8/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.6.8/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.6.8/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.6.8/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/tf/common.py` & `deeplake-3.6.8/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.6.8/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.6.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/integrations/wandb/wandb.py` & `deeplake-3.6.8/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/tests/cache_fixtures.py` & `deeplake-3.6.8/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/tests/client_fixtures.py` & `deeplake-3.6.8/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/tests/common.py` & `deeplake-3.6.8/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/tests/dataset_fixtures.py` & `deeplake-3.6.8/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/tests/path_fixtures.py` & `deeplake-3.6.8/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/tests/storage_fixtures.py` & `deeplake-3.6.8/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/access_method.py` & `deeplake-3.6.8/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/agreement.py` & `deeplake-3.6.8/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/array_list.py` & `deeplake-3.6.8/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/assert_byte_indexes.py` & `deeplake-3.6.8/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/auto.py` & `deeplake-3.6.8/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/bugout_reporter.py` & `deeplake-3.6.8/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/cache_chain.py` & `deeplake-3.6.8/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/casting.py` & `deeplake-3.6.8/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/check_latest_version.py` & `deeplake-3.6.8/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/chunk_engine.py` & `deeplake-3.6.8/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/class_label.py` & `deeplake-3.6.8/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/compute.py` & `deeplake-3.6.8/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/connect_dataset.py` & `deeplake-3.6.8/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/dataset.py` & `deeplake-3.6.8/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/diff.py` & `deeplake-3.6.8/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/downsample.py` & `deeplake-3.6.8/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/encoder.py` & `deeplake-3.6.8/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/exceptions.py` & `deeplake-3.6.8/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/exif.py` & `deeplake-3.6.8/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/from_tfds.py` & `deeplake-3.6.8/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/htype.py` & `deeplake-3.6.8/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/image.py` & `deeplake-3.6.8/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/invalid_view_op.py` & `deeplake-3.6.8/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/iteration_warning.py` & `deeplake-3.6.8/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/json.py` & `deeplake-3.6.8/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/keys.py` & `deeplake-3.6.8/deeplake/util/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,18 +178,24 @@
             key,
             ENCODED_SEQUENCE_NAMES_FOLDER,
             UNSHARDED_ENCODER_FILENAME,
         )
     )
 
 
-def dataset_exists(storage) -> bool:
+def dataset_exists(storage, commit_id=None) -> bool:
+    """
+    Returns true if a dataset exists at the given location.
+    NOTE: This does not verify if it is a VALID dataset, only that it exists and is likely a deeplake directory.
+    """
     try:
-        storage[get_dataset_meta_key(FIRST_COMMIT_ID)]
-        return True
+        return (
+            get_dataset_meta_key(commit_id or FIRST_COMMIT_ID) in storage
+            or get_version_control_info_key() in storage
+        )
     except S3GetAccessError as err:
         raise AuthorizationException("The dataset storage cannot be accessed") from err
     except (KeyError, S3GetError) as err:
         return False
 
 
 def tensor_exists(key: str, storage, commit_id: str) -> bool:
```

### Comparing `deeplake-3.6.7/deeplake/util/link.py` & `deeplake-3.6.8/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/logging.py` & `deeplake-3.6.8/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/merge.py` & `deeplake-3.6.8/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/modified.py` & `deeplake-3.6.8/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/notebook.py` & `deeplake-3.6.8/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/mesh.py` & `deeplake-3.6.8/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.6.8/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.6.8/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.6.8/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.6.8/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.6.8/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.6.8/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.6.8/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.6.8/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.6.8/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/path.py` & `deeplake-3.6.8/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/pretty_print.py` & `deeplake-3.6.8/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/remove_cache.py` & `deeplake-3.6.8/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/scheduling.py` & `deeplake-3.6.8/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/shape_interval.py` & `deeplake-3.6.8/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/spinner.py` & `deeplake-3.6.8/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/split.py` & `deeplake-3.6.8/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/storage.py` & `deeplake-3.6.8/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tag.py` & `deeplake-3.6.8/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tensor_db.py` & `deeplake-3.6.8/deeplake/util/tensor_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "db_engine", False
     )  # DB engine is kept for backward compatibility, can be removed if not used
     tensor_db = runtime.get("tensor_db", False) or db_engine
 
     if tensor_db and not is_hub_cloud_path(path):
         raise ValueError(
             f"Path {path} is not a valid Deep Lake cloud path."
-            " runtime = {'tensor_db': True} can only be used with Deep Lake cloud paths."
+            " runtime = {'tensor_db': True} can only be used with datasets stored in the Deep Lake Managed Tensor Database."
         )
 
     invalid_keys = set(runtime.keys()) - {"db_engine", "tensor_db"}
     if len(invalid_keys):
         raise ValueError(f"Invalid runtime parameters: {invalid_keys}.")
 
     return {"tensor_db": tensor_db}
```

### Comparing `deeplake-3.6.7/deeplake/util/testing.py` & `deeplake-3.6.8/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tests/test_auto.py` & `deeplake-3.6.8/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.6.8/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.6.8/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tests/test_read.py` & `deeplake-3.6.8/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.6.8/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tests/test_split.py` & `deeplake-3.6.8/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.6.8/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/tests/test_version_control.py` & `deeplake-3.6.8/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/transform.py` & `deeplake-3.6.8/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/version_control.py` & `deeplake-3.6.8/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/util/video.py` & `deeplake-3.6.8/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/visualizer/video_streaming.py` & `deeplake-3.6.8/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake/visualizer/visualizer.py` & `deeplake-3.6.8/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/deeplake.egg-info/PKG-INFO` & `deeplake-3.6.8/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.7
+Version: 3.6.8
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.7 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.8 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.7/deeplake.egg-info/SOURCES.txt` & `deeplake-3.6.8/deeplake.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,15 @@
 deeplake/util/object_3d/ply_readers.py
 deeplake/util/object_3d/point_cloud.py
 deeplake/util/object_3d/read_3d_data.py
 deeplake/util/tests/__init__.py
 deeplake/util/tests/test_auto.py
 deeplake/util/tests/test_connect_dataset.py
 deeplake/util/tests/test_iterable_ordered_dict.py
+deeplake/util/tests/test_keys.py
 deeplake/util/tests/test_read.py
 deeplake/util/tests/test_shape_interval.py
 deeplake/util/tests/test_shuffle.py
 deeplake/util/tests/test_split.py
 deeplake/util/tests/test_tensor_db.py
 deeplake/util/tests/test_token.py
 deeplake/util/tests/test_version_control.py
```

### Comparing `deeplake-3.6.7/deeplake.egg-info/requires.txt` & `deeplake-3.6.8/deeplake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.7/setup.py` & `deeplake-3.6.8/setup.py`

 * *Files identical despite different names*


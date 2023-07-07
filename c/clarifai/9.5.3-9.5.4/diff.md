# Comparing `tmp/clarifai-9.5.3.tar.gz` & `tmp/clarifai-9.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.5.3.tar", last modified: Fri Jun  2 20:33:48 2023, max compression
+gzip compressed data, was "clarifai-9.5.4.tar", last modified: Fri Jul  7 03:43:06 2023, max compression
```

## Comparing `clarifai-9.5.3.tar` & `clarifai-9.5.4.tar`

### file list

```diff
@@ -1,133 +1,222 @@
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.080970 clarifai-9.5.3/
--rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.5.3/LICENSE
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.5.3/MANIFEST.in
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-06-02 20:33:48.080786 clarifai-9.5.3/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.5.3/README.md
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.065951 clarifai-9.5.3/clarifai/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.066815 clarifai-9.5.3/clarifai/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12239 2023-06-02 04:02:11.000000 clarifai-9.5.3/clarifai/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.067566 clarifai-9.5.3/clarifai/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.068186 clarifai-9.5.3/clarifai/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.069286 clarifai-9.5.3/clarifai/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.5.3/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10349 2023-06-02 04:02:11.000000 clarifai-9.5.3/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.070407 clarifai-9.5.3/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1414 2023-05-01 19:51:07.000000 clarifai-9.5.3/clarifai/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.5.3/clarifai/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.063523 clarifai-9.5.3/clarifai/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.070669 clarifai-9.5.3/clarifai/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.070886 clarifai-9.5.3/clarifai/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.071157 clarifai-9.5.3/clarifai/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.071313 clarifai-9.5.3/clarifai/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.071527 clarifai-9.5.3/clarifai/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    13040 2023-06-02 04:02:11.000000 clarifai-9.5.3/clarifai/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.071805 clarifai-9.5.3/clarifai/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     5130 2023-04-11 15:50:37.000000 clarifai-9.5.3/clarifai/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.073480 clarifai-9.5.3/clarifai/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.5.3/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.5.3/clarifai/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.5.3/clarifai/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.5.3/clarifai/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.074026 clarifai-9.5.3/clarifai/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-06-02 20:10:24.000000 clarifai-9.5.3/clarifai/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.074468 clarifai-9.5.3/clarifai/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.5.3/clarifai/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.5.3/clarifai/urls/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.066578 clarifai-9.5.3/clarifai.egg-info/
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-06-02 20:33:47.000000 clarifai-9.5.3/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     4063 2023-06-02 20:33:48.000000 clarifai-9.5.3/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-06-02 20:33:47.000000 clarifai-9.5.3/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2023-06-02 20:33:47.000000 clarifai-9.5.3/clarifai.egg-info/requires.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-06-02 20:33:47.000000 clarifai-9.5.3/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.074717 clarifai-9.5.3/clarifai_utils/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.074953 clarifai-9.5.3/clarifai_utils/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12239 2023-06-02 04:02:11.000000 clarifai-9.5.3/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.075366 clarifai-9.5.3/clarifai_utils/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.075840 clarifai-9.5.3/clarifai_utils/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.076587 clarifai-9.5.3/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10349 2023-06-02 04:02:11.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.077427 clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1414 2023-05-01 19:51:07.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.064719 clarifai-9.5.3/clarifai_utils/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.077579 clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.077839 clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.078101 clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.078240 clarifai-9.5.3/clarifai_utils/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.078483 clarifai-9.5.3/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.5.3/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    13040 2023-06-02 04:02:11.000000 clarifai-9.5.3/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.078625 clarifai-9.5.3/clarifai_utils/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     5130 2023-04-11 15:50:37.000000 clarifai-9.5.3/clarifai_utils/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.079822 clarifai-9.5.3/clarifai_utils/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.5.3/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.5.3/clarifai_utils/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.5.3/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.5.3/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.080338 clarifai-9.5.3/clarifai_utils/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.5.3/clarifai_utils/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-06-02 20:10:24.000000 clarifai-9.5.3/clarifai_utils/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-06-02 20:33:48.080590 clarifai-9.5.3/clarifai_utils/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.5.3/clarifai_utils/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.5.3/clarifai_utils/urls/helper.py
--rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-06-02 20:33:48.081015 clarifai-9.5.3/setup.cfg
--rw-r--r--   0 zeiler     (503) staff       (20)      897 2023-06-02 20:33:36.000000 clarifai-9.5.3/setup.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.687991 clarifai-9.5.4/
+-rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.5.4/LICENSE
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.5.4/MANIFEST.in
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-07 03:43:06.687494 clarifai-9.5.4/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.5.4/README.md
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.086894 clarifai-9.5.4/clarifai/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.111755 clarifai-9.5.4/clarifai/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    12447 2023-07-06 20:14:23.000000 clarifai-9.5.4/clarifai/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.131953 clarifai-9.5.4/clarifai/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.5.4/clarifai/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.151928 clarifai-9.5.4/clarifai/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/data_upload/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/data_upload/convert_csv.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.163732 clarifai-9.5.4/clarifai/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.5.4/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10486 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2093 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.172579 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1606 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.074494 clarifai-9.5.4/clarifai/data_upload/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.173216 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.175154 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.177317 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.178043 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.180432 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13040 2023-06-02 04:02:11.000000 clarifai-9.5.4/clarifai/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.207181 clarifai-9.5.4/clarifai/dataset_export/
+-rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.263748 clarifai-9.5.4/clarifai/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.5.4/clarifai/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.269555 clarifai-9.5.4/clarifai/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     8691 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.297011 clarifai-9.5.4/clarifai/models/model_serving/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.346975 clarifai-9.5.4/clarifai/models/model_serving/cli/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/cli/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3119 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/cli/repository.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      112 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/constants.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076585 clarifai-9.5.4/clarifai/models/model_serving/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.075923 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076022 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.385846 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2021 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076307 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076416 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.401464 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1958 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076687 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076799 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.427973 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2625 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.478042 clarifai-9.5.4/clarifai/models/model_serving/model_config/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1763 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/model_config/deploy.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/model_config/serializer.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4489 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/model_config/triton_config.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.532663 clarifai-9.5.4/clarifai/models/model_serving/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1548 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3743 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/model_types.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2334 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/output.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/pb_model.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3408 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.562087 clarifai-9.5.4/clarifai/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-06-02 20:36:17.000000 clarifai-9.5.4/clarifai/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.564353 clarifai-9.5.4/clarifai/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.5.4/clarifai/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.5.4/clarifai/urls/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.096804 clarifai-9.5.4/clarifai.egg-info/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     7394 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)      255 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/entry_points.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       52 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/requires.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.565482 clarifai-9.5.4/clarifai_utils/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.568124 clarifai-9.5.4/clarifai_utils/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    12447 2023-07-06 20:14:23.000000 clarifai-9.5.4/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.576809 clarifai-9.5.4/clarifai_utils/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.5.4/clarifai_utils/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.581329 clarifai-9.5.4/clarifai_utils/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/data_upload/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/data_upload/convert_csv.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.586000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10486 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2093 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.594900 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1606 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.079318 clarifai-9.5.4/clarifai_utils/data_upload/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.596226 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.597910 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.600318 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.602003 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.606551 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13040 2023-06-02 04:02:11.000000 clarifai-9.5.4/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.608606 clarifai-9.5.4/clarifai_utils/dataset_export/
+-rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.630441 clarifai-9.5.4/clarifai_utils/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.5.4/clarifai_utils/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.634556 clarifai-9.5.4/clarifai_utils/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     8691 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.637112 clarifai-9.5.4/clarifai_utils/models/model_serving/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.643938 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3119 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/repository.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      112 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/constants.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.081330 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.080616 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.080717 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.647383 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2021 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.080977 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.081093 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.650612 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1958 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.081435 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.081532 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.652647 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2625 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.657629 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1763 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/deploy.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/serializer.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4489 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/triton_config.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.663741 clarifai-9.5.4/clarifai_utils/models/model_serving/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1548 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3743 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/model_types.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2334 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/output.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/pb_model.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3408 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.680353 clarifai-9.5.4/clarifai_utils/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-06-02 20:36:17.000000 clarifai-9.5.4/clarifai_utils/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.683313 clarifai-9.5.4/clarifai_utils/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.5.4/clarifai_utils/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.5.4/clarifai_utils/urls/helper.py
+-rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-07-07 03:43:06.688134 clarifai-9.5.4/setup.cfg
+-rw-r--r--   0 zeiler     (503) staff       (20)     1297 2023-07-07 03:42:20.000000 clarifai-9.5.4/setup.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.686764 clarifai-9.5.4/tests/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2300 2023-07-06 20:15:48.000000 clarifai-9.5.4/tests/test_auth.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4771 2023-07-07 03:39:45.000000 clarifai-9.5.4/tests/test_modules.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3716 2023-01-03 21:48:03.000000 clarifai-9.5.4/tests/test_stub.py
```

### Comparing `clarifai-9.5.3/LICENSE` & `clarifai-9.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/PKG-INFO` & `clarifai-9.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.5.3
+Version: 9.5.4
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.5.3/README.md` & `clarifai-9.5.4/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/auth/helper.py` & `clarifai-9.5.4/clarifai/auth/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -283,38 +283,45 @@
         host = self._base
         port = 80
       channel = ClarifaiChannel.get_insecure_grpc_channel(base=host, port=port)
     stub = service_pb2_grpc.V2Stub(channel)
     return stub
 
   @property
-  def ui(self):
+  def ui(self) -> str:
+    """ Return the domain for the UI. """
     if self._ui not in ui_https_cache:
       raise Exception("Cannot determine if ui %s is https" % self._ui)
     https = ui_https_cache[self._ui]
     if https:
       if not self._ui.startswith("https://"):
         return "https://" + self._ui
       return self._ui
     if not self._ui.startswith("http://"):
       return "http://" + self._ui
     return self._ui
 
   @property
-  def base(self):
+  def base(self) -> str:
+    """ Return the base domain for the API. """
     if self._base not in base_https_cache:
       raise Exception("Cannot determine if base %s is https" % self._base)
     https = base_https_cache[self._base]
     if https:
       if not self._base.startswith("https://"):
         return "https://" + self._base
       return self._base
     if not self._base.startswith("http://"):
       return "http://" + self._base
     return self._base
 
+  @property
+  def pat(self) -> str:
+    """ Return the personal access token. """
+    return self._pat
+
   def __str__(self):
     return "ClarifaiAuthHelper:\n- base: %s\n- user_id: %s\n- app_id: %s\n" % (
         self._base,
         self.user_id,
         self.app_id,
     )
```

### Comparing `clarifai-9.5.3/clarifai/client/abc.py` & `clarifai-9.5.4/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/client/stub.py` & `clarifai-9.5.4/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/base.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/features.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/image.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import Iterator, List, Tuple, Union
 
 from clarifai_grpc.grpc.api import resources_pb2
 from google.protobuf.struct_pb2 import Struct
 from tqdm import tqdm
 
 from .base import ClarifaiDataset
@@ -53,14 +54,15 @@
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image_path = item.image_path
       label = item.label if isinstance(item.label, list) else [item.label]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       geo_info = item.geo_info
+      metadata.update({"filename": os.path.basename(image_path), "split": self.split})
 
       input_proto = self.create_input_protos(image_path, label, input_id, self.dataset_id,
                                              geo_info, metadata)
       self._all_input_protos.append(input_proto)
 
     return iter(self._all_input_protos)
 
@@ -141,15 +143,15 @@
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path
       labels = item.classes  # list:[l1,...,ln]
       bboxes = item.bboxes  # [[xmin,ymin,xmax,ymax],...,[xmin,ymin,xmax,ymax]]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
-      metadata.update({"label": labels, "split": self.split})
+      metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = item.geo_info
 
       input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
                                                    metadata)
       self._all_input_protos.append(input_image_proto)
 
       # iter over bboxes and classes
@@ -236,15 +238,15 @@
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path  # image path
       labels = item.classes  # list of class labels
       _polygons = item.polygons  # list of polygons: [[[x,y],...,[x,y]],...]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
-      metadata.update({"label": labels, "split": self.split})
+      metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = item.geo_info
 
       input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
                                                    metadata)
       self._all_input_protos.append(input_image_proto)
 
       ## Iterate over each masked image and create a proto for upload to clarifai
```

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/text.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,14 @@
     	A list of input protos
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Loading text data"):
       metadata = Struct()
       text = item.text
       labels = item.labels if isinstance(item.labels, list) else [item.labels]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
-      metadata.update({"label": labels, "split": self.split})
+      metadata.update({"split": self.split})
 
       input_proto = self.create_input_protos(text, labels, input_id, self.dataset_id, metadata)
 
       self._all_input_protos.append(input_proto)
 
     return iter(self._all_input_protos)
```

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     format for upload.
     Returns:
       VisualClassificationFeatures type generator.
     """
     #Creating label map
     with open(os.path.join(self.data_dir, "LOC_synset_mapping.txt")) as _file:
       for _id in _file:
-        self.label_map[_id.split(' ')[0]] = [
-            label.rstrip().lstrip() for label in _id[_id.find(' ') + 1:].split(',')
-        ]
+        #Removing the spaces,upper quotes and Converting to set to remove repetitions. Then converting to list for compatibility.
+        self.label_map[_id.split(" ")[0]] = list({
+            "".join(("".join((label.rstrip().lstrip().split(" ")))).split("'"))
+            for label in _id[_id.find(" ") + 1:].split(",")
+        })
 
     for _folder in os.listdir(os.path.join(self.data_dir, self.split)):
       try:
         concept = self.label_map[_folder]  #concepts
       except:
         continue
       folder_path = os.path.join(self.data_dir, self.split) + "/" + _folder
```

### Comparing `clarifai-9.5.3/clarifai/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.5.4/clarifai/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.5.4/clarifai/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.5.4/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/examples.py` & `clarifai-9.5.4/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/data_upload/upload.py` & `clarifai-9.5.4/clarifai/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/dataset_export/dataset_export_inputs.py` & `clarifai-9.5.4/clarifai/dataset_export/dataset_export_inputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import os
 import tempfile
 import zipfile
 from io import BytesIO
 
 import requests
 from clarifai_grpc.grpc.api import resources_pb2
+from google.protobuf.json_format import MessageToDict
 from PIL import ImageFile
 from tqdm import tqdm
 
+from clarifai.auth.helper import ClarifaiAuthHelper
+
 
 class DatasetExportReader:
   """
   Unpacks the zipfile from DatasetVersionExport
   - Downloads the temp archive onto disk
   - Reads DatasetVersionExports archive in memory without extracting all
   - Yield each api.Input object.
   """
 
-  def __init__(self, archive_url=None, local_archive_path=None):
+  def __init__(self, session, archive_url=None, local_archive_path=None):
 
     self.input_count = 0
     self.temp_file = None
+    self.session = session
 
     assert archive_url or local_archive_path, "Must use one input."
 
     if archive_url:
       print('url: %s' % archive_url)
       self.temp_file = self._download_temp_archive(archive_url)
       self.archive = zipfile.ZipFile(self.temp_file)
@@ -40,15 +44,15 @@
     print("Obtained file name list. %d entries." % len(self.file_name_list))
     self.split_dir = os.path.dirname(self.file_name_list[0]) if len(self.file_name_list) else ""
 
   def _download_temp_archive(self, archive_url, chunk_size=128):
     """
     Downloads the temp archive of InputBatches.
     """
-    r = requests.get(archive_url, stream=True)
+    r = self.session.get(archive_url, stream=True)
     temp_file = tempfile.TemporaryFile()
     for chunk in r.iter_content(chunk_size=chunk_size):
       temp_file.write(chunk)
 
     return temp_file
 
   def __len__(self):
@@ -82,76 +86,120 @@
     if self.temp_file:
       self.temp_file.close()
 
 
 class InputDownloader:
   """
   Takes an iterator or a list of api.Input instances as input,
-  and has a method for downloading all inputs (currently only images) of that data.
+  and has a method for downloading all inputs (image/text/audio/video) of that data.
   Has the ability of either writing to a new ZIP archive OR a filesystem directory.
   """
 
-  def __init__(self, input_iterator):
+  def __init__(self, session, input_iterator):
     self.input_iterator = input_iterator
     self.num_inputs = 0
     self.split_prefix = None
+    self.session = session
+    self.input_ext = dict(image=".jpg", text=".txt", audio=".wav", video=".mp4")
     if isinstance(self.input_iterator, DatasetExportReader):
       self.split_prefix = self.input_iterator.split_dir
 
-  def _save_image_to_archive(self, new_archive, hosted_url, name):
+  def _save_image_to_archive(self, new_archive, hosted_url, file_name):
     """
     Use PIL ImageFile to return image parsed from the response bytestring (from requests) and append to zip file.
     """
     p = ImageFile.Parser()
-    p.feed(requests.get(hosted_url).content)
+    p.feed(self.session.get(hosted_url).content)
     image = p.close()
     image_file = BytesIO()
     image.save(image_file, 'JPEG')
-    new_archive.writestr(name, image_file.getvalue())
+    new_archive.writestr(file_name, image_file.getvalue())
+
+  def _save_text_to_archive(self, new_archive, hosted_url, file_name):
+    """
+    Gets the text response bytestring (from requests) and append to zip file.
+    """
+    text_content = self.session.get(hosted_url).content
+    new_archive.writestr(file_name, text_content)
 
-  def _write_image_archive(self, save_path, split):
+  def _save_audio_to_archive(self, new_archive, hosted_url, file_name):
+    """
+    Gets the audio response bytestring (from requests) as chunks and append to zip file.
     """
-    Writes the image archive into prefix dir.
+    audio_response = requests.get(hosted_url, stream=True)
+    audio_stream = BytesIO()
+    # Retrieve the audio content in chunks and write to the BytesIO object
+    for chunk in audio_response.iter_content(chunk_size=128):
+      audio_stream.write(chunk)
+    new_archive.writestr(file_name, audio_stream.getvalue())
+
+  def _save_video_to_archive(self, new_archive, hosted_url, file_name):
+    """
+    Gets the video response bytestring (from requests) as chunks and append to zip file.
+    """
+    video_response = self.session.get(hosted_url)
+    video_stream = BytesIO()
+    # Retrieve the video content in chunks and write to the BytesIO object
+    for chunk in video_response.iter_content(chunk_size=128):
+      video_stream.write(chunk)
+    new_archive.writestr(file_name, video_stream.getvalue())
+
+  def _write_input_archive(self, save_path, split):
+    """
+    Writes the input archive into prefix dir.
     """
     try:
       total = len(self.input_iterator)
     except TypeError:
       total = None
     with zipfile.ZipFile(save_path, "a") as new_archive:
-      for input_ in tqdm(self.input_iterator, desc="Writing image archive", total=total):
-        # checks for image
-        hosted = input_.data.image.hosted
+      for input_ in tqdm(self.input_iterator, desc="Writing input archive", total=total):
+        # checks for input
+        data_dict = MessageToDict(input_.data)
+        input_type = list(
+            filter(lambda x: x in list(data_dict.keys()), list(self.input_ext.keys())))[0]
+        hosted = getattr(input_.data, input_type).hosted
         if hosted.prefix:
           assert 'orig' in hosted.sizes
           hosted_url = f"{hosted.prefix}/orig/{hosted.suffix}"
-          full_name = os.path.join(split, input_.id + ".jpg")
-
-          self._save_image_to_archive(new_archive, hosted_url, full_name)
+          file_name = os.path.join(split, input_.id + self.input_ext[input_type])
+          if input_type == "image":
+            self._save_image_to_archive(new_archive, hosted_url, file_name)
+          elif input_type == "text":
+            self._save_text_to_archive(new_archive, hosted_url, file_name)
+          elif input_type == "audio":
+            self._save_audio_to_archive(new_archive, hosted_url, file_name)
+          elif input_type == "video":
+            self._save_video_to_archive(new_archive, hosted_url, file_name)
           self.num_inputs += 1
 
   def _check_output_archive(self, save_path):
     try:
       archive = zipfile.ZipFile(save_path, 'r')
     except zipfile.BadZipFile as e:
       raise e
     assert len(
         archive.namelist()) == self.num_inputs, "Archive has %d inputs | expecting %d inputs" % (
             len(archive.namelist()), self.num_inputs)
 
-  def download_image_archive(self, save_path, split=None):
+  def download_input_archive(self, save_path, split=None):
     """
-    Downloads the archive from the URL into an archive of images in the directory format {split}/{image}.
+    Downloads the archive from the URL into an archive of inputs in the directory format {split}/{input_type}.
     """
-    self._write_image_archive(save_path, split=split or self.split_prefix)
+    self._write_input_archive(save_path, split=split or self.split_prefix)
     self._check_output_archive(save_path)
 
 
 if __name__ == "__main__":
   import sys
   if len(sys.argv) < 2:
     print(f"usage: {sys.argv[0]} <archive-url> [<save-path>]")
     sys.exit(2)
   archive_url = sys.argv[1]
   save_path = sys.argv[2] if len(sys.argv) > 2 else "output.zip"
+  metadata = getattr(ClarifaiAuthHelper.from_env(), "metadata")[0]
+  # Create a session object and set auth header
+  session = requests.Session()
+  session.headers.update({'Authorization': metadata[1]})
 
-  with DatasetExportReader(archive_url=archive_url) as reader:
-    InputDownloader(reader).download_image_archive(save_path=save_path)
+  with DatasetExportReader(session=session, archive_url=archive_url) as reader:
+    InputDownloader(session, reader).download_input_archive(save_path=save_path)
```

### Comparing `clarifai-9.5.3/clarifai/listing/concepts.py` & `clarifai-9.5.4/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/listing/datasets.py` & `clarifai-9.5.4/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/listing/inputs.py` & `clarifai-9.5.4/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/listing/installed_module_versions.py` & `clarifai-9.5.4/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/listing/lister.py` & `clarifai-9.5.4/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/listing/models.py` & `clarifai-9.5.4/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/listing/module_versions.py` & `clarifai-9.5.4/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/listing/modules.py` & `clarifai-9.5.4/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/modules/css.py` & `clarifai-9.5.4/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/modules/pages.py` & `clarifai-9.5.4/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai/modules/style.css` & `clarifai-9.5.4/clarifai/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai.egg-info/PKG-INFO` & `clarifai-9.5.4/clarifai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.5.3
+Version: 9.5.4
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.5.3/clarifai_utils/auth/helper.py` & `clarifai-9.5.4/clarifai_utils/auth/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -283,38 +283,45 @@
         host = self._base
         port = 80
       channel = ClarifaiChannel.get_insecure_grpc_channel(base=host, port=port)
     stub = service_pb2_grpc.V2Stub(channel)
     return stub
 
   @property
-  def ui(self):
+  def ui(self) -> str:
+    """ Return the domain for the UI. """
     if self._ui not in ui_https_cache:
       raise Exception("Cannot determine if ui %s is https" % self._ui)
     https = ui_https_cache[self._ui]
     if https:
       if not self._ui.startswith("https://"):
         return "https://" + self._ui
       return self._ui
     if not self._ui.startswith("http://"):
       return "http://" + self._ui
     return self._ui
 
   @property
-  def base(self):
+  def base(self) -> str:
+    """ Return the base domain for the API. """
     if self._base not in base_https_cache:
       raise Exception("Cannot determine if base %s is https" % self._base)
     https = base_https_cache[self._base]
     if https:
       if not self._base.startswith("https://"):
         return "https://" + self._base
       return self._base
     if not self._base.startswith("http://"):
       return "http://" + self._base
     return self._base
 
+  @property
+  def pat(self) -> str:
+    """ Return the personal access token. """
+    return self._pat
+
   def __str__(self):
     return "ClarifaiAuthHelper:\n- base: %s\n- user_id: %s\n- app_id: %s\n" % (
         self._base,
         self.user_id,
         self.app_id,
     )
```

### Comparing `clarifai-9.5.3/clarifai_utils/client/abc.py` & `clarifai-9.5.4/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/client/stub.py` & `clarifai-9.5.4/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import Iterator, List, Tuple, Union
 
 from clarifai_grpc.grpc.api import resources_pb2
 from google.protobuf.struct_pb2 import Struct
 from tqdm import tqdm
 
 from .base import ClarifaiDataset
@@ -53,14 +54,15 @@
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image_path = item.image_path
       label = item.label if isinstance(item.label, list) else [item.label]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       geo_info = item.geo_info
+      metadata.update({"filename": os.path.basename(image_path), "split": self.split})
 
       input_proto = self.create_input_protos(image_path, label, input_id, self.dataset_id,
                                              geo_info, metadata)
       self._all_input_protos.append(input_proto)
 
     return iter(self._all_input_protos)
 
@@ -141,15 +143,15 @@
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path
       labels = item.classes  # list:[l1,...,ln]
       bboxes = item.bboxes  # [[xmin,ymin,xmax,ymax],...,[xmin,ymin,xmax,ymax]]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
-      metadata.update({"label": labels, "split": self.split})
+      metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = item.geo_info
 
       input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
                                                    metadata)
       self._all_input_protos.append(input_image_proto)
 
       # iter over bboxes and classes
@@ -236,15 +238,15 @@
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path  # image path
       labels = item.classes  # list of class labels
       _polygons = item.polygons  # list of polygons: [[[x,y],...,[x,y]],...]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
-      metadata.update({"label": labels, "split": self.split})
+      metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = item.geo_info
 
       input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
                                                    metadata)
       self._all_input_protos.append(input_image_proto)
 
       ## Iterate over each masked image and create a proto for upload to clarifai
```

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,14 @@
     	A list of input protos
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Loading text data"):
       metadata = Struct()
       text = item.text
       labels = item.labels if isinstance(item.labels, list) else [item.labels]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
-      metadata.update({"label": labels, "split": self.split})
+      metadata.update({"split": self.split})
 
       input_proto = self.create_input_protos(text, labels, input_id, self.dataset_id, metadata)
 
       self._all_input_protos.append(input_proto)
 
     return iter(self._all_input_protos)
```

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     format for upload.
     Returns:
       VisualClassificationFeatures type generator.
     """
     #Creating label map
     with open(os.path.join(self.data_dir, "LOC_synset_mapping.txt")) as _file:
       for _id in _file:
-        self.label_map[_id.split(' ')[0]] = [
-            label.rstrip().lstrip() for label in _id[_id.find(' ') + 1:].split(',')
-        ]
+        #Removing the spaces,upper quotes and Converting to set to remove repetitions. Then converting to list for compatibility.
+        self.label_map[_id.split(" ")[0]] = list({
+            "".join(("".join((label.rstrip().lstrip().split(" ")))).split("'"))
+            for label in _id[_id.find(" ") + 1:].split(",")
+        })
 
     for _folder in os.listdir(os.path.join(self.data_dir, self.split)):
       try:
         concept = self.label_map[_folder]  #concepts
       except:
         continue
       folder_path = os.path.join(self.data_dir, self.split) + "/" + _folder
```

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/examples.py` & `clarifai-9.5.4/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/data_upload/upload.py` & `clarifai-9.5.4/clarifai_utils/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/dataset_export/dataset_export_inputs.py` & `clarifai-9.5.4/clarifai_utils/dataset_export/dataset_export_inputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import os
 import tempfile
 import zipfile
 from io import BytesIO
 
 import requests
 from clarifai_grpc.grpc.api import resources_pb2
+from google.protobuf.json_format import MessageToDict
 from PIL import ImageFile
 from tqdm import tqdm
 
+from clarifai.auth.helper import ClarifaiAuthHelper
+
 
 class DatasetExportReader:
   """
   Unpacks the zipfile from DatasetVersionExport
   - Downloads the temp archive onto disk
   - Reads DatasetVersionExports archive in memory without extracting all
   - Yield each api.Input object.
   """
 
-  def __init__(self, archive_url=None, local_archive_path=None):
+  def __init__(self, session, archive_url=None, local_archive_path=None):
 
     self.input_count = 0
     self.temp_file = None
+    self.session = session
 
     assert archive_url or local_archive_path, "Must use one input."
 
     if archive_url:
       print('url: %s' % archive_url)
       self.temp_file = self._download_temp_archive(archive_url)
       self.archive = zipfile.ZipFile(self.temp_file)
@@ -40,15 +44,15 @@
     print("Obtained file name list. %d entries." % len(self.file_name_list))
     self.split_dir = os.path.dirname(self.file_name_list[0]) if len(self.file_name_list) else ""
 
   def _download_temp_archive(self, archive_url, chunk_size=128):
     """
     Downloads the temp archive of InputBatches.
     """
-    r = requests.get(archive_url, stream=True)
+    r = self.session.get(archive_url, stream=True)
     temp_file = tempfile.TemporaryFile()
     for chunk in r.iter_content(chunk_size=chunk_size):
       temp_file.write(chunk)
 
     return temp_file
 
   def __len__(self):
@@ -82,76 +86,120 @@
     if self.temp_file:
       self.temp_file.close()
 
 
 class InputDownloader:
   """
   Takes an iterator or a list of api.Input instances as input,
-  and has a method for downloading all inputs (currently only images) of that data.
+  and has a method for downloading all inputs (image/text/audio/video) of that data.
   Has the ability of either writing to a new ZIP archive OR a filesystem directory.
   """
 
-  def __init__(self, input_iterator):
+  def __init__(self, session, input_iterator):
     self.input_iterator = input_iterator
     self.num_inputs = 0
     self.split_prefix = None
+    self.session = session
+    self.input_ext = dict(image=".jpg", text=".txt", audio=".wav", video=".mp4")
     if isinstance(self.input_iterator, DatasetExportReader):
       self.split_prefix = self.input_iterator.split_dir
 
-  def _save_image_to_archive(self, new_archive, hosted_url, name):
+  def _save_image_to_archive(self, new_archive, hosted_url, file_name):
     """
     Use PIL ImageFile to return image parsed from the response bytestring (from requests) and append to zip file.
     """
     p = ImageFile.Parser()
-    p.feed(requests.get(hosted_url).content)
+    p.feed(self.session.get(hosted_url).content)
     image = p.close()
     image_file = BytesIO()
     image.save(image_file, 'JPEG')
-    new_archive.writestr(name, image_file.getvalue())
+    new_archive.writestr(file_name, image_file.getvalue())
+
+  def _save_text_to_archive(self, new_archive, hosted_url, file_name):
+    """
+    Gets the text response bytestring (from requests) and append to zip file.
+    """
+    text_content = self.session.get(hosted_url).content
+    new_archive.writestr(file_name, text_content)
 
-  def _write_image_archive(self, save_path, split):
+  def _save_audio_to_archive(self, new_archive, hosted_url, file_name):
+    """
+    Gets the audio response bytestring (from requests) as chunks and append to zip file.
     """
-    Writes the image archive into prefix dir.
+    audio_response = requests.get(hosted_url, stream=True)
+    audio_stream = BytesIO()
+    # Retrieve the audio content in chunks and write to the BytesIO object
+    for chunk in audio_response.iter_content(chunk_size=128):
+      audio_stream.write(chunk)
+    new_archive.writestr(file_name, audio_stream.getvalue())
+
+  def _save_video_to_archive(self, new_archive, hosted_url, file_name):
+    """
+    Gets the video response bytestring (from requests) as chunks and append to zip file.
+    """
+    video_response = self.session.get(hosted_url)
+    video_stream = BytesIO()
+    # Retrieve the video content in chunks and write to the BytesIO object
+    for chunk in video_response.iter_content(chunk_size=128):
+      video_stream.write(chunk)
+    new_archive.writestr(file_name, video_stream.getvalue())
+
+  def _write_input_archive(self, save_path, split):
+    """
+    Writes the input archive into prefix dir.
     """
     try:
       total = len(self.input_iterator)
     except TypeError:
       total = None
     with zipfile.ZipFile(save_path, "a") as new_archive:
-      for input_ in tqdm(self.input_iterator, desc="Writing image archive", total=total):
-        # checks for image
-        hosted = input_.data.image.hosted
+      for input_ in tqdm(self.input_iterator, desc="Writing input archive", total=total):
+        # checks for input
+        data_dict = MessageToDict(input_.data)
+        input_type = list(
+            filter(lambda x: x in list(data_dict.keys()), list(self.input_ext.keys())))[0]
+        hosted = getattr(input_.data, input_type).hosted
         if hosted.prefix:
           assert 'orig' in hosted.sizes
           hosted_url = f"{hosted.prefix}/orig/{hosted.suffix}"
-          full_name = os.path.join(split, input_.id + ".jpg")
-
-          self._save_image_to_archive(new_archive, hosted_url, full_name)
+          file_name = os.path.join(split, input_.id + self.input_ext[input_type])
+          if input_type == "image":
+            self._save_image_to_archive(new_archive, hosted_url, file_name)
+          elif input_type == "text":
+            self._save_text_to_archive(new_archive, hosted_url, file_name)
+          elif input_type == "audio":
+            self._save_audio_to_archive(new_archive, hosted_url, file_name)
+          elif input_type == "video":
+            self._save_video_to_archive(new_archive, hosted_url, file_name)
           self.num_inputs += 1
 
   def _check_output_archive(self, save_path):
     try:
       archive = zipfile.ZipFile(save_path, 'r')
     except zipfile.BadZipFile as e:
       raise e
     assert len(
         archive.namelist()) == self.num_inputs, "Archive has %d inputs | expecting %d inputs" % (
             len(archive.namelist()), self.num_inputs)
 
-  def download_image_archive(self, save_path, split=None):
+  def download_input_archive(self, save_path, split=None):
     """
-    Downloads the archive from the URL into an archive of images in the directory format {split}/{image}.
+    Downloads the archive from the URL into an archive of inputs in the directory format {split}/{input_type}.
     """
-    self._write_image_archive(save_path, split=split or self.split_prefix)
+    self._write_input_archive(save_path, split=split or self.split_prefix)
     self._check_output_archive(save_path)
 
 
 if __name__ == "__main__":
   import sys
   if len(sys.argv) < 2:
     print(f"usage: {sys.argv[0]} <archive-url> [<save-path>]")
     sys.exit(2)
   archive_url = sys.argv[1]
   save_path = sys.argv[2] if len(sys.argv) > 2 else "output.zip"
+  metadata = getattr(ClarifaiAuthHelper.from_env(), "metadata")[0]
+  # Create a session object and set auth header
+  session = requests.Session()
+  session.headers.update({'Authorization': metadata[1]})
 
-  with DatasetExportReader(archive_url=archive_url) as reader:
-    InputDownloader(reader).download_image_archive(save_path=save_path)
+  with DatasetExportReader(session=session, archive_url=archive_url) as reader:
+    InputDownloader(session, reader).download_input_archive(save_path=save_path)
```

### Comparing `clarifai-9.5.3/clarifai_utils/listing/concepts.py` & `clarifai-9.5.4/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/listing/datasets.py` & `clarifai-9.5.4/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/listing/inputs.py` & `clarifai-9.5.4/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.5.4/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/listing/lister.py` & `clarifai-9.5.4/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/listing/models.py` & `clarifai-9.5.4/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/listing/module_versions.py` & `clarifai-9.5.4/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/listing/modules.py` & `clarifai-9.5.4/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/modules/css.py` & `clarifai-9.5.4/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/modules/pages.py` & `clarifai-9.5.4/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/clarifai_utils/modules/style.css` & `clarifai-9.5.4/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.3/setup.py` & `clarifai-9.5.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_namespace_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.5.3",
+    version="9.5.4",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
@@ -21,9 +21,18 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     license="Apache 2.0",
     python_requires='>=3.8',
     install_requires=[
         "clarifai-grpc>=9.5.0",
+        "tritonclient==2.34.0",
+        "packaging",
     ],
+    entry_points={
+        "console_scripts": [
+            "clarifai-model-upload-init = clarifai.models.model_serving.cli.repository:model_upload_init",
+            "clarifai-triton-zip = clarifai.models.model_serving.cli.model_zip:main",
+            "clarifai-upload-model = clarifai.models.model_serving.cli.deploy_cli:main"
+        ],
+    },
     include_package_data=True)
```


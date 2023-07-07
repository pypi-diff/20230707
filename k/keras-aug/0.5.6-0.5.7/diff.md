# Comparing `tmp/keras-aug-0.5.6.tar.gz` & `tmp/keras-aug-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-aug-0.5.6.tar", last modified: Sat Jul  1 09:12:13 2023, max compression
+gzip compressed data, was "keras-aug-0.5.7.tar", last modified: Fri Jul  7 15:14:29 2023, max compression
```

## Comparing `keras-aug-0.5.6.tar` & `keras-aug-0.5.7.tar`

### file list

```diff
@@ -1,184 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.034714 keras-aug-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-07-01 09:11:37.000000 keras-aug-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-07-01 09:12:13.034714 keras-aug-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-01 09:11:37.000000 keras-aug-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:12.998714 keras-aug-0.5.6/keras_aug/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.002714 keras-aug-0.5.6/keras_aug/core/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.002714 keras-aug-0.5.6/keras_aug/core/factor_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/constant_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/normal_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/uniform_factor_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.006714 keras-aug-0.5.6/keras_aug/datapoints/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.006714 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/converter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/iou_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_dense_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_ragged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_ragged_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/validate_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/bounding_box/validate_format_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.010714 keras-aug-0.5.6/keras_aug/datapoints/image/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/get_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/get_matrix_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/datapoints/image/ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.010714 keras-aug-0.5.6/keras_aug/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.010714 keras-aug-0.5.6/keras_aug/layers/__internal__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/base_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/base_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/graph_xla_mode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/mixed_precision_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/output_common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/with_bounding_boxes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/__internal__/with_ragged_image_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.010714 keras-aug-0.5.6/keras_aug/layers/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.014714 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/aug_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/aug_mix_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/rand_augment_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/trivial_augment_wide.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/auto/trivial_augment_wide_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.018714 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_flip_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_resize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_rotate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.022714 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/channel_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_blur_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_channel_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_clahe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_clahe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gamma_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_hsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_hsv_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_posterize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_posterize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_sharpness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_sharpness_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_solarize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.022714 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/cut_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/cut_mix_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mix_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mix_up_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mosaic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.026714 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_channel_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_cutout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_cutout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_erase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_erase_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_grid_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.026714 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_apply_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_choice_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/repeated_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/augmentation/utility/repeated_augment_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.030714 keras-aug-0.5.6/keras_aug/layers/base/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24353 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/base/vectorized_base_random_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22106 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/base/vectorized_base_random_layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.030714 keras-aug-0.5.6/keras_aug/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.030714 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/center_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/pad_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/resize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.030714 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/auto_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/equalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/equalize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/grayscale_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/identity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/invert.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/invert_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/normalize_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/rescale_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.034714 keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.034714 keras-aug-0.5.6/keras_aug/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/augmentation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/conditional_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-01 09:11:37.000000 keras-aug-0.5.6/keras_aug/utils/distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:12:13.002714 keras-aug-0.5.6/keras_aug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 09:12:12.000000 keras-aug-0.5.6/keras_aug.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-01 09:11:37.000000 keras-aug-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:12:13.034714 keras-aug-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.997915 keras-aug-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-07-07 15:13:52.000000 keras-aug-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-07-07 15:14:28.997915 keras-aug-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-07 15:13:52.000000 keras-aug-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.969914 keras-aug-0.5.7/keras_aug/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.969914 keras-aug-0.5.7/keras_aug/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.973914 keras-aug-0.5.7/keras_aug/core/factor_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/constant_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/normal_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/uniform_factor_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/core/keras_random_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.973914 keras-aug-0.5.7/keras_aug/datapoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.973914 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/converter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/iou_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/to_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/to_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/to_ragged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/to_ragged_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/validate_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/bounding_box/validate_format_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.977914 keras-aug-0.5.7/keras_aug/datapoints/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/image/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/image/get_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/image/get_matrix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/image/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/datapoints/image/ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.977914 keras-aug-0.5.7/keras_aug/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.977914 keras-aug-0.5.7/keras_aug/layers/__internal__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/base_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/base_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/graph_xla_mode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/mixed_precision_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/output_common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/with_bounding_boxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/__internal__/with_ragged_image_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.977914 keras-aug-0.5.7/keras_aug/layers/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.977914 keras-aug-0.5.7/keras_aug/layers/augmentation/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13037 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/auto/aug_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/auto/aug_mix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/auto/rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/auto/rand_augment_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/auto/trivial_augment_wide.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/auto/trivial_augment_wide_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.981914 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_flip_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_resize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_rotate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.985914 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/channel_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_blur_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_channel_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_clahe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_clahe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_gamma_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_hsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_hsv_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_posterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_posterize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_sharpness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_sharpness_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_solarize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.989915 keras-aug-0.5.7/keras_aug/layers/augmentation/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/mix/cut_mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/mix/cut_mix_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/mix/mix_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/mix/mix_up_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/mix/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/mix/mosaic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.989915 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_channel_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_cutout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_erase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_erase_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_grid_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.989915 keras-aug-0.5.7/keras_aug/layers/augmentation/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/utility/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/utility/random_apply_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/utility/random_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/utility/random_choice_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/utility/repeated_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/augmentation/utility/repeated_augment_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.989915 keras-aug-0.5.7/keras_aug/layers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24357 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/base/vectorized_base_random_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22106 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/base/vectorized_base_random_layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.993914 keras-aug-0.5.7/keras_aug/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.993914 keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/center_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/pad_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/resize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.997915 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/auto_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/equalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/equalize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/grayscale_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/identity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/invert_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/normalize_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/rescale_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.997915 keras-aug-0.5.7/keras_aug/layers/preprocessing/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.997915 keras-aug-0.5.7/keras_aug/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/utils/augmentation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/utils/conditional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/utils/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-07 15:13:52.000000 keras-aug-0.5.7/keras_aug/utils/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:14:28.969914 keras-aug-0.5.7/keras_aug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-07-07 15:14:28.000000 keras-aug-0.5.7/keras_aug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-07 15:14:28.000000 keras-aug-0.5.7/keras_aug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:14:28.000000 keras-aug-0.5.7/keras_aug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 15:14:28.000000 keras-aug-0.5.7/keras_aug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 15:14:28.000000 keras-aug-0.5.7/keras_aug.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-07 15:13:52.000000 keras-aug-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:14:28.997915 keras-aug-0.5.7/setup.cfg
```

### Comparing `keras-aug-0.5.6/LICENSE` & `keras-aug-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/PKG-INFO` & `keras-aug-0.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-aug
-Version: 0.5.6
+Version: 0.5.7
 Summary: A library that includes pure TF/Keras preprocessing and augmentation layers
 Author: Hongyu, Chiu (james77777778)
 License:    Copyright 2023 The KerasAug Authors. All rights reserved.
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -238,15 +238,15 @@
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.12.0+-success.svg)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-aug/actions.yml?label=tests)](https://github.com/james77777778/keras-aug/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-aug/branch/main/graph/badge.svg?token=81ELI3VH7H)](https://codecov.io/gh/james77777778/keras-aug)
 [![PyPI](https://img.shields.io/pypi/v/keras-aug)](https://pypi.org/project/keras-aug/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-aug)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/keras-aug/issues)
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://keras-aug-rqtoxd8zk3.streamlit.app/)
 
 ## Description
 
 KerasAug is a library that includes pure TF/Keras preprocessing and augmentation layers, providing support for various data types such as images, labels, bounding boxes, segmentation masks, and more.
 
 <div align="center">
 <img width="45%" src="https://user-images.githubusercontent.com/20734616/238531125-f0a07f50-423b-4be2-9dcd-a3cc459a261c.gif"> <img width="45%" src="https://user-images.githubusercontent.com/20734616/238531295-22cd5567-0709-46d5-bf31-7baad05b91d2.gif">
@@ -257,32 +257,32 @@
 
 KerasAug aims to provide fast, robust and user-friendly preprocessing and augmentation layers, facilitating seamless integration with TensorFlow, Keras and KerasCV.
 
 KerasAug is:
 
 - 🚀 faster than [KerasCV](https://github.com/keras-team/keras-cv) which is an official Keras library
 - 🧰 supporting various data types, including **images, labels, bounding boxes, segmentation masks**, and more.
-- ❤️ dependent only on TensorFlow and KerasCV
+- ❤️ dependent only on TensorFlow
 - 🌟 seamlessly integrating with the `tf.data` and `tf.keras.Model` APIs
-- 🔥 compatible with GPU
+- 🔥 compatible with GPU and mixed precision (`mixed_float16` and `mixed_bfloat16`)
 
 Check out the demo website powered by Streamlit:
 
-<a href="https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/"><img width="50%" align="right" src="https://user-images.githubusercontent.com/20734616/242836830-bd0a457d-fa6f-410c-a267-af628f5bb5ec.JPG"></a>
+<a href="https://keras-aug-rqtoxd8zk3.streamlit.app/"><img width="50%" align="right" src="https://user-images.githubusercontent.com/20734616/242836830-bd0a457d-fa6f-410c-a267-af628f5bb5ec.JPG"></a>
 
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://keras-aug-rqtoxd8zk3.streamlit.app/)
 
 - Apply a transformation to the default or uploaded image
 - Adjust the arguments of the specified layer
 
 ## Why KerasAug?
 
 1. KerasAug is generally faster than KerasCV
 
-    > RandomCropAndResize in KerasAug exhibits a remarkable speed-up of **+1342%** compared to KerasAug. See [keras-aug/benchmarks](https://github.com/james77777778/keras-aug/tree/main/benchmarks) for more details.
+    > RandomCropAndResize in KerasAug exhibits a remarkable speed-up of **+1150%** compared to KerasAug. See [keras-aug/benchmarks](https://github.com/james77777778/keras-aug/tree/main/benchmarks) for more details.
 
 2. The APIs of KerasAug are highly stable compared to KerasCV
 
     > KerasCV struggles to reproduce the YOLOV8 training pipeline, whereas KerasAug executes it flawlessly. See [Quickstart](https://github.com/james77777778/keras-aug/tree/main#quickstart) for more details.
 
 3. KerasAug comes with built-in support for mixed precision training
 
@@ -524,39 +524,40 @@
 
 </details>
 
 ## Benchmark
 
 KerasAug is generally faster than KerasCV.
 
-| Type           | Layer                    | KerasAug | KerasCV   |        |
-|----------------|--------------------------|----------|-----------|--------|
-| Geometry       | RandomHFlip              | 2148     | 1859      | +15%   |
-|                | RandomVFlip              | 2182     | 2075      | +5%    |
-|                | RandomRotate             | 2451     | 1829      | +34%   |
-|                | RandomAffine             | 2141     | 1240      | +73%   |
-|                | RandomCropAndResize      | 3014     | 209       | +1342% |
-|                | Resize (224, 224)        | 2853     | 213       | +1239% |
-| Intensity      | RandomBrightness         | 3028     | 3097      | close  |
-|                | RandomContrast           | 2806     | 2645      | +6%    |
-|                | RandomBrightnessContrast | 3068     | 612       | +401%  |
-|                | RandomColorJitter        | 1932     | 1221      | +58%   |
-|                | RandomGaussianBlur       | 2758     | 207       | +1232% |
-|                | Grayscale                | 2841     | 2872      | close  |
-|                | Equalize                 | 206      | 139       | +48%   |
-|                | AutoContrast             | 3116     | 2991      | +4%    |
-|                | Posterize                | 2917     | 2445      | +19%   |
-|                | Solarize                 | 3025     | 2882      | +5%    |
-|                | Sharpness                | 2969     | 2915      | close  |
-| Regularization | RandomCutout             | 3222     | 3268      | close  |
-|                | RandomGridMask           | 947      | 197       | +381%  |
-| Mix            | CutMix                   | 2671     | 2445      | +9%    |
-|                | MixUp                    | 2593     | 1996      | +29%   |
-| Auto           | AugMix                   | 83       | X (Error) | X      |
-|                | RandAugment              | 282      | 249       | +13%   |
+| Type           | Layer                      | KerasAug | KerasCV   |        |
+|----------------|----------------------------|----------|-----------|--------|
+| Geometry       | RandomHFlip                | 2123     | 1956      | fair   |
+|                | RandomVFlip                | 1871     | 1767      | fair   |
+|                | RandomRotate               | 1703     | 1723      | fair   |
+|                | RandomAffine               | 2578     | 2355      | fair   |
+|                | RandomCropAndResize        | 2664     | 213       | +1150% |
+|                | Resize (224, 224)          | 2480     | 222       | +1017% |
+| Intensity      | RandomBrightness           | 3052     | 2768      | fair   |
+|                | RandomContrast\*           | 3099     | 2976      | fair   |
+|                | RandomBrightnessContrast\* | 2881     | 609       | +373%  |
+|                | RandomColorJitter\*        | 2013     | 597       | +237%  |
+|                | RandomGaussianBlur         | 2345     | 203       | +1055% |
+|                | Invert                     | 2691     | X         |        |
+|                | Grayscale                  | 2917     | 3116      | fair   |
+|                | Equalize                   | 196      | 139       | +41%   |
+|                | AutoContrast               | 3095     | 3025      | fair   |
+|                | Posterize                  | 3033     | 2144      | fair   |
+|                | Solarize                   | 3133     | 2972      | fair   |
+|                | Sharpness                  | 2982     | 2833      | fair   |
+| Regularization | RandomCutout               | 2994     | 2795      | fair   |
+|                | RandomGridMask             | 918      | 196       | +368%  |
+| Mix            | CutMix                     | 2967     | 2957      | fair   |
+|                | MixUp                      | 1897     | 1861      | fair   |
+| Auto           | AugMix                     | 79       | X (Error) |        |
+|                | RandAugment                | 301      | 246       | +22%   |
 
 > **Note**
 > FPS (frames per second)
 
 Please refer to [benchmarks/README.md](benchmarks/README.md) for more details.
 
 ## Citing KerasAug
```

### Comparing `keras-aug-0.5.6/README.md` & `keras-aug-0.5.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.12.0+-success.svg)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-aug/actions.yml?label=tests)](https://github.com/james77777778/keras-aug/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-aug/branch/main/graph/badge.svg?token=81ELI3VH7H)](https://codecov.io/gh/james77777778/keras-aug)
 [![PyPI](https://img.shields.io/pypi/v/keras-aug)](https://pypi.org/project/keras-aug/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-aug)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/keras-aug/issues)
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://keras-aug-rqtoxd8zk3.streamlit.app/)
 
 ## Description
 
 KerasAug is a library that includes pure TF/Keras preprocessing and augmentation layers, providing support for various data types such as images, labels, bounding boxes, segmentation masks, and more.
 
 <div align="center">
 <img width="45%" src="https://user-images.githubusercontent.com/20734616/238531125-f0a07f50-423b-4be2-9dcd-a3cc459a261c.gif"> <img width="45%" src="https://user-images.githubusercontent.com/20734616/238531295-22cd5567-0709-46d5-bf31-7baad05b91d2.gif">
@@ -23,32 +23,32 @@
 
 KerasAug aims to provide fast, robust and user-friendly preprocessing and augmentation layers, facilitating seamless integration with TensorFlow, Keras and KerasCV.
 
 KerasAug is:
 
 - 🚀 faster than [KerasCV](https://github.com/keras-team/keras-cv) which is an official Keras library
 - 🧰 supporting various data types, including **images, labels, bounding boxes, segmentation masks**, and more.
-- ❤️ dependent only on TensorFlow and KerasCV
+- ❤️ dependent only on TensorFlow
 - 🌟 seamlessly integrating with the `tf.data` and `tf.keras.Model` APIs
-- 🔥 compatible with GPU
+- 🔥 compatible with GPU and mixed precision (`mixed_float16` and `mixed_bfloat16`)
 
 Check out the demo website powered by Streamlit:
 
-<a href="https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/"><img width="50%" align="right" src="https://user-images.githubusercontent.com/20734616/242836830-bd0a457d-fa6f-410c-a267-af628f5bb5ec.JPG"></a>
+<a href="https://keras-aug-rqtoxd8zk3.streamlit.app/"><img width="50%" align="right" src="https://user-images.githubusercontent.com/20734616/242836830-bd0a457d-fa6f-410c-a267-af628f5bb5ec.JPG"></a>
 
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://keras-aug-rqtoxd8zk3.streamlit.app/)
 
 - Apply a transformation to the default or uploaded image
 - Adjust the arguments of the specified layer
 
 ## Why KerasAug?
 
 1. KerasAug is generally faster than KerasCV
 
-    > RandomCropAndResize in KerasAug exhibits a remarkable speed-up of **+1342%** compared to KerasAug. See [keras-aug/benchmarks](https://github.com/james77777778/keras-aug/tree/main/benchmarks) for more details.
+    > RandomCropAndResize in KerasAug exhibits a remarkable speed-up of **+1150%** compared to KerasAug. See [keras-aug/benchmarks](https://github.com/james77777778/keras-aug/tree/main/benchmarks) for more details.
 
 2. The APIs of KerasAug are highly stable compared to KerasCV
 
     > KerasCV struggles to reproduce the YOLOV8 training pipeline, whereas KerasAug executes it flawlessly. See [Quickstart](https://github.com/james77777778/keras-aug/tree/main#quickstart) for more details.
 
 3. KerasAug comes with built-in support for mixed precision training
 
@@ -290,39 +290,40 @@
 
 </details>
 
 ## Benchmark
 
 KerasAug is generally faster than KerasCV.
 
-| Type           | Layer                    | KerasAug | KerasCV   |        |
-|----------------|--------------------------|----------|-----------|--------|
-| Geometry       | RandomHFlip              | 2148     | 1859      | +15%   |
-|                | RandomVFlip              | 2182     | 2075      | +5%    |
-|                | RandomRotate             | 2451     | 1829      | +34%   |
-|                | RandomAffine             | 2141     | 1240      | +73%   |
-|                | RandomCropAndResize      | 3014     | 209       | +1342% |
-|                | Resize (224, 224)        | 2853     | 213       | +1239% |
-| Intensity      | RandomBrightness         | 3028     | 3097      | close  |
-|                | RandomContrast           | 2806     | 2645      | +6%    |
-|                | RandomBrightnessContrast | 3068     | 612       | +401%  |
-|                | RandomColorJitter        | 1932     | 1221      | +58%   |
-|                | RandomGaussianBlur       | 2758     | 207       | +1232% |
-|                | Grayscale                | 2841     | 2872      | close  |
-|                | Equalize                 | 206      | 139       | +48%   |
-|                | AutoContrast             | 3116     | 2991      | +4%    |
-|                | Posterize                | 2917     | 2445      | +19%   |
-|                | Solarize                 | 3025     | 2882      | +5%    |
-|                | Sharpness                | 2969     | 2915      | close  |
-| Regularization | RandomCutout             | 3222     | 3268      | close  |
-|                | RandomGridMask           | 947      | 197       | +381%  |
-| Mix            | CutMix                   | 2671     | 2445      | +9%    |
-|                | MixUp                    | 2593     | 1996      | +29%   |
-| Auto           | AugMix                   | 83       | X (Error) | X      |
-|                | RandAugment              | 282      | 249       | +13%   |
+| Type           | Layer                      | KerasAug | KerasCV   |        |
+|----------------|----------------------------|----------|-----------|--------|
+| Geometry       | RandomHFlip                | 2123     | 1956      | fair   |
+|                | RandomVFlip                | 1871     | 1767      | fair   |
+|                | RandomRotate               | 1703     | 1723      | fair   |
+|                | RandomAffine               | 2578     | 2355      | fair   |
+|                | RandomCropAndResize        | 2664     | 213       | +1150% |
+|                | Resize (224, 224)          | 2480     | 222       | +1017% |
+| Intensity      | RandomBrightness           | 3052     | 2768      | fair   |
+|                | RandomContrast\*           | 3099     | 2976      | fair   |
+|                | RandomBrightnessContrast\* | 2881     | 609       | +373%  |
+|                | RandomColorJitter\*        | 2013     | 597       | +237%  |
+|                | RandomGaussianBlur         | 2345     | 203       | +1055% |
+|                | Invert                     | 2691     | X         |        |
+|                | Grayscale                  | 2917     | 3116      | fair   |
+|                | Equalize                   | 196      | 139       | +41%   |
+|                | AutoContrast               | 3095     | 3025      | fair   |
+|                | Posterize                  | 3033     | 2144      | fair   |
+|                | Solarize                   | 3133     | 2972      | fair   |
+|                | Sharpness                  | 2982     | 2833      | fair   |
+| Regularization | RandomCutout               | 2994     | 2795      | fair   |
+|                | RandomGridMask             | 918      | 196       | +368%  |
+| Mix            | CutMix                     | 2967     | 2957      | fair   |
+|                | MixUp                      | 1897     | 1861      | fair   |
+| Auto           | AugMix                     | 79       | X (Error) |        |
+|                | RandAugment                | 301      | 246       | +22%   |
 
 > **Note**
 > FPS (frames per second)
 
 Please refer to [benchmarks/README.md](benchmarks/README.md) for more details.
 
 ## Citing KerasAug
```

### Comparing `keras-aug-0.5.6/keras_aug/conftest.py` & `keras-aug-0.5.7/keras_aug/conftest.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/core/__init__.py` & `keras-aug-0.5.7/keras_aug/core/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/constant_factor_sampler.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/constant_factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/constant_factor_sampler_test.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/constant_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/factor_sampler.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/factor_sampler.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/normal_factor_sampler.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/normal_factor_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import keras
-import keras.backend
 import tensorflow as tf
 
 from keras_aug.core.factor_sampler.factor_sampler import FactorSampler
+from keras_aug.core.keras_random_generator import KerasRandomGenerator
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class NormalFactorSampler(FactorSampler):
     """NormalFactorSampler samples factors from a normal distribution.
 
     Args:
@@ -22,17 +22,15 @@
 
     def __init__(self, mean, stddev, min_value, max_value, seed=None):
         self.mean = mean
         self.stddev = stddev
         self.min_value = min_value
         self.max_value = max_value
         self.seed = seed
-        self.rng = keras.backend.RandomGenerator(
-            seed=seed, rng_type="stateless"
-        )
+        self.rng = KerasRandomGenerator(seed=seed, rng_type="stateless")
 
     def __call__(self, shape=(), dtype="float32"):
         return tf.clip_by_value(
             self.rng.random_normal(
                 shape=shape,
                 mean=self.mean,
                 stddev=self.stddev,
```

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/normal_factor_sampler_test.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/normal_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/signed_constant_factor_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import keras
-import keras.backend
 import tensorflow as tf
 
 from keras_aug.core.factor_sampler.factor_sampler import FactorSampler
+from keras_aug.core.keras_random_generator import KerasRandomGenerator
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class SignedConstantFactorSampler(FactorSampler):
     """SignedConstantFactorSampler samples the same factor for every call to
     ``__call__()`` and randomly inverts the sampled factors.
 
@@ -22,17 +22,15 @@
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
     """
 
     def __init__(self, value, rate=0.5, seed=None):
         self.value = value
         self.rate = rate
         self.seed = seed
-        self.rng = keras.backend.RandomGenerator(
-            seed=seed, rng_type="stateless"
-        )
+        self.rng = KerasRandomGenerator(seed=seed, rng_type="stateless")
 
     def __call__(self, shape=(), dtype="float32"):
         factors = tf.ones(shape=shape, dtype=dtype) * self.value
         negates = self.rng.random_uniform(
             shape=shape, minval=0, maxval=1, dtype=tf.float32
         )
         negates = tf.cast(tf.where(negates > self.rate, -1.0, 1.0), dtype=dtype)
```

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/signed_constant_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/signed_normal_factor_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import keras
-import keras.backend
 import tensorflow as tf
 
 from keras_aug.core.factor_sampler.factor_sampler import FactorSampler
+from keras_aug.core.keras_random_generator import KerasRandomGenerator
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class SignedNormalFactorSampler(FactorSampler):
     """SignedNormalFactorSampler samples factors from a normal distribution and
     randomly inverts the sampled factors.
 
@@ -30,17 +30,15 @@
     def __init__(self, mean, stddev, min_value, max_value, rate=0.5, seed=None):
         self.mean = mean
         self.stddev = stddev
         self.min_value = min_value
         self.max_value = max_value
         self.rate = rate
         self.seed = seed
-        self.rng = keras.backend.RandomGenerator(
-            seed=seed, rng_type="stateless"
-        )
+        self.rng = KerasRandomGenerator(seed=seed, rng_type="stateless")
 
     def __call__(self, shape=(), dtype="float32"):
         if self.stddev != 0:
             factors = self.rng.random_normal(
                 shape=shape,
                 mean=self.mean,
                 stddev=self.stddev,
```

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/signed_normal_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/uniform_factor_sampler.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/uniform_factor_sampler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import keras
-import keras.backend
 
 from keras_aug.core.factor_sampler.factor_sampler import FactorSampler
+from keras_aug.core.keras_random_generator import KerasRandomGenerator
 
 
 @keras.utils.register_keras_serializable(package="keras_aug")
 class UniformFactorSampler(FactorSampler):
     """UniformFactorSampler samples factors uniformly from a range.
 
     Args:
@@ -17,17 +17,15 @@
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
     """
 
     def __init__(self, lower, upper, seed=None):
         self.lower = lower
         self.upper = upper
         self.seed = seed
-        self.rng = keras.backend.RandomGenerator(
-            seed=seed, rng_type="stateless"
-        )
+        self.rng = KerasRandomGenerator(seed=seed, rng_type="stateless")
 
     def __call__(self, shape=(), dtype="float32"):
         return self.rng.random_uniform(
             shape,
             minval=self.lower,
             maxval=self.upper,
             dtype=dtype,
```

### Comparing `keras-aug-0.5.6/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py` & `keras-aug-0.5.7/keras_aug/core/factor_sampler/uniform_factor_sampler_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/__init__.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/converter.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/converter.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/converter_test.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/converter_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/iou.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/iou.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/iou_test.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/iou_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_dense.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/to_dense.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_dense_test.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/to_dense_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_ragged.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/to_ragged.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/to_ragged_test.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/to_ragged_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/utils.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/utils.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/utils_test.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/utils_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/validate_format.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/validate_format.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/bounding_box/validate_format_test.py` & `keras-aug-0.5.7/keras_aug/datapoints/bounding_box/validate_format_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/image/__init__.py` & `keras-aug-0.5.7/keras_aug/datapoints/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/image/fill.py` & `keras-aug-0.5.7/keras_aug/datapoints/image/fill.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/image/get_matrix.py` & `keras-aug-0.5.7/keras_aug/datapoints/image/get_matrix.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/datapoints/image/ops.py` & `keras-aug-0.5.7/keras_aug/datapoints/image/ops.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/__init__.py` & `keras-aug-0.5.7/keras_aug/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/__internal__/base_layer.py` & `keras-aug-0.5.7/keras_aug/layers/__internal__/base_layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Copied from:
-https://github.com/keras-team/keras/blob/f9336cc5114b4a9429a242deb264b707379646b7/keras/engine/base_layer.py
+https://github.com/keras-team/keras/blob/4829ddfc5fdcb84efe19b5e571f4be8dda89a3e1/keras/engine/base_layer.py
 
 Remove __init__ docstring to prevent docstring population
 """  # noqa: E501
 
 import tensorflow as tf
-from keras import backend
 from tensorflow import keras
 
+from keras_aug.core.keras_random_generator import KerasRandomGenerator
+
 
 class BaseRandomLayer(keras.layers.Layer):
     """A layer handle the random number creation and savemodel behavior.
 
     Args:
           seed: optional integer, used to create RandomGenerator.
           force_generator: boolean, default to False, whether to force the
@@ -26,15 +27,15 @@
     """
 
     @tf.__internal__.tracking.no_automatic_dependency_tracking
     def __init__(
         self, seed=None, force_generator=False, rng_type=None, **kwargs
     ):
         super().__init__(**kwargs)
-        self._random_generator = backend.RandomGenerator(
+        self._random_generator = KerasRandomGenerator(
             seed, force_generator=force_generator, rng_type=rng_type
         )
 
     def build(self, input_shape):
         super().build(input_shape)
         self._random_generator._maybe_init()
```

### Comparing `keras-aug-0.5.6/keras_aug/layers/__internal__/base_layer_test.py` & `keras-aug-0.5.7/keras_aug/layers/__internal__/base_layer_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tempfile
 
 import tensorflow as tf
-from keras import backend
 
+from keras_aug.core.keras_random_generator import KerasRandomGenerator
 from keras_aug.layers.__internal__.base_layer import BaseRandomLayer
 
 
 class BaseRandomLayerTest(tf.test.TestCase):
     def test_saved_model(self):
         base_random_layer = BaseRandomLayer(
             force_generator=True, rng_type="stateless"
@@ -32,8 +32,8 @@
     def test_lookup_dependency(self):
         base_random_layer = BaseRandomLayer(
             force_generator=True, rng_type="stateless"
         )
 
         rng = base_random_layer._lookup_dependency("_random_generator")
 
-        self.assertTrue(isinstance(rng, backend.RandomGenerator))
+        self.assertTrue(isinstance(rng, KerasRandomGenerator))
```

### Comparing `keras-aug-0.5.6/keras_aug/layers/__internal__/config_test.py` & `keras-aug-0.5.7/keras_aug/layers/__internal__/config_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/__internal__/graph_xla_mode_test.py` & `keras-aug-0.5.7/keras_aug/layers/__internal__/graph_xla_mode_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/__internal__/mixed_precision_test.py` & `keras-aug-0.5.7/keras_aug/layers/__internal__/mixed_precision_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/__internal__/output_common_test.py` & `keras-aug-0.5.7/keras_aug/layers/__internal__/output_common_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/__internal__/with_bounding_boxes_test.py` & `keras-aug-0.5.7/keras_aug/layers/__internal__/with_bounding_boxes_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/__internal__/with_ragged_image_test.py` & `keras-aug-0.5.7/keras_aug/layers/__internal__/with_ragged_image_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/__init__.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/aug_mix.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/auto/aug_mix.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/aug_mix_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/auto/aug_mix_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/rand_augment.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/auto/rand_augment.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/rand_augment_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/auto/rand_augment_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/auto/trivial_augment_wide.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/auto/trivial_augment_wide.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_affine.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_affine.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_affine_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_affine_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_crop_and_resize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_crop_and_resize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_crop_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_flip.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_flip_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_flip_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_resize.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_resize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_resize_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_resize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_rotate.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_rotate.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_rotate_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_rotate_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_zoom_and_crop.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/geometry/random_zoom_and_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/channel_shuffle.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/channel_shuffle_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_blur.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_blur.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_blur_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_blur_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_channel_shift.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_channel_shift.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_channel_shift_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_clahe.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_clahe.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_clahe_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_clahe_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_color_jitter.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_color_jitter_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gamma.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_gamma.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gamma_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_gamma_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_gaussian_blur_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_hsv.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_hsv.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_hsv_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_hsv_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_jpeg_quality.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_jpeg_quality_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_posterize.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_posterize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_posterize_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_posterize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_sharpness.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_sharpness.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_sharpness_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_sharpness_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_solarize.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_solarize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/intensity/random_solarize_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/intensity/random_solarize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/cut_mix.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/mix/cut_mix.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/cut_mix_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/mix/cut_mix_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mix_up.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/mix/mix_up.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mix_up_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/mix/mix_up_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mosaic.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/mix/mosaic.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/mix/mosaic_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/mix/mosaic_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_channel_dropout.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_channel_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_channel_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_cutout.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_cutout.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_cutout_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_cutout_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_erase.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_erase.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_erase_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_erase_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_grid_mask.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_grid_mask.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/regularization/random_grid_mask_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_apply.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/utility/random_apply.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_apply_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/utility/random_apply_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_choice.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/utility/random_choice.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/random_choice_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/utility/random_choice_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/repeated_augment.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/utility/repeated_augment.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/augmentation/utility/repeated_augment_test.py` & `keras-aug-0.5.7/keras_aug/layers/augmentation/utility/repeated_augment_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/base/vectorized_base_random_layer.py` & `keras-aug-0.5.7/keras_aug/layers/base/vectorized_base_random_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         class SubclassLayer(VectorizedBaseImageAugmentationLayer):
             def __init__(self):
                 super().__init__()
                 self.force_output_dense_images = True
 
     Note that since the randomness is also a common functionality, this layer
-    also includes a keras.backend.RandomGenerator, which can be used to
+    also includes a keras.src.backend.RandomGenerator, which can be used to
     produce the random numbers. The random number generator is stored in the
     `self._random_generator` attribute.
 
     References:
         - `KerasCV <https://github.com/keras-team/keras-cv>`_
     """
```

### Comparing `keras-aug-0.5.6/keras_aug/layers/base/vectorized_base_random_layer_test.py` & `keras-aug-0.5.7/keras_aug/layers/base/vectorized_base_random_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/__init__.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/center_crop.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/center_crop_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/center_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/pad_if_needed.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/pad_if_needed_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/resize.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/resize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/geometry/resize_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/geometry/resize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/auto_contrast.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/auto_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/auto_contrast_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/equalize.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/equalize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/equalize_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/equalize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/grayscale.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/grayscale.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/grayscale_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/grayscale_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/identity.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/identity.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/identity_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/identity_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/invert.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/invert.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/normalize.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/normalize.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/normalize_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/normalize_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/rescale.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/rescale.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/intensity/rescale_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/intensity/rescale_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/utility/sanitize_bounding_box.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py` & `keras-aug-0.5.7/keras_aug/layers/preprocessing/utility/sanitize_bounding_box_test.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/utils/augmentation.py` & `keras-aug-0.5.7/keras_aug/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/utils/augmentation_test.py` & `keras-aug-0.5.7/keras_aug/utils/augmentation_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
 from absl.testing import parameterized
-from keras.backend import RandomGenerator
 
 from keras_aug import core
+from keras_aug.core.keras_random_generator import KerasRandomGenerator
 from keras_aug.utils import augmentation as augmentation_utils
 
 
 class AugmentationUtilsTest(tf.test.TestCase, parameterized.TestCase):
     def test_get_padding_position_invalid(self):
         with self.assertRaises(NotImplementedError):
             augmentation_utils.get_padding_position("hello")
@@ -51,15 +51,15 @@
                 ([3], [0], [7], [0]),
                 "bottom_right",
             ),
             ("random", ([1], [2], [3], [4]), None, "random"),
         ]
     )
     def test_get_position_params(self, values, expected_values, position_name):
-        rng = RandomGenerator(2023)
+        rng = KerasRandomGenerator(2023)
         tops, bottoms, lefts, rights = values
         position = augmentation_utils.get_padding_position(position_name)
 
         tops, bottoms, lefts, rights = augmentation_utils.get_position_params(
             tops, bottoms, lefts, rights, position, rng
         )
         if position_name == "random":
```

### Comparing `keras-aug-0.5.6/keras_aug/utils/conditional_imports.py` & `keras-aug-0.5.7/keras_aug/utils/conditional_imports.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/utils/demo.py` & `keras-aug-0.5.7/keras_aug/utils/demo.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug/utils/distribution.py` & `keras-aug-0.5.7/keras_aug/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `keras-aug-0.5.6/keras_aug.egg-info/PKG-INFO` & `keras-aug-0.5.7/keras_aug.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-aug
-Version: 0.5.6
+Version: 0.5.7
 Summary: A library that includes pure TF/Keras preprocessing and augmentation layers
 Author: Hongyu, Chiu (james77777778)
 License:    Copyright 2023 The KerasAug Authors. All rights reserved.
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -238,15 +238,15 @@
 ![Python](https://img.shields.io/badge/python-v3.8.0+-success.svg)
 ![Tensorflow](https://img.shields.io/badge/tensorflow-v2.12.0+-success.svg)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-aug/actions.yml?label=tests)](https://github.com/james77777778/keras-aug/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-aug/branch/main/graph/badge.svg?token=81ELI3VH7H)](https://codecov.io/gh/james77777778/keras-aug)
 [![PyPI](https://img.shields.io/pypi/v/keras-aug)](https://pypi.org/project/keras-aug/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-aug)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/keras-aug/issues)
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://keras-aug-rqtoxd8zk3.streamlit.app/)
 
 ## Description
 
 KerasAug is a library that includes pure TF/Keras preprocessing and augmentation layers, providing support for various data types such as images, labels, bounding boxes, segmentation masks, and more.
 
 <div align="center">
 <img width="45%" src="https://user-images.githubusercontent.com/20734616/238531125-f0a07f50-423b-4be2-9dcd-a3cc459a261c.gif"> <img width="45%" src="https://user-images.githubusercontent.com/20734616/238531295-22cd5567-0709-46d5-bf31-7baad05b91d2.gif">
@@ -257,32 +257,32 @@
 
 KerasAug aims to provide fast, robust and user-friendly preprocessing and augmentation layers, facilitating seamless integration with TensorFlow, Keras and KerasCV.
 
 KerasAug is:
 
 - 🚀 faster than [KerasCV](https://github.com/keras-team/keras-cv) which is an official Keras library
 - 🧰 supporting various data types, including **images, labels, bounding boxes, segmentation masks**, and more.
-- ❤️ dependent only on TensorFlow and KerasCV
+- ❤️ dependent only on TensorFlow
 - 🌟 seamlessly integrating with the `tf.data` and `tf.keras.Model` APIs
-- 🔥 compatible with GPU
+- 🔥 compatible with GPU and mixed precision (`mixed_float16` and `mixed_bfloat16`)
 
 Check out the demo website powered by Streamlit:
 
-<a href="https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/"><img width="50%" align="right" src="https://user-images.githubusercontent.com/20734616/242836830-bd0a457d-fa6f-410c-a267-af628f5bb5ec.JPG"></a>
+<a href="https://keras-aug-rqtoxd8zk3.streamlit.app/"><img width="50%" align="right" src="https://user-images.githubusercontent.com/20734616/242836830-bd0a457d-fa6f-410c-a267-af628f5bb5ec.JPG"></a>
 
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://james77777778-keras-aug-streamlit-appapp-mxd7v1.streamlit.app/)
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://keras-aug-rqtoxd8zk3.streamlit.app/)
 
 - Apply a transformation to the default or uploaded image
 - Adjust the arguments of the specified layer
 
 ## Why KerasAug?
 
 1. KerasAug is generally faster than KerasCV
 
-    > RandomCropAndResize in KerasAug exhibits a remarkable speed-up of **+1342%** compared to KerasAug. See [keras-aug/benchmarks](https://github.com/james77777778/keras-aug/tree/main/benchmarks) for more details.
+    > RandomCropAndResize in KerasAug exhibits a remarkable speed-up of **+1150%** compared to KerasAug. See [keras-aug/benchmarks](https://github.com/james77777778/keras-aug/tree/main/benchmarks) for more details.
 
 2. The APIs of KerasAug are highly stable compared to KerasCV
 
     > KerasCV struggles to reproduce the YOLOV8 training pipeline, whereas KerasAug executes it flawlessly. See [Quickstart](https://github.com/james77777778/keras-aug/tree/main#quickstart) for more details.
 
 3. KerasAug comes with built-in support for mixed precision training
 
@@ -524,39 +524,40 @@
 
 </details>
 
 ## Benchmark
 
 KerasAug is generally faster than KerasCV.
 
-| Type           | Layer                    | KerasAug | KerasCV   |        |
-|----------------|--------------------------|----------|-----------|--------|
-| Geometry       | RandomHFlip              | 2148     | 1859      | +15%   |
-|                | RandomVFlip              | 2182     | 2075      | +5%    |
-|                | RandomRotate             | 2451     | 1829      | +34%   |
-|                | RandomAffine             | 2141     | 1240      | +73%   |
-|                | RandomCropAndResize      | 3014     | 209       | +1342% |
-|                | Resize (224, 224)        | 2853     | 213       | +1239% |
-| Intensity      | RandomBrightness         | 3028     | 3097      | close  |
-|                | RandomContrast           | 2806     | 2645      | +6%    |
-|                | RandomBrightnessContrast | 3068     | 612       | +401%  |
-|                | RandomColorJitter        | 1932     | 1221      | +58%   |
-|                | RandomGaussianBlur       | 2758     | 207       | +1232% |
-|                | Grayscale                | 2841     | 2872      | close  |
-|                | Equalize                 | 206      | 139       | +48%   |
-|                | AutoContrast             | 3116     | 2991      | +4%    |
-|                | Posterize                | 2917     | 2445      | +19%   |
-|                | Solarize                 | 3025     | 2882      | +5%    |
-|                | Sharpness                | 2969     | 2915      | close  |
-| Regularization | RandomCutout             | 3222     | 3268      | close  |
-|                | RandomGridMask           | 947      | 197       | +381%  |
-| Mix            | CutMix                   | 2671     | 2445      | +9%    |
-|                | MixUp                    | 2593     | 1996      | +29%   |
-| Auto           | AugMix                   | 83       | X (Error) | X      |
-|                | RandAugment              | 282      | 249       | +13%   |
+| Type           | Layer                      | KerasAug | KerasCV   |        |
+|----------------|----------------------------|----------|-----------|--------|
+| Geometry       | RandomHFlip                | 2123     | 1956      | fair   |
+|                | RandomVFlip                | 1871     | 1767      | fair   |
+|                | RandomRotate               | 1703     | 1723      | fair   |
+|                | RandomAffine               | 2578     | 2355      | fair   |
+|                | RandomCropAndResize        | 2664     | 213       | +1150% |
+|                | Resize (224, 224)          | 2480     | 222       | +1017% |
+| Intensity      | RandomBrightness           | 3052     | 2768      | fair   |
+|                | RandomContrast\*           | 3099     | 2976      | fair   |
+|                | RandomBrightnessContrast\* | 2881     | 609       | +373%  |
+|                | RandomColorJitter\*        | 2013     | 597       | +237%  |
+|                | RandomGaussianBlur         | 2345     | 203       | +1055% |
+|                | Invert                     | 2691     | X         |        |
+|                | Grayscale                  | 2917     | 3116      | fair   |
+|                | Equalize                   | 196      | 139       | +41%   |
+|                | AutoContrast               | 3095     | 3025      | fair   |
+|                | Posterize                  | 3033     | 2144      | fair   |
+|                | Solarize                   | 3133     | 2972      | fair   |
+|                | Sharpness                  | 2982     | 2833      | fair   |
+| Regularization | RandomCutout               | 2994     | 2795      | fair   |
+|                | RandomGridMask             | 918      | 196       | +368%  |
+| Mix            | CutMix                     | 2967     | 2957      | fair   |
+|                | MixUp                      | 1897     | 1861      | fair   |
+| Auto           | AugMix                     | 79       | X (Error) |        |
+|                | RandAugment                | 301      | 246       | +22%   |
 
 > **Note**
 > FPS (frames per second)
 
 Please refer to [benchmarks/README.md](benchmarks/README.md) for more details.
 
 ## Citing KerasAug
```

### Comparing `keras-aug-0.5.6/keras_aug.egg-info/SOURCES.txt` & `keras-aug-0.5.7/keras_aug.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 keras_aug/conftest.py
 keras_aug.egg-info/PKG-INFO
 keras_aug.egg-info/SOURCES.txt
 keras_aug.egg-info/dependency_links.txt
 keras_aug.egg-info/requires.txt
 keras_aug.egg-info/top_level.txt
 keras_aug/core/__init__.py
+keras_aug/core/keras_random_generator.py
 keras_aug/core/factor_sampler/__init__.py
 keras_aug/core/factor_sampler/constant_factor_sampler.py
 keras_aug/core/factor_sampler/constant_factor_sampler_test.py
 keras_aug/core/factor_sampler/factor_sampler.py
 keras_aug/core/factor_sampler/normal_factor_sampler.py
 keras_aug/core/factor_sampler/normal_factor_sampler_test.py
 keras_aug/core/factor_sampler/signed_constant_factor_sampler.py
```

### Comparing `keras-aug-0.5.6/pyproject.toml` & `keras-aug-0.5.7/pyproject.toml`

 * *Files identical despite different names*


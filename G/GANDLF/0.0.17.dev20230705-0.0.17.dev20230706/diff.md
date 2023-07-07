# Comparing `tmp/GANDLF-0.0.17.dev20230705.tar.gz` & `tmp/GANDLF-0.0.17.dev20230706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230705.tar", last modified: Wed Jul  5 03:20:30 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230706.tar", last modified: Thu Jul  6 03:21:49 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230705.tar` & `GANDLF-0.0.17.dev20230706.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.785234 GANDLF-0.0.17.dev20230705/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.749234 GANDLF-0.0.17.dev20230705/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.749234 GANDLF-0.0.17.dev20230705/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.753234 GANDLF-0.0.17.dev20230705/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/generate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.757234 GANDLF-0.0.17.dev20230705/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21706 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.757234 GANDLF-0.0.17.dev20230705/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.757234 GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.757234 GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.761234 GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.761234 GANDLF-0.0.17.dev20230705/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.761234 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.765234 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.765234 GANDLF-0.0.17.dev20230705/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.765234 GANDLF-0.0.17.dev20230705/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.769234 GANDLF-0.0.17.dev20230705/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/metrics/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/metrics/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.773234 GANDLF-0.0.17.dev20230705/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.777234 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.781234 GANDLF-0.0.17.dev20230705/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29704 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.781234 GANDLF-0.0.17.dev20230705/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.785234 GANDLF-0.0.17.dev20230705/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-05 03:20:24.000000 GANDLF-0.0.17.dev20230705/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:20:30.749234 GANDLF-0.0.17.dev20230705/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-05 03:20:30.000000 GANDLF-0.0.17.dev20230705/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-05 03:20:30.000000 GANDLF-0.0.17.dev20230705/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:20:30.000000 GANDLF-0.0.17.dev20230705/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:18:13.000000 GANDLF-0.0.17.dev20230705/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-05 03:20:30.000000 GANDLF-0.0.17.dev20230705/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 03:20:30.000000 GANDLF-0.0.17.dev20230705/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-05 03:20:30.785234 GANDLF-0.0.17.dev20230705/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_generateMetrics
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 03:20:30.785234 GANDLF-0.0.17.dev20230705/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-05 03:17:55.000000 GANDLF-0.0.17.dev20230705/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.669128 GANDLF-0.0.17.dev20230706/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.625127 GANDLF-0.0.17.dev20230706/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.625127 GANDLF-0.0.17.dev20230706/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.629127 GANDLF-0.0.17.dev20230706/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.633127 GANDLF-0.0.17.dev20230706/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21706 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.633127 GANDLF-0.0.17.dev20230706/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.633127 GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.633127 GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.637127 GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.637127 GANDLF-0.0.17.dev20230706/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.641127 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.641127 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.645128 GANDLF-0.0.17.dev20230706/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.645128 GANDLF-0.0.17.dev20230706/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.649128 GANDLF-0.0.17.dev20230706/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/metrics/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/metrics/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.657128 GANDLF-0.0.17.dev20230706/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.665128 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.665128 GANDLF-0.0.17.dev20230706/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29704 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.665128 GANDLF-0.0.17.dev20230706/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.669128 GANDLF-0.0.17.dev20230706/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 03:21:43.000000 GANDLF-0.0.17.dev20230706/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:21:49.625127 GANDLF-0.0.17.dev20230706/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-06 03:21:49.000000 GANDLF-0.0.17.dev20230706/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-07-06 03:21:49.000000 GANDLF-0.0.17.dev20230706/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:21:49.000000 GANDLF-0.0.17.dev20230706/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:19:38.000000 GANDLF-0.0.17.dev20230706/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-06 03:21:49.000000 GANDLF-0.0.17.dev20230706/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 03:21:49.000000 GANDLF-0.0.17.dev20230706/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-06 03:21:49.669128 GANDLF-0.0.17.dev20230706/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 03:21:49.673128 GANDLF-0.0.17.dev20230706/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-06 03:19:22.000000 GANDLF-0.0.17.dev20230706/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230705/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230706/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230706/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230706/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230706/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230706/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230706/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/generate_metrics.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/generate_metrics.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/patch_extraction.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from GANDLF.data.patch_miner.opm.patch_manager import PatchManager
 from GANDLF.data.patch_miner.opm.utils import (
     alpha_rgb_2d_channel_check,
     patch_size_check,
     parse_config,
     generate_initial_mask,
     get_patch_size_in_microns,
+    patch_artifact_check,
+    # pen_marking_check,
 )
 from GANDLF.utils import (
     parseTrainingCSV,
 )
 
 
 def parse_gandlf_csv(fpath):
@@ -42,25 +44,22 @@
         config (Union[str, dict, none]): The input yaml config.
         output_path (_type_): _description_
     """
 
     Image.MAX_IMAGE_PIXELS = None
     warnings.simplefilter("ignore")
 
+    # initialize default config
+    cfg = {}
     if config is not None:
         cfg = config
         if isinstance(config, str):
             cfg = parse_config(config)
-    else:
-        cfg = {}
-        cfg["scale"] = 16
-
-    if "patch_size" not in cfg:
-        cfg["patch_size"] = (256, 256)
-
+    cfg["scale"] = cfg.get("scale", 16)
+    cfg["patch_size"] = cfg.get("patch_size", (256, 256))
     original_patch_size = cfg["patch_size"]
 
     if not os.path.exists(output_path):
         Path(output_path).mkdir(parents=True, exist_ok=True)
 
     output_path = os.path.abspath(output_path)
 
@@ -79,14 +78,16 @@
 
         # Generate an initial validity mask
         mask, scale = generate_initial_mask(slide, cfg["scale"])
         print("Setting valid mask...")
         manager.set_valid_mask(mask, scale)
         # Reject patch if any pixels are transparent
         manager.add_patch_criteria(alpha_rgb_2d_channel_check)
+        #manager.add_patch_criteria(pen_marking_check) ### will be added to main code after rigourous experimentation
+        manager.add_patch_criteria(patch_artifact_check)
         # Reject patch if image dimensions are not equal to PATCH_SIZE
         patch_dims_check = partial(
             patch_size_check,
             patch_height=cfg["patch_size"][0],
             patch_width=cfg["patch_size"][1],
         )
         manager.add_patch_criteria(patch_dims_check)
```

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230706/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230706/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230706/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230706/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230706/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230706/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230706/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,18 +144,16 @@
             )
 
             # Update the mined mask
             self.mined_mask[
                 max(mined_start_x, 0) : self.width_bound_check(mined_end_x),
                 max(mined_start_y, 0) : self.width_bound_check(mined_end_y),
             ] = True
-
             # Append this patch to the list of patches to be saved
             self.patches.append(patch)
-
             return True
 
         except Exception as e:
             # If it fails for any reason, print the exception and return
             print("Exception thrown when adding patch:", e)
             return False
```

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/patch_miner/opm/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 # from skimage.filters.rank import maximum
 from skimage.filters import gaussian
 
 # from skimage.morphology.footprints import disk
 from skimage.morphology import remove_small_holes
 from skimage.color.colorconv import rgb2hsv
+import cv2
+#from skimage.exposure import rescale_intensity
+#from skimage.color import rgb2hed
 
 # import matplotlib.pyplot as plt
 import yaml
 import tiffslide
 
 # RGB Masking (pen) constants
 RGB_RED_CHANNEL = 0
@@ -231,14 +234,63 @@
     # If the image is two dims, return True
     elif len(img.shape) == 2:
         return True
     # Other images (4D, RGBA+____, etc.), return False.
     else:
         return False
 
+#def pen_marking_check(img, intensity_thresh=225, intensity_thresh_saturation =50, intensity_thresh_b = 128):
+#    """
+#    This function is used to curate patches from the input image. It is used to remove patches that have pen markings.
+#    Args:
+#        img (np.ndarray): Input Patch Array to check the artifact/background.
+#        intensity_thresh (int, optional): Threshold to check whiteness in the patch. Defaults to 225.
+#        intensity_thresh_saturation (int, optional): Threshold to check saturation in the patch. Defaults to 50.
+#        intensity_thresh_b (int, optional) : Threshold to check blackness in the patch
+#        patch_size (int, optional): Tiling Size of the WSI/patch size. Defaults to 256. patch_size=config["patch_size"]
+#    Returns:
+#        bool: Whether the patch is valid (True) or not (False)
+#    """
+#    patch_size= (256,256)
+#    ihc_hed = rgb2hed(img)
+#    patch_hsv = cv2.cvtColor(img, cv2.COLOR_RGB2HSV)
+#    e = rescale_intensity(ihc_hed[:, :, 1], out_range=(0, 255), in_range=(0, np.percentile(ihc_hed[:, :, 1], 99)))
+#    if np.sum(e < 50) / (patch_size[0] * patch_size[1]) > 0.95 or (np.sum(patch_hsv[...,0] < 128) / (patch_size[0] * patch_size[1])) > 0.97:
+#        return False
+#    #Assume patch is valid
+#    return True
+
+def patch_artifact_check(img, intensity_thresh = 250, intensity_thresh_saturation = 5, intensity_thresh_b = 128, patch_size = (256,256)):
+    """
+    This function is used to curate patches from the input image. It is used to remove patches that are mostly background.
+    Args:
+        img (np.ndarray): Input Patch Array to check the artifact/background.
+        intensity_thresh (int, optional): Threshold to check whiteness in the patch. Defaults to 225.
+        intensity_thresh_saturation (int, optional): Threshold to check saturation in the patch. Defaults to 50.
+        intensity_thresh_b (int, optional) : Threshold to check blackness in the patch
+        patch_size (int, optional): Tiling Size of the WSI/patch size. Defaults to 256. patch_size=config["patch_size"]
+    Returns:
+        bool: Whether the patch is valid (True) or not (False)
+    """
+    #patch_size = config["patch_size"]
+    patch_hsv = cv2.cvtColor(img, cv2.COLOR_RGB2HSV)
+    count_white_pixels = np.sum(np.logical_and.reduce(img > intensity_thresh, axis=2))
+    percent_pixels = count_white_pixels / (patch_size[0] * patch_size[1])
+    count_black_pixels = np.sum(np.logical_and.reduce(img < intensity_thresh_b, axis=2))
+    percent_pixel_b = count_black_pixels / (patch_size[0] * patch_size[1])
+    percent_pixel_2 = np.sum(patch_hsv[...,1] < intensity_thresh_saturation) / (patch_size[0] * patch_size[1])
+    percent_pixel_3 = np.sum(patch_hsv[...,2] > intensity_thresh) / (patch_size[0] * patch_size[1])
+
+    if percent_pixel_2 > 0.99 or np.mean(patch_hsv[...,1]) < 5 or percent_pixel_3 > 0.99:
+        if percent_pixel_2 < 0.1:
+            return False
+    elif (percent_pixel_2 > 0.99 and percent_pixel_3 > 0.99) or percent_pixel_b > 0.99 or percent_pixels > 0.9:
+        return False
+    # assume that the patch is valid
+    return True
 
 def parse_config(config_file):
     """
     Parse config file and return a dictionary of config values.
     :param config_file: path to config file
     :return: dictionary of config values
     """
@@ -248,14 +300,15 @@
     config["scale"] = config.get("scale", 16)
     config["num_patches"] = config.get("num_patches", -1)
     config["num_workers"] = config.get("num_workers", 1)
     config["save_patches"] = config.get("save_patches", True)
     config["value_map"] = config.get("value_map", None)
     config["read_type"] = config.get("read_type", "random")
     config["overlap_factor"] = config.get("overlap_factor", 0.0)
+    config["patch_size"] = config.get("patch_size", [256,256])
 
     return config
 
 
 def is_mask_too_big(mask):
     """
     Function that returns a boolean value indicating whether the mask is too big to make processing slow.
```

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230706/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230706/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230706/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230706/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230706/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230706/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230706/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230706/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230706/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230706/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230706/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230706/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230706/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/metrics/synthesis.py` & `GANDLF-0.0.17.dev20230706/GANDLF/metrics/synthesis.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230706/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230706/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230706/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230706/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230706/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230706/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230706/GANDLF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230705
+Version: 0.0.17.dev20230706
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230705 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230706 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230705/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230706/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/HISTORY.md` & `GANDLF-0.0.17.dev20230706/HISTORY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/LICENSE` & `GANDLF-0.0.17.dev20230706/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/PKG-INFO` & `GANDLF-0.0.17.dev20230706/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230705
+Version: 0.0.17.dev20230706
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230705 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230706 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230705/README.md` & `GANDLF-0.0.17.dev20230706/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/SECURITY.md` & `GANDLF-0.0.17.dev20230706/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230706/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_collectStats` & `GANDLF-0.0.17.dev20230706/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230706/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230706/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_deploy` & `GANDLF-0.0.17.dev20230706/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_generateMetrics` & `GANDLF-0.0.17.dev20230706/gandlf_generateMetrics`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230706/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230706/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_preprocess` & `GANDLF-0.0.17.dev20230706/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230706/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_run` & `GANDLF-0.0.17.dev20230706/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230706/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230705/setup.py` & `GANDLF-0.0.17.dev20230706/setup.py`

 * *Files identical despite different names*


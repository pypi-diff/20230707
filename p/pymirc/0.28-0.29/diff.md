# Comparing `tmp/pymirc-0.28.tar.gz` & `tmp/pymirc-0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymirc-0.28.tar", last modified: Fri Oct 14 19:14:37 2022, max compression
+gzip compressed data, was "pymirc-0.29.tar", last modified: Thu Jul  6 23:50:16 2023, max compression
```

## Comparing `pymirc-0.28.tar` & `pymirc-0.29.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.294312 pymirc-0.28/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-14 19:14:27.000000 pymirc-0.28/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.286312 pymirc-0.28/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.286312 pymirc-0.28/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-10-14 19:14:27.000000 pymirc-0.28/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-10-14 19:14:27.000000 pymirc-0.28/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-14 19:14:27.000000 pymirc-0.28/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-10-14 19:14:27.000000 pymirc-0.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:27.000000 pymirc-0.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-10-14 19:14:37.294312 pymirc-0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-10-14 19:14:27.000000 pymirc-0.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.286312 pymirc-0.28/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.290312 pymirc-0.28/examples/fileio/
--rw-r--r--   0 runner    (1001) docker     (121)     4489 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/convert_kul_ct_recon_to_dicom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2394 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/convert_kul_nifti_to_dicom.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/ct_dcm_tags_to_copy.txt
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/dcm_tags_to_copy.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/ibsi_read_rtstruct_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/interpolate_rtdose.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/labelvolume_to_rtstruct.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/pixel_segmentation_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/read_dcm_overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/read_dcm_rt_struct.py
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/rt_struct_to_nifti.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/rtdose_tags_to_copy.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/view_nrrd_seg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-10-14 19:14:27.000000 pymirc-0.28/examples/fileio/voxel_segmentation_to_surface_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.290312 pymirc-0.28/examples/image_operations/
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-10-14 19:14:27.000000 pymirc-0.28/examples/image_operations/volume_warp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.290312 pymirc-0.28/examples/keras_mnist_segmentation/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/compare_dice.py
--rw-r--r--   0 runner    (1001) docker     (121)     4079 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/create_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/evaluate_mnist_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5126 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/mnist_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/mnist_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5960 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/mnist_seg_with_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/slow_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4617 2022-10-14 19:14:27.000000 pymirc-0.28/examples/keras_mnist_segmentation/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.290312 pymirc-0.28/examples/registration/
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-10-14 19:14:27.000000 pymirc-0.28/examples/registration/rigid_registration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.290312 pymirc-0.28/examples/viewer/
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-10-14 19:14:27.000000 pymirc-0.28/examples/viewer/read_pet_ct_dicom_and_display.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.290312 pymirc-0.28/pymirc/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.290312 pymirc-0.28/pymirc/fileio/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10197 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/fileio/labelvol_to_rtstruct.py
--rw-r--r--   0 runner    (1001) docker     (121)    14021 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/fileio/radioPharmaceuticalInfoSequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    26281 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/fileio/read_dicom.py
--rw-r--r--   0 runner    (1001) docker     (121)     8154 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/fileio/read_rtstruct.py
--rw-r--r--   0 runner    (1001) docker     (121)    17859 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/fileio/write_dicom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.294312 pymirc-0.28/pymirc/image_operations/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5297 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/aff_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/backward_3d_warp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5592 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/binary_2d_image_to_contours.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/forward_3d_warp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6074 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/grad.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5025 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/mincostpath.py
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/random_deformation_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/reorient.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/resample_cont_cont.py
--rw-r--r--   0 runner    (1001) docker     (121)     5442 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/resample_img_cont.py
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/rigid_registration.py
--rw-r--r--   0 runner    (1001) docker     (121)     9259 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/image_operations/zoom3d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.294312 pymirc-0.28/pymirc/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5173 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/metrics/cost_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3693 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/metrics/tf_losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     9217 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/metrics/tf_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.294312 pymirc-0.28/pymirc/viewer/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19356 2022-10-14 19:14:27.000000 pymirc-0.28/pymirc/viewer/threeaxisviewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.290312 pymirc-0.28/pymirc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-10-14 19:14:37.000000 pymirc-0.28/pymirc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-10-14 19:14:37.000000 pymirc-0.28/pymirc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 19:14:37.000000 pymirc-0.28/pymirc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-14 19:14:37.000000 pymirc-0.28/pymirc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-14 19:14:37.000000 pymirc-0.28/pymirc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-14 19:14:27.000000 pymirc-0.28/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 19:14:37.294312 pymirc-0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-10-14 19:14:27.000000 pymirc-0.28/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-14 19:14:27.000000 pymirc-0.28/style_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.294312 pymirc-0.28/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)    22229 2022-10-14 19:14:27.000000 pymirc-0.28/tutorial/challenge.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.286312 pymirc-0.28/tutorial/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.294312 pymirc-0.28/tutorial/data/demo/
--rw-r--r--   0 runner    (1001) docker     (121)   208031 2022-10-14 19:14:27.000000 pymirc-0.28/tutorial/data/demo/T1maps.png
--rw-r--r--   0 runner    (1001) docker     (121)    72192 2022-10-14 19:14:27.000000 pymirc-0.28/tutorial/data/demo/example_contours.png
--rw-r--r--   0 runner    (1001) docker     (121)    65245 2022-10-14 19:14:27.000000 pymirc-0.28/tutorial/data/demo/example_groundtruth.png
--rw-r--r--   0 runner    (1001) docker     (121)    47498 2022-10-14 19:14:27.000000 pymirc-0.28/tutorial/data/demo/short-axis.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 19:14:37.294312 pymirc-0.28/tutorial/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-10-14 19:14:27.000000 pymirc-0.28/tutorial/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-10-14 19:14:27.000000 pymirc-0.28/tutorial/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-10-14 19:14:27.000000 pymirc-0.28/tutorial/utils/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.444650 pymirc-0.29/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 23:50:02.000000 pymirc-0.29/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.424650 pymirc-0.29/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.428650 pymirc-0.29/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-06 23:50:02.000000 pymirc-0.29/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-06 23:50:02.000000 pymirc-0.29/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-06 23:50:02.000000 pymirc-0.29/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-06 23:50:02.000000 pymirc-0.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:02.000000 pymirc-0.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-06 23:50:16.444650 pymirc-0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 23:50:02.000000 pymirc-0.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.424650 pymirc-0.29/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.432649 pymirc-0.29/examples/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/convert_kul_ct_recon_to_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/convert_kul_nifti_to_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/ct_dcm_tags_to_copy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/dcm_tags_to_copy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/ibsi_read_rtstruct_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/interpolate_rtdose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/labelvolume_to_rtstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/pixel_segmentation_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/read_dcm_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/read_dcm_rt_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/rt_struct_to_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/rtdose_tags_to_copy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/view_nrrd_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-06 23:50:02.000000 pymirc-0.29/examples/fileio/voxel_segmentation_to_surface_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.432649 pymirc-0.29/examples/image_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 23:50:02.000000 pymirc-0.29/examples/image_operations/volume_warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.436650 pymirc-0.29/examples/keras_mnist_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/compare_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/create_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/evaluate_mnist_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/mnist_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/mnist_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/mnist_seg_with_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/slow_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-06 23:50:02.000000 pymirc-0.29/examples/keras_mnist_segmentation/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.436650 pymirc-0.29/examples/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-06 23:50:02.000000 pymirc-0.29/examples/registration/rigid_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.436650 pymirc-0.29/examples/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-06 23:50:02.000000 pymirc-0.29/examples/viewer/read_pet_ct_dicom_and_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.436650 pymirc-0.29/pymirc/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.440650 pymirc-0.29/pymirc/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/fileio/labelvol_to_rtstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/fileio/radioPharmaceuticalInfoSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26242 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/fileio/read_dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/fileio/read_rtstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/fileio/write_dicom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.440650 pymirc-0.29/pymirc/image_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/aff_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/backward_3d_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/binary_2d_image_to_contours.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/forward_3d_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/grad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5025 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/mincostpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/random_deformation_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/reorient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/resample_cont_cont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/resample_img_cont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/rigid_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/image_operations/zoom3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.444650 pymirc-0.29/pymirc/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/metrics/cost_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/metrics/tf_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/metrics/tf_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.444650 pymirc-0.29/pymirc/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-07-06 23:50:02.000000 pymirc-0.29/pymirc/viewer/threeaxisviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.436650 pymirc-0.29/pymirc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-06 23:50:16.000000 pymirc-0.29/pymirc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-06 23:50:16.000000 pymirc-0.29/pymirc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:50:16.000000 pymirc-0.29/pymirc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 23:50:16.000000 pymirc-0.29/pymirc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 23:50:16.000000 pymirc-0.29/pymirc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 23:50:02.000000 pymirc-0.29/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:50:16.448650 pymirc-0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-06 23:50:02.000000 pymirc-0.29/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 23:50:02.000000 pymirc-0.29/style_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.444650 pymirc-0.29/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-06 23:50:02.000000 pymirc-0.29/tutorial/challenge.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.424650 pymirc-0.29/tutorial/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.444650 pymirc-0.29/tutorial/data/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)   208031 2023-07-06 23:50:02.000000 pymirc-0.29/tutorial/data/demo/T1maps.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72192 2023-07-06 23:50:02.000000 pymirc-0.29/tutorial/data/demo/example_contours.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65245 2023-07-06 23:50:02.000000 pymirc-0.29/tutorial/data/demo/example_groundtruth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47498 2023-07-06 23:50:02.000000 pymirc-0.29/tutorial/data/demo/short-axis.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:50:16.444650 pymirc-0.29/tutorial/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-06 23:50:02.000000 pymirc-0.29/tutorial/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-06 23:50:02.000000 pymirc-0.29/tutorial/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-06 23:50:02.000000 pymirc-0.29/tutorial/utils/metrics.py
```

### Comparing `pymirc-0.28/.github/workflows/publish-to-pypi.yml` & `pymirc-0.29/.github/workflows/publish-to-test-pypi.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-name: Publish Python distributions to PyPI
+name: Publish Python distributions to TestPyPI
 
 on:
   push:
     tags:
-      - "v[0-9]+.[0-9]+"
-      - "v[0-9]+.[0-9]+"
-      - "v[0-9]+.[0-9]+.[0-9]+"
-      - "v[0-9]+.[0-9]+.[0-9]+"
+      - "v[0-9]+[a-z][0-9]+"
+      - "v[0-9]+.[0-9]+[a-z][0-9]+"
+      - "v[0-9]+.[0-9]+.[0-9]+[a-z][0-9]+"
 
 jobs:
   build-n-publish:
-    name: Build and publish Python distributions package to PyPI
+    name: Build and publish Python distributions package to TestPyPI
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@master
       - name: Set up Python 3.10
         uses: actions/setup-python@v3
         with:
@@ -31,11 +30,12 @@
           python -m
           build
           --sdist
           --wheel
           --outdir dist/
           .
 
-      - name: Publish distribution package to PyPI
+      - name: Publish distribution package to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+          repository_url: https://test.pypi.org/legacy/
```

### Comparing `pymirc-0.28/.github/workflows/publish-to-test-pypi.yml` & `pymirc-0.29/.github/workflows/publish-to-pypi.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-name: Publish Python distributions to TestPyPI
+name: Publish Python distributions to PyPI
 
 on:
   push:
     tags:
-      - "v[0-9]+.[0-9]+a[0-9]+"
-      - "v[0-9]+.[0-9]+b[0-9]+"
-      - "v[0-9]+.[0-9]+.[0-9]+a[0-9]+"
-      - "v[0-9]+.[0-9]+.[0-9]+b[0-9]+"
+      - "v[0-9]+"
+      - "v[0-9]+.[0-9]+"
+      - "v[0-9]+.[0-9]+.[0-9]+"
 
 jobs:
   build-n-publish:
-    name: Build and publish Python distributions package to TestPyPI
+    name: Build and publish Python distributions package to PyPI
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@master
       - name: Set up Python 3.10
         uses: actions/setup-python@v3
         with:
@@ -31,12 +30,11 @@
           python -m
           build
           --sdist
           --wheel
           --outdir dist/
           .
 
-      - name: Publish distribution package to Test PyPI
+      - name: Publish distribution package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `pymirc-0.28/.gitignore` & `pymirc-0.29/.gitignore`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/LICENSE` & `pymirc-0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/PKG-INFO` & `pymirc-0.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymirc
-Version: 0.28
+Version: 0.29
 Summary: Python imaging utilities developed in the medical imaging research center of KU Leuven
 Home-page: https://github.com/gschramm/pymirc
 Author: Georg Schramm, Tom Eelbode, Jeroen Bertels
 Author-email: georg.schramm@kuleuven.be
 License: LGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pymirc-0.28/README.md` & `pymirc-0.29/README.md`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/convert_kul_ct_recon_to_dicom.py` & `pymirc-0.29/examples/fileio/convert_kul_ct_recon_to_dicom.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/convert_kul_nifti_to_dicom.py` & `pymirc-0.29/examples/fileio/convert_kul_nifti_to_dicom.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/ct_dcm_tags_to_copy.txt` & `pymirc-0.29/examples/fileio/ct_dcm_tags_to_copy.txt`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/ibsi_read_rtstruct_test.py` & `pymirc-0.29/examples/fileio/ibsi_read_rtstruct_test.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/interpolate_rtdose.py` & `pymirc-0.29/examples/fileio/interpolate_rtdose.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/labelvolume_to_rtstruct.py` & `pymirc-0.29/examples/fileio/labelvolume_to_rtstruct.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/pixel_segmentation_to_contour.py` & `pymirc-0.29/examples/fileio/pixel_segmentation_to_contour.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/read_dcm_overlay.py` & `pymirc-0.29/examples/fileio/read_dcm_overlay.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/read_dcm_rt_struct.py` & `pymirc-0.29/examples/fileio/read_dcm_rt_struct.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/rt_struct_to_nifti.py` & `pymirc-0.29/examples/fileio/rt_struct_to_nifti.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/view_nrrd_seg.py` & `pymirc-0.29/examples/fileio/view_nrrd_seg.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/fileio/voxel_segmentation_to_surface_mesh.py` & `pymirc-0.29/examples/fileio/voxel_segmentation_to_surface_mesh.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/image_operations/volume_warp.py` & `pymirc-0.29/examples/image_operations/volume_warp.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/README.md` & `pymirc-0.29/examples/keras_mnist_segmentation/README.md`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/compare_dice.py` & `pymirc-0.29/examples/keras_mnist_segmentation/compare_dice.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/create_data.py` & `pymirc-0.29/examples/keras_mnist_segmentation/create_data.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/evaluate_mnist_model.py` & `pymirc-0.29/examples/keras_mnist_segmentation/evaluate_mnist_model.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/mnist_class.py` & `pymirc-0.29/examples/keras_mnist_segmentation/mnist_class.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/mnist_generator.py` & `pymirc-0.29/examples/keras_mnist_segmentation/mnist_generator.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/mnist_seg_with_generator.py` & `pymirc-0.29/examples/keras_mnist_segmentation/mnist_seg_with_generator.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/slow_generator.py` & `pymirc-0.29/examples/keras_mnist_segmentation/slow_generator.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/keras_mnist_segmentation/unet.py` & `pymirc-0.29/examples/keras_mnist_segmentation/unet.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/registration/rigid_registration.py` & `pymirc-0.29/examples/registration/rigid_registration.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/examples/viewer/read_pet_ct_dicom_and_display.py` & `pymirc-0.29/examples/viewer/read_pet_ct_dicom_and_display.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/fileio/labelvol_to_rtstruct.py` & `pymirc-0.29/pymirc/fileio/labelvol_to_rtstruct.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/fileio/radioPharmaceuticalInfoSequence.py` & `pymirc-0.29/pymirc/fileio/radioPharmaceuticalInfoSequence.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/fileio/read_dicom.py` & `pymirc-0.29/pymirc/fileio/read_dicom.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,32 +85,32 @@
           # this is for multi slice data from PMOD
           try:
             iop = self.firstdcmheader.PerFrameFunctionalGroupsSequence[0].PlaneOrientationSequence[0].ImageOrientationPatient
           except AttributeError:
             # this is for multi slice data from RayStation
             iop = self.firstdcmheader.ImageOrientationPatient
 
-      self.x = np.array(iop[:3], dtype = np.float) 
-      self.y = np.array(iop[3:], dtype = np.float) 
+      self.x = np.array(iop[:3], dtype = float) 
+      self.y = np.array(iop[3:], dtype = float) 
 
       # set member variable that shows whether data has been read in
       self.read_all_dcms = True
       
     else:
-      self.x = np.array(self.firstdcmheader.ImageOrientationPatient[0:3], dtype = np.float) 
-      self.y = np.array(self.firstdcmheader.ImageOrientationPatient[3:] , dtype = np.float) 
+      self.x = np.array(self.firstdcmheader.ImageOrientationPatient[0:3], dtype = float) 
+      self.y = np.array(self.firstdcmheader.ImageOrientationPatient[3:] , dtype = float) 
 
       # set member variable that shows whether data has been read in
       self.read_all_dcms = False
 
     self.n = np.cross(self.x,self.y)
 
     # get the row and column pixelspacing 
     if 'PixelSpacing' in self.firstdcmheader:
-      self.pixelspacing = np.array(self.firstdcmheader.PixelSpacing, dtype = np.float) 
+      self.pixelspacing = np.array(self.firstdcmheader.PixelSpacing, dtype = float) 
     else:
       self.pixelspacing = np.array(self.firstdcmheader.SharedFunctionalGroupsSequence[0].PixelMeasuresSequence[0].PixelSpacing)
      
     self.dr           = self.pixelspacing[0]
     self.dc           = self.pixelspacing[1]
 
     # approximately transform slices in patient coord. system
@@ -386,24 +386,24 @@
         self.normdir *= -1
 
     ipp = None
 
     if 'DetectorInformationSequence' in dcm_data:
       if 'ImagePositionPatient' in dcm_data.DetectorInformationSequence[0]:
         ipp = dcm_data.DetectorInformationSequence[0].ImagePositionPatient
-        self.offset = np.array(ipp, dtype = np.float)
+        self.offset = np.array(ipp, dtype = float)
     elif 'PerFrameFunctionalGroupsSequence' in dcm_data:
       if 'PlanePositionSequence' in dcm_data.PerFrameFunctionalGroupsSequence[0]:
         # this is for molecubes dicom data
         ipp = dcm_data.PerFrameFunctionalGroupsSequence[0].PlanePositionSequence[0].ImagePositionPatient
-        self.offset = np.array(ipp, dtype = np.float)
+        self.offset = np.array(ipp, dtype = float)
     elif 'ImagePositionPatient' in dcm_data:
       # this is for RayStation dicom data
       ipp = dcm_data.ImagePositionPatient
-      self.offset = np.array(ipp, dtype = np.float)
+      self.offset = np.array(ipp, dtype = float)
 
     if ipp is None:
       self.offset = np.zeros(3)
       warnings.warn('Cannot find ImagePositionPatient in dicom header. Setting it to [0,0,0]')
 
     # reorient the patient volume to standard LPS orientation
     patvol = self.reorient_volume(pixelarray)
@@ -443,30 +443,30 @@
     self.sorted_SOPClassUIDs    = [x.SOPClassUID for x in dicomlistsorted]
     self.sorted_SOPInstanceUIDs = [x.SOPInstanceUID for x in dicomlistsorted]
 
     self.Nslices           = len(dicomlistsorted)
     self.Nrows, self.Ncols = pixelarraylistsorted[0].shape
 
     if 'RescaleSlope' in dicomlistsorted[0]: 
-        RescaleSlopes  = [np.float(x.RescaleSlope) for x in dicomlistsorted]
+        RescaleSlopes  = [float(x.RescaleSlope) for x in dicomlistsorted]
     else:
         RescaleSlopes = [1.0] * len(dicomlistsorted)
 
     if 'RescaleIntercept' in dicomlistsorted[0]: 
-        RescaleIntercepts = [np.float(x.RescaleIntercept) for x in dicomlistsorted]
+        RescaleIntercepts = [float(x.RescaleIntercept) for x in dicomlistsorted]
     else:
         RescaleIntercepts = [0.0] * len(dicomlistsorted)
     
     # rescale the pixelarrays with the rescale slopes and intercepts
     for i in range(len(pixelarraylistsorted)): 
         pixelarraylistsorted[i] = pixelarraylistsorted[i]*RescaleSlopes[i] + RescaleIntercepts[i]
 
     # get the first and last ImagePositionPatient vectors
-    self.T1 = np.array(dicomlistsorted[0].ImagePositionPatient , dtype = np.float)
-    self.TN = np.array(dicomlistsorted[-1].ImagePositionPatient, dtype = np.float)
+    self.T1 = np.array(dicomlistsorted[0].ImagePositionPatient , dtype = float)
+    self.TN = np.array(dicomlistsorted[-1].ImagePositionPatient, dtype = float)
     self.dT = self.T1 - self.TN
 
     # get the distance between the dicom slices
     self.sliceDistance = sorted(d)[1] - sorted(d)[0]
   
     # calculate the (x,y,z) offset of voxel [0,0,0]  
     self.offset = 1.0*self.T1
@@ -581,15 +581,15 @@
 
     return np.swapaxes(np.array(overlay_imgs),0,2)
 
   #--------------------------------------------------------------------------
   def distanceMeasure(self,dicomslice):
     # see http://nipy.org/nibabel/dicom/dicom_orientation.html
     # d = position vector in the direction of the normal vector
-    T  = np.array(dicomslice.ImagePositionPatient, dtype = np.float)
+    T  = np.array(dicomslice.ImagePositionPatient, dtype = float)
     d = np.dot(T,self.n)
     return d
 
   #def setAttibute(self, attribute, value):
   #  for dcm in dicomlist: setattr(dcm,attribute,value) 
   #  for dcm2 in dicomlistsorted: setattr(dcm2,attribute,value)
```

### Comparing `pymirc-0.28/pymirc/fileio/read_rtstruct.py` & `pymirc-0.29/pymirc/fileio/read_rtstruct.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/fileio/write_dicom.py` & `pymirc-0.29/pymirc/fileio/write_dicom.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/__init__.py` & `pymirc-0.29/pymirc/image_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/aff_transform.py` & `pymirc-0.29/pymirc/image_operations/aff_transform.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/backward_3d_warp.py` & `pymirc-0.29/pymirc/image_operations/backward_3d_warp.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/binary_2d_image_to_contours.py` & `pymirc-0.29/pymirc/image_operations/binary_2d_image_to_contours.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/grad.py` & `pymirc-0.29/pymirc/image_operations/grad.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/mincostpath.py` & `pymirc-0.29/pymirc/image_operations/mincostpath.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/random_deformation_field.py` & `pymirc-0.29/pymirc/image_operations/random_deformation_field.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/reorient.py` & `pymirc-0.29/pymirc/image_operations/reorient.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/resample_cont_cont.py` & `pymirc-0.29/pymirc/image_operations/resample_cont_cont.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/resample_img_cont.py` & `pymirc-0.29/pymirc/image_operations/resample_img_cont.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     normval   = np.sqrt(normcols**2 + normrows**2)
     normcols /= normval
     normrows /= normval
   
     # This way, the inside of a cyclic contour is at the bottom in the
     # resampled image if the contour is given in clockwise direction.
     #----------------------------
-    steps  = -np.arange(nroutrows, dtype = np.float) * stepsize
+    steps  = -np.arange(nroutrows, dtype = float) * stepsize
     steps -= steps.mean()
   
     if outside_above:
       testval = (normcols * (cencols - cencols.mean()) + normrows * (cenrows - cenrows.mean())).sum()
       if testval < 0: steps = np.flip(steps)
   
     resamplestruct = {'ncols'     : ncols,
```

### Comparing `pymirc-0.28/pymirc/image_operations/rigid_registration.py` & `pymirc-0.29/pymirc/image_operations/rigid_registration.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/image_operations/zoom3d.py` & `pymirc-0.29/pymirc/image_operations/zoom3d.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/metrics/cost_functions.py` & `pymirc-0.29/pymirc/metrics/cost_functions.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/metrics/tf_losses.py` & `pymirc-0.29/pymirc/metrics/tf_losses.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/metrics/tf_metrics.py` & `pymirc-0.29/pymirc/metrics/tf_metrics.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc/viewer/threeaxisviewer.py` & `pymirc-0.29/pymirc/viewer/threeaxisviewer.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/pymirc.egg-info/PKG-INFO` & `pymirc-0.29/pymirc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymirc
-Version: 0.28
+Version: 0.29
 Summary: Python imaging utilities developed in the medical imaging research center of KU Leuven
 Home-page: https://github.com/gschramm/pymirc
 Author: Georg Schramm, Tom Eelbode, Jeroen Bertels
 Author-email: georg.schramm@kuleuven.be
 License: LGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pymirc-0.28/pymirc.egg-info/SOURCES.txt` & `pymirc-0.29/pymirc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/setup.py` & `pymirc-0.29/setup.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/tutorial/challenge.ipynb` & `pymirc-0.29/tutorial/challenge.ipynb`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/tutorial/data/demo/T1maps.png` & `pymirc-0.29/tutorial/data/demo/T1maps.png`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/tutorial/data/demo/example_contours.png` & `pymirc-0.29/tutorial/data/demo/example_contours.png`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/tutorial/data/demo/example_groundtruth.png` & `pymirc-0.29/tutorial/data/demo/example_groundtruth.png`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/tutorial/data/demo/short-axis.png` & `pymirc-0.29/tutorial/data/demo/short-axis.png`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/tutorial/utils/evaluation.py` & `pymirc-0.29/tutorial/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/tutorial/utils/losses.py` & `pymirc-0.29/tutorial/utils/losses.py`

 * *Files identical despite different names*

### Comparing `pymirc-0.28/tutorial/utils/metrics.py` & `pymirc-0.29/tutorial/utils/metrics.py`

 * *Files identical despite different names*


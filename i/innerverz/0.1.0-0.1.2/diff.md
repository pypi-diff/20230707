# Comparing `tmp/innerverz-0.1.0.tar.gz` & `tmp/innerverz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.1.0.tar", last modified: Wed Jul  5 23:43:33 2023, max compression
+gzip compressed data, was "innerverz-0.1.2.tar", last modified: Fri Jul  7 09:58:02 2023, max compression
```

## Comparing `innerverz-0.1.0.tar` & `innerverz-0.1.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.913983 innerverz-0.1.0/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.0/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-05 23:43:33.914079 innerverz-0.1.0/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.0/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.894504 innerverz-0.1.0/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1741 2023-07-05 10:37:06.000000 innerverz-0.1.0/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.895453 innerverz-0.1.0/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.1.0/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.1.0/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.896035 innerverz-0.1.0/innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.1.0/innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2612 2023-07-05 10:22:28.000000 innerverz-0.1.0/innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.1.0/innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.1.0/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.896500 innerverz-0.1.0/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.1.0/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 07:04:21.000000 innerverz-0.1.0/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.897643 innerverz-0.1.0/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.1.0/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.1.0/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.898553 innerverz-0.1.0/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.898850 innerverz-0.1.0/innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    26982 2023-06-03 07:04:12.000000 innerverz-0.1.0/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.899445 innerverz-0.1.0/innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3607 2023-07-04 11:21:58.000000 innerverz-0.1.0/innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.900312 innerverz-0.1.0/innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)    10096 2023-07-05 10:24:58.000000 innerverz-0.1.0/innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.900761 innerverz-0.1.0/innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.901315 innerverz-0.1.0/innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5352 2023-07-05 10:25:15.000000 innerverz-0.1.0/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.902022 innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.902563 innerverz-0.1.0/innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3874 2023-07-04 11:15:07.000000 innerverz-0.1.0/innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.903017 innerverz-0.1.0/innerverz/face_matting/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.1.0/innerverz/face_matting/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8100 2023-07-05 10:55:26.000000 innerverz-0.1.0/innerverz/face_matting/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.904060 innerverz-0.1.0/innerverz/face_matting/nets/
--rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.904537 innerverz-0.1.0/innerverz/face_matting/nets/decoders/
--rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/decoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-05 10:54:16.000000 innerverz-0.1.0/innerverz/face_matting/nets/decoders/resnet_decoder.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.904889 innerverz-0.1.0/innerverz/face_matting/nets/encoders/
--rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-05 10:54:29.000000 innerverz-0.1.0/innerverz/face_matting/nets/encoders/MatteFormer.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/encoders/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-05 11:01:53.000000 innerverz-0.1.0/innerverz/face_matting/nets/generators.py
--rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/ops.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.905233 innerverz-0.1.0/innerverz/face_matting/nets/raft/
--rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/raft/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/raft/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.905939 innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.1.0/innerverz/face_matting/nets/utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.1.0/innerverz/face_matting/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.906495 innerverz-0.1.0/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2908 2023-07-04 11:15:48.000000 innerverz-0.1.0/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.907038 innerverz-0.1.0/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5523 2023-07-05 10:29:48.000000 innerverz-0.1.0/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.907744 innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.908358 innerverz-0.1.0/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2423 2023-07-04 11:16:46.000000 innerverz-0.1.0/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.909058 innerverz-0.1.0/innerverz/landmark_warping/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-07-04 12:10:40.000000 innerverz-0.1.0/innerverz/landmark_warping/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3319 2023-07-05 11:26:45.000000 innerverz-0.1.0/innerverz/landmark_warping/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-05 11:02:06.000000 innerverz-0.1.0/innerverz/landmark_warping/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.909596 innerverz-0.1.0/innerverz/landmark_warping/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-04 10:48:50.000000 innerverz-0.1.0/innerverz/landmark_warping/sub_nets/LadderEncoder.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-05 10:42:47.000000 innerverz-0.1.0/innerverz/landmark_warping/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-05 10:51:39.000000 innerverz-0.1.0/innerverz/landmark_warping/sub_nets/dense_motion.py
--rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-04 10:48:50.000000 innerverz-0.1.0/innerverz/landmark_warping/sub_nets/util.py
--rw-r--r--   0 jjy        (501) staff       (20)     4687 2023-07-04 10:39:19.000000 innerverz-0.1.0/innerverz/landmark_warping/test.py
--rw-r--r--   0 jjy        (501) staff       (20)     1585 2023-07-04 10:39:19.000000 innerverz-0.1.0/innerverz/landmark_warping/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.910321 innerverz-0.1.0/innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.1.0/innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2510 2023-07-04 12:34:32.000000 innerverz-0.1.0/innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.1.0/innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/reage/net_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.1.0/innerverz/reage/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.911052 innerverz-0.1.0/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 10:45:51.000000 innerverz-0.1.0/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.911771 innerverz-0.1.0/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2390 2023-07-05 10:28:22.000000 innerverz-0.1.0/innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.912364 innerverz-0.1.0/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.912979 innerverz-0.1.0/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.913113 innerverz-0.1.0/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.1.0/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.913848 innerverz-0.1.0/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.1.0/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-05 23:43:33.895190 innerverz-0.1.0/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-05 23:43:33.000000 innerverz-0.1.0/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     4776 2023-07-05 23:43:33.000000 innerverz-0.1.0/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-05 23:43:33.000000 innerverz-0.1.0/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-05 23:43:33.000000 innerverz-0.1.0/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-05 23:43:33.000000 innerverz-0.1.0/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.0/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-05 23:43:33.914569 innerverz-0.1.0/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-05 23:43:18.000000 innerverz-0.1.0/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.680818 innerverz-0.1.2/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.1.2/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-07 09:58:02.680923 innerverz-0.1.2/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.1.2/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.658133 innerverz-0.1.2/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1739 2023-07-07 08:56:24.000000 innerverz-0.1.2/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.659499 innerverz-0.1.2/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3488 2023-07-04 08:52:32.000000 innerverz-0.1.2/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.660042 innerverz-0.1.2/innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2612 2023-07-05 10:22:28.000000 innerverz-0.1.2/innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.660509 innerverz-0.1.2/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 07:04:21.000000 innerverz-0.1.2/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.661610 innerverz-0.1.2/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.1.2/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.662424 innerverz-0.1.2/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.662678 innerverz-0.1.2/innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26982 2023-06-03 07:04:12.000000 innerverz-0.1.2/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.663214 innerverz-0.1.2/innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3607 2023-07-04 11:21:58.000000 innerverz-0.1.2/innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.664140 innerverz-0.1.2/innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)    10096 2023-07-05 10:24:58.000000 innerverz-0.1.2/innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.664574 innerverz-0.1.2/innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.665120 innerverz-0.1.2/innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5352 2023-07-05 10:25:15.000000 innerverz-0.1.2/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.666151 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.667820 innerverz-0.1.2/innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3874 2023-07-04 11:15:07.000000 innerverz-0.1.2/innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.668237 innerverz-0.1.2/innerverz/face_matting/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-07-04 12:12:59.000000 innerverz-0.1.2/innerverz/face_matting/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8100 2023-07-05 10:55:26.000000 innerverz-0.1.2/innerverz/face_matting/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.668772 innerverz-0.1.2/innerverz/face_matting/nets/
+-rw-r--r--   0 jjy        (501) staff       (20)       68 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.669036 innerverz-0.1.2/innerverz/face_matting/nets/decoders/
+-rw-r--r--   0 jjy        (501) staff       (20)      219 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/decoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8175 2023-07-05 10:54:16.000000 innerverz-0.1.2/innerverz/face_matting/nets/decoders/resnet_decoder.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.669337 innerverz-0.1.2/innerverz/face_matting/nets/encoders/
+-rw-r--r--   0 jjy        (501) staff       (20)    24822 2023-07-05 10:54:29.000000 innerverz-0.1.2/innerverz/face_matting/nets/encoders/MatteFormer.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/encoders/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4386 2023-07-05 11:01:53.000000 innerverz-0.1.2/innerverz/face_matting/nets/generators.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2650 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/ops.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.669610 innerverz-0.1.2/innerverz/face_matting/nets/raft/
+-rw-r--r--   0 jjy        (501) staff       (20)       20 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.670261 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4796 2023-07-04 12:12:37.000000 innerverz-0.1.2/innerverz/face_matting/nets/utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 12:13:24.000000 innerverz-0.1.2/innerverz/face_matting/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.671375 innerverz-0.1.2/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2907 2023-07-07 08:51:48.000000 innerverz-0.1.2/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.672108 innerverz-0.1.2/innerverz/face_reshaping/
+-rw-r--r--   0 jjy        (501) staff       (20)       32 2023-07-07 08:56:40.000000 innerverz-0.1.2/innerverz/face_reshaping/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3309 2023-07-07 08:57:28.000000 innerverz-0.1.2/innerverz/face_reshaping/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4248 2023-07-05 11:02:06.000000 innerverz-0.1.2/innerverz/face_reshaping/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.672650 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)     4670 2023-07-04 10:48:50.000000 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/LadderEncoder.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-07-05 10:42:47.000000 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2839 2023-07-05 10:51:39.000000 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/dense_motion.py
+-rw-r--r--   0 jjy        (501) staff       (20)    14452 2023-07-04 10:48:50.000000 innerverz-0.1.2/innerverz/face_reshaping/sub_nets/util.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4687 2023-07-04 10:39:19.000000 innerverz-0.1.2/innerverz/face_reshaping/test.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1585 2023-07-04 10:39:19.000000 innerverz-0.1.2/innerverz/face_reshaping/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.673232 innerverz-0.1.2/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5523 2023-07-05 10:29:48.000000 innerverz-0.1.2/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.674845 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.675402 innerverz-0.1.2/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2423 2023-07-04 11:16:46.000000 innerverz-0.1.2/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.676068 innerverz-0.1.2/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.1.2/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2510 2023-07-04 12:34:32.000000 innerverz-0.1.2/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.1.2/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/reage/net_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.1.2/innerverz/reage/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.676979 innerverz-0.1.2/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3157 2023-07-04 10:45:51.000000 innerverz-0.1.2/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.677588 innerverz-0.1.2/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2390 2023-07-05 10:28:22.000000 innerverz-0.1.2/innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.678113 innerverz-0.1.2/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.679428 innerverz-0.1.2/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.679722 innerverz-0.1.2/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-30 02:29:25.000000 innerverz-0.1.2/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.680670 innerverz-0.1.2/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.1.2/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-07-07 09:58:02.659219 innerverz-0.1.2/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      229 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     4758 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-07-07 09:58:02.000000 innerverz-0.1.2/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.1.2/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-07-07 09:58:02.681258 innerverz-0.1.2/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      808 2023-07-07 09:57:56.000000 innerverz-0.1.2/setup.py
```

### Comparing `innerverz-0.1.0/LICENSE.txt` & `innerverz-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/__init__.py` & `innerverz-0.1.2/innerverz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,9 +124,9 @@
 from .utils import *
 from .face_color_transfer import *
 from .deca import *
 from .face_enhancer import *
 from .relighter import *
 from .video_faceparser import *
 from .reage import *
-from .landmark_warping import *
+from .face_reshaping import *
 from .face_matting import *
```

### Comparing `innerverz-0.1.0/innerverz/data_process/main.py` & `innerverz-0.1.2/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deblurrer/main.py` & `innerverz-0.1.2/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deblurrer/nets.py` & `innerverz-0.1.2/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deblurrer/test.py` & `innerverz-0.1.2/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/main.py` & `innerverz-0.1.2/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/models/FLAME.py` & `innerverz-0.1.2/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/models/decoders.py` & `innerverz-0.1.2/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/models/detectors.py` & `innerverz-0.1.2/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/models/encoders.py` & `innerverz-0.1.2/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/models/face_detectors.py` & `innerverz-0.1.2/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/models/lbs.py` & `innerverz-0.1.2/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/models/resnet.py` & `innerverz-0.1.2/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/test.py` & `innerverz-0.1.2/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/utils/cfg.py` & `innerverz-0.1.2/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.1.2/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/utils/renderer.py` & `innerverz-0.1.2/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.1.2/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.1.2/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deca/utils/util.py` & `innerverz-0.1.2/innerverz/deca/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deep3dmm/main.py` & `innerverz-0.1.2/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deep3dmm/nets.py` & `innerverz-0.1.2/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/deep3dmm/test.py` & `innerverz-0.1.2/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.1.2/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_alignment/landmark.py` & `innerverz-0.1.2/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_alignment/main.py` & `innerverz-0.1.2/innerverz/face_alignment/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_alignment/retina_face.py` & `innerverz-0.1.2/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_alignment/test.py` & `innerverz-0.1.2/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.1.2/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_alignment/utils/transform.py` & `innerverz-0.1.2/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_color_transfer/main.py` & `innerverz-0.1.2/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_color_transfer/nets.py` & `innerverz-0.1.2/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.2/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_color_transfer/test.py` & `innerverz-0.1.2/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_enhancer/main.py` & `innerverz-0.1.2/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_enhancer/nets.py` & `innerverz-0.1.2/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_enhancer/test.py` & `innerverz-0.1.2/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/main.py` & `innerverz-0.1.2/innerverz/face_matting/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/decoders/resnet_decoder.py` & `innerverz-0.1.2/innerverz/face_matting/nets/decoders/resnet_decoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/encoders/MatteFormer.py` & `innerverz-0.1.2/innerverz/face_matting/nets/encoders/MatteFormer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/generators.py` & `innerverz-0.1.2/innerverz/face_matting/nets/generators.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/ops.py` & `innerverz-0.1.2/innerverz/face_matting/nets/ops.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/raft/main.py` & `innerverz-0.1.2/innerverz/face_matting/nets/raft/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/corr.py` & `innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/extractor.py` & `innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/update.py` & `innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/raft/utils/util.py` & `innerverz-0.1.2/innerverz/face_matting/nets/raft/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/nets/utils.py` & `innerverz-0.1.2/innerverz/face_matting/nets/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_matting/test.py` & `innerverz-0.1.2/innerverz/face_matting/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_parser/main.py` & `innerverz-0.1.2/innerverz/face_parser/main.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         
         Returns
         ---------
         dict
             - 'label'
             - 'onehot'
         """
-        
         super(FaceParser, self).__init__()
 
         self.device = device
         self.parsing_net = BiSeNet(n_classes=19).to(self.device)
         
         url_id = get_url_id('~/.invz_pack/', folder_name, ckpt_name)
         root = os.path.join('~/.invz_pack/', folder_name)
@@ -66,14 +65,15 @@
             - min max : (0, 18)
         """
         label = self.parsing_net(tensor_img)
         _label = F.interpolate(label, (output_size,output_size), mode='bilinear').max(1)[1]
         _label = arrange_mask(_label, output_size)
         
         self.dicts['label'] = _label
+        
         return self.dicts
     
     def get_onehot(self, tensor_img, size=512):
         """
         Input
         ---------
             - dtype : tensor
@@ -85,8 +85,8 @@
             - dtype : tensor
             - shape : (b, 19, size, size)
             - min max : (0 or 1)
         """
         label = self.get_label(tensor_img, size)
         onehot = get_one_hot(label.unsqueeze(0))
         self.dicts['onehot'] = onehot
-        return self.dicts
+        return self.dicts
```

### Comparing `innerverz-0.1.0/innerverz/face_parser/nets.py` & `innerverz-0.1.2/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/face_parser/test.py` & `innerverz-0.1.2/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/head_color_transfer/main.py` & `innerverz-0.1.2/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/head_color_transfer/nets.py` & `innerverz-0.1.2/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.1.2/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/head_color_transfer/test.py` & `innerverz-0.1.2/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/id_extractor/main.py` & `innerverz-0.1.2/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/id_extractor/nets.py` & `innerverz-0.1.2/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/id_extractor/test.py` & `innerverz-0.1.2/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/landmark_warping/main.py` & `innerverz-0.1.2/innerverz/face_reshaping/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import sys
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from .sub_nets import MyGenerator
+from .nets import MyGenerator
 from .util import set_random_colors, plot_kpts
 from ..utils import check_ckpt_exist, get_url_id
 
-class Landmark_Warping(nn.Module):
-    def __init__(self, img_size : int = 512, folder_name='landmark_warping', ckpt_name = 'G_38k_unalign_multiaug.pt', force=False, device = 'cuda'):
+class Face_Reshaping(nn.Module):
+    def __init__(self, img_size : int = 512, folder_name='face_reshaping', ckpt_name = 'G_38k_unalign_multiaug.pt', force=False, device = 'cuda'):
         """
             Related Links
             --------
             https://meta-portrait.github.io/
             
             Options
             --------
@@ -65,15 +65,15 @@
             - output
                 - dicts 'result'
                     - dtype : tensor
                     - shape : (b, 3, h, w)
                     - min max : (-1 1)
                 
         """
-        super(Landmark_Warping, self).__init__()
+        super(Face_Reshaping, self).__init__()
         self.device = device
         self.img_size = img_size
         self.generator = MyGenerator().to(self.device)
         
         url_id = get_url_id('~/.invz_pack/', folder_name, ckpt_name)
         root = os.path.join('~/.invz_pack/', folder_name)
         ckpt_path = check_ckpt_exist(root, ckpt_name = ckpt_name, url_id = url_id, force = force)
```

### Comparing `innerverz-0.1.0/innerverz/landmark_warping/nets.py` & `innerverz-0.1.2/innerverz/face_reshaping/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/landmark_warping/sub_nets/LadderEncoder.py` & `innerverz-0.1.2/innerverz/face_reshaping/sub_nets/LadderEncoder.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/landmark_warping/sub_nets/dense_motion.py` & `innerverz-0.1.2/innerverz/face_reshaping/sub_nets/dense_motion.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/landmark_warping/sub_nets/util.py` & `innerverz-0.1.2/innerverz/face_reshaping/sub_nets/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/landmark_warping/test.py` & `innerverz-0.1.2/innerverz/face_reshaping/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/landmark_warping/util.py` & `innerverz-0.1.2/innerverz/face_reshaping/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/reage/main.py` & `innerverz-0.1.2/innerverz/reage/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/reage/net.py` & `innerverz-0.1.2/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/reage/net_utils.py` & `innerverz-0.1.2/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/reage/test.py` & `innerverz-0.1.2/innerverz/reage/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/relighter/main.py` & `innerverz-0.1.2/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/relighter/nets.py` & `innerverz-0.1.2/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/relighter/test.py` & `innerverz-0.1.2/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/upsampler/main.py` & `innerverz-0.1.2/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/upsampler/nets.py` & `innerverz-0.1.2/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/upsampler/test.py` & `innerverz-0.1.2/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/utils/download.py` & `innerverz-0.1.2/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/utils/input.py` & `innerverz-0.1.2/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/utils/utils.py` & `innerverz-0.1.2/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/video_faceparser/main.py` & `innerverz-0.1.2/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/video_faceparser/nets.py` & `innerverz-0.1.2/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.1.2/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.1.2/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/video_faceparser/utils/update.py` & `innerverz-0.1.2/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz/video_faceparser/utils/util.py` & `innerverz-0.1.2/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.1.0/innerverz.egg-info/SOURCES.txt` & `innerverz-0.1.2/innerverz.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -78,36 +78,36 @@
 innerverz/face_matting/nets/raft/utils/extractor.py
 innerverz/face_matting/nets/raft/utils/update.py
 innerverz/face_matting/nets/raft/utils/util.py
 innerverz/face_parser/__init__.py
 innerverz/face_parser/main.py
 innerverz/face_parser/nets.py
 innerverz/face_parser/test.py
+innerverz/face_reshaping/__init__.py
+innerverz/face_reshaping/main.py
+innerverz/face_reshaping/nets.py
+innerverz/face_reshaping/test.py
+innerverz/face_reshaping/util.py
+innerverz/face_reshaping/sub_nets/LadderEncoder.py
+innerverz/face_reshaping/sub_nets/__init__.py
+innerverz/face_reshaping/sub_nets/dense_motion.py
+innerverz/face_reshaping/sub_nets/util.py
 innerverz/head_color_transfer/__init__.py
 innerverz/head_color_transfer/main.py
 innerverz/head_color_transfer/nets.py
 innerverz/head_color_transfer/test.py
 innerverz/head_color_transfer/sub_nets/__init__.py
 innerverz/head_color_transfer/sub_nets/blend_net.py
 innerverz/head_color_transfer/sub_nets/discriminator.py
 innerverz/head_color_transfer/sub_nets/vgg19_net.py
 innerverz/head_color_transfer/sub_nets/warp_net.py
 innerverz/id_extractor/__init__.py
 innerverz/id_extractor/main.py
 innerverz/id_extractor/nets.py
 innerverz/id_extractor/test.py
-innerverz/landmark_warping/__init__.py
-innerverz/landmark_warping/main.py
-innerverz/landmark_warping/nets.py
-innerverz/landmark_warping/test.py
-innerverz/landmark_warping/util.py
-innerverz/landmark_warping/sub_nets/LadderEncoder.py
-innerverz/landmark_warping/sub_nets/__init__.py
-innerverz/landmark_warping/sub_nets/dense_motion.py
-innerverz/landmark_warping/sub_nets/util.py
 innerverz/reage/__init__.py
 innerverz/reage/main.py
 innerverz/reage/net.py
 innerverz/reage/net_utils.py
 innerverz/reage/test.py
 innerverz/relighter/__init__.py
 innerverz/relighter/main.py
```

### Comparing `innerverz-0.1.0/setup.py` & `innerverz-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.1.0",
+    version="0.1.2",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```


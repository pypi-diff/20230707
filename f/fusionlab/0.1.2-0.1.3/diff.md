# Comparing `tmp/fusionlab-0.1.2.tar.gz` & `tmp/fusionlab-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusionlab-0.1.2.tar", last modified: Fri Jun  2 07:56:10 2023, max compression
+gzip compressed data, was "fusionlab-0.1.3.tar", last modified: Fri Jul  7 01:26:44 2023, max compression
```

## Comparing `fusionlab-0.1.2.tar` & `fusionlab-0.1.3.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.659056 fusionlab-0.1.2/
--rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.2/LICENSE
--rw-r--r--   0 cyli       (502) staff       (20)     3337 2023-06-02 07:56:10.658918 fusionlab-0.1.2/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     2874 2023-06-02 07:07:59.000000 fusionlab-0.1.2/README.md
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.645246 fusionlab-0.1.2/fusionlab/
--rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)       63 2023-06-02 07:55:20.000000 fusionlab-0.1.2/fusionlab/__version__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.646571 fusionlab-0.1.2/fusionlab/classification/
--rw-r--r--   0 cyli       (502) staff       (20)      310 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/classification/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      924 2023-05-21 15:35:40.000000 fusionlab-0.1.2/fusionlab/classification/base.py
--rw-r--r--   0 cyli       (502) staff       (20)      701 2023-05-21 15:35:40.000000 fusionlab-0.1.2/fusionlab/classification/lstm.py
--rw-r--r--   0 cyli       (502) staff       (20)     1368 2023-05-21 15:39:08.000000 fusionlab-0.1.2/fusionlab/classification/vgg.py
--rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/configs.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.648114 fusionlab-0.1.2/fusionlab/datasets/
--rw-r--r--   0 cyli       (502) staff       (20)      486 2023-06-02 07:24:15.000000 fusionlab-0.1.2/fusionlab/datasets/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/datasets/a12lead.py
--rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/datasets/cinc2017.py
--rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/datasets/csvread.py
--rw-r--r--   0 cyli       (502) staff       (20)     9199 2023-06-02 07:54:07.000000 fusionlab-0.1.2/fusionlab/datasets/ludb.py
--rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/datasets/muse.py
--rw-r--r--   0 cyli       (502) staff       (20)     1506 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/datasets/utils.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.648238 fusionlab-0.1.2/fusionlab/encoders/
--rw-r--r--   0 cyli       (502) staff       (20)      507 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.648800 fusionlab-0.1.2/fusionlab/encoders/alexnet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/alexnet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-05-22 15:23:04.000000 fusionlab-0.1.2/fusionlab/encoders/alexnet/alexnet.py
--rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.2/fusionlab/encoders/alexnet/tfalexnet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.649319 fusionlab-0.1.2/fusionlab/encoders/inceptionv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/inceptionv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-05-22 15:20:40.000000 fusionlab-0.1.2/fusionlab/encoders/inceptionv1/inceptionv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.2/fusionlab/encoders/inceptionv1/tfinceptionv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.649879 fusionlab-0.1.2/fusionlab/encoders/resnetv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/resnetv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-05-22 15:21:31.000000 fusionlab-0.1.2/fusionlab/encoders/resnetv1/resnetv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.2/fusionlab/encoders/resnetv1/tfresnetv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.650424 fusionlab-0.1.2/fusionlab/encoders/vgg/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/encoders/vgg/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.2/fusionlab/encoders/vgg/tfvgg.py
--rw-r--r--   0 cyli       (502) staff       (20)     4751 2023-05-22 15:25:07.000000 fusionlab-0.1.2/fusionlab/encoders/vgg/vgg.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.651158 fusionlab-0.1.2/fusionlab/functional/
--rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/tfdice.py
--rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/functional/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.651413 fusionlab-0.1.2/fusionlab/layers/
--rw-r--r--   0 cyli       (502) staff       (20)      255 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/layers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)    15525 2023-05-30 12:59:43.000000 fusionlab-0.1.2/fusionlab/layers/factories.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.653071 fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1045 2023-05-20 16:17:48.000000 fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/se.py
--rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/tfse.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.653777 fusionlab-0.1.2/fusionlab/losses/
--rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/losses/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.654234 fusionlab-0.1.2/fusionlab/losses/diceloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/losses/diceloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/losses/diceloss/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.2/fusionlab/losses/diceloss/tfdice.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.654773 fusionlab-0.1.2/fusionlab/losses/iouloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/losses/iouloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/losses/iouloss/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.2/fusionlab/losses/iouloss/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.655331 fusionlab-0.1.2/fusionlab/losses/tversky/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.2/fusionlab/losses/tversky/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.2/fusionlab/losses/tversky/tftversky.py
--rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.2/fusionlab/losses/tversky/tversky.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.655580 fusionlab-0.1.2/fusionlab/metrics/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.2/fusionlab/metrics/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.655923 fusionlab-0.1.2/fusionlab/segmentation/
--rw-r--r--   0 cyli       (502) staff       (20)      378 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      388 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/base.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.656396 fusionlab-0.1.2/fusionlab/segmentation/resunet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.2/fusionlab/segmentation/resunet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     5240 2023-06-02 02:24:31.000000 fusionlab-0.1.2/fusionlab/segmentation/resunet/resunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/resunet/tfresunet.py
--rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/tfbase.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.656758 fusionlab-0.1.2/fusionlab/segmentation/unet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.2/fusionlab/segmentation/unet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/unet/tfunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     5383 2023-05-21 15:35:40.000000 fusionlab-0.1.2/fusionlab/segmentation/unet/unet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.657107 fusionlab-0.1.2/fusionlab/segmentation/unet2plus/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.2/fusionlab/segmentation/unet2plus/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/segmentation/unet2plus/tfunet2plus.py
--rw-r--r--   0 cyli       (502) staff       (20)     5631 2023-05-21 15:35:40.000000 fusionlab-0.1.2/fusionlab/segmentation/unet2plus/unet2plus.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.657849 fusionlab-0.1.2/fusionlab/trainers/
--rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.2/fusionlab/trainers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/trainers/dcgan.py
--rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.2/fusionlab/trainers/test.py
--rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/trainers/trainer.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.658556 fusionlab-0.1.2/fusionlab/utils/
--rw-r--r--   0 cyli       (502) staff       (20)       60 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/utils/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      218 2022-12-31 04:40:09.000000 fusionlab-0.1.2/fusionlab/utils/basic.py
--rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 07:07:59.000000 fusionlab-0.1.2/fusionlab/utils/trace.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-06-02 07:56:10.645914 fusionlab-0.1.2/fusionlab.egg-info/
--rw-r--r--   0 cyli       (502) staff       (20)     3337 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     2501 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/SOURCES.txt
--rw-r--r--   0 cyli       (502) staff       (20)        1 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/dependency_links.txt
--rw-r--r--   0 cyli       (502) staff       (20)      191 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/requires.txt
--rw-r--r--   0 cyli       (502) staff       (20)       10 2023-06-02 07:56:10.000000 fusionlab-0.1.2/fusionlab.egg-info/top_level.txt
--rw-r--r--   0 cyli       (502) staff       (20)       38 2023-06-02 07:56:10.659100 fusionlab-0.1.2/setup.cfg
--rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.2/setup.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.654669 fusionlab-0.1.3/
+-rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.3/LICENSE
+-rw-r--r--   0 cyli       (502) staff       (20)     3762 2023-07-07 01:26:44.654502 fusionlab-0.1.3/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     3299 2023-07-01 03:49:44.000000 fusionlab-0.1.3/README.md
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.632531 fusionlab-0.1.3/fusionlab/
+-rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)       63 2023-07-01 03:50:01.000000 fusionlab-0.1.3/fusionlab/__version__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.634401 fusionlab-0.1.3/fusionlab/classification/
+-rw-r--r--   0 cyli       (502) staff       (20)      387 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/classification/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3353 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/classification/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)      711 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/classification/lstm.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1473 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/classification/vgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/configs.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.635915 fusionlab-0.1.3/fusionlab/datasets/
+-rw-r--r--   0 cyli       (502) staff       (20)      558 2023-07-01 03:49:44.000000 fusionlab-0.1.3/fusionlab/datasets/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/datasets/a12lead.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/datasets/cinc2017.py
+-rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/datasets/csvread.py
+-rw-r--r--   0 cyli       (502) staff       (20)    13273 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/datasets/ludb.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/datasets/muse.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4586 2023-07-01 03:49:44.000000 fusionlab-0.1.3/fusionlab/datasets/utils.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.636210 fusionlab-0.1.3/fusionlab/encoders/
+-rw-r--r--   0 cyli       (502) staff       (20)      507 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.636732 fusionlab-0.1.3/fusionlab/encoders/alexnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/alexnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/encoders/alexnet/alexnet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.3/fusionlab/encoders/alexnet/tfalexnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.637405 fusionlab-0.1.3/fusionlab/encoders/inceptionv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/inceptionv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/encoders/inceptionv1/inceptionv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.3/fusionlab/encoders/inceptionv1/tfinceptionv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.645166 fusionlab-0.1.3/fusionlab/encoders/resnetv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/resnetv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/encoders/resnetv1/resnetv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.3/fusionlab/encoders/resnetv1/tfresnetv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.645887 fusionlab-0.1.3/fusionlab/encoders/vgg/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/encoders/vgg/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.3/fusionlab/encoders/vgg/tfvgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4753 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/encoders/vgg/vgg.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.647468 fusionlab-0.1.3/fusionlab/functional/
+-rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/tfdice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/functional/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.647766 fusionlab-0.1.3/fusionlab/layers/
+-rw-r--r--   0 cyli       (502) staff       (20)      255 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/layers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)    17810 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/layers/factories.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.648470 fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1045 2023-05-20 16:17:48.000000 fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/se.py
+-rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/tfse.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.648729 fusionlab-0.1.3/fusionlab/losses/
+-rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/losses/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.649202 fusionlab-0.1.3/fusionlab/losses/diceloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/losses/diceloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/losses/diceloss/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.3/fusionlab/losses/diceloss/tfdice.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.649776 fusionlab-0.1.3/fusionlab/losses/iouloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/losses/iouloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/losses/iouloss/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.3/fusionlab/losses/iouloss/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.650359 fusionlab-0.1.3/fusionlab/losses/tversky/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.3/fusionlab/losses/tversky/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.3/fusionlab/losses/tversky/tftversky.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.3/fusionlab/losses/tversky/tversky.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.650605 fusionlab-0.1.3/fusionlab/metrics/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.3/fusionlab/metrics/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.651009 fusionlab-0.1.3/fusionlab/segmentation/
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1770 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/base.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.651443 fusionlab-0.1.3/fusionlab/segmentation/resunet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.3/fusionlab/segmentation/resunet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5271 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/resunet/resunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/segmentation/resunet/tfresunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/segmentation/tfbase.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.651877 fusionlab-0.1.3/fusionlab/segmentation/unet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.3/fusionlab/segmentation/unet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/segmentation/unet/tfunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5414 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/unet/unet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.652361 fusionlab-0.1.3/fusionlab/segmentation/unet2plus/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.3/fusionlab/segmentation/unet2plus/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/segmentation/unet2plus/tfunet2plus.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5662 2023-07-01 03:49:33.000000 fusionlab-0.1.3/fusionlab/segmentation/unet2plus/unet2plus.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.653167 fusionlab-0.1.3/fusionlab/trainers/
+-rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.3/fusionlab/trainers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/trainers/dcgan.py
+-rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.3/fusionlab/trainers/test.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/trainers/trainer.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.654147 fusionlab-0.1.3/fusionlab/utils/
+-rw-r--r--   0 cyli       (502) staff       (20)       93 2023-07-01 03:49:44.000000 fusionlab-0.1.3/fusionlab/utils/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      218 2022-12-31 04:40:09.000000 fusionlab-0.1.3/fusionlab/utils/basic.py
+-rw-r--r--   0 cyli       (502) staff       (20)      406 2023-07-01 03:49:44.000000 fusionlab-0.1.3/fusionlab/utils/plots.py
+-rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 08:43:17.000000 fusionlab-0.1.3/fusionlab/utils/trace.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-07 01:26:44.633307 fusionlab-0.1.3/fusionlab.egg-info/
+-rw-r--r--   0 cyli       (502) staff       (20)     3762 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     2526 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/SOURCES.txt
+-rw-r--r--   0 cyli       (502) staff       (20)        1 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/dependency_links.txt
+-rw-r--r--   0 cyli       (502) staff       (20)      191 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/requires.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       10 2023-07-07 01:26:44.000000 fusionlab-0.1.3/fusionlab.egg-info/top_level.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       38 2023-07-07 01:26:44.654721 fusionlab-0.1.3/setup.cfg
+-rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.3/setup.py
```

### Comparing `fusionlab-0.1.2/LICENSE` & `fusionlab-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/PKG-INFO` & `fusionlab-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.2
+Version: 0.1.3
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,37 +19,38 @@
 
 <p align="center">
     <br>
     <img src="assets/imgs/fusionlab_banner.png" width="400"/>
     <br>
 <p>
 
-![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
+[![PyPI version](https://badge.fury.io/py/fusionlab.svg)](https://badge.fury.io/py/fusionlab) ![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
 
 FusionLab is an open-source frameworks built for Deep Learning research written in PyTorch and Tensorflow. The code is easy to read and modify 
 especially for newbie. Feel free to send pull requests :D
 
 * [What's New](#News)
 * [Installation](#Installation)
 * [How to use](#How-to-use)
 * [Encoders](#Encoders)
 * [Losses](#Losses)
 * [Segmentation](#Segmentation)
+* [1D, 2D, 3D Model](#n-dimensional-model)
 * [Acknowledgements](#Acknowledgements)
 
 ## Installation
 
 ### With pip
 
 ```bash
 pip install fusionlab
 ```
 
 #### For Mac M1 chip users
-Go to [Install on Macbook M1 chip](./configs/Install%20on%20Macbook%20M1.md) 
+[Install on Macbook M1 chip](./configs/Install%20on%20Macbook%20M1.md) 
 
 ## How to use
 
 ```python
 import fusionlab as fl
 
 # PyTorch
@@ -70,34 +71,32 @@
 * Tversky Loss
 * IoU Loss
 
 
 ```python
 # Dice Loss (Multiclass)
 import fusionlab as fl
-import torch
-import tensorflow as tf
 
 # PyTorch
-pred = torch.normal(0., 1., (1, 3, 4, 4)) # (N, C, *)
+pred = torch.randn(1, 3, 4, 4) # (N, C, *)
 target = torch.randint(0, 3, (1, 4, 4)) # (N, *)
 loss_fn = fl.losses.DiceLoss()
 loss = loss_fn(pred, target)
 
 # Tensorflow
 pred = tf.random.normal((1, 4, 4, 3), 0., 1.) # (N, *, C)
 target = tf.random.uniform((1, 4, 4), 0, 3) # (N, *)
 loss_fn = fl.losses.TFDiceLoss("multiclass")
 loss = loss_fn(target, pred)
 
 
 # Dice Loss (Binary)
 
 # PyTorch
-pred = torch.normal(0, 1, (1, 1, 4, 4)) # (N, 1, *)
+pred = torch.randn(1, 1, 4, 4) # (N, 1, *)
 target = torch.randint(0, 3, (1, 4, 4)) # (N, *)
 loss_fn = fl.losses.DiceLoss("binary")
 loss = loss_fn(pred, target)
 
 # Tensorflow
 pred = tf.random.normal((1, 4, 4, 1), 0., 1.) # (N, *, 1)
 target = tf.random.uniform((1, 4, 4), 0, 3) # (N, *)
@@ -108,44 +107,58 @@
 ```
 
 ## Segmentation
 
 ```python
 import fusionlab as fl
 # PyTorch UNet
-unet = fl.segmentation.UNet(cin=3, num_cls=10, base_dim=64)
+unet = fl.segmentation.UNet(cin=3, num_cls=10)
 
 # Tensorflow UNet
-import tensorflow as tf
-
 # Multiclass Segmentation
 unet = tf.keras.Sequential([
    fl.segmentation.TFUNet(num_cls=10, base_dim=64),
    tf.keras.layers.Activation(tf.nn.softmax),
 ])
-unet.compile(loss=fl.losses.TFDiceLoss("multiclass"))
 
 # Binary Segmentation
 unet = tf.keras.Sequential([
    fl.segmentation.TFUNet(num_cls=1, base_dim=64),
    tf.keras.layers.Activation(tf.nn.sigmoid),
 ])
-unet.compile(loss=fl.losses.TFDiceLoss("binary"))
-
-
 ```
 
 [Segmentation model list](fusionlab/segmentation/README.md)
 
 * UNet
 * ResUNet
 * UNet2plus
 
+## N Dimensional Model
+
+some model can be used in 1D, 2D, 3D
+
+```python
+import fusionlab as fl
+
+resnet1d = fl.encoders.ResNet50V1(cin=3, spatial_dims=1)
+resnet2d = fl.encoders.ResNet50V1(cin=3, spatial_dims=2)
+resnet3d = fl.encoders.ResNet50V1(cin=3, spatial_dims=3)
+
+unet1d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=1)
+unet2d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=2)
+unet3d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=3)
+```
+
 ## News
 
+0.1.2
+
+* Add LUDB dataset
+
 0.0.52
 
 * Tversky Loss for Torch and TF
 
 ## Acknowledgements
 
 * [BloodAxe/pytorch-toolbelt](https://github.com/BloodAxe/pytorch-toolbelt)
```

### Comparing `fusionlab-0.1.2/README.md` & `fusionlab-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 
 <p align="center">
     <br>
     <img src="assets/imgs/fusionlab_banner.png" width="400"/>
     <br>
 <p>
 
-![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
+[![PyPI version](https://badge.fury.io/py/fusionlab.svg)](https://badge.fury.io/py/fusionlab) ![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
 
 FusionLab is an open-source frameworks built for Deep Learning research written in PyTorch and Tensorflow. The code is easy to read and modify 
 especially for newbie. Feel free to send pull requests :D
 
 * [What's New](#News)
 * [Installation](#Installation)
 * [How to use](#How-to-use)
 * [Encoders](#Encoders)
 * [Losses](#Losses)
 * [Segmentation](#Segmentation)
+* [1D, 2D, 3D Model](#n-dimensional-model)
 * [Acknowledgements](#Acknowledgements)
 
 ## Installation
 
 ### With pip
 
 ```bash
 pip install fusionlab
 ```
 
 #### For Mac M1 chip users
-Go to [Install on Macbook M1 chip](./configs/Install%20on%20Macbook%20M1.md) 
+[Install on Macbook M1 chip](./configs/Install%20on%20Macbook%20M1.md) 
 
 ## How to use
 
 ```python
 import fusionlab as fl
 
 # PyTorch
@@ -53,34 +54,32 @@
 * Tversky Loss
 * IoU Loss
 
 
 ```python
 # Dice Loss (Multiclass)
 import fusionlab as fl
-import torch
-import tensorflow as tf
 
 # PyTorch
-pred = torch.normal(0., 1., (1, 3, 4, 4)) # (N, C, *)
+pred = torch.randn(1, 3, 4, 4) # (N, C, *)
 target = torch.randint(0, 3, (1, 4, 4)) # (N, *)
 loss_fn = fl.losses.DiceLoss()
 loss = loss_fn(pred, target)
 
 # Tensorflow
 pred = tf.random.normal((1, 4, 4, 3), 0., 1.) # (N, *, C)
 target = tf.random.uniform((1, 4, 4), 0, 3) # (N, *)
 loss_fn = fl.losses.TFDiceLoss("multiclass")
 loss = loss_fn(target, pred)
 
 
 # Dice Loss (Binary)
 
 # PyTorch
-pred = torch.normal(0, 1, (1, 1, 4, 4)) # (N, 1, *)
+pred = torch.randn(1, 1, 4, 4) # (N, 1, *)
 target = torch.randint(0, 3, (1, 4, 4)) # (N, *)
 loss_fn = fl.losses.DiceLoss("binary")
 loss = loss_fn(pred, target)
 
 # Tensorflow
 pred = tf.random.normal((1, 4, 4, 1), 0., 1.) # (N, *, 1)
 target = tf.random.uniform((1, 4, 4), 0, 3) # (N, *)
@@ -91,44 +90,58 @@
 ```
 
 ## Segmentation
 
 ```python
 import fusionlab as fl
 # PyTorch UNet
-unet = fl.segmentation.UNet(cin=3, num_cls=10, base_dim=64)
+unet = fl.segmentation.UNet(cin=3, num_cls=10)
 
 # Tensorflow UNet
-import tensorflow as tf
-
 # Multiclass Segmentation
 unet = tf.keras.Sequential([
    fl.segmentation.TFUNet(num_cls=10, base_dim=64),
    tf.keras.layers.Activation(tf.nn.softmax),
 ])
-unet.compile(loss=fl.losses.TFDiceLoss("multiclass"))
 
 # Binary Segmentation
 unet = tf.keras.Sequential([
    fl.segmentation.TFUNet(num_cls=1, base_dim=64),
    tf.keras.layers.Activation(tf.nn.sigmoid),
 ])
-unet.compile(loss=fl.losses.TFDiceLoss("binary"))
-
-
 ```
 
 [Segmentation model list](fusionlab/segmentation/README.md)
 
 * UNet
 * ResUNet
 * UNet2plus
 
+## N Dimensional Model
+
+some model can be used in 1D, 2D, 3D
+
+```python
+import fusionlab as fl
+
+resnet1d = fl.encoders.ResNet50V1(cin=3, spatial_dims=1)
+resnet2d = fl.encoders.ResNet50V1(cin=3, spatial_dims=2)
+resnet3d = fl.encoders.ResNet50V1(cin=3, spatial_dims=3)
+
+unet1d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=1)
+unet2d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=2)
+unet3d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=3)
+```
+
 ## News
 
+0.1.2
+
+* Add LUDB dataset
+
 0.0.52
 
 * Tversky Loss for Torch and TF
 
 ## Acknowledgements
 
 * [BloodAxe/pytorch-toolbelt](https://github.com/BloodAxe/pytorch-toolbelt)
```

### Comparing `fusionlab-0.1.2/fusionlab/__init__.py` & `fusionlab-0.1.3/fusionlab/__init__.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/classification/lstm.py` & `fusionlab-0.1.3/fusionlab/classification/lstm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from torch import nn
-from fusionlab.classification.base import RNNClassification
+from fusionlab.classification.base import RNNClassificationModel
 
 
-class LSTMClassifier(RNNClassification):
+class LSTMClassifier(RNNClassificationModel):
     def __init__(self, cin, cout, hidden_size=512):
         super().__init__()
         self.encoder = nn.LSTM(input_size=cin, hidden_size=hidden_size, batch_first=True) # define LSTM layer
         self.head = nn.Linear(hidden_size, cout) # define output head layer
 
 if __name__ == '__main__':
     inputs = torch.randn(1, 5, 3) # create random input tensor
```

### Comparing `fusionlab-0.1.2/fusionlab/classification/vgg.py` & `fusionlab-0.1.3/fusionlab/classification/vgg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # VGG Classifier
 import torch
 from torch import nn
-from fusionlab.classification.base import CNNClassification
+from fusionlab.classification.base import CNNClassificationModel
 from fusionlab.encoders import VGG16, VGG19
 from fusionlab.layers import AdaptiveAvgPool
 
-class VGG16Classifier(CNNClassification):
-    def __init__(self, spatial_dims, cin, cout):
+class VGG16Classifier(CNNClassificationModel):
+    def __init__(self, cin, num_cls, spatial_dims=2):
         super().__init__()
-        self.encoder = VGG16(spatial_dims, cin) # Create VGG16 instance
+        self.num_cls = num_cls
+        self.encoder = VGG16(cin, spatial_dims) # Create VGG16 instance
         self.globalpooling = AdaptiveAvgPool(spatial_dims, 1)
-        self.head = nn.Linear(512, cout)
+        self.head = nn.Linear(512, num_cls)
 
-class VGG19Classifier(CNNClassification):
-    def __init__(self, spatial_dims, cin, cout):
+class VGG19Classifier(CNNClassificationModel):
+    def __init__(self, cin, num_cls, spatial_dims=2):
         super().__init__()
-        self.encoder = VGG19(spatial_dims, cin) # Create VGG16 instance
+        self.num_cls = num_cls
+        self.encoder = VGG19(cin, spatial_dims) # Create VGG16 instance
         self.globalpooling = AdaptiveAvgPool(spatial_dims, 1)
-        self.head = nn.Linear(512, cout)
+        self.head = nn.Linear(512, num_cls)
 
 
 if __name__ == '__main__':
-    inputs = torch.randn(1, 224, 3) # create random input tensor
-    model = VGG16Classifier(spatial_dims=1, cin=3, cout=2) # create model instance
+    inputs = torch.randn(1, 3, 224) # create random input tensor
+    model = VGG16Classifier(cin=3, num_cls=2, spatial_dims=1) # create model instance
     outputs = model(inputs) # pass input through model
     assert list(outputs.shape) == [1, 2] # check output shape is correct
 
-    inputs = torch.randn(1, 224, 3) # create random input tensor
-    model = VGG19Classifier(spatial_dims=1,cin=3, cout=2) # create model instance
+    inputs = torch.randn(1, 3, 224) # create random input tensor
+    model = VGG19Classifier(cin=3, num_cls=2, spatial_dims=1) # create model instance
+    
     outputs = model(inputs) # pass input through model
     assert list(outputs.shape) == [1, 2] # check output shape is correct
```

### Comparing `fusionlab-0.1.2/fusionlab/datasets/a12lead.py` & `fusionlab-0.1.3/fusionlab/datasets/a12lead.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/datasets/cinc2017.py` & `fusionlab-0.1.3/fusionlab/datasets/cinc2017.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/datasets/muse.py` & `fusionlab-0.1.3/fusionlab/datasets/muse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/encoders/alexnet/alexnet.py` & `fusionlab-0.1.3/fusionlab/encoders/alexnet/alexnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn as nn
 from fusionlab.layers.factories import ConvND, MaxPool
 
 # Official pytorch ref: https://github.com/pytorch/vision/blob/main/torchvision/models/alexnet.py
 class AlexNet(nn.Module):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__()
         self.features = nn.Sequential(
             ConvND(spatial_dims, cin, 64, kernel_size=11, stride=4, padding=2),
             nn.ReLU(inplace=True),
             MaxPool(spatial_dims, kernel_size=3, stride=2),
             ConvND(spatial_dims, 64, 192, kernel_size=5, padding=2),
             nn.ReLU(inplace=True),
```

### Comparing `fusionlab-0.1.2/fusionlab/encoders/alexnet/tfalexnet.py` & `fusionlab-0.1.3/fusionlab/encoders/alexnet/tfalexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/encoders/inceptionv1/inceptionv1.py` & `fusionlab-0.1.3/fusionlab/encoders/inceptionv1/inceptionv1.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         x2 = self.branch5(x)
         x3 = self.pool(x)
         x = torch.cat((x0, x1, x2, x3), 1)
         return x
 
 
 class InceptionNetV1(nn.Module):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__()
         self.stem = nn.Sequential(
             ConvBlock(cin, 64, 7, spatial_dims, stride=2),
             MaxPool(spatial_dims, 3, 2, padding=autopad(3)),
             ConvBlock(64, 192, 3, spatial_dims),
             MaxPool(spatial_dims, 3, 2, padding=autopad(3)),
         )
```

### Comparing `fusionlab-0.1.2/fusionlab/encoders/inceptionv1/tfinceptionv1.py` & `fusionlab-0.1.3/fusionlab/encoders/inceptionv1/tfinceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/encoders/resnetv1/resnetv1.py` & `fusionlab-0.1.3/fusionlab/encoders/resnetv1/resnetv1.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 class StageBlock(nn.Sequential):
     def __init__(self, cin, dims, stride, repeats):
         super().__init__()
 
 
 class ResNet50V1(nn.Module):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__()
         self.conv1 = Stem(cin, spatial_dims)
         self.conv2 = nn.Sequential(
             Bottleneck(64, [64, 256], 3, spatial_dims, stride=1),
             Bottleneck(256, [64, 256], 3, spatial_dims),
             Bottleneck(256, [64, 256], 3, spatial_dims),
         )
```

### Comparing `fusionlab-0.1.2/fusionlab/encoders/resnetv1/tfresnetv1.py` & `fusionlab-0.1.3/fusionlab/encoders/resnetv1/tfresnetv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/encoders/vgg/tfvgg.py` & `fusionlab-0.1.3/fusionlab/encoders/vgg/tfvgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/encoders/vgg/vgg.py` & `fusionlab-0.1.3/fusionlab/encoders/vgg/vgg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn as nn
 from fusionlab.layers import ConvND, MaxPool
 
 # Official pytorch ref: https://github.com/pytorch/vision/blob/main/torchvision/models/vgg.py
 class VGG16(nn.Module):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__()
         ksize = 3
         self.features = nn.Sequential(
             ConvND(spatial_dims, cin, 64, ksize, padding=1),
             nn.ReLU(inplace=True),
             ConvND(spatial_dims, 64, 64, ksize, padding=1),
             nn.ReLU(inplace=True),
@@ -46,15 +46,15 @@
         )
 
     def forward(self, x):
         return self.features(x)
 
 
 class VGG19(nn.Module):
-    def __init__(self, spatial_dims=2, cin=3):
+    def __init__(self, cin=3, spatial_dims=2):
         super().__init__()
         ksize = 3
         self.features = nn.Sequential(
             ConvND(spatial_dims, cin, 64, ksize, padding=1),
             nn.ReLU(inplace=True),
             ConvND(spatial_dims, 64, 64, ksize, padding=1),
             nn.ReLU(inplace=True),
@@ -102,28 +102,28 @@
 
 
 
 
 if __name__ == '__main__':
     # VGG16
     inputs = torch.normal(0, 1, (1, 3, 224))
-    output = VGG16(spatial_dims=1, cin=3)(inputs)
+    output = VGG16(cin=3, spatial_dims=1)(inputs)
     shape = list(output.shape)
     assert shape[2:] == [7]
 
     # VGG19
     inputs = torch.normal(0, 1, (1, 3, 224))
-    output = VGG19(spatial_dims=1, cin=3)(inputs)
+    output = VGG19(cin=3, spatial_dims=1)(inputs)
     shape = list(output.shape)
     assert shape[2:] == [7]
 
     # VGG16
     inputs = torch.normal(0, 1, (1, 3, 224, 224))
-    output = VGG16(spatial_dims=2, cin=3)(inputs)
+    output = VGG16(cin=3,  spatial_dims=2)(inputs)
     shape = list(output.shape)
     assert shape[2:] == [7, 7]
 
     # VGG19
     inputs = torch.normal(0, 1, (1, 3, 224, 224))
-    output = VGG19(spatial_dims=2, cin=3)(inputs)
+    output = VGG19(cin=3,  spatial_dims=2)(inputs)
     shape = list(output.shape)
     assert shape[2:] == [7, 7]
```

### Comparing `fusionlab-0.1.2/fusionlab/functional/tfdice.py` & `fusionlab-0.1.3/fusionlab/functional/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/functional/tfiou.py` & `fusionlab-0.1.3/fusionlab/functional/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/layers/factories.py` & `fusionlab-0.1.3/fusionlab/layers/factories.py`

 * *Files 17% similar despite different names*

```diff
@@ -329,13 +329,61 @@
         pad_type=getattr(nn, f'ConstantPad{spatial_dims}d')
         return pad_type(
             padding=padding,
             value=value)
 
 
 if __name__ == '__main__':
+
+    # Test Code for ConvND
     inputs = torch.randn(1, 3, 16) # create random input tensor
     layer = ConvND(spatial_dims=1, in_channels=3, out_channels=2, kernel_size=5) # create model instance
     outputs = layer(inputs) # pass input through model
     print(outputs.shape)
     assert list(outputs.shape) == [1, 2, 12] # check output shape is correct
 
+    # Test code for ConvT
+    inputs = torch.randn(1, 3, 16) # create random input tensor
+    layer = ConvT(spatial_dims=1, in_channels=3, out_channels=2, kernel_size=5) # create model instance
+    outputs = layer(inputs) # pass input through model
+    print(outputs.shape)
+    assert list(outputs.shape) == [1, 2, 20] # check output shape is correct
+
+    # Test code for Upsample
+    inputs = torch.randn(1, 3, 16) # create random input tensor
+    layer = Upsample(spatial_dims=1, scale_factor=2) # create model instance
+    outputs = layer(inputs) # pass input through model
+    print(outputs.shape)
+    assert list(outputs.shape) == [1, 3, 32] # check output shape is correct
+
+    # Test code for BatchNormND
+    inputs = torch.randn(1, 3, 16) # create random input tensor
+    layer = BatchNorm(spatial_dims=1, num_features=3) # create model instance
+    outputs = layer(inputs) # pass input through model
+
+    # Test code for MaxPool
+    for Module in [MaxPool, AvgPool]:
+        inputs = torch.randn(1, 3, 16) # create random input tensor
+        layer = Module(spatial_dims=1, kernel_size=2) # create model instance
+        outputs = layer(inputs) # pass input through model
+        print(outputs.shape)
+        assert list(outputs.shape) == [1, 3, 8] # check output shape is correct
+
+    # Test code for Pool
+    for Module in [AdaptiveMaxPool, AdaptiveAvgPool]:
+        inputs = torch.randn(1, 3, 16) # create random input tensor
+        layer = Module(spatial_dims=1, output_size=8) # create model instance
+        outputs = layer(inputs) # pass input through model
+        print(outputs.shape)
+        assert list(outputs.shape) == [1, 3, 8] # check output shape is correct
+
+    # Test code for Padding
+    inputs = torch.randn(1, 3, 16) # create random input tensor
+    layer = ReplicationPad(spatial_dims=1, padding=2) # create model instance
+    outputs = layer(inputs) # pass input through model
+    print(outputs.shape)
+    assert list(outputs.shape) == [1, 3, 20] # check output shape is correct
+    
+    layer = ConstantPad(spatial_dims=1, padding=2, value=0) # create model instance
+    outputs = layer(inputs) # pass input through model
+    print(outputs.shape)
+    assert list(outputs.shape) == [1, 3, 20] # check output shape is correct
```

### Comparing `fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/se.py` & `fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/se.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/layers/squeeze_excitation/tfse.py` & `fusionlab-0.1.3/fusionlab/layers/squeeze_excitation/tfse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/losses/diceloss/dice.py` & `fusionlab-0.1.3/fusionlab/losses/diceloss/dice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/losses/diceloss/tfdice.py` & `fusionlab-0.1.3/fusionlab/losses/diceloss/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/losses/iouloss/iou.py` & `fusionlab-0.1.3/fusionlab/losses/iouloss/iou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/losses/iouloss/tfiou.py` & `fusionlab-0.1.3/fusionlab/losses/iouloss/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/losses/tversky/tftversky.py` & `fusionlab-0.1.3/fusionlab/losses/tversky/tftversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/losses/tversky/tversky.py` & `fusionlab-0.1.3/fusionlab/losses/tversky/tversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/segmentation/resunet/resunet.py` & `fusionlab-0.1.3/fusionlab/segmentation/resunet/resunet.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from fusionlab.layers.factories import ConvND, ConvT, BatchNorm
 
 
 
 class ResUNet(SegmentationModel):
     def __init__(self, cin, num_cls, base_dim, spatial_dims=2):
         super().__init__()
+        self.num_cls = num_cls
         self.encoder = Encoder(cin, base_dim, spatial_dims)
         self.bridger = Bridger()
         self.decoder = Decoder(base_dim, spatial_dims)
         self.head = Head(base_dim, num_cls, spatial_dims)
 
 
 class Encoder(nn.Module):
```

### Comparing `fusionlab-0.1.2/fusionlab/segmentation/resunet/tfresunet.py` & `fusionlab-0.1.3/fusionlab/segmentation/resunet/tfresunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/segmentation/tfbase.py` & `fusionlab-0.1.3/fusionlab/segmentation/tfbase.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/segmentation/unet/tfunet.py` & `fusionlab-0.1.3/fusionlab/segmentation/unet/tfunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/segmentation/unet/unet.py` & `fusionlab-0.1.3/fusionlab/segmentation/unet/unet.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         Args:
             cin (int): input channels
             num_cls (int): number of classes
             base_dim (int): 1st stage dim of conv output
         """
         super().__init__()
         stage = 5
+        self.num_cls = num_cls
         self.encoder = Encoder(cin, base_dim=base_dim, spatial_dims=spatial_dims)
         self.bridger = Bridger()
         self.decoder = Decoder(cin=base_dim*(2**(stage-1)),
                                base_dim=base_dim*(2**(stage-2)), 
                                spatial_dims=spatial_dims)  # 1024, 512
         self.head = Head(base_dim, num_cls, spatial_dims=spatial_dims)
```

### Comparing `fusionlab-0.1.2/fusionlab/segmentation/unet2plus/tfunet2plus.py` & `fusionlab-0.1.3/fusionlab/segmentation/unet2plus/tfunet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/segmentation/unet2plus/unet2plus.py` & `fusionlab-0.1.3/fusionlab/segmentation/unet2plus/unet2plus.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # ref: https://github.com/4uiiurz1/pytorch-nested-unet
 
 
 class UNet2plus(SegmentationModel):
     def __init__(self, cin, num_cls, base_dim, spatial_dims=2):
         super().__init__()
+        self.num_cls = num_cls
         self.encoder = Encoder(cin, base_dim, spatial_dims)
         self.bridger = Bridger()
         self.decoder = Decoder(base_dim, spatial_dims)
         self.head = Head(base_dim, num_cls, spatial_dims)
 
 
 class BasicBlock(nn.Sequential):
```

### Comparing `fusionlab-0.1.2/fusionlab/trainers/dcgan.py` & `fusionlab-0.1.3/fusionlab/trainers/dcgan.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/trainers/trainer.py` & `fusionlab-0.1.3/fusionlab/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab/utils/trace.py` & `fusionlab-0.1.3/fusionlab/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.2/fusionlab.egg-info/PKG-INFO` & `fusionlab-0.1.3/fusionlab.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.2
+Version: 0.1.3
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,37 +19,38 @@
 
 <p align="center">
     <br>
     <img src="assets/imgs/fusionlab_banner.png" width="400"/>
     <br>
 <p>
 
-![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
+[![PyPI version](https://badge.fury.io/py/fusionlab.svg)](https://badge.fury.io/py/fusionlab) ![Test](https://github.com/taipingeric/fusionlab/actions/workflows/python-app.yml/badge.svg)  [![Downloads](https://static.pepy.tech/badge/fusionlab)](https://pepy.tech/project/fusionlab)
 
 FusionLab is an open-source frameworks built for Deep Learning research written in PyTorch and Tensorflow. The code is easy to read and modify 
 especially for newbie. Feel free to send pull requests :D
 
 * [What's New](#News)
 * [Installation](#Installation)
 * [How to use](#How-to-use)
 * [Encoders](#Encoders)
 * [Losses](#Losses)
 * [Segmentation](#Segmentation)
+* [1D, 2D, 3D Model](#n-dimensional-model)
 * [Acknowledgements](#Acknowledgements)
 
 ## Installation
 
 ### With pip
 
 ```bash
 pip install fusionlab
 ```
 
 #### For Mac M1 chip users
-Go to [Install on Macbook M1 chip](./configs/Install%20on%20Macbook%20M1.md) 
+[Install on Macbook M1 chip](./configs/Install%20on%20Macbook%20M1.md) 
 
 ## How to use
 
 ```python
 import fusionlab as fl
 
 # PyTorch
@@ -70,34 +71,32 @@
 * Tversky Loss
 * IoU Loss
 
 
 ```python
 # Dice Loss (Multiclass)
 import fusionlab as fl
-import torch
-import tensorflow as tf
 
 # PyTorch
-pred = torch.normal(0., 1., (1, 3, 4, 4)) # (N, C, *)
+pred = torch.randn(1, 3, 4, 4) # (N, C, *)
 target = torch.randint(0, 3, (1, 4, 4)) # (N, *)
 loss_fn = fl.losses.DiceLoss()
 loss = loss_fn(pred, target)
 
 # Tensorflow
 pred = tf.random.normal((1, 4, 4, 3), 0., 1.) # (N, *, C)
 target = tf.random.uniform((1, 4, 4), 0, 3) # (N, *)
 loss_fn = fl.losses.TFDiceLoss("multiclass")
 loss = loss_fn(target, pred)
 
 
 # Dice Loss (Binary)
 
 # PyTorch
-pred = torch.normal(0, 1, (1, 1, 4, 4)) # (N, 1, *)
+pred = torch.randn(1, 1, 4, 4) # (N, 1, *)
 target = torch.randint(0, 3, (1, 4, 4)) # (N, *)
 loss_fn = fl.losses.DiceLoss("binary")
 loss = loss_fn(pred, target)
 
 # Tensorflow
 pred = tf.random.normal((1, 4, 4, 1), 0., 1.) # (N, *, 1)
 target = tf.random.uniform((1, 4, 4), 0, 3) # (N, *)
@@ -108,44 +107,58 @@
 ```
 
 ## Segmentation
 
 ```python
 import fusionlab as fl
 # PyTorch UNet
-unet = fl.segmentation.UNet(cin=3, num_cls=10, base_dim=64)
+unet = fl.segmentation.UNet(cin=3, num_cls=10)
 
 # Tensorflow UNet
-import tensorflow as tf
-
 # Multiclass Segmentation
 unet = tf.keras.Sequential([
    fl.segmentation.TFUNet(num_cls=10, base_dim=64),
    tf.keras.layers.Activation(tf.nn.softmax),
 ])
-unet.compile(loss=fl.losses.TFDiceLoss("multiclass"))
 
 # Binary Segmentation
 unet = tf.keras.Sequential([
    fl.segmentation.TFUNet(num_cls=1, base_dim=64),
    tf.keras.layers.Activation(tf.nn.sigmoid),
 ])
-unet.compile(loss=fl.losses.TFDiceLoss("binary"))
-
-
 ```
 
 [Segmentation model list](fusionlab/segmentation/README.md)
 
 * UNet
 * ResUNet
 * UNet2plus
 
+## N Dimensional Model
+
+some model can be used in 1D, 2D, 3D
+
+```python
+import fusionlab as fl
+
+resnet1d = fl.encoders.ResNet50V1(cin=3, spatial_dims=1)
+resnet2d = fl.encoders.ResNet50V1(cin=3, spatial_dims=2)
+resnet3d = fl.encoders.ResNet50V1(cin=3, spatial_dims=3)
+
+unet1d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=1)
+unet2d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=2)
+unet3d = fl.segmentation.UNet(cin=3, num_cls=10, spatial_dims=3)
+```
+
 ## News
 
+0.1.2
+
+* Add LUDB dataset
+
 0.0.52
 
 * Tversky Loss for Torch and TF
 
 ## Acknowledgements
 
 * [BloodAxe/pytorch-toolbelt](https://github.com/BloodAxe/pytorch-toolbelt)
```

### Comparing `fusionlab-0.1.2/fusionlab.egg-info/SOURCES.txt` & `fusionlab-0.1.3/fusionlab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,8 +68,9 @@
 fusionlab/segmentation/unet2plus/unet2plus.py
 fusionlab/trainers/__init__.py
 fusionlab/trainers/dcgan.py
 fusionlab/trainers/test.py
 fusionlab/trainers/trainer.py
 fusionlab/utils/__init__.py
 fusionlab/utils/basic.py
+fusionlab/utils/plots.py
 fusionlab/utils/trace.py
```

### Comparing `fusionlab-0.1.2/setup.py` & `fusionlab-0.1.3/setup.py`

 * *Files identical despite different names*


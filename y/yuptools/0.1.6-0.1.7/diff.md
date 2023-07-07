# Comparing `tmp/yuptools-0.1.6.tar.gz` & `tmp/yuptools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuptools-0.1.6.tar", last modified: Fri Jul  7 09:35:18 2023, max compression
+gzip compressed data, was "yuptools-0.1.7.tar", last modified: Fri Jul  7 10:34:14 2023, max compression
```

## Comparing `yuptools-0.1.6.tar` & `yuptools-0.1.7.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:18.506030 yuptools-0.1.6/
--rw-rw-rw-   0        0        0     1088 2023-04-21 08:53:14.000000 yuptools-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3198 2023-07-07 09:35:18.505193 yuptools-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2957 2023-07-07 09:34:58.000000 yuptools-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 09:35:18.507028 yuptools-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-07-07 09:34:58.000000 yuptools-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:13.552817 yuptools-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:13.673847 yuptools-0.1.6/src/yuptools/
--rw-rw-rw-   0        0        0      240 2023-05-21 22:00:40.000000 yuptools-0.1.6/src/yuptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:13.965351 yuptools-0.1.6/src/yuptools/attacks/
--rw-rw-rw-   0        0        0       43 2023-05-21 01:50:37.000000 yuptools-0.1.6/src/yuptools/attacks/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-05-23 23:07:37.000000 yuptools-0.1.6/src/yuptools/attacks/fgsm.py
--rw-rw-rw-   0        0        0     2872 2023-05-22 04:35:07.000000 yuptools-0.1.6/src/yuptools/attacks/ifgsm.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:14.248871 yuptools-0.1.6/src/yuptools/datasets/
--rw-rw-rw-   0        0        0       86 2023-05-25 12:15:58.000000 yuptools-0.1.6/src/yuptools/datasets/__init__.py
--rw-rw-rw-   0        0        0     4145 2023-05-25 08:06:05.000000 yuptools-0.1.6/src/yuptools/datasets/base.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:14.697930 yuptools-0.1.6/src/yuptools/datasets/class_labels/
--rw-rw-rw-   0        0        0       17 2023-05-25 12:15:58.000000 yuptools-0.1.6/src/yuptools/datasets/class_labels/__init__.py
--rw-rw-rw-   0        0        0      191 2023-04-19 07:36:49.000000 yuptools-0.1.6/src/yuptools/datasets/class_labels/cifar10.py
--rw-rw-rw-   0        0        0     1935 2023-04-19 07:36:49.000000 yuptools-0.1.6/src/yuptools/datasets/class_labels/cifar100.py
--rw-rw-rw-   0        0        0      207 2023-04-20 00:48:17.000000 yuptools-0.1.6/src/yuptools/datasets/class_labels/fashionmnist.py
--rw-rw-rw-   0        0        0    18494 2023-04-19 10:46:55.000000 yuptools-0.1.6/src/yuptools/datasets/class_labels/imagenet.py
--rw-rw-rw-   0        0        0      151 2023-04-20 00:52:35.000000 yuptools-0.1.6/src/yuptools/datasets/class_labels/mnist.py
--rw-rw-rw-   0        0        0     9466 2023-05-21 01:56:33.000000 yuptools-0.1.6/src/yuptools/datasets/image_classification.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:14.852655 yuptools-0.1.6/src/yuptools/models/
--rw-rw-rw-   0        0        0       97 2023-05-23 23:21:32.000000 yuptools-0.1.6/src/yuptools/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:15.204628 yuptools-0.1.6/src/yuptools/models/classification/
--rw-rw-rw-   0        0        0       67 2023-05-19 05:42:06.000000 yuptools-0.1.6/src/yuptools/models/classification/__init__.py
--rw-rw-rw-   0        0        0     5799 2023-07-07 09:34:58.000000 yuptools-0.1.6/src/yuptools/models/classification/base.py
--rw-rw-rw-   0        0        0     1146 2023-05-19 04:08:19.000000 yuptools-0.1.6/src/yuptools/models/classification/config.py
--rw-rw-rw-   0        0        0     3122 2023-06-26 07:32:05.000000 yuptools-0.1.6/src/yuptools/models/classification/models.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:15.584443 yuptools-0.1.6/src/yuptools/models/classification/nets/
--rw-rw-rw-   0        0        0       86 2023-03-22 22:54:35.000000 yuptools-0.1.6/src/yuptools/models/classification/nets/__init__.py
--rw-rw-rw-   0        0        0     7111 2023-03-03 05:35:17.000000 yuptools-0.1.6/src/yuptools/models/classification/nets/deit.py
--rw-rw-rw-   0        0        0     6904 2023-03-03 05:35:17.000000 yuptools-0.1.6/src/yuptools/models/classification/nets/mixer.py
--rw-rw-rw-   0        0        0    23022 2023-03-03 05:35:17.000000 yuptools-0.1.6/src/yuptools/models/classification/nets/poolformer.py
--rw-rw-rw-   0        0        0    11940 2023-03-03 05:35:17.000000 yuptools-0.1.6/src/yuptools/models/classification/nets/pvt.py
--rw-rw-rw-   0        0        0      919 2023-05-19 04:46:33.000000 yuptools-0.1.6/src/yuptools/models/classification/warnings.py
--rw-rw-rw-   0        0        0      705 2023-05-19 02:49:58.000000 yuptools-0.1.6/src/yuptools/models/classification/weights.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:16.007921 yuptools-0.1.6/src/yuptools/models/replace/
--rw-rw-rw-   0        0        0       68 2023-05-19 06:29:29.000000 yuptools-0.1.6/src/yuptools/models/replace/__init__.py
--rw-rw-rw-   0        0        0      420 2023-05-19 06:26:47.000000 yuptools-0.1.6/src/yuptools/models/replace/activation.py
--rw-rw-rw-   0        0        0     1457 2023-05-21 00:57:35.000000 yuptools-0.1.6/src/yuptools/models/replace/base.py
--rw-rw-rw-   0        0        0     2034 2023-05-19 06:26:47.000000 yuptools-0.1.6/src/yuptools/models/replace/common.py
--rw-rw-rw-   0        0        0      270 2023-05-19 06:26:47.000000 yuptools-0.1.6/src/yuptools/models/replace/config.py
--rw-rw-rw-   0        0        0     1879 2023-05-19 06:26:47.000000 yuptools-0.1.6/src/yuptools/models/replace/normalization.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:16.282079 yuptools-0.1.6/src/yuptools/models/test/
--rw-rw-rw-   0        0        0       79 2023-05-25 13:39:36.000000 yuptools-0.1.6/src/yuptools/models/test/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-05-25 12:37:07.000000 yuptools-0.1.6/src/yuptools/models/test/accuracy.py
--rw-rw-rw-   0        0        0     3232 2023-05-25 14:07:05.000000 yuptools-0.1.6/src/yuptools/models/test/calibration.py
--rw-rw-rw-   0        0        0     2933 2023-05-24 00:54:12.000000 yuptools-0.1.6/src/yuptools/models/test/linearity.py
--rw-rw-rw-   0        0        0     2464 2023-05-23 23:49:47.000000 yuptools-0.1.6/src/yuptools/models/xray.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:16.593221 yuptools-0.1.6/src/yuptools/plotlib/
--rw-rw-rw-   0        0        0       43 2023-05-31 07:59:55.000000 yuptools-0.1.6/src/yuptools/plotlib/__init__.py
--rw-rw-rw-   0        0        0     2039 2023-05-31 08:53:42.000000 yuptools-0.1.6/src/yuptools/plotlib/bar.py
--rw-rw-rw-   0        0        0     4146 2023-05-31 08:42:30.000000 yuptools-0.1.6/src/yuptools/plotlib/base.py
--rw-rw-rw-   0        0        0     1492 2023-04-21 08:19:35.000000 yuptools-0.1.6/src/yuptools/plotlib/common.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:17.151365 yuptools-0.1.6/src/yuptools/tools/
--rw-rw-rw-   0        0        0      128 2023-05-25 07:16:55.000000 yuptools-0.1.6/src/yuptools/tools/__init__.py
--rw-rw-rw-   0        0        0      287 2023-05-17 21:43:57.000000 yuptools-0.1.6/src/yuptools/tools/attrtools.py
--rw-rw-rw-   0        0        0     1881 2023-05-25 09:04:38.000000 yuptools-0.1.6/src/yuptools/tools/dictools.py
--rw-rw-rw-   0        0        0     1589 2023-05-24 00:34:34.000000 yuptools-0.1.6/src/yuptools/tools/linalgtools.py
--rw-rw-rw-   0        0        0     1482 2023-05-19 01:20:48.000000 yuptools-0.1.6/src/yuptools/tools/listools.py
--rw-rw-rw-   0        0        0     1295 2023-05-17 19:18:18.000000 yuptools-0.1.6/src/yuptools/tools/pathtools.py
--rw-rw-rw-   0        0        0      627 2023-05-22 04:21:26.000000 yuptools-0.1.6/src/yuptools/tools/randtools.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:17.900725 yuptools-0.1.6/src/yuptools/train/
--rw-rw-rw-   0        0        0      152 2023-05-25 08:33:17.000000 yuptools-0.1.6/src/yuptools/train/__init__.py
--rw-rw-rw-   0        0        0     9748 2023-05-25 09:22:49.000000 yuptools-0.1.6/src/yuptools/train/base.py
--rw-rw-rw-   0        0        0      663 2023-05-25 07:46:49.000000 yuptools-0.1.6/src/yuptools/train/criterion.py
--rw-rw-rw-   0        0        0      509 2023-05-25 06:43:18.000000 yuptools-0.1.6/src/yuptools/train/dataloader.py
--rw-rw-rw-   0        0        0     2323 2023-05-25 07:46:00.000000 yuptools-0.1.6/src/yuptools/train/optimizer.py
--rw-rw-rw-   0        0        0     2687 2023-05-25 07:01:42.000000 yuptools-0.1.6/src/yuptools/train/scheduler.py
--rw-rw-rw-   0        0        0      627 2023-05-25 09:22:44.000000 yuptools-0.1.6/src/yuptools/train/trainer.py
--rw-rw-rw-   0        0        0     4104 2023-05-25 07:01:42.000000 yuptools-0.1.6/src/yuptools/train/warmup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:18.208668 yuptools-0.1.6/src/yuptools/travel/
--rw-rw-rw-   0        0        0       75 2023-07-06 02:38:18.000000 yuptools-0.1.6/src/yuptools/travel/__init__.py
--rw-rw-rw-   0        0        0      633 2023-06-26 03:54:06.000000 yuptools-0.1.6/src/yuptools/travel/config.py
--rw-rw-rw-   0        0        0     4784 2023-06-26 04:02:22.000000 yuptools-0.1.6/src/yuptools/travel/direction.py
--rw-rw-rw-   0        0        0     2985 2023-07-07 09:20:08.000000 yuptools-0.1.6/src/yuptools/travel/footprint.py
--rw-rw-rw-   0        0        0     5815 2023-07-07 09:20:08.000000 yuptools-0.1.6/src/yuptools/travel/travel.py
--rw-rw-rw-   0        0        0      675 2023-05-22 03:25:19.000000 yuptools-0.1.6/src/yuptools/travel/warnings.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:18.277536 yuptools-0.1.6/src/yuptools/web/
--rw-rw-rw-   0        0        0       23 2023-05-21 21:08:21.000000 yuptools-0.1.6/src/yuptools/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:18.466961 yuptools-0.1.6/src/yuptools/web/chrome/
--rw-rw-rw-   0        0        0       23 2023-05-21 21:08:21.000000 yuptools-0.1.6/src/yuptools/web/chrome/__init__.py
--rw-rw-rw-   0        0        0      129 2023-05-21 21:14:42.000000 yuptools-0.1.6/src/yuptools/web/chrome/config.py
--rw-rw-rw-   0        0        0     4115 2023-05-21 21:14:42.000000 yuptools-0.1.6/src/yuptools/web/chrome/driver.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:35:13.717837 yuptools-0.1.6/src/yuptools.egg-info/
--rw-rw-rw-   0        0        0     3198 2023-07-07 09:35:13.000000 yuptools-0.1.6/src/yuptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2601 2023-07-07 09:35:13.000000 yuptools-0.1.6/src/yuptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 09:35:13.000000 yuptools-0.1.6/src/yuptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-07-07 09:35:13.000000 yuptools-0.1.6/src/yuptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 09:35:13.000000 yuptools-0.1.6/src/yuptools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:14.373441 yuptools-0.1.7/
+-rw-rw-rw-   0        0        0     1088 2023-04-21 08:53:14.000000 yuptools-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3198 2023-07-07 10:34:14.371443 yuptools-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2957 2023-07-07 10:34:08.000000 yuptools-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:34:14.373441 yuptools-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-07-07 10:34:08.000000 yuptools-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:12.859985 yuptools-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:12.900875 yuptools-0.1.7/src/yuptools/
+-rw-rw-rw-   0        0        0      240 2023-05-21 22:00:40.000000 yuptools-0.1.7/src/yuptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:12.975952 yuptools-0.1.7/src/yuptools/attacks/
+-rw-rw-rw-   0        0        0       43 2023-05-21 01:50:37.000000 yuptools-0.1.7/src/yuptools/attacks/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-05-23 23:07:37.000000 yuptools-0.1.7/src/yuptools/attacks/fgsm.py
+-rw-rw-rw-   0        0        0     2872 2023-05-22 04:35:07.000000 yuptools-0.1.7/src/yuptools/attacks/ifgsm.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.043543 yuptools-0.1.7/src/yuptools/datasets/
+-rw-rw-rw-   0        0        0       86 2023-05-25 12:15:58.000000 yuptools-0.1.7/src/yuptools/datasets/__init__.py
+-rw-rw-rw-   0        0        0     4145 2023-05-25 08:06:05.000000 yuptools-0.1.7/src/yuptools/datasets/base.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.180306 yuptools-0.1.7/src/yuptools/datasets/class_labels/
+-rw-rw-rw-   0        0        0       17 2023-05-25 12:15:58.000000 yuptools-0.1.7/src/yuptools/datasets/class_labels/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-04-19 07:36:49.000000 yuptools-0.1.7/src/yuptools/datasets/class_labels/cifar10.py
+-rw-rw-rw-   0        0        0     1935 2023-04-19 07:36:49.000000 yuptools-0.1.7/src/yuptools/datasets/class_labels/cifar100.py
+-rw-rw-rw-   0        0        0      207 2023-04-20 00:48:17.000000 yuptools-0.1.7/src/yuptools/datasets/class_labels/fashionmnist.py
+-rw-rw-rw-   0        0        0    18494 2023-04-19 10:46:55.000000 yuptools-0.1.7/src/yuptools/datasets/class_labels/imagenet.py
+-rw-rw-rw-   0        0        0      151 2023-04-20 00:52:35.000000 yuptools-0.1.7/src/yuptools/datasets/class_labels/mnist.py
+-rw-rw-rw-   0        0        0     9466 2023-05-21 01:56:33.000000 yuptools-0.1.7/src/yuptools/datasets/image_classification.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.220423 yuptools-0.1.7/src/yuptools/models/
+-rw-rw-rw-   0        0        0       97 2023-05-23 23:21:32.000000 yuptools-0.1.7/src/yuptools/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.337678 yuptools-0.1.7/src/yuptools/models/classification/
+-rw-rw-rw-   0        0        0       67 2023-05-19 05:42:06.000000 yuptools-0.1.7/src/yuptools/models/classification/__init__.py
+-rw-rw-rw-   0        0        0     5799 2023-07-07 09:34:58.000000 yuptools-0.1.7/src/yuptools/models/classification/base.py
+-rw-rw-rw-   0        0        0     1146 2023-05-19 04:08:19.000000 yuptools-0.1.7/src/yuptools/models/classification/config.py
+-rw-rw-rw-   0        0        0     3122 2023-06-26 07:32:05.000000 yuptools-0.1.7/src/yuptools/models/classification/models.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.432108 yuptools-0.1.7/src/yuptools/models/classification/nets/
+-rw-rw-rw-   0        0        0       86 2023-03-22 22:54:35.000000 yuptools-0.1.7/src/yuptools/models/classification/nets/__init__.py
+-rw-rw-rw-   0        0        0     7111 2023-03-03 05:35:17.000000 yuptools-0.1.7/src/yuptools/models/classification/nets/deit.py
+-rw-rw-rw-   0        0        0     6904 2023-03-03 05:35:17.000000 yuptools-0.1.7/src/yuptools/models/classification/nets/mixer.py
+-rw-rw-rw-   0        0        0    23022 2023-03-03 05:35:17.000000 yuptools-0.1.7/src/yuptools/models/classification/nets/poolformer.py
+-rw-rw-rw-   0        0        0    11940 2023-03-03 05:35:17.000000 yuptools-0.1.7/src/yuptools/models/classification/nets/pvt.py
+-rw-rw-rw-   0        0        0      919 2023-05-19 04:46:33.000000 yuptools-0.1.7/src/yuptools/models/classification/warnings.py
+-rw-rw-rw-   0        0        0      705 2023-05-19 02:49:58.000000 yuptools-0.1.7/src/yuptools/models/classification/weights.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.551806 yuptools-0.1.7/src/yuptools/models/replace/
+-rw-rw-rw-   0        0        0       68 2023-05-19 06:29:29.000000 yuptools-0.1.7/src/yuptools/models/replace/__init__.py
+-rw-rw-rw-   0        0        0      420 2023-05-19 06:26:47.000000 yuptools-0.1.7/src/yuptools/models/replace/activation.py
+-rw-rw-rw-   0        0        0     1457 2023-05-21 00:57:35.000000 yuptools-0.1.7/src/yuptools/models/replace/base.py
+-rw-rw-rw-   0        0        0     2034 2023-05-19 06:26:47.000000 yuptools-0.1.7/src/yuptools/models/replace/common.py
+-rw-rw-rw-   0        0        0      270 2023-05-19 06:26:47.000000 yuptools-0.1.7/src/yuptools/models/replace/config.py
+-rw-rw-rw-   0        0        0     1879 2023-05-19 06:26:47.000000 yuptools-0.1.7/src/yuptools/models/replace/normalization.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.650098 yuptools-0.1.7/src/yuptools/models/test/
+-rw-rw-rw-   0        0        0       79 2023-05-25 13:39:36.000000 yuptools-0.1.7/src/yuptools/models/test/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-05-25 12:37:07.000000 yuptools-0.1.7/src/yuptools/models/test/accuracy.py
+-rw-rw-rw-   0        0        0     3232 2023-05-25 14:07:05.000000 yuptools-0.1.7/src/yuptools/models/test/calibration.py
+-rw-rw-rw-   0        0        0     2933 2023-05-24 00:54:12.000000 yuptools-0.1.7/src/yuptools/models/test/linearity.py
+-rw-rw-rw-   0        0        0     2464 2023-05-23 23:49:47.000000 yuptools-0.1.7/src/yuptools/models/xray.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.736366 yuptools-0.1.7/src/yuptools/plotlib/
+-rw-rw-rw-   0        0        0       43 2023-05-31 07:59:55.000000 yuptools-0.1.7/src/yuptools/plotlib/__init__.py
+-rw-rw-rw-   0        0        0     2039 2023-05-31 08:53:42.000000 yuptools-0.1.7/src/yuptools/plotlib/bar.py
+-rw-rw-rw-   0        0        0     4146 2023-05-31 08:42:30.000000 yuptools-0.1.7/src/yuptools/plotlib/base.py
+-rw-rw-rw-   0        0        0     1492 2023-04-21 08:19:35.000000 yuptools-0.1.7/src/yuptools/plotlib/common.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:13.884900 yuptools-0.1.7/src/yuptools/tools/
+-rw-rw-rw-   0        0        0      128 2023-05-25 07:16:55.000000 yuptools-0.1.7/src/yuptools/tools/__init__.py
+-rw-rw-rw-   0        0        0      287 2023-05-17 21:43:57.000000 yuptools-0.1.7/src/yuptools/tools/attrtools.py
+-rw-rw-rw-   0        0        0     1881 2023-05-25 09:04:38.000000 yuptools-0.1.7/src/yuptools/tools/dictools.py
+-rw-rw-rw-   0        0        0     1589 2023-05-24 00:34:34.000000 yuptools-0.1.7/src/yuptools/tools/linalgtools.py
+-rw-rw-rw-   0        0        0     1482 2023-05-19 01:20:48.000000 yuptools-0.1.7/src/yuptools/tools/listools.py
+-rw-rw-rw-   0        0        0     1295 2023-05-17 19:18:18.000000 yuptools-0.1.7/src/yuptools/tools/pathtools.py
+-rw-rw-rw-   0        0        0      627 2023-05-22 04:21:26.000000 yuptools-0.1.7/src/yuptools/tools/randtools.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:14.054248 yuptools-0.1.7/src/yuptools/train/
+-rw-rw-rw-   0        0        0      152 2023-05-25 08:33:17.000000 yuptools-0.1.7/src/yuptools/train/__init__.py
+-rw-rw-rw-   0        0        0     9748 2023-05-25 09:22:49.000000 yuptools-0.1.7/src/yuptools/train/base.py
+-rw-rw-rw-   0        0        0      663 2023-05-25 07:46:49.000000 yuptools-0.1.7/src/yuptools/train/criterion.py
+-rw-rw-rw-   0        0        0      509 2023-05-25 06:43:18.000000 yuptools-0.1.7/src/yuptools/train/dataloader.py
+-rw-rw-rw-   0        0        0     2323 2023-05-25 07:46:00.000000 yuptools-0.1.7/src/yuptools/train/optimizer.py
+-rw-rw-rw-   0        0        0     2687 2023-05-25 07:01:42.000000 yuptools-0.1.7/src/yuptools/train/scheduler.py
+-rw-rw-rw-   0        0        0      627 2023-05-25 09:22:44.000000 yuptools-0.1.7/src/yuptools/train/trainer.py
+-rw-rw-rw-   0        0        0     4104 2023-05-25 07:01:42.000000 yuptools-0.1.7/src/yuptools/train/warmup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:14.273747 yuptools-0.1.7/src/yuptools/travel/
+-rw-rw-rw-   0        0        0       75 2023-07-06 02:38:18.000000 yuptools-0.1.7/src/yuptools/travel/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-06-26 03:54:06.000000 yuptools-0.1.7/src/yuptools/travel/config.py
+-rw-rw-rw-   0        0        0     4775 2023-07-07 09:38:36.000000 yuptools-0.1.7/src/yuptools/travel/direction.py
+-rw-rw-rw-   0        0        0     2975 2023-07-07 09:38:36.000000 yuptools-0.1.7/src/yuptools/travel/footprint.py
+-rw-rw-rw-   0        0        0     5815 2023-07-07 09:20:08.000000 yuptools-0.1.7/src/yuptools/travel/travel.py
+-rw-rw-rw-   0        0        0      675 2023-05-22 03:25:19.000000 yuptools-0.1.7/src/yuptools/travel/warnings.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:14.291727 yuptools-0.1.7/src/yuptools/web/
+-rw-rw-rw-   0        0        0       23 2023-05-21 21:08:21.000000 yuptools-0.1.7/src/yuptools/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:14.351642 yuptools-0.1.7/src/yuptools/web/chrome/
+-rw-rw-rw-   0        0        0       23 2023-05-21 21:08:21.000000 yuptools-0.1.7/src/yuptools/web/chrome/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-05-21 21:14:42.000000 yuptools-0.1.7/src/yuptools/web/chrome/config.py
+-rw-rw-rw-   0        0        0     4115 2023-05-21 21:14:42.000000 yuptools-0.1.7/src/yuptools/web/chrome/driver.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:34:12.929799 yuptools-0.1.7/src/yuptools.egg-info/
+-rw-rw-rw-   0        0        0     3198 2023-07-07 10:34:12.000000 yuptools-0.1.7/src/yuptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2601 2023-07-07 10:34:12.000000 yuptools-0.1.7/src/yuptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:34:12.000000 yuptools-0.1.7/src/yuptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-07-07 10:34:12.000000 yuptools-0.1.7/src/yuptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 10:34:12.000000 yuptools-0.1.7/src/yuptools.egg-info/top_level.txt
```

### Comparing `yuptools-0.1.6/LICENSE` & `yuptools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/PKG-INFO` & `yuptools-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuptools
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/yupeeee/YupTools
 Author: Juyeop Kim
 Author-email: juyeopkim@yonsei.ac.kr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,18 +13,18 @@
 YupTools is a Python package based on PyTorch.
 
 ---
 
 
 ## Installation
 
-Latest version: 0.1.6 <br>
+Latest version: 0.1.7 <br>
 **Note: [Manual installation of PyTorch](https://pytorch.org/get-started/locally/) is required.**
 ```
-pip install yuptools==0.1.6
+pip install yuptools==0.1.7
 ```
 
 
 ### Requirements
 
 ```
 Python >= 3.8
```

### Comparing `yuptools-0.1.6/README.md` & `yuptools-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 YupTools is a Python package based on PyTorch.
 
 ---
 
 
 ## Installation
 
-Latest version: 0.1.6 <br>
+Latest version: 0.1.7 <br>
 **Note: [Manual installation of PyTorch](https://pytorch.org/get-started/locally/) is required.**
 ```
-pip install yuptools==0.1.6
+pip install yuptools==0.1.7
 ```
 
 
 ### Requirements
 
 ```
 Python >= 3.8
```

### Comparing `yuptools-0.1.6/setup.py` & `yuptools-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="yuptools",
-    version="0.1.6",
+    version="0.1.7",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Juyeop Kim",
     author_email="juyeopkim@yonsei.ac.kr",
     url="https://github.com/yupeeee/YupTools",
     license="MIT",
```

### Comparing `yuptools-0.1.6/src/yuptools/attacks/fgsm.py` & `yuptools-0.1.7/src/yuptools/attacks/fgsm.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/attacks/ifgsm.py` & `yuptools-0.1.7/src/yuptools/attacks/ifgsm.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/datasets/base.py` & `yuptools-0.1.7/src/yuptools/datasets/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/datasets/class_labels/cifar100.py` & `yuptools-0.1.7/src/yuptools/datasets/class_labels/cifar100.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/datasets/class_labels/imagenet.py` & `yuptools-0.1.7/src/yuptools/datasets/class_labels/imagenet.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/datasets/image_classification.py` & `yuptools-0.1.7/src/yuptools/datasets/image_classification.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/base.py` & `yuptools-0.1.7/src/yuptools/models/classification/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/config.py` & `yuptools-0.1.7/src/yuptools/models/classification/config.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/models.py` & `yuptools-0.1.7/src/yuptools/models/classification/models.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/nets/deit.py` & `yuptools-0.1.7/src/yuptools/models/classification/nets/deit.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/nets/mixer.py` & `yuptools-0.1.7/src/yuptools/models/classification/nets/mixer.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/nets/poolformer.py` & `yuptools-0.1.7/src/yuptools/models/classification/nets/poolformer.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/nets/pvt.py` & `yuptools-0.1.7/src/yuptools/models/classification/nets/pvt.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/warnings.py` & `yuptools-0.1.7/src/yuptools/models/classification/warnings.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/classification/weights.py` & `yuptools-0.1.7/src/yuptools/models/classification/weights.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/replace/base.py` & `yuptools-0.1.7/src/yuptools/models/replace/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/replace/common.py` & `yuptools-0.1.7/src/yuptools/models/replace/common.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/replace/normalization.py` & `yuptools-0.1.7/src/yuptools/models/replace/normalization.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/test/accuracy.py` & `yuptools-0.1.7/src/yuptools/models/test/accuracy.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/test/calibration.py` & `yuptools-0.1.7/src/yuptools/models/test/calibration.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/test/linearity.py` & `yuptools-0.1.7/src/yuptools/models/test/linearity.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/models/xray.py` & `yuptools-0.1.7/src/yuptools/models/xray.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/plotlib/bar.py` & `yuptools-0.1.7/src/yuptools/plotlib/bar.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/plotlib/base.py` & `yuptools-0.1.7/src/yuptools/plotlib/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/plotlib/common.py` & `yuptools-0.1.7/src/yuptools/plotlib/common.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/tools/dictools.py` & `yuptools-0.1.7/src/yuptools/tools/dictools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/tools/linalgtools.py` & `yuptools-0.1.7/src/yuptools/tools/linalgtools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/tools/listools.py` & `yuptools-0.1.7/src/yuptools/tools/listools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/tools/pathtools.py` & `yuptools-0.1.7/src/yuptools/tools/pathtools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/tools/randtools.py` & `yuptools-0.1.7/src/yuptools/tools/randtools.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/train/base.py` & `yuptools-0.1.7/src/yuptools/train/base.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/train/criterion.py` & `yuptools-0.1.7/src/yuptools/train/criterion.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/train/optimizer.py` & `yuptools-0.1.7/src/yuptools/train/optimizer.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/train/scheduler.py` & `yuptools-0.1.7/src/yuptools/train/scheduler.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/train/trainer.py` & `yuptools-0.1.7/src/yuptools/train/trainer.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/train/warmup.py` & `yuptools-0.1.7/src/yuptools/train/warmup.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/travel/config.py` & `yuptools-0.1.7/src/yuptools/travel/config.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/travel/direction.py` & `yuptools-0.1.7/src/yuptools/travel/direction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union
+from typing import Optional
 
 import torch
 
 from .config import *
 from .warnings import *
 
 __all__ = [
@@ -16,15 +16,15 @@
 ) -> torch.Tensor:
     return destinations - data
 
 
 def random_direction(
         data: torch.Tensor,
         signed: bool = False,
-        seed: int = None,
+        seed: Optional[int] = None,
 ) -> torch.Tensor:
     from ..tools.linalgtools import repeat_tensor
     from ..tools.randtools import set_random_seed, unset_random_seed
 
     num_data = len(data)
 
     set_random_seed(seed)
@@ -45,16 +45,16 @@
 
     return direction
 
 
 def post_process(
         direction: torch.Tensor,
         perp: bool = False,
-        normalize: Union[str, None] = default_normalize,
-        seed: Union[int, None] = None,
+        normalize: Optional[str] = default_normalize,
+        seed: Optional[int] = None,
 ) -> torch.Tensor:
     from ..tools.linalgtools import normalize_v, orthogonal_to_v
 
     # assertions
     is_valid_direction_normalize_method(normalize)
 
     shape = direction.shape
@@ -86,16 +86,16 @@
 
 class DirectionGenerator:
     def __init__(
             self,
             model: Optional[torch.nn.Module] = None,
             method: str = default_method,
             perp: bool = False,
-            normalize: Union[str, None] = default_normalize,
-            seed: Union[int, None] = default_seed,
+            normalize: Optional[str] = default_normalize,
+            seed: Optional[int] = default_seed,
             use_cuda: bool = False,
     ) -> None:
         # assertions
         is_valid_direction_method(method)
 
         self.model = model
         self.method = method
```

### Comparing `yuptools-0.1.6/src/yuptools/travel/footprint.py` & `yuptools-0.1.7/src/yuptools/travel/footprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union
+from typing import Optional
 
 import torch
 
 from .config import *
 
 __all__ = [
     "Footprint",
@@ -14,15 +14,15 @@
             self,
             step: int,
             model: torch.nn.Module,
             method: str = default_method,
             perp: bool = False,
             normalize: str = default_normalize,
             bound: bool = False,
-            seed: Union[int, None] = default_seed,
+            seed: Optional[int] = default_seed,
             use_cuda: bool = False,
     ) -> None:
         from .direction import DirectionGenerator
 
         self.step = step
         self.model = model
         self.method = method
```

### Comparing `yuptools-0.1.6/src/yuptools/travel/travel.py` & `yuptools-0.1.7/src/yuptools/travel/travel.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/travel/warnings.py` & `yuptools-0.1.7/src/yuptools/travel/warnings.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools/web/chrome/driver.py` & `yuptools-0.1.7/src/yuptools/web/chrome/driver.py`

 * *Files identical despite different names*

### Comparing `yuptools-0.1.6/src/yuptools.egg-info/PKG-INFO` & `yuptools-0.1.7/src/yuptools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuptools
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/yupeeee/YupTools
 Author: Juyeop Kim
 Author-email: juyeopkim@yonsei.ac.kr
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,18 +13,18 @@
 YupTools is a Python package based on PyTorch.
 
 ---
 
 
 ## Installation
 
-Latest version: 0.1.6 <br>
+Latest version: 0.1.7 <br>
 **Note: [Manual installation of PyTorch](https://pytorch.org/get-started/locally/) is required.**
 ```
-pip install yuptools==0.1.6
+pip install yuptools==0.1.7
 ```
 
 
 ### Requirements
 
 ```
 Python >= 3.8
```

### Comparing `yuptools-0.1.6/src/yuptools.egg-info/SOURCES.txt` & `yuptools-0.1.7/src/yuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


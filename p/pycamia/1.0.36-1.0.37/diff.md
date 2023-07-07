# Comparing `tmp/pycamia-1.0.36.tar.gz` & `tmp/pycamia-1.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycamia-1.0.36.tar", last modified: Wed Jul  5 09:06:00 2023, max compression
+gzip compressed data, was "pycamia-1.0.37.tar", last modified: Thu Jul  6 12:58:11 2023, max compression
```

## Comparing `pycamia-1.0.36.tar` & `pycamia-1.0.37.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.446710 pycamia-1.0.36/
--rw-r--r--   0 admin      (501) staff       (20)       62 2023-07-05 09:05:57.000000 pycamia-1.0.36/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-05 09:06:00.446557 pycamia-1.0.36/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     7041 2023-07-05 09:06:00.000000 pycamia-1.0.36/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.433543 pycamia-1.0.36/batorch/
--rw-r--r--   0 admin      (501) staff       (20)     8723 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     6980 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/device.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.434960 pycamia-1.0.36/batorch/nn/
--rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/_reduction.py
--rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/common_types.py
--rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/functional.py
--rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/grad.py
--rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/init.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.439127 pycamia-1.0.36/batorch/nn/modules/
--rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/_functions.py
--rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/activation.py
--rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/adaptive.py
--rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/batchnorm.py
--rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/container.py
--rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/conv.py
--rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/distance.py
--rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/dropout.py
--rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/flatten.py
--rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/fold.py
--rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/instancenorm.py
--rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/linear.py
--rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/loss.py
--rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/module.py
--rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/normalization.py
--rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/padding.py
--rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/pixelshuffle.py
--rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/pooling.py
--rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/sparse.py
--rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/transformer.py
--rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/upsampling.py
--rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/modules/utils.py
--rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/parameter.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.440437 pycamia-1.0.36/batorch/nn/utils/
--rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2919 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/clip_grad.py
--rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/convert_parameters.py
--rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/fusion.py
--rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/memory_format.py
--rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/prune.py
--rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/rnn.py
--rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/spectral_norm.py
--rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/nn/utils/weight_norm.py
--rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/optimizer.py
--rwxr-xr-x   0 admin      (501) staff       (20)   106574 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/tensor.py
--rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/tensor2.py
--rw-r--r--   0 admin      (501) staff       (20)    24001 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/tensorfunc.py
--rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/torch_namespace.py
--rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-05 09:05:59.000000 pycamia-1.0.36/batorch/torchext.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.441923 pycamia-1.0.36/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2396 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    37891 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/metrics.py
--rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/micfunctions.so
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98769 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.442510 pycamia-1.0.36/micomputing/zxhtools/
--rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/zxhtools/TRS.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.443087 pycamia-1.0.36/micomputing/zxhtools/__pycache__/
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/zxhtools/exec.py
--rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/zxhtools/image2.AFF
--rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-05 09:05:57.000000 pycamia-1.0.36/micomputing/zxhtools/image2.FFD
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.445173 pycamia-1.0.36/pycamia/
--rw-r--r--   0 admin      (501) staff       (20)     1944 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3453 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/decorators.py
--rw-r--r--   0 admin      (501) staff       (20)     9424 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/environment.py
--rw-r--r--   0 admin      (501) staff       (20)     4260 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/exception.py
--rw-r--r--   0 admin      (501) staff       (20)      683 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/functions.py
--rw-r--r--   0 admin      (501) staff       (20)     3814 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/inout.py
--rw-r--r--   0 admin      (501) staff       (20)    15488 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/listop.py
--rw-r--r--   0 admin      (501) staff       (20)     6550 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/logging.py
--rw-r--r--   0 admin      (501) staff       (20)     7135 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/manager.py
--rw-r--r--   0 admin      (501) staff       (20)     5867 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/math.py
--rw-r--r--   0 admin      (501) staff       (20)     1061 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/more.py
--rw-r--r--   0 admin      (501) staff       (20)     1091 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/numpyop.py
--rw-r--r--   0 admin      (501) staff       (20)     9791 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/strop.py
--rw-r--r--   0 admin      (501) staff       (20)    21362 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/system.py
--rw-r--r--   0 admin      (501) staff       (20)    12327 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia/timing.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.445710 pycamia-1.0.36/pycamia.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     2425 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       39 2023-07-05 09:06:00.000000 pycamia-1.0.36/pycamia.egg-info/top_level.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-05 09:06:00.446298 pycamia-1.0.36/pyoverload/
--rw-r--r--   0 admin      (501) staff       (20)      958 2023-07-05 09:05:59.000000 pycamia-1.0.36/pyoverload/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    11636 2023-07-05 09:05:59.000000 pycamia-1.0.36/pyoverload/override.py
--rw-r--r--   0 admin      (501) staff       (20)    32070 2023-07-05 09:05:59.000000 pycamia-1.0.36/pyoverload/typehint.py
--rw-r--r--   0 admin      (501) staff       (20)     9157 2023-07-05 09:05:59.000000 pycamia-1.0.36/pyoverload/utils.py
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-05 09:06:00.446765 pycamia-1.0.36/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     7720 2023-07-05 09:06:00.000000 pycamia-1.0.36/setup_pycamia.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.558431 pycamia-1.0.37/
+-rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-06 12:58:09.000000 pycamia-1.0.37/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-06 12:58:11.558280 pycamia-1.0.37/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     7041 2023-07-06 12:58:11.000000 pycamia-1.0.37/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.544922 pycamia-1.0.37/batorch/
+-rw-r--r--   0 admin      (501) staff       (20)    20151 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7450 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/device.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.546020 pycamia-1.0.37/batorch/nn/
+-rw-r--r--   0 admin      (501) staff       (20)      343 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1599 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/_reduction.py
+-rw-r--r--   0 admin      (501) staff       (20)     1766 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/common_types.py
+-rw-r--r--   0 admin      (501) staff       (20)   186195 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/functional.py
+-rw-r--r--   0 admin      (501) staff       (20)    14006 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/grad.py
+-rw-r--r--   0 admin      (501) staff       (20)    18207 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/init.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.549856 pycamia-1.0.37/batorch/nn/modules/
+-rw-r--r--   0 admin      (501) staff       (20)     4618 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7250 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    48520 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/activation.py
+-rw-r--r--   0 admin      (501) staff       (20)    10997 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/adaptive.py
+-rw-r--r--   0 admin      (501) staff       (20)    25981 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/batchnorm.py
+-rw-r--r--   0 admin      (501) staff       (20)    23822 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/container.py
+-rw-r--r--   0 admin      (501) staff       (20)    51560 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/conv.py
+-rw-r--r--   0 admin      (501) staff       (20)     2662 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/distance.py
+-rw-r--r--   0 admin      (501) staff       (20)     8997 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/dropout.py
+-rw-r--r--   0 admin      (501) staff       (20)     4861 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/flatten.py
+-rw-r--r--   0 admin      (501) staff       (20)    12545 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/fold.py
+-rw-r--r--   0 admin      (501) staff       (20)    13332 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/instancenorm.py
+-rw-r--r--   0 admin      (501) staff       (20)     6191 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/linear.py
+-rw-r--r--   0 admin      (501) staff       (20)    77226 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/loss.py
+-rw-r--r--   0 admin      (501) staff       (20)     7100 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/module.py
+-rw-r--r--   0 admin      (501) staff       (20)     9717 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/normalization.py
+-rw-r--r--   0 admin      (501) staff       (20)    16584 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/padding.py
+-rw-r--r--   0 admin      (501) staff       (20)     1728 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/pixelshuffle.py
+-rw-r--r--   0 admin      (501) staff       (20)    48072 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/pooling.py
+-rw-r--r--   0 admin      (501) staff       (20)    48452 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    17824 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/sparse.py
+-rw-r--r--   0 admin      (501) staff       (20)    17745 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/transformer.py
+-rw-r--r--   0 admin      (501) staff       (20)    10086 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/upsampling.py
+-rw-r--r--   0 admin      (501) staff       (20)      957 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/modules/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     2734 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/parameter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.551132 pycamia-1.0.37/batorch/nn/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      409 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2914 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/clip_grad.py
+-rw-r--r--   0 admin      (501) staff       (20)     3027 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/convert_parameters.py
+-rw-r--r--   0 admin      (501) staff       (20)      813 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/fusion.py
+-rw-r--r--   0 admin      (501) staff       (20)     3801 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/memory_format.py
+-rw-r--r--   0 admin      (501) staff       (20)    52652 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/prune.py
+-rw-r--r--   0 admin      (501) staff       (20)    17955 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/rnn.py
+-rw-r--r--   0 admin      (501) staff       (20)    13674 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/spectral_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)     4287 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/nn/utils/weight_norm.py
+-rw-r--r--   0 admin      (501) staff       (20)    20603 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/optimizer.py
+-rwxr-xr-x   0 admin      (501) staff       (20)   106172 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/tensor.py
+-rw-r--r--   0 admin      (501) staff       (20)    45557 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/tensor2.py
+-rw-r--r--   0 admin      (501) staff       (20)    24015 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/tensorfunc.py
+-rw-r--r--   0 admin      (501) staff       (20)     9875 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/torch_namespace.py
+-rw-r--r--   0 admin      (501) staff       (20)    13174 2023-07-06 12:58:10.000000 pycamia-1.0.37/batorch/torchext.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.552605 pycamia-1.0.37/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2360 2023-07-06 12:58:08.000000 pycamia-1.0.37/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    38276 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54244 2023-07-06 12:58:08.000000 pycamia-1.0.37/micomputing/metrics.py
+-rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/micfunctions.so
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-06 12:58:08.000000 pycamia-1.0.37/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    98904 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.553137 pycamia-1.0.37/micomputing/zxhtools/
+-rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/zxhtools/TRS.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.553704 pycamia-1.0.37/micomputing/zxhtools/__pycache__/
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/zxhtools/exec.py
+-rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/zxhtools/image2.AFF
+-rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-06 12:58:09.000000 pycamia-1.0.37/micomputing/zxhtools/image2.FFD
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.556671 pycamia-1.0.37/pycamia/
+-rw-r--r--   0 admin      (501) staff       (20)     1944 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     3453 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/decorators.py
+-rw-r--r--   0 admin      (501) staff       (20)     9424 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/environment.py
+-rw-r--r--   0 admin      (501) staff       (20)     4260 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/exception.py
+-rw-r--r--   0 admin      (501) staff       (20)      683 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/functions.py
+-rw-r--r--   0 admin      (501) staff       (20)     3814 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/inout.py
+-rw-r--r--   0 admin      (501) staff       (20)    15488 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/listop.py
+-rw-r--r--   0 admin      (501) staff       (20)     6550 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/logging.py
+-rw-r--r--   0 admin      (501) staff       (20)     7124 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/manager.py
+-rw-r--r--   0 admin      (501) staff       (20)     5867 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/math.py
+-rw-r--r--   0 admin      (501) staff       (20)     1061 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/more.py
+-rw-r--r--   0 admin      (501) staff       (20)     1091 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/numpyop.py
+-rw-r--r--   0 admin      (501) staff       (20)     9791 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/strop.py
+-rw-r--r--   0 admin      (501) staff       (20)    21362 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/system.py
+-rw-r--r--   0 admin      (501) staff       (20)    12327 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia/timing.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.557320 pycamia-1.0.37/pycamia.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     8214 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     2425 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       39 2023-07-06 12:58:11.000000 pycamia-1.0.37/pycamia.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-06 12:58:11.558003 pycamia-1.0.37/pyoverload/
+-rw-r--r--   0 admin      (501) staff       (20)      958 2023-07-06 12:58:10.000000 pycamia-1.0.37/pyoverload/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    11636 2023-07-06 12:58:10.000000 pycamia-1.0.37/pyoverload/override.py
+-rw-r--r--   0 admin      (501) staff       (20)    32070 2023-07-06 12:58:10.000000 pycamia-1.0.37/pyoverload/typehint.py
+-rw-r--r--   0 admin      (501) staff       (20)     9157 2023-07-06 12:58:10.000000 pycamia-1.0.37/pyoverload/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-06 12:58:11.558485 pycamia-1.0.37/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     7720 2023-07-06 12:58:11.000000 pycamia-1.0.37/setup_pycamia.py
```

### Comparing `pycamia-1.0.36/PKG-INFO` & `pycamia-1.0.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycamia
-Version: 1.0.36
+Version: 1.0.37
 Summary: The main package and a background support of project PyCAMIA. 
 Home-page: https://github.com/Bertie97/PyZMyc/pycamia
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pycamia
```

### Comparing `pycamia-1.0.36/README.md` & `pycamia-1.0.37/README.md`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/device.py` & `pycamia-1.0.37/batorch/device.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,40 +14,42 @@
     GPUs
     AutoDevice
     FixedDevice
     free_memory_amount
     all_memory_amount
 """.split()
 
+GPU_priority = ['cuda', 'mps']
+
 import os, torch
 with __info__:
     import pynvml, psutil
     from pycamia import alias, ByteSize
 
 GB = 1.074e+9
-_cpu = torch.device("cpu")
 warning_free_memory_threshold = eval(os.environ.get('CUDA_RUN_MEMORY', '5')) # Run with at lease *GB
 
 free_memory_amount = None
 all_memory_amount = None
 
 @alias("free_memory_amount", amount="free")
 @alias("all_memory_amount", amount="total")
 def memory_amount(device_id, amount="total"):
-    if device_id < 0:
+    if device_id == 'cpu':
         info = psutil.virtual_memory()
-    else:
+    elif device_id == 'mps':
+        return dict(free=0, total=0)[amount]
+    elif device_id.startswith('cuda'):
         pynvml.nvmlInit()
         h = pynvml.nvmlDeviceGetHandleByIndex(device_id)
         info = pynvml.nvmlDeviceGetMemoryInfo(h)
     return getattr(info, amount)
 
 def device_by_id(device_id):
-    if device_id < 0: return _cpu
-    return torch.device(f"cuda:{device_id}")
+    return torch.device(device_id)
 
 class AutoDevice:
     """
     auto find and set a device. 
     
     Args:
         fixed_device (torch.device): use a fixed device. 
@@ -61,112 +63,115 @@
     >>> tensor.to(gpu.device)
     <tensor>
     >>> gpu.auto = False
     >>> gpu(tensor)
     <tensor>
     """
     def __init__(self, *devices, required_devices=1, auto=True, required_memory=None, verbose=True, always_proceed=False):
-        if len(devices) == 0: devices = [-1]
+        if len(devices) == 0: devices = ['cpu']
         self.required_devices = required_devices
         self.required_memory = required_memory
         self.always_proceed = always_proceed
         self.verbose = verbose
         self.auto = auto
         self.available_gpu_ids = []
         self._working_devices = None
         self.default_devices = devices
 
     @property
     def working_devices(self):
-        if self._working_devices is None:
-            if self.auto: self.auto_select()
-            else: self._working_devices = [d if isinstance(d, int) else (-1 if d.index is None else d.index) for d in self.default_devices]
+        if self.auto: self.auto_select()
+        elif self._working_devices is None:
+            self._working_devices = [f"cuda:{d}" if isinstance(d, int) else str(d) for d in self.default_devices]
         return self._working_devices
 
     @alias("device_id")
     @property
-    def main_device_id(self): return self.working_devices[0] if self.auto else -1
+    def main_device_id(self): return self.working_devices[0]
         
     @alias("device")
     @property
     def main_device(self): return device_by_id(self.main_device_id)
 
     @property
     def working_memory(self):
         return ByteSize(free_memory_amount(self.main_device_id))
 
     def auto_select(self):
-        if not torch.cuda.is_available():
-            if self.verbose: print("Warning: cannot find cuda, using cpu instead. ")
-            self.auto = False
-            self._working_devices = [-1]
-            self.required_devices = 1
-            return
-
-        self.available_gpu_ids = list(range(torch.cuda.device_count()))
-        available_gpus_memory = [free_memory_amount(i) for i in self.available_gpu_ids]
-
-        threshold = warning_free_memory_threshold if self.required_memory is None else self.required_memory / self.required_devices / 2
-        sorted_memory = sorted(enumerate(available_gpus_memory), key=lambda x: -x[1])
-        candidates = [(i, m) for i, m in sorted_memory if m > threshold * GB][:self.required_devices]
-        if len(candidates) > 0: most_available_gpus, most_available_gpu_memory = zip(*candidates)
-        else: 
-            print(f"Warning: no gpu device is available, reset environment variable CUDA_RUN_MEMORY to change the memory required...")
-            print(f"Most memory: {sorted_memory[0][1] / GB:.5} GB in GPU {sorted_memory[0][0]}. ")
-            if not self.always_proceed:
-                tag = input("Do you want to proceed with CPU? [yes/no/y/n]:")
-                if 'y' not in tag.lower(): raise RuntimeError("Not enough GPU resource.")
-            self.auto = False
-            self._working_devices = [-1]
+        self.auto = False
+        for gpu_family in GPU_priority:
+            if gpu_family == 'cuda' and torch.cuda.is_available():
+                self.available_gpu_ids = list(range(torch.cuda.device_count()))
+                available_gpus_memory = [free_memory_amount(i) for i in self.available_gpu_ids]
+
+                threshold = warning_free_memory_threshold if self.required_memory is None else self.required_memory / self.required_devices / 2
+                sorted_memory = sorted(enumerate(available_gpus_memory), key=lambda x: -x[1])
+                candidates = [(i, m) for i, m in sorted_memory if m > threshold * GB][:self.required_devices]
+                if len(candidates) > 0: most_available_gpus, most_available_gpu_memory = zip(*candidates)
+                else: 
+                    print(f"Warning: no gpu device is available, reset environment variable CUDA_RUN_MEMORY to change the memory required...")
+                    print(f"Most memory: {sorted_memory[0][1] / GB:.5} GB in GPU {sorted_memory[0][0]}. ")
+                    if not self.always_proceed:
+                        tag = input("Do you want to proceed with CPU? [yes/no/y/n]:")
+                        if 'y' not in tag.lower(): raise RuntimeError("Not enough GPU resource.")
+                    continue
+                if self.required_memory and sum(most_available_gpu_memory) < self.required_memory and self.verbose:
+                    print(f"Warning: all remaining memory of gpu devices is not enough (on: {most_available_gpus})...")
+                    print(f"Total free memory: {sum(most_available_gpu_memory) / GB:.5} GB. ")
+                    if not self.always_proceed:
+                        tag = input("Do you want to proceed? [yes/no/y/n]:")
+                        if 'y' not in tag.lower(): raise RuntimeError("Not enough free memory left.")
+                elif len(most_available_gpus) < self.required_devices and self.verbose:
+                    print(f"Warning: not enough gpus available (available: {most_available_gpus})...")
+                    print(f"Total free memory: {sum(most_available_gpu_memory) / GB:.5} GB. ")
+                    if not self.always_proceed:
+                        tag = input("Do you want to proceed? [yes/no/y/n]:")
+                        if 'y' not in tag.lower(): raise RuntimeError("Not enough free devices left.")
+                if self.verbose: print(f"Setting working devices: {most_available_gpus}, main device: {most_available_gpus[0]}. proceeding...")
+                self._working_devices = [f"cuda:{i}" for i in most_available_gpus]
+                break
+            elif gpu_family == 'mps' and torch.backends.mps.is_available():
+                self._working_devices = ['mps']
+                self.required_devices = 1
+                break
+        else:
+            if self.verbose: print("Warning: cannot find any gpu, using cpu instead. ")
+            self._working_devices = ['cpu']
             self.required_devices = 1
-            return
-        if self.required_memory and sum(most_available_gpu_memory) < self.required_memory and self.verbose:
-            print(f"Warning: all remaining memory of gpu devices is not enough (on: {most_available_gpus})...")
-            print(f"Total free memory: {sum(most_available_gpu_memory) / GB:.5} GB. ")
-            if not self.always_proceed:
-                tag = input("Do you want to proceed? [yes/no/y/n]:")
-                if 'y' not in tag.lower(): raise RuntimeError("Not enough free memory left.")
-        elif len(most_available_gpus) < self.required_devices and self.verbose:
-            print(f"Warning: not enough gpus available (available: {most_available_gpus})...")
-            print(f"Total free memory: {sum(most_available_gpu_memory) / GB:.5} GB. ")
-            if not self.always_proceed:
-                tag = input("Do you want to proceed? [yes/no/y/n]:")
-                if 'y' not in tag.lower(): raise RuntimeError("Not enough free devices left.")
-        if self.verbose: print(f"Setting working devices: {most_available_gpus}, main device: {most_available_gpus[0]}. proceeding...")
-        self._working_devices = most_available_gpus
     
     def turn_on(self):
-        if self.auto: return self
-        self.auto = True
-        self.auto_select()
+        if not self.auto:
+            self.auto = True
+            self.auto_select()
         return self
     
     def turn_off(self):
-        if not self.auto: return self
-        self.auto = False
+        if self.auto: self.auto = False
         return self
     
     def __eq__(self, other):
         if isinstance(other, torch.device): return self.main_device == other
         if isinstance(other, AutoDevice): return self.main_device == other.main_device
         return self == other
     
     def __call__(self, x):
+        mdevice = self.main_device
         if isinstance(x, torch.Tensor):
-            if x.device == self.main_device: return x
-            if self.auto: return x.to(self.main_device)
+            if x.device == mdevice: return x
+            return x.to(mdevice)
         elif isinstance(x, torch.nn.Module):
-            if len(self.working_devices) <= 1: return x.to(self.main_device)
-            if self.auto: return torch.nn.DataParallel(x.to(self.main_device), device_ids=self.working_devices)
+            if len(self.working_devices) <= 1: return x.to(mdevice)
+            return torch.nn.DataParallel(x.to(mdevice), device_ids=[int(x.split(':')[-1]) for x in self.working_devices])
         elif isinstance(x, torch.optim.Optimizer):
             if len(self.working_devices) <= 1: return x
-            if self.auto: return torch.nn.DataParallel(x, device_ids=self.working_devices)
-        else: return torch.as_tensor(x, device=self.main_device)
+            return torch.nn.DataParallel(x, device_ids=[int(x.split(':')[-1]) for x in self.working_devices])
+        else: return torch.as_tensor(x, device=mdevice)
         return x
     
 class FixedDevice(AutoDevice):
     def __init__(self, *devices, required_devices=1, auto=False, required_memory=None, verbose=False):
         super().__init__(*devices, required_devices=required_devices, auto=auto, required_memory=required_memory, verbose=verbose) 
 
-CPU = FixedDevice(_cpu)
+CPU = FixedDevice(torch.device("cpu"))
+mps = FixedDevice(torch.device("mps"))
 GPU = FixedDevice(torch.device("cuda:0"))
 GPUs = [FixedDevice(torch.device(f"cuda:{i}")) for i in range(torch.cuda.device_count())]
```

### Comparing `pycamia-1.0.36/batorch/nn/_reduction.py` & `pycamia-1.0.37/batorch/nn/_reduction.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/common_types.py` & `pycamia-1.0.37/batorch/nn/common_types.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/functional.py` & `pycamia-1.0.37/batorch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/grad.py` & `pycamia-1.0.37/batorch/nn/grad.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/init.py` & `pycamia-1.0.37/batorch/nn/init.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/__init__.py` & `pycamia-1.0.37/batorch/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/_functions.py` & `pycamia-1.0.37/batorch/nn/modules/_functions.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/activation.py` & `pycamia-1.0.37/batorch/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/adaptive.py` & `pycamia-1.0.37/batorch/nn/modules/adaptive.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/batchnorm.py` & `pycamia-1.0.37/batorch/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/container.py` & `pycamia-1.0.37/batorch/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/conv.py` & `pycamia-1.0.37/batorch/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/distance.py` & `pycamia-1.0.37/batorch/nn/modules/distance.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/dropout.py` & `pycamia-1.0.37/batorch/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/flatten.py` & `pycamia-1.0.37/batorch/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/fold.py` & `pycamia-1.0.37/batorch/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/instancenorm.py` & `pycamia-1.0.37/batorch/nn/modules/instancenorm.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/linear.py` & `pycamia-1.0.37/batorch/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/loss.py` & `pycamia-1.0.37/batorch/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/module.py` & `pycamia-1.0.37/batorch/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/normalization.py` & `pycamia-1.0.37/batorch/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/padding.py` & `pycamia-1.0.37/batorch/nn/modules/padding.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/pixelshuffle.py` & `pycamia-1.0.37/batorch/nn/modules/pixelshuffle.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/pooling.py` & `pycamia-1.0.37/batorch/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/rnn.py` & `pycamia-1.0.37/batorch/nn/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/sparse.py` & `pycamia-1.0.37/batorch/nn/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/transformer.py` & `pycamia-1.0.37/batorch/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/upsampling.py` & `pycamia-1.0.37/batorch/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/modules/utils.py` & `pycamia-1.0.37/batorch/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/parameter.py` & `pycamia-1.0.37/batorch/nn/parameter.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/utils/clip_grad.py` & `pycamia-1.0.37/batorch/nn/utils/clip_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 import batorch as torch
-from torch._six import inf
+from torch import inf
 from typing import Union, Iterable
 
 _tensor_or_tensors = Union[torch.Tensor, Iterable[torch.Tensor]]
 
 
 def clip_grad_norm_(parameters: _tensor_or_tensors, max_norm: float, norm_type: float = 2.0) -> torch.Tensor:
     r"""Clips gradient norm of an iterable of parameters.
```

### Comparing `pycamia-1.0.36/batorch/nn/utils/convert_parameters.py` & `pycamia-1.0.37/batorch/nn/utils/convert_parameters.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/utils/fusion.py` & `pycamia-1.0.37/batorch/nn/utils/fusion.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/utils/memory_format.py` & `pycamia-1.0.37/batorch/nn/utils/memory_format.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/utils/prune.py` & `pycamia-1.0.37/batorch/nn/utils/prune.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/utils/rnn.py` & `pycamia-1.0.37/batorch/nn/utils/rnn.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/utils/spectral_norm.py` & `pycamia-1.0.37/batorch/nn/utils/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/nn/utils/weight_norm.py` & `pycamia-1.0.37/batorch/nn/utils/weight_norm.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/optimizer.py` & `pycamia-1.0.37/batorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/tensor.py` & `pycamia-1.0.37/batorch/tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,21 +26,18 @@
     batch_tensor
     channel_tensor
 """.split()
 
 import builtins, sys
 from functools import wraps
 from typing import Generator
-from .tensorfunc import __all__ as tf_list
-from .torch_namespace import *
 from .device import GB, CPU, GPU, GPUs, AutoDevice, FixedDevice
 
 with __info__:
     import torch
-    import batorch as bt
     from pycamia import ByteSize
     from pycamia import avouch, alias, execblock
     from pycamia import get_alphas, arg_tuple, max_argmax
     from pycamia import argmax as _argmax, item, to_list
     from pyoverload import Type, Array, isoftype, Iterable
 
 INT = builtins.int
@@ -368,28 +365,28 @@
     
     def with_dimsize(self, k, dim):
         if isinstance(dim, list) and len(dim) in {0, 1}: dim = self.batch_dimension
         elif isinstance(dim, dict) and len(dim) == 0: dim = self.channel_dimension
         elif isinstance(dim, set) and len(dim) == 1: dim = self.channel_dimension
         elif isinstance(dim, INT) and dim < 0: dim += self.n_dim
 
-        return self[:dim] + bt.Size([k] if dim == self.batch_dimension else ({k} if dim == self.channel_dimension else k)) + self[dim+1:]
+        return self[:dim] + Size([k] if dim == self.batch_dimension else ({k} if dim == self.channel_dimension else k)) + self[dim+1:]
 
     @property
     def space(self):
         s = self._special
         t = tuple(self)
         return t[:s[0]] + t[s[0]+1:s[1]] + t[s[1]+1:]
 
     def reset_space(self, *p):
         p = arg_tuple(p)
         s = self._special
-        if s[0] == self.n_dim: return bt.Size(p)
+        if s[0] == self.n_dim: return Size(p)
         t = tuple(self)
-        return bt.Size(p[:s[0]] + t[s[0]:s[0]+1] + p[s[0]:s[1]-1] + t[s[1]:s[1]+1] + p[s[1]-1:]).special_from_(self)
+        return Size(p[:s[0]] + t[s[0]:s[0]+1] + p[s[0]:s[1]-1] + t[s[1]:s[1]+1] + p[s[1]-1:]).special_from_(self)
 
     @property
     def nele(self):
         p = 1
         for i in self:
             if i == -1: return -1
             p *= i
@@ -956,17 +953,14 @@
         m, M = self.min(), self.max()
         if m == M:
             if M >= 1: return ones_like(self)
             if m <= 0: return zeros_like(self)
             return self
         return (self - m) / (M - m)
 
-    for func in tf_list:
-        exec(f"def {func}(*args, **kwargs): return bt.{func}(*args, **kwargs)")
-
     def tensor(self): return super()._make_subclass(torch.Tensor, self, self.requires_grad)
 
     def one_(self): return self.zero_().add_(1)
     
     def autodevice_(self):
         return _device(self)
 
@@ -1376,15 +1370,15 @@
 
         split one dimension source into multiple dimensions: target
         data of size (2, 4, 5) can be transform to (2, 2, 2, 5) with data.splitdim(1, 2, 2).
         Note that batch representations for source and target are different
             (splitdim([1], [2], 2) means split the batchdim at index 1 into a size of ([2], 2), which is 2x2 with batchdim at index 0).
             One can use -1 for arbitrary size. 
         """
-        size = bt.Size(arg_tuple(size))
+        size = Size(arg_tuple(size))
         avouch(len(size) >= 2, f"Please input an at-least-two-dim-shape to split dimension {source} into in method 'splitdim', not {size}. ")
 
         new_size = self.shape[:source] + size + self.shape[source + 1:]
         prod = 1
         ni = None
         for i, x in enumerate(size):
             if isinstance(x, list) and len(x) == 1: x = x[0]
@@ -1393,28 +1387,28 @@
             elif isinstance(x, dict) and len(x) == 0: x = -1
             if x != -1: prod *= x; continue
             ni = i
         if ni is not None:
             x = self.shape[source] // prod
             if size.batch_dimension == ni: x = [x]
             elif size.channel_dimension == ni: x = {x}
-            new_size = new_size[:source + ni] + bt.Size(x) + new_size[source + ni + 1:]
+            new_size = new_size[:source + ni] + Size(x) + new_size[source + ni + 1:]
 
         return self.view(new_size)
 
     def tobytes(self): return self.detach().cpu().numpy().tobytes()
 
     def cat(self, other, dim=0):
         return cat((self, other), dim=dim)
 
     def stack(self, other, dim=0):
         return stack((self, other), dim=dim)
     
     def inv(self):
-        return bt.inv(self)
+        return inv(self)
 
     def view(self, *args):
         if len(args) == 1 and isinstance(args[0], tuple): args = args[0]
         ibatch = ichannel = None
         new_size = []
         for i, x in enumerate(args):
             if isinstance(x, list) and len(x) == 0: ibatch = i; x = -1
@@ -1464,15 +1458,15 @@
         if self._channel_dimension != self.ndim:
             dim_list.remove(self._channel_dimension)
             order.append(self._channel_dimension)
         self.permute_(*(order + dim_list))
         return self
     
     def quantile(self, *args, **kwargs):
-        q = bt.tensor(kwargs.get('q', args[0]))
+        q = tensor(kwargs.get('q', args[0]))
         dim = kwargs.get('dim', args[1] if len(args) >= 2 else None)
         if dim is None: return super().quantile(*args, **kwargs).as_subclass(Tensor)
         if q.ndim > 0: return super().quantile(*args, **kwargs).as_subclass(Tensor).special_from_(self.unsqueeze(0))
         return super().quantile(*args, **kwargs).as_subclass(Tensor).special_from_(self)
     
     ## dtypes
     @alias("as_type")
@@ -1566,15 +1560,23 @@
             yield self[i]
 
     def __getattr__(self, key):
         if not self.init:
             if key == '_special': return [self.ndim, self.ndim]
             elif key == '_batch_first': return True
         try: ret = super().__getattribute__(key)
-        except: raise AttributeError(f"'batorch.tensor' object has no attribute '{key}'")
+        except AttributeError:
+            if key in __all__:
+                obj = eval(key)
+                if callable(obj):
+                    def obj_holder(*args, **kwargs):
+                        return obj(self, *args, **kwargs)
+                    return obj_holder
+                else: return obj
+            else: raise AttributeError(f"'batorch.tensor' object has no attribute '{key}'")
         return ret
 
     def __matmul__(self, other, **kwargs):
         if isinstance(other, torch.Tensor) and self.has_special or isinstance(other, Tensor) and other.has_special:
             # if self.nspace == 0 and self.has_channel: self.with_channeldim(None)
             # if other.nspace == 0 and other.has_channel: other.with_channeldim(None)
             space1 = self.space
@@ -2149,15 +2151,15 @@
                 return super().__torch_function__(func, types, args, kwargs)
 
             func_name = sfunc.split(' of ')[0].split(' at ')[0].split()[-1].strip("'").split('.')[-1]
             if func_name in ('__get__', '__set__', '__delete__'):
                 return super().__torch_function__(func, types, args, kwargs)
 
             self = args[0]
-            types = tuple(cls if t in [torch.nn.Parameter, bt.nn.Parameter] else t for t in types)
+            types = tuple(cls if t.__name__ == "Parameter" else t for t in types)
             torch_func_name = Tensor.__torch_function_map__.get(func_name, None)
             if isinstance(self, Tensor) and self.init and self.has_special: pass
             elif torch_func_name in ('__torch_function_resizing_func__', '__torch_function_full_func__', '__torch_function_resizing_as_func__', '__torch_function_randint_func__'): pass
             else:
                 with torch._C.DisableTorchFunction():
                     ret = super().__torch_function__(func, types, args, kwargs)
                 def apply(r): r.special_from_()
@@ -2287,15 +2289,15 @@
 def cat(*list_of_tensors, dim=None, **kwargs) -> Tensor:
     if dim is None:
         if len(list_of_tensors) > 1 and not isinstance(list_of_tensors[-1], Tensor):
             dim = list_of_tensors[-1]
             list_of_tensors =list_of_tensors[:-1]
         else: dim = 0
     list_of_tensors = arg_tuple(list_of_tensors)
-    if len(list_of_tensors) == 0: return bt.tensor([])
+    if len(list_of_tensors) == 0: return tensor([])
     pivot = list_of_tensors[_argmax([x.ndim for x in list_of_tensors])[0]]
     list_of_tensors = [x.expand_to(pivot, dim=dim) for x in list_of_tensors if x.nele > 0]
     avouch(ALL([SUM([a != b for a, b in zip(x.shape, pivot.shape)]) <= 1 for x in list_of_tensors]), 
            "Tensors can only be concatenated when all of them have a same shape except for one dimension. " + 
            f"Current: {[x.shape for x in list_of_tensors]}")
     ibatch = ichannel = None
     if isinstance(dim, list) and len(dim) == 1: dim = dim[0]; ibatch = dim
@@ -2317,15 +2319,15 @@
 def stack(*list_of_tensors, dim=None, **kwargs) -> Tensor:
     if dim is None:
         if len(list_of_tensors) > 1 and not isinstance(list_of_tensors[-1], torch.Tensor):
             dim = list_of_tensors[-1]
             list_of_tensors = list_of_tensors[:-1]
         else: dim = 0
     list_of_tensors = arg_tuple(list_of_tensors)
-    if len(list_of_tensors) == 0: return bt.tensor([])
+    if len(list_of_tensors) == 0: return tensor([])
     pivot = list_of_tensors[_argmax([x.ndim for x in list_of_tensors])[0]]
     if ALL([x.shape == pivot.shape for x in list_of_tensors]): pass
     else:
         list_of_tensors = [x.expand_to(pivot) for x in list_of_tensors if x.nele > 0]
         avouch(ALL([x.shape == pivot.shape for x in list_of_tensors]), 
             "Tensors can only be stacked when all of them have an exact same shape. ")
     ibatch = ichannel = None
@@ -2358,22 +2360,22 @@
     
 def diag(x) -> Tensor:
     if not isinstance(x, Tensor): x = tensor(x)
     if x.n_space == 1:
         d = item([i for i in RANGE(x.n_dim) if i not in x._special])
         n = x.size(d)
         shape_out = x.shape[:d+1] + (n,) + x.shape[d+1:]
-        out = bt.zeros(shape_out).type(x.type())
-        out[(slice(None),)*d + (bt.arange(n), bt.arange(n)) + (slice(None),)*(x.n_dim-d-1)] = \
-            x[(slice(None),)*d + (bt.arange(n),) + (slice(None),)*(x.n_dim-d-1)]
+        out = zeros(shape_out).type(x.type())
+        out[(slice(None),)*d + (arange(n), arange(n)) + (slice(None),)*(x.n_dim-d-1)] = \
+            x[(slice(None),)*d + (arange(n),) + (slice(None),)*(x.n_dim-d-1)]
         return out
     elif x.n_space == 2:
         p, q = [i for i in RANGE(x.n_dim) if i not in x._special]
         shape_out = x.shape[:q] + (1,) + x.shape[q+1:]
-        ind = bt.arange(x.size(p)).expand_to(shape_out, axis=p, dim=q)
+        ind = arange(x.size(p)).expand_to(shape_out, axis=p, dim=q)
         return x.gather(q, ind).squeeze(q)
     return torch.diag(x).as_subclass(Tensor).special_from_(x)
 
 @alias("tr")
 def trace(x) -> Tensor:
     return diag(x).sum(-1)
 
@@ -2404,60 +2406,51 @@
 
 def channel_tensor(*args, **kwargs) -> Tensor:
     if len(args) == 1 and not isinstance(args[0], (INT, FLOAT)): args = args[0]
     if not isinstance(args, Tensor): args = tensor(list(args), **kwargs)
     avouch(args.ndim == 1, "batorch.channel_tensor only takes 1D data. ")
     return args.channel_dimension_(0)
 
-# print(torch_type_list - (torch_type_list - globals()))
-# print(torch_dtype_list - (torch_dtype_list - globals()))
-# print(torch_func_list - (torch_func_list - globals()))
-
-for key in torch_dtype_list:
-    if not (key in __all__ or key in globals()):
-        exec(f"{key} = torch.{key}")
-        __all__.append(key)
-
-for key in torch_type_list:
-    if not (key in __all__ or key in globals()):
-        exec(f"{key} = torch.{key}")
-        __all__.append(key)
-
 generating_funcs = """
     range arange linspace
 """.split()
 
-for key in torch_func_list:
-    if key in {"typename"}: continue
+stop_set = {"typename"}
+
+for key in dir(torch):
+    if key in stop_set: continue
     if key in __all__: continue
     if key in globals(): continue
-    if key in dir(torch):
-        func = key
-        __all__.append(func)
-        if func in generating_funcs:
-            doit = "ret.requires_grad_(rg)"
-        else: doit = ''
-        execblock(f"""
-        def {func}(*args, **kwargs) -> Tensor:
-            ref_shape = None
-            if len(args) > 0 and isinstance(args[0], Tensor): ref_shape = args[0].shape
-            rg = kwargs.pop('requires_grad', False)
-            ret = torch.{func}(*args, **kwargs)
-            def apply(ret):
-                with torch._C.DisableTorchFunction():
-                    if isinstance(ret, Tensor) and not ret.init or not isinstance(ret, Tensor) and isinstance(ret, torch.Tensor):
-                        ref = None
-                        if ref_shape is not None and len(ret.shape) == len(ref_shape): ref = ref_shape
-                        ret = ret.as_subclass(Tensor).autodevice_()
-                        ret = ret.as_subclass(Tensor).special_from_(ref)
-                        {doit}
-                        return ret
-
-                    if not isinstance(ret, torch.Tensor) and isoftype(ret, (tuple, list, Iterable)):
-                        # Also handles things like namedtuples
-                        return type(ret)(apply(r) for r in ret)
-
+    if not callable(eval(f"torch.{key}")):
+        exec(f"{key} = torch.{key}")
+        __all__.append(key)
+        continue
+    func = key
+    __all__.append(func)
+    if func in generating_funcs:
+        doit = "ret.requires_grad_(rg)"
+    else: doit = ''
+    execblock(f"""
+    def {func}(*args, **kwargs) -> Tensor:
+        ref_shape = None
+        if len(args) > 0 and isinstance(args[0], Tensor): ref_shape = args[0].shape
+        rg = kwargs.pop('requires_grad', False)
+        ret = torch.{func}(*args, **kwargs)
+        def apply(ret):
+            with torch._C.DisableTorchFunction():
+                if isinstance(ret, Tensor) and not ret.init or not isinstance(ret, Tensor) and isinstance(ret, torch.Tensor):
+                    ref = None
+                    if ref_shape is not None and len(ret.shape) == len(ref_shape): ref = ref_shape
+                    ret = ret.as_subclass(Tensor).autodevice_()
+                    ret = ret.as_subclass(Tensor).special_from_(ref)
+                    {doit}
                     return ret
-            return apply(ret)
-        """)
+
+                if not isinstance(ret, torch.Tensor) and isoftype(ret, (tuple, list, Iterable)):
+                    # Also handles things like namedtuples
+                    return type(ret)(apply(r) for r in ret)
+
+                return ret
+        return apply(ret)
+    """)
 
 inv = eval('inverse')
```

### Comparing `pycamia-1.0.36/batorch/tensor2.py` & `pycamia-1.0.37/batorch/tensor2.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/tensorfunc.py` & `pycamia-1.0.37/batorch/tensorfunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 
 def one_hot(k, n):
     """
     Create an one-hot vector as a zero `bt.Tensor` with length `n` and the `k`-th element 1. 
     e.g. k == -1 gives tensor([0, 0, ..., 0, 1])
     """
     l = [0] * n; l[k] = 1
-    return batorch_tensor(l)
+    return bt.to_device(batorch_tensor(l))
 
 def permute_space(data, *dims):
     """
     permute the space section in data. len(dims) should be data.n_space. 
     """
     data = batorch_tensor(data)
     if len(dims) == 1 and isinstance(dims[0], (list, tuple)): dims = dims[0]
```

### Comparing `pycamia-1.0.36/batorch/torch_namespace.py` & `pycamia-1.0.37/batorch/torch_namespace.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/batorch/torchext.py` & `pycamia-1.0.37/batorch/torchext.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/__init__.py` & `pycamia-1.0.37/micomputing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.36',
+    version = '1.1.37',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
-    update = '2023-07-05 16:28:37',
+    update = '2023-07-05 17:05:57',
     package_data = True
 ).check()
 
 from . import plot as plt
 from .stdio import IMG, dcm2nii, nii2dcm #*
 from .data import Info, Subject, ImageObject, Dataset, MedicalDataset #*
 from .network import U_Net, CNN, FCN
 from .funcs import reorient, rescale, reflect, dilate, blur, bending, distance_map, registration, local_prior, center_of_gravity #*
 from .trans import Transformation, SpatialTransformation, ImageTransformation, ComposedTransformation, CompoundTransformation, Identity, Id, Rotation90, Rotation180, Rotation270, Reflect, Reflection, Permutedim, DimPermutation, Rescale, Rescaling, Translate, Translation, Rigid, Rig, Affine, Aff, PolyAffine, logEu, LocallyAffine, LARM, FreeFormDeformation, FFD, DenseDisplacementField, DDF, MultiLayerPerception, MLP, Normalize, resample, interpolation, interpolation_forward, Affine2D2Matrix, Quaterns2Matrix, Matrix2Quaterns #*
 from .metrics import metric, ITKMetric, ITKLabelMetric, MutualInformation, NormalizedMutualInformation, KLDivergence, CorrelationOfLocalEstimation, NormalizedVectorInformation, Cos2Theta, SumSquaredDifference, MeanSquaredErrors, PeakSignalToNoiseRatio, CrossEntropy, CrossCorrelation, NormalizedCrossCorrelation, StructuralSimilarity, Dice, DiceScore, DiceScoreCoefficient, LabelDice, LabelDiceScore, LabelDiceScoreCoefficient, ITKDiceScore, ITKJaccardCoefficient, ITKVolumeSimilarity, ITKFalsePositive, ITKFalseNegative, ITKHausdorffDistance, ITKMedianSurfaceDistance, ITKAverageSurfaceDistance, ITKDivergenceOfSurfaceDistance, ITKLabelDiceScore, ITKLabelJaccardCoefficient, ITKLabelVolumeSimilarity, ITKLabelFalsePositive, ITKLabelFalseNegative, ITKLabelHausdorffDistance, ITKLabelMedianSurfaceDistance, ITKLabelAverageSurfaceDistance, ITKLabelDivergenceOfSurfaceDistance, LocalNonOrthogonality, RigidProjectionError #*
 
-import zxhtools
-import micfunctions
```

### Comparing `pycamia-1.0.36/micomputing/data.py` & `pycamia-1.0.37/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/funcs.py` & `pycamia-1.0.37/micomputing/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,21 +34,27 @@
 eps = 1e-6
 
 with __info__:
     from pycamia import avouch, to_tuple, to_list, restore_type_wrapper, prod, Version, Path
     from batorch import torch as torch
     import batorch as bt
 
-    dll = ctypes.cdll.LoadLibrary(Path(__file__).parent/'micfunctions.so')
-    distance_map_func = dll.distance_map
-    distance_map_func.argtypes = [np.ctypeslib.ndpointer(dtype=np.int32,ndim=1,flags="C_CONTIGUOUS"),
-                                  np.ctypeslib.ndpointer(dtype=np.float32,ndim=1,flags="C_CONTIGUOUS"),
-                                  ctypes.c_int,
-                                  np.ctypeslib.ndpointer(dtype=np.int32,ndim=1,flags="C_CONTIGUOUS"),
-                                  np.ctypeslib.ndpointer(dtype=np.float32,ndim=1,flags="C_CONTIGUOUS")]
+for trial in range(2):
+    try:
+        dll = ctypes.cdll.LoadLibrary(Path(__file__).parent/'micfunctions.so')
+        distance_map_func = dll.distance_map
+        distance_map_func.argtypes = [np.ctypeslib.ndpointer(dtype=np.int32,ndim=1,flags="C_CONTIGUOUS"),
+                                    np.ctypeslib.ndpointer(dtype=np.float32,ndim=1,flags="C_CONTIGUOUS"),
+                                    ctypes.c_int,
+                                    np.ctypeslib.ndpointer(dtype=np.int32,ndim=1,flags="C_CONTIGUOUS"),
+                                    np.ctypeslib.ndpointer(dtype=np.float32,ndim=1,flags="C_CONTIGUOUS")]
+        break
+    except OSError: # Try to compile dll or warn the user
+        if trial == 0: os.system("g++ -o micfunctions.so -shared -fPIC micfuncions.cpp")
+        else: print("Unable to compile C++ DLL: micfunctions, 'micomputing.dilate' is not functional, please install command 'g++' or use 'micomputing.dilate_sitk' instead.")
 
 def torch_tensor(x):
     if not isinstance(x, torch.Tensor): return torch.tensor(x)
     elif type(x) != torch.Tensor: return x.as_subclass(torch.Tensor)
     return x
     
 def batorch_tensor(x):
@@ -254,24 +260,24 @@
     if not mask.has_batch: squeeze_batch = True; mask.unsqueeze_([])
     min_values, indices = distance_map_cpp(bt.stack([mask == l for l in class_labels], {}), spacing=spacing).min({})
     res = bt.tensor(class_labels)[indices].float() * (min_values <= distance).float()
     if squeeze_batch: res.squeeze_([])
     return res
 
 @restore_type_wrapper
-def dilate_cpp(mask, distance = 0, spacing = 1, class_labels = None):
+def dilate_sitk(mask, distance = 0, spacing = 1, class_labels = None):
     """mask: ([n_batch], n@1, ..., n@n_dim)"""
     mask = batorch_tensor(mask)
     if not class_labels: class_labels = sorted(mask.unique().tolist())[1:]
     if len(class_labels) == 0: return mask
     spacing = to_tuple(spacing)
     if len(spacing) == 1: spacing *= mask.n_space
     squeeze_batch = False
     if not mask.has_batch: squeeze_batch = True; mask.unsqueeze_([])
-    min_values, indices = distance_map_cpp(bt.stack([mask == l for l in class_labels], {}), spacing=spacing).min({})
+    min_values, indices = distance_map(bt.stack([mask == l for l in class_labels], {}), spacing=spacing).min({})
     res = bt.tensor(class_labels)[indices].float() * (min_values <= distance).float()
     if squeeze_batch: res.squeeze_([])
     return res
 
 @restore_type_wrapper
 def dilate_python(mask, distance = 0, spacing = 1, class_labels = None):
     """mask: ([n_batch], n@1, ..., n@n_dim)"""
```

### Comparing `pycamia-1.0.36/micomputing/metrics.py` & `pycamia-1.0.37/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/micfunctions.so` & `pycamia-1.0.37/micomputing/micfunctions.so`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/network.py` & `pycamia-1.0.37/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/plot.py` & `pycamia-1.0.37/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/stdio.py` & `pycamia-1.0.37/micomputing/stdio.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/test.py` & `pycamia-1.0.37/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/trans.py` & `pycamia-1.0.37/micomputing/trans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1075,5100 +1075,5108 @@
 00004320: 2067 6574 2060 6166 6669 6e65 6020 6672   get `affine` fr
 00004330: 6f6d 2063 6f6d 706f 7365 6420 7472 616e  om composed tran
 00004340: 7366 6f72 6d61 7469 6f6e 2077 6974 6820  sformation with 
 00004350: 6e6f 6e2d 7370 6174 6961 6c20 7472 616e  non-spatial tran
 00004360: 7366 6f72 6d61 7469 6f6e 2e20 2229 0a20  sformation. "). 
 00004370: 2020 2020 2020 2063 6f6d 7020 3d20 7365         comp = se
 00004380: 6c66 2e63 6f6d 706f 7365 2829 0a20 2020  lf.compose().   
-00004390: 2020 2020 2069 6620 6c65 6e28 636f 6d70       if len(comp
-000043a0: 2920 3e20 313a 2072 6574 7572 6e0a 2020  ) > 1: return.  
-000043b0: 2020 2020 2020 7472 616e 7320 3d20 636f        trans = co
-000043c0: 6d70 2e74 7261 6e73 5f6c 6973 745b 305d  mp.trans_list[0]
-000043d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000043e0: 7472 616e 732e 6166 6669 6e65 286e 5f64  trans.affine(n_d
-000043f0: 696d 290a 0a20 2020 2064 6566 2063 6f6d  im)..    def com
-00004400: 706f 7365 2873 656c 6629 3a0a 2020 2020  pose(self):.    
-00004410: 2020 2020 6f75 745f 6c69 7374 203d 205b      out_list = [
-00004420: 5d0a 2020 2020 2020 2020 6e5f 6469 6d20  ].        n_dim 
-00004430: 3d20 7365 6c66 2e6e 5f64 696d 0a20 2020  = self.n_dim.   
-00004440: 2020 2020 2063 7572 5f61 6666 696e 6520       cur_affine 
-00004450: 3d20 4e6f 6e65 0a20 2020 2020 2020 2066  = None.        f
-00004460: 6f72 2074 2069 6e20 7365 6c66 2e74 7261  or t in self.tra
-00004470: 6e73 5f6c 6973 743a 0a20 2020 2020 2020  ns_list:.       
-00004480: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00004490: 7374 616e 6365 2874 2c20 5370 6174 6961  stance(t, Spatia
-000044a0: 6c54 7261 6e73 666f 726d 6174 696f 6e29  lTransformation)
-000044b0: 3a20 6f75 745f 6c69 7374 2e61 7070 656e  : out_list.appen
-000044c0: 6428 7429 0a20 2020 2020 2020 2020 2020  d(t).           
-000044d0: 2061 6666 203d 2074 2e61 6666 696e 6528   aff = t.affine(
-000044e0: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
-000044f0: 2020 2069 6620 6166 6620 6973 204e 6f6e     if aff is Non
-00004500: 6520 616e 6420 6375 725f 6166 6669 6e65  e and cur_affine
-00004510: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00004520: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00004530: 745f 6c69 7374 2e65 7874 656e 6428 5b41  t_list.extend([A
-00004540: 6666 696e 6528 6375 725f 6166 6669 6e65  ffine(cur_affine
-00004550: 292c 2074 5d29 0a20 2020 2020 2020 2020  ), t]).         
-00004560: 2020 2020 2020 2063 7572 5f61 6666 696e         cur_affin
-00004570: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
-00004580: 2020 2020 2065 6c69 6620 6166 6620 6973       elif aff is
-00004590: 204e 6f6e 653a 206f 7574 5f6c 6973 742e   None: out_list.
-000045a0: 6170 7065 6e64 2874 290a 2020 2020 2020  append(t).      
-000045b0: 2020 2020 2020 656c 6966 2061 6666 2e73        elif aff.s
-000045c0: 7061 6365 2021 3d20 286e 5f64 696d 2b31  pace != (n_dim+1
-000045d0: 2c20 6e5f 6469 6d2b 3129 3a0a 2020 2020  , n_dim+1):.    
-000045e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000045f0: 6520 5479 7065 4572 726f 7228 6622 556e  e TypeError(f"Un
-00004600: 636f 6e73 6973 7465 6e74 2074 7261 6e73  consistent trans
-00004610: 666f 726d 6174 696f 6e20 7769 7468 2061  formation with a
-00004620: 6666 696e 6520 6f66 2073 697a 6520 7b61  ffine of size {a
-00004630: 6666 2e73 7061 6365 7d20 696e 2043 6f6d  ff.space} in Com
-00004640: 706f 7365 6454 7261 6e73 666f 726d 6174  posedTransformat
-00004650: 696f 6e2e 2022 290a 2020 2020 2020 2020  ion. ").        
-00004660: 2020 2020 656c 6966 2063 7572 5f61 6666      elif cur_aff
-00004670: 696e 6520 6973 204e 6f6e 653a 2063 7572  ine is None: cur
-00004680: 5f61 6666 696e 6520 3d20 6166 660a 2020  _affine = aff.  
-00004690: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-000046a0: 6375 725f 6166 6669 6e65 203d 2063 7572  cur_affine = cur
-000046b0: 5f61 6666 696e 6520 4020 6166 660a 2020  _affine @ aff.  
-000046c0: 2020 2020 2020 6966 2063 7572 5f61 6666        if cur_aff
-000046d0: 696e 6520 6973 206e 6f74 204e 6f6e 653a  ine is not None:
-000046e0: 206f 7574 5f6c 6973 742e 6170 7065 6e64   out_list.append
-000046f0: 2841 6666 696e 6528 6375 725f 6166 6669  (Affine(cur_affi
-00004700: 6e65 2929 0a20 2020 2020 2020 2072 6574  ne)).        ret
-00004710: 7572 6e20 436f 6d70 6f73 6564 5472 616e  urn ComposedTran
-00004720: 7366 6f72 6d61 7469 6f6e 282a 6f75 745f  sformation(*out_
-00004730: 6c69 7374 2c20 6d6f 6465 203d 2073 656c  list, mode = sel
-00004740: 662e 6d6f 6465 290a 0a20 2020 2064 6566  f.mode)..    def
-00004750: 2074 6f5f 6469 6374 2873 656c 6629 3a0a   to_dict(self):.
-00004760: 2020 2020 2020 2020 6469 6320 3d20 7375          dic = su
-00004770: 7065 7228 292e 746f 5f64 6963 7428 290a  per().to_dict().
-00004780: 2020 2020 2020 2020 6469 635b 2774 7261          dic['tra
-00004790: 6e73 5f6c 6973 7427 5d20 3d20 5b74 2e74  ns_list'] = [t.t
-000047a0: 6f5f 6469 6374 2829 2066 6f72 2074 2069  o_dict() for t i
-000047b0: 6e20 7365 6c66 2e74 7261 6e73 5f6c 6973  n self.trans_lis
-000047c0: 745d 0a20 2020 2020 2020 2072 6574 7572  t].        retur
-000047d0: 6e20 6469 630a 0a23 2323 2323 2323 2323  n dic..#########
-000047e0: 2323 2053 7061 7469 616c 2054 7261 6e73  ## Spatial Trans
-000047f0: 666f 726d 6174 696f 6e73 2023 2323 2323  formations #####
-00004800: 2323 2323 2323 0a0a 636c 6173 7320 5370  ######..class Sp
-00004810: 6174 6961 6c54 7261 6e73 666f 726d 6174  atialTransformat
-00004820: 696f 6e28 5472 616e 7366 6f72 6d61 7469  ion(Transformati
-00004830: 6f6e 293a 0a20 2020 200a 2020 2020 6465  on):.    .    de
-00004840: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00004850: 202a 7061 7261 6d73 2c20 2a2a 6b77 7061   *params, **kwpa
-00004860: 7261 6d73 293a 0a20 2020 2020 2020 2073  rams):.        s
-00004870: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00004880: 2a70 6172 616d 732c 202a 2a6b 7770 6172  *params, **kwpar
-00004890: 616d 7329 0a20 2020 2020 2020 2073 656c  ams).        sel
-000048a0: 662e 6261 636b 7761 7264 203d 2054 7275  f.backward = Tru
-000048b0: 650a 2020 2020 2020 2020 0a20 2020 2064  e.        .    d
-000048c0: 6566 205f 5f63 616c 6c5f 5f28 7365 6c66  ef __call__(self
-000048d0: 2c20 5829 3a0a 2020 2020 2020 2020 2222  , X):.        ""
-000048e0: 220a 2020 2020 2020 2020 5820 5b62 742e  ".        X [bt.
-000048f0: 5465 6e73 6f72 5d3a 2043 6f6f 7264 696e  Tensor]: Coordin
-00004900: 6174 6573 2074 6f20 6265 2074 7261 6e73  ates to be trans
-00004910: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
-00004920: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00004930: 7463 683a 206f 7074 696f 6e61 6c5d 2c20  tch: optional], 
-00004940: 7b6e 5f64 696d 7d2c 206e 5f31 2c20 6e5f  {n_dim}, n_1, n_
-00004950: 322c 202e 2e2e 2c20 6e5f 7229 0a20 2020  2, ..., n_r).   
-00004960: 2020 2020 206f 7574 7075 7420 5b62 742e       output [bt.
-00004970: 5465 6e73 6f72 5d3a 2054 6865 2074 7261  Tensor]: The tra
-00004980: 6e73 666f 726d 6564 2063 6f6f 7264 696e  nsformed coordin
-00004990: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
-000049a0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-000049b0: 685d 2c20 7b6e 5f64 696d 7d2c 206e 5f31  h], {n_dim}, n_1
-000049c0: 2c20 6e5f 322c 202e 2e2e 2c20 6e5f 7229  , n_2, ..., n_r)
-000049d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000049e0: 2020 2020 2061 766f 7563 6828 582e 6861       avouch(X.ha
-000049f0: 735f 6368 616e 6e65 6c2c 2066 2250 6c65  s_channel, f"Ple
-00004a00: 6173 6520 7573 6520 6261 746f 7263 6820  ase use batorch 
-00004a10: 7465 6e73 6f72 206f 6620 7369 7a65 205c  tensor of size \
-00004a20: 0a20 2020 2020 2020 2020 2020 2028 5b6e  .            ([n
-00004a30: 5f62 6174 6368 3a6f 7074 696f 6e61 6c5d  _batch:optional]
-00004a40: 2c20 7b7b 6e5f 6469 6d7d 7d2c 206e 5f31  , {{n_dim}}, n_1
-00004a50: 2c20 6e5f 322c 202e 2e2e 2c20 6e5f 7229  , n_2, ..., n_r)
-00004a60: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-00004a70: 2020 2066 6f72 207b 7365 6c66 2e5f 5f63     for {self.__c
-00004a80: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f2e  lass__.__name__.
-00004a90: 7370 6c69 7428 272e 2729 5b2d 315d 7d20  split('.')[-1]} 
-00004aa0: 5472 616e 7366 6f72 6d61 7469 6f6e 2c20  Transformation, 
-00004ab0: 696e 7374 6561 6420 6f66 207b 582e 7368  instead of {X.sh
-00004ac0: 6170 657d 2e20 2229 0a20 2020 2020 2020  ape}. ").       
-00004ad0: 2069 6620 7365 6c66 2e6e 5f64 696d 2069   if self.n_dim i
-00004ae0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00004af0: 2020 2020 2020 2020 6176 6f75 6368 2858          avouch(X
-00004b00: 2e6e 5f63 6861 6e6e 656c 203d 3d20 7365  .n_channel == se
-00004b10: 6c66 2e6e 5f64 696d 2c20 6622 7b73 656c  lf.n_dim, f"{sel
-00004b20: 662e 6e5f 6469 6d7d 4420 7b73 656c 662e  f.n_dim}D {self.
-00004b30: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
-00004b40: 5f5f 2e73 706c 6974 2827 2e27 295b 2d31  __.split('.')[-1
-00004b50: 5d7d 2054 7261 6e73 666f 726d 6174 696f  ]} Transformatio
-00004b60: 6e20 5c0a 2020 2020 2020 2020 2020 2020  n \.            
-00004b70: 2020 2020 646f 6573 206e 6f74 2074 616b      does not tak
-00004b80: 6520 636f 6f72 6469 6e61 7465 7320 6f66  e coordinates of
-00004b90: 2073 697a 6520 7b58 2e73 6861 7065 7d22   size {X.shape}"
-00004ba0: 290a 2020 2020 2020 2020 6966 2058 2e68  ).        if X.h
-00004bb0: 6173 5f62 6174 6368 3a20 6176 6f75 6368  as_batch: avouch
-00004bc0: 2873 656c 662e 6e5f 6261 7463 6820 6973  (self.n_batch is
-00004bd0: 204e 6f6e 6520 6f72 2073 656c 662e 6e5f   None or self.n_
-00004be0: 6261 7463 6820 3d3d 2031 206f 7220 582e  batch == 1 or X.
-00004bf0: 6e5f 6261 7463 6820 3d3d 2031 206f 7220  n_batch == 1 or 
-00004c00: 582e 6e5f 6261 7463 6820 3d3d 2073 656c  X.n_batch == sel
-00004c10: 662e 6e5f 6261 7463 682c 200a 2020 2020  f.n_batch, .    
-00004c20: 2020 2020 2020 2020 6622 7b73 656c 662e          f"{self.
-00004c30: 6e5f 6469 6d7d 4420 7b73 656c 662e 5f5f  n_dim}D {self.__
-00004c40: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
-00004c50: 2e73 706c 6974 2827 2e27 295b 2d31 5d7d  .split('.')[-1]}
-00004c60: 2054 7261 6e73 666f 726d 6174 696f 6e20   Transformation 
-00004c70: 7769 7468 2062 6174 6368 2073 697a 6520  with batch size 
-00004c80: 7b73 656c 662e 6e5f 6261 7463 687d 205c  {self.n_batch} \
-00004c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ca0: 2064 6f65 7320 6e6f 7420 7461 6b65 2063   does not take c
-00004cb0: 6f6f 7264 696e 6174 6573 2077 6974 6820  oordinates with 
-00004cc0: 7772 6f6e 6720 6261 7463 6820 7369 7a65  wrong batch size
-00004cd0: 2e20 4375 7272 656e 7420 7369 7a65 3a20  . Current size: 
-00004ce0: 7b58 2e73 6861 7065 7d2e 2229 0a20 2020  {X.shape}.").   
-00004cf0: 2020 2020 2059 203d 2058 2e66 6c6f 6174       Y = X.float
-00004d00: 2829 2e63 6c6f 6e65 2829 0a20 2020 2020  ().clone().     
-00004d10: 2020 2069 6620 6e6f 7420 592e 6861 735f     if not Y.has_
-00004d20: 6261 7463 683a 0a20 2020 2020 2020 2020  batch:.         
-00004d30: 2020 2069 6620 7365 6c66 2e6e 5f62 6174     if self.n_bat
-00004d40: 6368 2069 7320 6e6f 7420 4e6f 6e65 3a20  ch is not None: 
-00004d50: 5920 3d20 592e 6d75 6c74 6970 6c79 2873  Y = Y.multiply(s
-00004d60: 656c 662e 6e5f 6261 7463 682c 205b 5d29  elf.n_batch, [])
-00004d70: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00004d80: 653a 2059 203d 2059 2e75 6e73 7175 6565  e: Y = Y.unsquee
-00004d90: 7a65 285b 5d29 0a20 2020 2020 2020 2072  ze([]).        r
-00004da0: 6574 7572 6e20 590a 0a20 2020 2064 6566  eturn Y..    def
-00004db0: 205f 5f6d 6174 6d75 6c5f 5f28 782c 2079   __matmul__(x, y
-00004dc0: 293a 0a20 2020 2020 2020 2069 6620 6973  ):.        if is
-00004dd0: 5f73 7061 7469 616c 5f74 7261 6e73 666f  _spatial_transfo
-00004de0: 726d 6174 696f 6e28 7829 2061 6e64 2069  rmation(x) and i
-00004df0: 735f 7370 6174 6961 6c5f 7472 616e 7366  s_spatial_transf
-00004e00: 6f72 6d61 7469 6f6e 2879 293a 0a20 2020  ormation(y):.   
-00004e10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00004e20: 436f 6d70 6f73 6564 5472 616e 7366 6f72  ComposedTransfor
-00004e30: 6d61 7469 6f6e 2878 2c20 792c 206d 6f64  mation(x, y, mod
-00004e40: 653d 2273 7061 7469 616c 2229 0a20 2020  e="spatial").   
-00004e50: 2020 2020 2072 6574 7572 6e20 436f 6d70       return Comp
-00004e60: 6f73 6564 5472 616e 7366 6f72 6d61 7469  osedTransformati
-00004e70: 6f6e 2878 2c20 7929 0a20 2020 200a 2020  on(x, y).    .  
-00004e80: 2020 6465 6620 6166 6669 6e65 2873 656c    def affine(sel
-00004e90: 662c 206e 5f64 696d 3d4e 6f6e 6529 3a0a  f, n_dim=None):.
-00004ea0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00004eb0: 6f6e 650a 2020 2020 0a20 2020 2040 616c  one.    .    @al
-00004ec0: 6961 7328 2774 6f44 4446 2729 0a20 2020  ias('toDDF').   
-00004ed0: 2064 6566 2074 6f5f 4444 4628 7365 6c66   def to_DDF(self
-00004ee0: 2c20 2a73 6861 7065 293a 0a20 2020 2020  , *shape):.     
-00004ef0: 2020 2073 6861 7065 203d 2061 7267 5f74     shape = arg_t
-00004f00: 7570 6c65 2873 6861 7065 290a 2020 2020  uple(shape).    
-00004f10: 2020 2020 6772 6964 203d 2062 742e 696d      grid = bt.im
-00004f20: 6167 655f 6772 6964 282a 7368 6170 6529  age_grid(*shape)
-00004f30: 2e75 6e73 7175 6565 7a65 285b 5d29 2e66  .unsqueeze([]).f
-00004f40: 6c6f 6174 2829 0a20 2020 2020 2020 2072  loat().        r
-00004f50: 6574 7572 6e20 7365 6c66 2867 7269 6429  eturn self(grid)
-00004f60: 202d 2067 7269 640a 0a20 2020 2064 6566   - grid..    def
-00004f70: 2074 6f5f 696d 6167 655f 7370 6163 6528   to_image_space(
-00004f80: 7365 6c66 2c20 736f 7572 6365 2c20 7461  self, source, ta
-00004f90: 7267 6574 293a 0a20 2020 2020 2020 2069  rget):.        i
-00004fa0: 6620 6973 696e 7374 616e 6365 2873 6f75  f isinstance(sou
-00004fb0: 7263 652c 2073 7472 293a 2073 6f75 7263  rce, str): sourc
-00004fc0: 6520 3d20 494d 4728 736f 7572 6365 290a  e = IMG(source).
-00004fd0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00004fe0: 7461 6e63 6528 7461 7267 6574 2c20 7374  tance(target, st
-00004ff0: 7229 3a20 7461 7267 6574 203d 2049 4d47  r): target = IMG
-00005000: 2874 6172 6765 7429 0a20 2020 2020 2020  (target).       
-00005010: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-00005020: 6f75 7263 652c 2049 4d47 293a 2073 6f75  ource, IMG): sou
-00005030: 7263 6520 3d20 736f 7572 6365 2e61 6666  rce = source.aff
-00005040: 696e 650a 2020 2020 2020 2020 6966 2069  ine.        if i
-00005050: 7369 6e73 7461 6e63 6528 7461 7267 6574  sinstance(target
-00005060: 2c20 494d 4729 3a20 7461 7267 6574 203d  , IMG): target =
-00005070: 2074 6172 6765 742e 6166 6669 6e65 0a20   target.affine. 
-00005080: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00005090: 6c66 2e74 6f28 2769 6d61 6765 272c 2073  lf.to('image', s
-000050a0: 6f75 7263 655f 6166 6669 6e65 3d73 6f75  ource_affine=sou
-000050b0: 7263 652c 2074 6172 6765 745f 6166 6669  rce, target_affi
-000050c0: 6e65 3d74 6172 6765 7429 0a0a 2020 2020  ne=target)..    
-000050d0: 6465 6620 746f 5f77 6f72 6c64 5f73 7061  def to_world_spa
-000050e0: 6365 2873 656c 662c 2073 6f75 7263 652c  ce(self, source,
-000050f0: 2074 6172 6765 7429 3a0a 2020 2020 2020   target):.      
-00005100: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00005110: 736f 7572 6365 2c20 7374 7229 3a20 736f  source, str): so
-00005120: 7572 6365 203d 2049 4d47 2873 6f75 7263  urce = IMG(sourc
-00005130: 6529 0a20 2020 2020 2020 2069 6620 6973  e).        if is
-00005140: 696e 7374 616e 6365 2874 6172 6765 742c  instance(target,
-00005150: 2073 7472 293a 2074 6172 6765 7420 3d20   str): target = 
-00005160: 494d 4728 7461 7267 6574 290a 2020 2020  IMG(target).    
-00005170: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00005180: 6528 736f 7572 6365 2c20 494d 4729 3a20  e(source, IMG): 
-00005190: 736f 7572 6365 203d 2073 6f75 7263 652e  source = source.
-000051a0: 6166 6669 6e65 0a20 2020 2020 2020 2069  affine.        i
-000051b0: 6620 6973 696e 7374 616e 6365 2874 6172  f isinstance(tar
-000051c0: 6765 742c 2049 4d47 293a 2074 6172 6765  get, IMG): targe
-000051d0: 7420 3d20 7461 7267 6574 2e61 6666 696e  t = target.affin
-000051e0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-000051f0: 2073 656c 662e 746f 2827 776f 726c 6427   self.to('world'
-00005200: 2c20 736f 7572 6365 5f61 6666 696e 653d  , source_affine=
-00005210: 736f 7572 6365 2c20 7461 7267 6574 5f61  source, target_a
-00005220: 6666 696e 653d 7461 7267 6574 290a 0a20  ffine=target).. 
-00005230: 2020 2064 6566 2074 6f28 7365 6c66 2c20     def to(self, 
-00005240: 7370 6163 6520 3d20 2277 6f72 6c64 222c  space = "world",
-00005250: 2073 6f75 7263 655f 6166 6669 6e65 203d   source_affine =
-00005260: 2062 742e 6579 6528 3429 2c20 7461 7267   bt.eye(4), targ
-00005270: 6574 5f61 6666 696e 6520 3d20 6274 2e65  et_affine = bt.e
-00005280: 7965 2834 2929 3a0a 2020 2020 2020 2020  ye(4)):.        
-00005290: 7461 7267 6574 5f61 6666 696e 6520 3d20  target_affine = 
-000052a0: 6261 746f 7263 685f 7465 6e73 6f72 2874  batorch_tensor(t
-000052b0: 6172 6765 745f 6166 6669 6e65 292e 666c  arget_affine).fl
-000052c0: 6f61 7428 290a 2020 2020 2020 2020 736f  oat().        so
-000052d0: 7572 6365 5f61 6666 696e 6520 3d20 6261  urce_affine = ba
-000052e0: 746f 7263 685f 7465 6e73 6f72 2873 6f75  torch_tensor(sou
-000052f0: 7263 655f 6166 6669 6e65 292e 666c 6f61  rce_affine).floa
-00005300: 7428 290a 2020 2020 2020 2020 6966 2074  t().        if t
-00005310: 6172 6765 745f 6166 6669 6e65 2e6e 6469  arget_affine.ndi
-00005320: 6d20 3c3d 2032 3a20 7461 7267 6574 5f61  m <= 2: target_a
-00005330: 6666 696e 6520 3d20 6274 2e75 6e73 7175  ffine = bt.unsqu
-00005340: 6565 7a65 2874 6172 6765 745f 6166 6669  eeze(target_affi
-00005350: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
-00005360: 6f75 7263 655f 6166 6669 6e65 2e6e 6469  ource_affine.ndi
-00005370: 6d20 3c3d 2032 3a20 736f 7572 6365 5f61  m <= 2: source_a
-00005380: 6666 696e 6520 3d20 6274 2e75 6e73 7175  ffine = bt.unsqu
-00005390: 6565 7a65 2873 6f75 7263 655f 6166 6669  eeze(source_affi
-000053a0: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
-000053b0: 7061 6365 2e6c 6f77 6572 2829 203d 3d20  pace.lower() == 
-000053c0: 2277 6f72 6c64 2220 6f72 2073 7061 6365  "world" or space
-000053d0: 2e6c 6f77 6572 2829 203d 3d20 2270 6879  .lower() == "phy
-000053e0: 7369 6361 6c22 3a20 7461 6666 696e 6520  sical": taffine 
-000053f0: 3d20 6274 2e69 6e76 2874 6172 6765 745f  = bt.inv(target_
-00005400: 6166 6669 6e65 293b 2073 6166 6669 6e65  affine); saffine
-00005410: 203d 2073 6f75 7263 655f 6166 6669 6e65   = source_affine
-00005420: 0a20 2020 2020 2020 2065 6c69 6620 7370  .        elif sp
-00005430: 6163 652e 6c6f 7765 7228 2920 3d3d 2022  ace.lower() == "
-00005440: 696d 6167 6522 206f 7220 7370 6163 652e  image" or space.
-00005450: 6c6f 7765 7228 2920 3d3d 2022 696e 6465  lower() == "inde
-00005460: 7822 3a20 7461 6666 696e 6520 3d20 7461  x": taffine = ta
-00005470: 7267 6574 5f61 6666 696e 653b 2073 6166  rget_affine; saf
-00005480: 6669 6e65 203d 2062 742e 696e 7628 736f  fine = bt.inv(so
-00005490: 7572 6365 5f61 6666 696e 6529 0a20 2020  urce_affine).   
-000054a0: 2020 2020 2065 6c73 653a 2072 6169 7365       else: raise
-000054b0: 2054 7970 6545 7272 6f72 2822 496e 7661   TypeError("Inva
-000054c0: 6c69 6420 7370 6163 6520 666f 7220 6d65  lid space for me
-000054d0: 7468 6f64 2027 746f 272c 2075 7365 2027  thod 'to', use '
-000054e0: 776f 726c 6427 2f27 7068 7973 6963 616c  world'/'physical
-000054f0: 2720 6f72 2027 696d 6167 6527 2f27 696e  ' or 'image'/'in
-00005500: 6465 7827 2069 6e73 7465 6164 2e22 290a  dex' instead.").
-00005510: 2020 2020 2020 2020 7265 7475 726e 2043          return C
-00005520: 6f6d 706f 7365 6454 7261 6e73 666f 726d  omposedTransform
-00005530: 6174 696f 6e28 4166 6669 6e65 2873 6166  ation(Affine(saf
-00005540: 6669 6e65 292c 2073 656c 662c 2041 6666  fine), self, Aff
-00005550: 696e 6528 7461 6666 696e 6529 2c20 6d6f  ine(taffine), mo
-00005560: 6465 3d27 7370 6174 6961 6c27 290a 2020  de='spatial').  
-00005570: 2020 0a20 2020 2064 6566 206e 756d 5f69    .    def num_i
-00005580: 6e76 2873 656c 662c 202a 7369 7a65 2c20  nv(self, *size, 
-00005590: 7665 7262 6f73 653d 4661 6c73 6529 3a0a  verbose=False):.
-000055a0: 2020 2020 2020 2020 6672 6f6d 202e 6675          from .fu
-000055b0: 6e63 7320 696d 706f 7274 2062 656e 6469  ncs import bendi
-000055c0: 6e67 0a20 2020 2020 2020 2073 697a 6520  ng.        size 
-000055d0: 3d20 6172 675f 7475 706c 6528 7369 7a65  = arg_tuple(size
-000055e0: 290a 2020 2020 2020 2020 5820 3d20 6274  ).        X = bt
-000055f0: 2e69 6d61 6765 5f67 7269 6428 2a73 697a  .image_grid(*siz
-00005600: 6529 2e75 6e73 7175 6565 7a65 285b 5d29  e).unsqueeze([])
-00005610: 2e66 6c6f 6174 2829 0a20 2020 2020 2020  .float().       
-00005620: 2069 6e76 5f64 6973 7020 3d20 2d20 7365   inv_disp = - se
-00005630: 6c66 2e74 6f5f 4444 4628 2a73 697a 6529  lf.to_DDF(*size)
-00005640: 2e63 6c6f 6e65 2829 2e64 6574 6163 6828  .clone().detach(
-00005650: 290a 2020 2020 2020 2020 696e 765f 6469  ).        inv_di
-00005660: 7370 2e72 6571 7569 7265 735f 6772 6164  sp.requires_grad
-00005670: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00005680: 6f70 7469 6d69 7a65 7220 3d20 6274 2e43  optimizer = bt.C
-00005690: 4144 414d 285b 696e 765f 6469 7370 5d2c  ADAM([inv_disp],
-000056a0: 206c 7220 3d20 3165 2d32 290a 2020 2020   lr = 1e-2).    
-000056b0: 2020 2020 7072 6576 5f6c 6f73 7320 3d20      prev_loss = 
-000056c0: 4e6f 6e65 0a20 2020 2020 2020 2066 6f72  None.        for
-000056d0: 2069 2069 6e20 7261 6e67 6528 3430 3029   i in range(400)
-000056e0: 3a0a 2020 2020 2020 2020 2020 2020 6974  :.            it
-000056f0: 7261 6e73 203d 2044 656e 7365 4469 7370  rans = DenseDisp
-00005700: 6c61 6365 6d65 6e74 4669 656c 6428 696e  lacementField(in
-00005710: 765f 6469 7370 290a 2020 2020 2020 2020  v_disp).        
-00005720: 2020 2020 6c6f 7373 203d 2028 6974 7261      loss = (itra
-00005730: 6e73 2873 656c 6628 5829 2920 2d20 5829  ns(self(X)) - X)
-00005740: 2e6e 6f72 6d32 2829 2e6d 6561 6e28 2920  .norm2().mean() 
-00005750: 2b20 3165 2d31 202a 2062 656e 6469 6e67  + 1e-1 * bending
-00005760: 2869 6e76 5f64 6973 7029 0a20 2020 2020  (inv_disp).     
-00005770: 2020 2020 2020 206f 7074 696d 697a 6572         optimizer
-00005780: 2e6d 696e 696d 697a 6528 6c6f 7373 292e  .minimize(loss).
-00005790: 7374 6570 2829 0a20 2020 2020 2020 2020  step().         
-000057a0: 2020 2069 6620 7665 7262 6f73 653a 2070     if verbose: p
-000057b0: 7269 6e74 2866 2269 7465 7261 7469 6f6e  rint(f"iteration
-000057c0: 207b 692b 317d 3a20 6c6f 7373 203d 207b   {i+1}: loss = {
-000057d0: 6c6f 7373 2e69 7465 6d28 297d 2229 0a20  loss.item()}"). 
-000057e0: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
-000057f0: 6576 5f6c 6f73 7320 6973 206e 6f74 204e  ev_loss is not N
-00005800: 6f6e 6520 616e 6420 6c6f 7373 2e69 7465  one and loss.ite
-00005810: 6d28 2920 3e3d 2070 7265 765f 6c6f 7373  m() >= prev_loss
-00005820: 3a20 6e6f 6472 6f70 5f63 6f75 6e74 202b  : nodrop_count +
-00005830: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00005840: 656c 7365 3a20 6e6f 6472 6f70 5f63 6f75  else: nodrop_cou
-00005850: 6e74 203d 2030 0a20 2020 2020 2020 2020  nt = 0.         
-00005860: 2020 2069 6620 6e6f 6472 6f70 5f63 6f75     if nodrop_cou
-00005870: 6e74 203e 3d20 363a 0a20 2020 2020 2020  nt >= 6:.       
-00005880: 2020 2020 2020 2020 2069 6620 7665 7262           if verb
-00005890: 6f73 653a 2070 7269 6e74 2866 2253 746f  ose: print(f"Sto
-000058a0: 7020 6174 2069 7465 7261 7469 6f6e 207b  p at iteration {
-000058b0: 692b 317d 2064 7565 2074 6f20 6e6f 2064  i+1} due to no d
-000058c0: 726f 7070 696e 672e 2022 290a 2020 2020  ropping. ").    
-000058d0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000058e0: 6b0a 2020 2020 2020 2020 2020 2020 6966  k.            if
-000058f0: 206c 6f73 732e 6974 656d 2829 203c 2031   loss.item() < 1
-00005900: 652d 333a 0a20 2020 2020 2020 2020 2020  e-3:.           
-00005910: 2020 2020 2069 6620 7665 7262 6f73 653a       if verbose:
-00005920: 2070 7269 6e74 2866 2253 746f 7020 6174   print(f"Stop at
-00005930: 2069 7465 7261 7469 6f6e 207b 692b 317d   iteration {i+1}
-00005940: 2064 7565 2074 6f20 736d 616c 6c20 6c6f   due to small lo
-00005950: 7373 2e20 2229 0a20 2020 2020 2020 2020  ss. ").         
-00005960: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00005970: 2020 2020 2072 6574 7572 6e20 4465 6e73       return Dens
-00005980: 6544 6973 706c 6163 656d 656e 7446 6965  eDisplacementFie
-00005990: 6c64 2869 6e76 5f64 6973 7029 0a20 2020  ld(inv_disp).   
-000059a0: 200a 2020 2020 6465 6620 666f 7263 655f   .    def force_
-000059b0: 696e 7628 7365 6c66 2c20 2a73 697a 6529  inv(self, *size)
-000059c0: 3a0a 2020 2020 2020 2020 6966 2068 6173  :.        if has
-000059d0: 6174 7472 2873 656c 662c 2027 696e 7627  attr(self, 'inv'
-000059e0: 293a 2072 6574 7572 6e20 7365 6c66 2e69  ): return self.i
-000059f0: 6e76 2829 0a20 2020 2020 2020 2065 6c73  nv().        els
-00005a00: 653a 2072 6574 7572 6e20 7365 6c66 2e6e  e: return self.n
-00005a10: 756d 5f69 6e76 282a 7369 7a65 290a 0a40  um_inv(*size)..@
-00005a20: 616c 6961 7328 2249 6422 290a 636c 6173  alias("Id").clas
-00005a30: 7320 4964 656e 7469 7479 2853 7061 7469  s Identity(Spati
-00005a40: 616c 5472 616e 7366 6f72 6d61 7469 6f6e  alTransformation
-00005a50: 293a 0a0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-00005a60: 6974 5f5f 2873 656c 6629 3a0a 2020 2020  it__(self):.    
-00005a70: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00005a80: 4964 656e 7469 7479 2074 7261 6e73 666f  Identity transfo
-00005a90: 726d 6174 696f 6e2e 0a20 2020 2020 2020  rmation..       
-00005aa0: 2020 2020 200a 2020 2020 2020 2020 5768       .        Wh
-00005ab0: 656e 2069 7420 6973 2063 616c 6c65 643a  en it is called:
-00005ac0: 0a20 2020 2020 2020 2020 2020 2058 205b  .            X [
-00005ad0: 6274 2e54 656e 736f 725d 3a20 436f 6f72  bt.Tensor]: Coor
-00005ae0: 6469 6e61 7465 7320 746f 2062 6520 7472  dinates to be tr
-00005af0: 616e 7366 6f72 6d65 642e 0a20 2020 2020  ansformed..     
-00005b00: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-00005b10: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
-00005b20: 6e61 6c5d 2c20 7b6e 5f64 696d 7d2c 206e  nal], {n_dim}, n
-00005b30: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
-00005b40: 7229 0a20 2020 2020 2020 2020 2020 206f  r).            o
-00005b50: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
-00005b60: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
-00005b70: 6564 2063 6f6f 7264 696e 6174 6573 2e20  ed coordinates. 
-00005b80: 2853 616d 6520 6173 2058 2066 6f72 2049  (Same as X for I
-00005b90: 6465 6e74 6974 7929 0a20 2020 2020 2020  dentity).       
-00005ba0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-00005bb0: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-00005bc0: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
-00005bd0: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
-00005be0: 2727 270a 2020 2020 2020 2020 7375 7065  '''.        supe
-00005bf0: 7228 292e 5f5f 696e 6974 5f5f 2829 0a20  r().__init__(). 
-00005c00: 2020 2020 2020 200a 2020 2020 6465 6620         .    def 
-00005c10: 6166 6669 6e65 2873 656c 662c 206e 5f64  affine(self, n_d
-00005c20: 696d 3d4e 6f6e 6529 3a0a 2020 2020 2020  im=None):.      
-00005c30: 2020 6966 206e 5f64 696d 2069 7320 4e6f    if n_dim is No
-00005c40: 6e65 3a20 7265 7475 726e 0a20 2020 2020  ne: return.     
-00005c50: 2020 2072 6574 7572 6e20 6274 2e65 7965     return bt.eye
-00005c60: 286e 5f64 696d 202b 2031 292e 756e 7371  (n_dim + 1).unsq
-00005c70: 7565 657a 6528 5b5d 290a 0a20 2020 2064  ueeze([])..    d
-00005c80: 6566 2069 6e76 2873 656c 6629 3a20 7265  ef inv(self): re
-00005c90: 7475 726e 2049 6465 6e74 6974 7928 292e  turn Identity().
-00005ca0: 6261 636b 7761 7264 5f28 7365 6c66 2e62  backward_(self.b
-00005cb0: 6163 6b77 6172 6429 0a0a 636c 6173 7320  ackward)..class 
-00005cc0: 526f 7461 7469 6f6e 3930 2853 7061 7469  Rotation90(Spati
-00005cd0: 616c 5472 616e 7366 6f72 6d61 7469 6f6e  alTransformation
-00005ce0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00005cf0: 745f 5f28 7365 6c66 2c20 6469 6d31 2c20  t__(self, dim1, 
-00005d00: 6469 6d32 2c20 696d 6167 655f 7369 7a65  dim2, image_size
-00005d10: 3d4e 6f6e 652c 2072 6573 697a 655f 696d  =None, resize_im
-00005d20: 6167 653d 5472 7565 293a 0a20 2020 2020  age=True):.     
-00005d30: 2020 2027 2727 0a20 2020 2020 2020 2054     '''.        T
-00005d40: 7261 6e73 666f 726d 6174 696f 6e20 7468  ransformation th
-00005d50: 6174 2072 6f74 6174 6573 2061 6e20 696d  at rotates an im
-00005d60: 6167 6520 6f66 2060 696d 6167 655f 7369  age of `image_si
-00005d70: 7a65 6020 6279 2039 3020 6465 6772 6565  ze` by 90 degree
-00005d80: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00005d90: 2020 2020 4e6f 7465 3a20 5468 6520 726f      Note: The ro
-00005da0: 7461 7469 6f6e 2069 7320 666f 7220 636f  tation is for co
-00005db0: 6f72 6469 6e61 7465 732c 2068 656e 6365  ordinates, hence
-00005dc0: 2074 6865 2069 6d61 6765 2072 6f74 6174   the image rotat
-00005dd0: 6573 2063 6c6f 636b 7769 7365 2e20 0a20  es clockwise. . 
-00005de0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00005df0: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
-00005e00: 2020 2020 6469 6d31 2c20 6469 6d32 205b      dim1, dim2 [
-00005e10: 696e 745d 3a20 5468 6520 706c 616e 6520  int]: The plane 
-00005e20: 7765 2072 6f74 6174 6520 6f6e 2e20 4469  we rotate on. Di
-00005e30: 7265 6374 696f 6e20 6f66 2074 6865 2072  rection of the r
-00005e40: 6f74 6174 696f 6e20 6973 2066 726f 6d20  otation is from 
-00005e50: 6064 696d 3160 2074 6f20 6064 696d 3260  `dim1` to `dim2`
-00005e60: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005e70: 2020 692e 652e 2063 6f75 6e74 6572 2d63    i.e. counter-c
-00005e80: 6c6f 636b 7769 7365 2072 6f74 6174 696f  lockwise rotatio
-00005e90: 6e20 7769 7468 2064 696d 3120 6173 2078  n with dim1 as x
-00005ea0: 2d61 7869 7320 616e 6420 6469 6d32 2061  -axis and dim2 a
-00005eb0: 7320 792d 6178 6973 3a20 5b64 696d 312c  s y-axis: [dim1,
-00005ec0: 2064 696d 325d 2063 6f6f 7264 696e 6174   dim2] coordinat
-00005ed0: 6573 2028 782c 2079 2920 6265 636f 6d65  es (x, y) become
-00005ee0: 7320 2879 6d61 782d 792c 2078 292e 0a20  s (ymax-y, x).. 
-00005ef0: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-00005f00: 5f73 697a 6520 5b74 7570 6c65 206f 7220  _size [tuple or 
-00005f10: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
-00005f20: 7369 7a65 206f 6620 7468 6520 696d 6167  size of the imag
-00005f30: 652c 206f 7220 7468 6520 696d 6167 6520  e, or the image 
-00005f40: 6974 7365 6c66 2e20 0a20 2020 2020 2020  itself. .       
-00005f50: 2020 2020 200a 2020 2020 2020 2020 5768       .        Wh
-00005f60: 656e 2069 7420 6973 2063 616c 6c65 643a  en it is called:
-00005f70: 0a20 2020 2020 2020 2020 2020 2058 205b  .            X [
-00005f80: 6274 2e54 656e 736f 725d 3a20 436f 6f72  bt.Tensor]: Coor
-00005f90: 6469 6e61 7465 7320 746f 2062 6520 7472  dinates to be tr
-00005fa0: 616e 7366 6f72 6d65 642e 0a20 2020 2020  ansformed..     
-00005fb0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-00005fc0: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
-00005fd0: 6e61 6c5d 2c20 7b6e 5f64 696d 7d2c 206e  nal], {n_dim}, n
-00005fe0: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
-00005ff0: 7229 0a20 2020 2020 2020 2020 2020 206f  r).            o
-00006000: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
-00006010: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
-00006020: 6564 2063 6f6f 7264 696e 6174 6573 2e0a  ed coordinates..
-00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
-00006050: 2c20 7b6e 5f64 696d 7d2c 206e 5f31 2c20  , {n_dim}, n_1, 
-00006060: 6e5f 322c 202e 2e2e 2c20 6e5f 7229 0a20  n_2, ..., n_r). 
-00006070: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00006080: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00006090: 745f 5f28 6469 6d31 3d64 696d 312c 2064  t__(dim1=dim1, d
-000060a0: 696d 323d 6469 6d32 2c20 696d 6167 655f  im2=dim2, image_
-000060b0: 7369 7a65 3d69 6d61 6765 5f73 697a 652c  size=image_size,
-000060c0: 2072 6573 697a 655f 696d 6167 653d 7265   resize_image=re
-000060d0: 7369 7a65 5f69 6d61 6765 290a 0a20 2020  size_image)..   
-000060e0: 2020 2020 2073 656c 662e 6469 6d31 2c20       self.dim1, 
-000060f0: 7365 6c66 2e64 696d 3220 3d20 6469 6d31  self.dim2 = dim1
-00006100: 2c20 6469 6d32 0a20 2020 2020 2020 2069  , dim2.        i
-00006110: 6620 6973 696e 7374 616e 6365 2869 6d61  f isinstance(ima
-00006120: 6765 5f73 697a 652c 2062 742e 746f 7263  ge_size, bt.torc
-00006130: 682e 5465 6e73 6f72 293a 2069 6d61 6765  h.Tensor): image
-00006140: 5f73 697a 6520 3d20 696d 6167 655f 7369  _size = image_si
-00006150: 7a65 2e73 6861 7065 0a20 2020 2020 2020  ze.shape.       
-00006160: 2073 656c 662e 696d 6167 655f 7369 7a65   self.image_size
-00006170: 203d 2069 6d61 6765 5f73 697a 650a 2020   = image_size.  
-00006180: 2020 2020 2020 6966 2069 6d61 6765 5f73        if image_s
-00006190: 697a 6520 6973 206e 6f74 204e 6f6e 653a  ize is not None:
-000061a0: 2073 656c 662e 6e5f 6469 6d20 3d20 6c65   self.n_dim = le
-000061b0: 6e28 696d 6167 655f 7369 7a65 290a 2020  n(image_size).  
-000061c0: 2020 2020 2020 6966 2072 6573 697a 655f        if resize_
-000061d0: 696d 6167 653a 2073 656c 662e 7265 7368  image: self.resh
-000061e0: 6170 6520 3d20 5b28 312c 292c 2028 6469  ape = [(1,), (di
-000061f0: 6d31 2c20 6469 6d32 295d 0a0a 2020 2020  m1, dim2)]..    
-00006200: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-00006210: 662c 2058 293a 0a20 2020 2020 2020 2058  f, X):.        X
-00006220: 203d 2073 7570 6572 2829 2e5f 5f63 616c   = super().__cal
-00006230: 6c5f 5f28 5829 0a20 2020 2020 2020 2064  l__(X).        d
-00006240: 696d 312c 2064 696d 3220 3d20 7365 6c66  im1, dim2 = self
-00006250: 2e64 696d 312c 2073 656c 662e 6469 6d32  .dim1, self.dim2
-00006260: 0a20 2020 2020 2020 2073 656c 6563 7431  .        select1
-00006270: 203d 2028 736c 6963 6528 4e6f 6e65 292c   = (slice(None),
-00006280: 2920 2a20 582e 6368 616e 6e65 6c5f 6469  ) * X.channel_di
-00006290: 6d20 2b20 2864 696d 312c 290a 2020 2020  m + (dim1,).    
-000062a0: 2020 2020 7365 6c65 6374 3220 3d20 2873      select2 = (s
-000062b0: 6c69 6365 284e 6f6e 6529 2c29 202a 2058  lice(None),) * X
-000062c0: 2e63 6861 6e6e 656c 5f64 696d 202b 2028  .channel_dim + (
-000062d0: 6469 6d32 2c29 0a20 2020 2020 2020 2069  dim2,).        i
-000062e0: 6620 7365 6c66 2e69 6d61 6765 5f73 697a  f self.image_siz
-000062f0: 6520 6973 204e 6f6e 653a 206d 6178 5f72  e is None: max_r
-00006300: 616e 6765 203d 2058 5b73 656c 6563 7432  ange = X[select2
-00006310: 5d2e 6d61 7828 290a 2020 2020 2020 2020  ].max().        
-00006320: 656c 7365 3a20 6d61 785f 7261 6e67 6520  else: max_range 
-00006330: 3d20 7365 6c66 2e69 6d61 6765 5f73 697a  = self.image_siz
-00006340: 655b 6469 6d32 5d0a 2020 2020 2020 2020  e[dim2].        
-00006350: 585b 7365 6c65 6374 315d 203d 2058 5b73  X[select1] = X[s
-00006360: 656c 6563 7431 5d20 2b20 6d61 785f 7261  elect1] + max_ra
-00006370: 6e67 6520 2d20 585b 7365 6c65 6374 325d  nge - X[select2]
-00006380: 0a20 2020 2020 2020 2058 5b73 656c 6563  .        X[selec
-00006390: 7432 5d20 3d20 585b 7365 6c65 6374 315d  t2] = X[select1]
-000063a0: 202b 2058 5b73 656c 6563 7432 5d20 2d20   + X[select2] - 
-000063b0: 6d61 785f 7261 6e67 650a 2020 2020 2020  max_range.      
-000063c0: 2020 585b 7365 6c65 6374 315d 203d 2058    X[select1] = X
-000063d0: 5b73 656c 6563 7431 5d20 2d20 585b 7365  [select1] - X[se
-000063e0: 6c65 6374 325d 0a20 2020 2020 2020 2072  lect2].        r
-000063f0: 6574 7572 6e20 580a 2020 2020 2020 2020  eturn X.        
-00006400: 0a20 2020 2064 6566 2061 6666 696e 6528  .    def affine(
-00006410: 7365 6c66 2c20 6e5f 6469 6d3d 4e6f 6e65  self, n_dim=None
-00006420: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00006430: 6c66 2e69 6d61 6765 5f73 697a 6520 6973  lf.image_size is
-00006440: 204e 6f6e 653a 2072 6574 7572 6e0a 2020   None: return.  
-00006450: 2020 2020 2020 6966 206e 5f64 696d 2069        if n_dim i
-00006460: 7320 4e6f 6e65 2061 6e64 2073 656c 662e  s None and self.
-00006470: 6e5f 6469 6d20 6973 204e 6f6e 653a 2072  n_dim is None: r
-00006480: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00006490: 206e 5f64 696d 2069 7320 4e6f 6e65 3a20   n_dim is None: 
-000064a0: 6e5f 6469 6d20 3d20 7365 6c66 2e6e 5f64  n_dim = self.n_d
-000064b0: 696d 0a20 2020 2020 2020 2061 766f 7563  im.        avouc
-000064c0: 6828 7365 6c66 2e6e 5f64 696d 2069 7320  h(self.n_dim is 
-000064d0: 4e6f 6e65 206f 7220 7365 6c66 2e6e 5f64  None or self.n_d
-000064e0: 696d 203d 3d20 6e5f 6469 6d29 0a20 2020  im == n_dim).   
-000064f0: 2020 2020 2064 696d 312c 2064 696d 3220       dim1, dim2 
-00006500: 3d20 7365 6c66 2e64 696d 312c 2073 656c  = self.dim1, sel
-00006510: 662e 6469 6d32 0a20 2020 2020 2020 2061  f.dim2.        a
-00006520: 6666 203d 2062 742e 6579 6528 6e5f 6469  ff = bt.eye(n_di
-00006530: 6d20 2b20 3129 0a20 2020 2020 2020 2061  m + 1).        a
-00006540: 6666 5b64 696d 315d 5b64 696d 315d 203d  ff[dim1][dim1] =
-00006550: 2030 2e0a 2020 2020 2020 2020 6166 665b   0..        aff[
-00006560: 6469 6d31 5d5b 6469 6d32 5d20 3d20 2d31  dim1][dim2] = -1
-00006570: 2e0a 2020 2020 2020 2020 6166 665b 6469  ..        aff[di
-00006580: 6d31 5d5b 2d31 5d20 3d20 666c 6f61 7428  m1][-1] = float(
-00006590: 7365 6c66 2e69 6d61 6765 5f73 697a 655b  self.image_size[
-000065a0: 6469 6d32 5d29 0a20 2020 2020 2020 2061  dim2]).        a
-000065b0: 6666 5b64 696d 325d 5b64 696d 325d 203d  ff[dim2][dim2] =
-000065c0: 2030 2e0a 2020 2020 2020 2020 6166 665b   0..        aff[
-000065d0: 6469 6d32 5d5b 6469 6d31 5d20 3d20 312e  dim2][dim1] = 1.
-000065e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000065f0: 6166 662e 756e 7371 7565 657a 6528 5b5d  aff.unsqueeze([]
-00006600: 290a 2020 2020 0a20 2020 2064 6566 2069  ).    .    def i
-00006610: 6e76 2873 656c 6629 3a20 7265 7475 726e  nv(self): return
-00006620: 2052 6f74 6174 696f 6e32 3730 2873 656c   Rotation270(sel
-00006630: 662e 6469 6d31 2c20 7365 6c66 2e64 696d  f.dim1, self.dim
-00006640: 322c 2069 6d61 6765 5f73 697a 6520 3d20  2, image_size = 
-00006650: 7365 6c66 2e69 6d61 6765 5f73 697a 652c  self.image_size,
-00006660: 2072 6573 697a 655f 696d 6167 6520 3d20   resize_image = 
-00006670: 7365 6c66 2e72 6573 697a 655f 696d 6167  self.resize_imag
-00006680: 6529 2e62 6163 6b77 6172 645f 2873 656c  e).backward_(sel
-00006690: 662e 6261 636b 7761 7264 290a 0a63 6c61  f.backward)..cla
-000066a0: 7373 2052 6f74 6174 696f 6e32 3730 2853  ss Rotation270(S
-000066b0: 7061 7469 616c 5472 616e 7366 6f72 6d61  patialTransforma
-000066c0: 7469 6f6e 293a 0a20 2020 2064 6566 205f  tion):.    def _
-000066d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6469  _init__(self, di
-000066e0: 6d31 2c20 6469 6d32 2c20 696d 6167 655f  m1, dim2, image_
-000066f0: 7369 7a65 3d4e 6f6e 652c 2072 6573 697a  size=None, resiz
-00006700: 655f 696d 6167 653d 5472 7565 293a 0a20  e_image=True):. 
-00006710: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00006720: 2020 2054 7261 6e73 666f 726d 6174 696f     Transformatio
-00006730: 6e20 7468 6174 2072 6f74 6174 6573 2061  n that rotates a
-00006740: 6e20 696d 6167 6520 6279 2032 3730 2064  n image by 270 d
-00006750: 6567 7265 6573 2e0a 2020 2020 2020 2020  egrees..        
-00006760: 0a20 2020 2020 2020 204e 6f74 653a 2054  .        Note: T
-00006770: 6865 2072 6f74 6174 696f 6e20 6973 2066  he rotation is f
-00006780: 6f72 2063 6f6f 7264 696e 6174 6573 2c20  or coordinates, 
-00006790: 6865 6e63 6520 7468 6520 696d 6167 6520  hence the image 
-000067a0: 726f 7461 7465 7320 636c 6f63 6b77 6973  rotates clockwis
-000067b0: 652e 200a 2020 2020 2020 2020 0a20 2020  e. .        .   
-000067c0: 2020 2020 2050 6172 616d 733a 0a20 2020       Params:.   
-000067d0: 2020 2020 2020 2020 2064 696d 312c 2064           dim1, d
-000067e0: 696d 3220 5b69 6e74 5d3a 2054 6865 2070  im2 [int]: The p
-000067f0: 6c61 6e65 2077 6520 726f 7461 7465 206f  lane we rotate o
-00006800: 6e2e 2044 6972 6563 7469 6f6e 206f 6620  n. Direction of 
-00006810: 7468 6520 726f 7461 7469 6f6e 2069 7320  the rotation is 
-00006820: 6672 6f6d 2060 6469 6d31 6020 746f 2060  from `dim1` to `
-00006830: 6469 6d32 602e 0a20 2020 2020 2020 2020  dim2`..         
-00006840: 2020 2020 2020 2069 2e65 2e20 636f 756e         i.e. coun
-00006850: 7465 722d 636c 6f63 6b77 6973 6520 726f  ter-clockwise ro
-00006860: 7461 7469 6f6e 2077 6974 6820 6469 6d31  tation with dim1
-00006870: 2061 7320 782d 6178 6973 2061 6e64 2064   as x-axis and d
-00006880: 696d 3220 6173 2079 2d61 7869 733a 205b  im2 as y-axis: [
-00006890: 6469 6d31 2c20 6469 6d32 5d20 636f 6f72  dim1, dim2] coor
-000068a0: 6469 6e61 7465 7320 2878 2c20 7929 2062  dinates (x, y) b
-000068b0: 6563 6f6d 6573 2028 792c 2078 6d61 782d  ecomes (y, xmax-
-000068c0: 7829 2e0a 2020 2020 2020 2020 2020 2020  x)..            
-000068d0: 696d 6167 655f 7369 7a65 205b 7475 706c  image_size [tupl
-000068e0: 6520 6f72 2062 742e 5465 6e73 6f72 5d3a  e or bt.Tensor]:
-000068f0: 2054 6865 2073 697a 6520 6f66 2074 6865   The size of the
-00006900: 2069 6d61 6765 2c20 6f72 2074 6865 2069   image, or the i
-00006910: 6d61 6765 2069 7473 656c 662e 200a 2020  mage itself. .  
-00006920: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00006930: 2020 2057 6865 6e20 6974 2069 7320 6361     When it is ca
-00006940: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
-00006950: 2020 5820 5b62 742e 5465 6e73 6f72 5d3a    X [bt.Tensor]:
-00006960: 2043 6f6f 7264 696e 6174 6573 2074 6f20   Coordinates to 
-00006970: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
-00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006990: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
-000069a0: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
-000069b0: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
-000069c0: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
-000069d0: 2020 2020 6f75 7470 7574 205b 6274 2e54      output [bt.T
-000069e0: 656e 736f 725d 3a20 5468 6520 7472 616e  ensor]: The tran
-000069f0: 7366 6f72 6d65 6420 636f 6f72 6469 6e61  sformed coordina
-00006a00: 7465 732e 0a20 2020 2020 2020 2020 2020  tes..           
-00006a10: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
-00006a20: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
-00006a30: 6e5f 312c 206e 5f32 2c20 2e2e 2e2c 206e  n_1, n_2, ..., n
-00006a40: 5f72 290a 2020 2020 2020 2020 2727 270a  _r).        '''.
-00006a50: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00006a60: 5f5f 696e 6974 5f5f 2864 696d 313d 6469  __init__(dim1=di
-00006a70: 6d31 2c20 6469 6d32 3d64 696d 322c 2069  m1, dim2=dim2, i
-00006a80: 6d61 6765 5f73 697a 653d 696d 6167 655f  mage_size=image_
-00006a90: 7369 7a65 2c20 7265 7369 7a65 5f69 6d61  size, resize_ima
-00006aa0: 6765 3d72 6573 697a 655f 696d 6167 6529  ge=resize_image)
-00006ab0: 0a0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
-00006ac0: 696d 312c 2073 656c 662e 6469 6d32 203d  im1, self.dim2 =
-00006ad0: 2064 696d 312c 2064 696d 320a 2020 2020   dim1, dim2.    
-00006ae0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00006af0: 6528 696d 6167 655f 7369 7a65 2c20 6274  e(image_size, bt
-00006b00: 2e74 6f72 6368 2e54 656e 736f 7229 3a20  .torch.Tensor): 
-00006b10: 696d 6167 655f 7369 7a65 203d 2069 6d61  image_size = ima
-00006b20: 6765 5f73 697a 652e 7368 6170 650a 2020  ge_size.shape.  
-00006b30: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
-00006b40: 5f73 697a 6520 3d20 696d 6167 655f 7369  _size = image_si
-00006b50: 7a65 0a20 2020 2020 2020 2069 6620 696d  ze.        if im
-00006b60: 6167 655f 7369 7a65 2069 7320 6e6f 7420  age_size is not 
-00006b70: 4e6f 6e65 3a20 7365 6c66 2e6e 5f64 696d  None: self.n_dim
-00006b80: 203d 206c 656e 2869 6d61 6765 5f73 697a   = len(image_siz
-00006b90: 6529 0a20 2020 2020 2020 2069 6620 7265  e).        if re
-00006ba0: 7369 7a65 5f69 6d61 6765 3a20 7365 6c66  size_image: self
-00006bb0: 2e72 6573 6861 7065 203d 205b 2831 2c29  .reshape = [(1,)
-00006bc0: 2c20 2864 696d 312c 2064 696d 3229 5d0a  , (dim1, dim2)].
-00006bd0: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
-00006be0: 5f28 7365 6c66 2c20 5829 3a0a 2020 2020  _(self, X):.    
-00006bf0: 2020 2020 5820 3d20 7375 7065 7228 292e      X = super().
-00006c00: 5f5f 6361 6c6c 5f5f 2858 290a 2020 2020  __call__(X).    
-00006c10: 2020 2020 6469 6d31 2c20 6469 6d32 203d      dim1, dim2 =
-00006c20: 2073 656c 662e 6469 6d31 2c20 7365 6c66   self.dim1, self
-00006c30: 2e64 696d 320a 2020 2020 2020 2020 7365  .dim2.        se
-00006c40: 6c65 6374 3120 3d20 2873 6c69 6365 284e  lect1 = (slice(N
-00006c50: 6f6e 6529 2c29 202a 2058 2e63 6861 6e6e  one),) * X.chann
-00006c60: 656c 5f64 696d 202b 2028 6469 6d31 2c29  el_dim + (dim1,)
-00006c70: 0a20 2020 2020 2020 2073 656c 6563 7432  .        select2
-00006c80: 203d 2028 736c 6963 6528 4e6f 6e65 292c   = (slice(None),
-00006c90: 2920 2a20 582e 6368 616e 6e65 6c5f 6469  ) * X.channel_di
-00006ca0: 6d20 2b20 2864 696d 322c 290a 2020 2020  m + (dim2,).    
-00006cb0: 2020 2020 6966 2073 656c 662e 696d 6167      if self.imag
-00006cc0: 655f 7369 7a65 2069 7320 4e6f 6e65 3a20  e_size is None: 
-00006cd0: 6d61 785f 7261 6e67 6520 3d20 585b 7365  max_range = X[se
-00006ce0: 6c65 6374 315d 2e6d 6178 2829 0a20 2020  lect1].max().   
-00006cf0: 2020 2020 2065 6c73 653a 206d 6178 5f72       else: max_r
-00006d00: 616e 6765 203d 2073 656c 662e 696d 6167  ange = self.imag
-00006d10: 655f 7369 7a65 5b64 696d 315d 0a20 2020  e_size[dim1].   
-00006d20: 2020 2020 2058 5b73 656c 6563 7432 5d20       X[select2] 
-00006d30: 3d20 585b 7365 6c65 6374 325d 202b 206d  = X[select2] + m
-00006d40: 6178 5f72 616e 6765 202d 2058 5b73 656c  ax_range - X[sel
-00006d50: 6563 7431 5d0a 2020 2020 2020 2020 585b  ect1].        X[
-00006d60: 7365 6c65 6374 315d 203d 2058 5b73 656c  select1] = X[sel
-00006d70: 6563 7432 5d20 2b20 585b 7365 6c65 6374  ect2] + X[select
-00006d80: 315d 202d 206d 6178 5f72 616e 6765 0a20  1] - max_range. 
-00006d90: 2020 2020 2020 2058 5b73 656c 6563 7432         X[select2
-00006da0: 5d20 3d20 585b 7365 6c65 6374 325d 202d  ] = X[select2] -
-00006db0: 2058 5b73 656c 6563 7431 5d0a 2020 2020   X[select1].    
-00006dc0: 2020 2020 7265 7475 726e 2058 0a20 2020      return X.   
-00006dd0: 2020 2020 200a 2020 2020 6465 6620 6166       .    def af
-00006de0: 6669 6e65 2873 656c 662c 206e 5f64 696d  fine(self, n_dim
-00006df0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00006e00: 6966 2073 656c 662e 696d 6167 655f 7369  if self.image_si
-00006e10: 7a65 2069 7320 4e6f 6e65 3a20 7265 7475  ze is None: retu
-00006e20: 726e 0a20 2020 2020 2020 2069 6620 6e5f  rn.        if n_
-00006e30: 6469 6d20 6973 204e 6f6e 6520 616e 6420  dim is None and 
-00006e40: 7365 6c66 2e6e 5f64 696d 2069 7320 4e6f  self.n_dim is No
-00006e50: 6e65 3a20 7265 7475 726e 0a20 2020 2020  ne: return.     
-00006e60: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
-00006e70: 6f6e 653a 206e 5f64 696d 203d 2073 656c  one: n_dim = sel
-00006e80: 662e 6e5f 6469 6d0a 2020 2020 2020 2020  f.n_dim.        
-00006e90: 6176 6f75 6368 2873 656c 662e 6e5f 6469  avouch(self.n_di
-00006ea0: 6d20 6973 204e 6f6e 6520 6f72 2073 656c  m is None or sel
-00006eb0: 662e 6e5f 6469 6d20 3d3d 206e 5f64 696d  f.n_dim == n_dim
-00006ec0: 290a 2020 2020 2020 2020 6469 6d31 2c20  ).        dim1, 
-00006ed0: 6469 6d32 203d 2073 656c 662e 6469 6d31  dim2 = self.dim1
-00006ee0: 2c20 7365 6c66 2e64 696d 320a 2020 2020  , self.dim2.    
-00006ef0: 2020 2020 6166 6620 3d20 6274 2e65 7965      aff = bt.eye
-00006f00: 286e 5f64 696d 202b 2031 290a 2020 2020  (n_dim + 1).    
-00006f10: 2020 2020 6166 665b 6469 6d31 5d5b 6469      aff[dim1][di
-00006f20: 6d31 5d20 3d20 302e 0a20 2020 2020 2020  m1] = 0..       
-00006f30: 2061 6666 5b64 696d 315d 5b64 696d 325d   aff[dim1][dim2]
-00006f40: 203d 2031 2e0a 2020 2020 2020 2020 6166   = 1..        af
-00006f50: 665b 6469 6d32 5d5b 6469 6d32 5d20 3d20  f[dim2][dim2] = 
-00006f60: 302e 0a20 2020 2020 2020 2061 6666 5b64  0..        aff[d
-00006f70: 696d 325d 5b64 696d 315d 203d 202d 312e  im2][dim1] = -1.
-00006f80: 0a20 2020 2020 2020 2061 6666 5b64 696d  .        aff[dim
-00006f90: 325d 5b2d 315d 203d 2066 6c6f 6174 2873  2][-1] = float(s
-00006fa0: 656c 662e 696d 6167 655f 7369 7a65 5b64  elf.image_size[d
-00006fb0: 696d 315d 290a 2020 2020 2020 2020 7265  im1]).        re
-00006fc0: 7475 726e 2061 6666 2e75 6e73 7175 6565  turn aff.unsquee
-00006fd0: 7a65 285b 5d29 0a20 2020 200a 2020 2020  ze([]).    .    
-00006fe0: 6465 6620 696e 7628 7365 6c66 293a 2072  def inv(self): r
-00006ff0: 6574 7572 6e20 526f 7461 7469 6f6e 3930  eturn Rotation90
-00007000: 2873 656c 662e 6469 6d31 2c20 7365 6c66  (self.dim1, self
-00007010: 2e64 696d 322c 2069 6d61 6765 5f73 697a  .dim2, image_siz
-00007020: 6520 3d20 7365 6c66 2e69 6d61 6765 5f73  e = self.image_s
-00007030: 697a 652c 2072 6573 697a 655f 696d 6167  ize, resize_imag
-00007040: 6520 3d20 7365 6c66 2e72 6573 697a 655f  e = self.resize_
-00007050: 696d 6167 6529 2e62 6163 6b77 6172 645f  image).backward_
-00007060: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
-00007070: 0a63 6c61 7373 2052 6f74 6174 696f 6e31  .class Rotation1
-00007080: 3830 2853 7061 7469 616c 5472 616e 7366  80(SpatialTransf
-00007090: 6f72 6d61 7469 6f6e 293a 0a20 2020 2064  ormation):.    d
-000070a0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000070b0: 2c20 6469 6d31 2c20 6469 6d32 2c20 696d  , dim1, dim2, im
-000070c0: 6167 655f 7369 7a65 3d4e 6f6e 6529 3a0a  age_size=None):.
-000070d0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000070e0: 2020 2020 5472 616e 7366 6f72 6d61 7469      Transformati
-000070f0: 6f6e 2074 6861 7420 726f 7461 7465 7320  on that rotates 
-00007100: 616e 2069 6d61 6765 2062 7920 3138 3020  an image by 180 
-00007110: 6465 6772 6565 732e 0a20 2020 2020 2020  degrees..       
-00007120: 200a 2020 2020 2020 2020 5061 7261 6d73   .        Params
-00007130: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
-00007140: 6d31 2c20 6469 6d32 205b 696e 745d 3a20  m1, dim2 [int]: 
-00007150: 5468 6520 706c 616e 6520 7765 2072 6f74  The plane we rot
-00007160: 6174 6520 6f6e 2e20 4469 7265 6374 696f  ate on. Directio
-00007170: 6e20 6f66 2074 6865 2072 6f74 6174 696f  n of the rotatio
-00007180: 6e20 6973 2066 726f 6d20 6064 696d 3160  n is from `dim1`
-00007190: 2074 6f20 6064 696d 3260 2e0a 2020 2020   to `dim2`..    
-000071a0: 2020 2020 2020 2020 2020 2020 692e 652e              i.e.
-000071b0: 2072 6f74 6174 696f 6e20 7769 7468 2064   rotation with d
-000071c0: 696d 3120 6173 2078 2d61 7869 7320 616e  im1 as x-axis an
-000071d0: 6420 6469 6d32 2061 7320 792d 6178 6973  d dim2 as y-axis
-000071e0: 3a20 5b64 696d 312c 2064 696d 325d 2063  : [dim1, dim2] c
-000071f0: 6f6f 7264 696e 6174 6573 2028 782c 2079  oordinates (x, y
-00007200: 2920 6265 636f 6d65 7320 2878 6d61 782d  ) becomes (xmax-
-00007210: 782c 2079 6d61 782d 7929 2e0a 2020 2020  x, ymax-y)..    
-00007220: 2020 2020 2020 2020 696d 6167 655f 7369          image_si
-00007230: 7a65 205b 7475 706c 6520 6f72 2062 742e  ze [tuple or bt.
-00007240: 5465 6e73 6f72 5d3a 2054 6865 2073 697a  Tensor]: The siz
-00007250: 6520 6f66 2074 6865 2069 6d61 6765 2c20  e of the image, 
-00007260: 6f72 2074 6865 2069 6d61 6765 2069 7473  or the image its
-00007270: 656c 662e 200a 2020 2020 2020 2020 2020  elf. .          
-00007280: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
-00007290: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
-000072a0: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
-000072b0: 5465 6e73 6f72 5d3a 2043 6f6f 7264 696e  Tensor]: Coordin
-000072c0: 6174 6573 2074 6f20 6265 2074 7261 6e73  ates to be trans
-000072d0: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
-000072e0: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
-000072f0: 6e5f 6261 7463 683a 6f70 7469 6f6e 616c  n_batch:optional
-00007300: 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f 312c  ], {n_dim}, n_1,
-00007310: 206e 5f32 2c20 2e2e 2e2c 206e 5f72 290a   n_2, ..., n_r).
-00007320: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00007330: 7574 205b 6274 2e54 656e 736f 725d 3a20  ut [bt.Tensor]: 
-00007340: 5468 6520 7472 616e 7366 6f72 6d65 6420  The transformed 
-00007350: 636f 6f72 6469 6e61 7465 732e 0a20 2020  coordinates..   
-00007360: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-00007370: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
-00007380: 6e5f 6469 6d7d 2c20 6e5f 312c 206e 5f32  n_dim}, n_1, n_2
-00007390: 2c20 2e2e 2e2c 206e 5f72 290a 2020 2020  , ..., n_r).    
-000073a0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000073b0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-000073c0: 2864 696d 313d 6469 6d31 2c20 6469 6d32  (dim1=dim1, dim2
-000073d0: 3d64 696d 322c 2069 6d61 6765 5f73 697a  =dim2, image_siz
-000073e0: 653d 696d 6167 655f 7369 7a65 290a 0a20  e=image_size).. 
-000073f0: 2020 2020 2020 2073 656c 662e 6469 6d31         self.dim1
-00007400: 2c20 7365 6c66 2e64 696d 3220 3d20 6469  , self.dim2 = di
-00007410: 6d31 2c20 6469 6d32 0a20 2020 2020 2020  m1, dim2.       
-00007420: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
-00007430: 6d61 6765 5f73 697a 652c 2062 742e 746f  mage_size, bt.to
-00007440: 7263 682e 5465 6e73 6f72 293a 2069 6d61  rch.Tensor): ima
-00007450: 6765 5f73 697a 6520 3d20 696d 6167 655f  ge_size = image_
-00007460: 7369 7a65 2e73 6861 7065 0a20 2020 2020  size.shape.     
-00007470: 2020 2073 656c 662e 696d 6167 655f 7369     self.image_si
-00007480: 7a65 203d 2069 6d61 6765 5f73 697a 650a  ze = image_size.
-00007490: 2020 2020 2020 2020 6966 2069 6d61 6765          if image
-000074a0: 5f73 697a 6520 6973 206e 6f74 204e 6f6e  _size is not Non
-000074b0: 653a 2073 656c 662e 6e5f 6469 6d20 3d20  e: self.n_dim = 
-000074c0: 6c65 6e28 696d 6167 655f 7369 7a65 290a  len(image_size).
-000074d0: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
-000074e0: 5f28 7365 6c66 2c20 5829 3a0a 2020 2020  _(self, X):.    
-000074f0: 2020 2020 5820 3d20 7375 7065 7228 292e      X = super().
-00007500: 5f5f 6361 6c6c 5f5f 2858 290a 2020 2020  __call__(X).    
-00007510: 2020 2020 6469 6d31 2c20 6469 6d32 203d      dim1, dim2 =
-00007520: 2073 656c 662e 6469 6d31 2c20 7365 6c66   self.dim1, self
-00007530: 2e64 696d 320a 2020 2020 2020 2020 7365  .dim2.        se
-00007540: 6c65 6374 3120 3d20 2873 6c69 6365 284e  lect1 = (slice(N
-00007550: 6f6e 6529 2c29 202a 2058 2e63 6861 6e6e  one),) * X.chann
-00007560: 656c 5f64 696d 202b 2028 6469 6d31 2c29  el_dim + (dim1,)
-00007570: 0a20 2020 2020 2020 2073 656c 6563 7432  .        select2
-00007580: 203d 2028 736c 6963 6528 4e6f 6e65 292c   = (slice(None),
-00007590: 2920 2a20 582e 6368 616e 6e65 6c5f 6469  ) * X.channel_di
-000075a0: 6d20 2b20 2864 696d 322c 290a 2020 2020  m + (dim2,).    
-000075b0: 2020 2020 6966 2073 656c 662e 696d 6167      if self.imag
-000075c0: 655f 7369 7a65 2069 7320 4e6f 6e65 3a20  e_size is None: 
-000075d0: 6d61 785f 7261 6e67 6531 2c20 6d61 785f  max_range1, max_
-000075e0: 7261 6e67 6532 203d 2058 5b73 656c 6563  range2 = X[selec
-000075f0: 7431 5d2e 6d61 7828 292c 2058 5b73 656c  t1].max(), X[sel
-00007600: 6563 7432 5d2e 6d61 7828 290a 2020 2020  ect2].max().    
-00007610: 2020 2020 656c 7365 3a20 6d61 785f 7261      else: max_ra
-00007620: 6e67 6531 2c20 6d61 785f 7261 6e67 6532  nge1, max_range2
-00007630: 203d 2073 656c 662e 696d 6167 655f 7369   = self.image_si
-00007640: 7a65 5b64 696d 315d 2c20 7365 6c66 2e69  ze[dim1], self.i
-00007650: 6d61 6765 5f73 697a 655b 6469 6d32 5d0a  mage_size[dim2].
-00007660: 2020 2020 2020 2020 585b 7365 6c65 6374          X[select
-00007670: 315d 203d 206d 6178 5f72 616e 6765 3120  1] = max_range1 
-00007680: 2d20 585b 7365 6c65 6374 315d 0a20 2020  - X[select1].   
-00007690: 2020 2020 2058 5b73 656c 6563 7432 5d20       X[select2] 
-000076a0: 3d20 6d61 785f 7261 6e67 6532 202d 2058  = max_range2 - X
-000076b0: 5b73 656c 6563 7432 5d0a 2020 2020 2020  [select2].      
-000076c0: 2020 7265 7475 726e 2058 0a20 2020 2020    return X.     
-000076d0: 2020 200a 2020 2020 6465 6620 6166 6669     .    def affi
-000076e0: 6e65 2873 656c 662c 206e 5f64 696d 3d4e  ne(self, n_dim=N
-000076f0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-00007700: 2073 656c 662e 696d 6167 655f 7369 7a65   self.image_size
-00007710: 2069 7320 4e6f 6e65 3a20 7265 7475 726e   is None: return
-00007720: 0a20 2020 2020 2020 2069 6620 6e5f 6469  .        if n_di
-00007730: 6d20 6973 204e 6f6e 6520 616e 6420 7365  m is None and se
-00007740: 6c66 2e6e 5f64 696d 2069 7320 4e6f 6e65  lf.n_dim is None
-00007750: 3a20 7265 7475 726e 0a20 2020 2020 2020  : return.       
-00007760: 2069 6620 6e5f 6469 6d20 6973 204e 6f6e   if n_dim is Non
-00007770: 653a 206e 5f64 696d 203d 2073 656c 662e  e: n_dim = self.
-00007780: 6e5f 6469 6d0a 2020 2020 2020 2020 6176  n_dim.        av
-00007790: 6f75 6368 2873 656c 662e 6e5f 6469 6d20  ouch(self.n_dim 
-000077a0: 6973 204e 6f6e 6520 6f72 2073 656c 662e  is None or self.
-000077b0: 6e5f 6469 6d20 3d3d 206e 5f64 696d 290a  n_dim == n_dim).
-000077c0: 2020 2020 2020 2020 6469 6d31 2c20 6469          dim1, di
-000077d0: 6d32 203d 2073 656c 662e 6469 6d31 2c20  m2 = self.dim1, 
-000077e0: 7365 6c66 2e64 696d 320a 2020 2020 2020  self.dim2.      
-000077f0: 2020 6166 6620 3d20 6274 2e65 7965 286e    aff = bt.eye(n
-00007800: 5f64 696d 202b 2031 290a 2020 2020 2020  _dim + 1).      
-00007810: 2020 6166 665b 6469 6d31 5d5b 6469 6d31    aff[dim1][dim1
-00007820: 5d20 3d20 2d31 2e0a 2020 2020 2020 2020  ] = -1..        
-00007830: 6166 665b 6469 6d31 5d5b 2d31 5d20 3d20  aff[dim1][-1] = 
-00007840: 666c 6f61 7428 7365 6c66 2e69 6d61 6765  float(self.image
-00007850: 5f73 697a 655b 6469 6d31 5d29 0a20 2020  _size[dim1]).   
-00007860: 2020 2020 2061 6666 5b64 696d 325d 5b64       aff[dim2][d
-00007870: 696d 325d 203d 202d 312e 0a20 2020 2020  im2] = -1..     
-00007880: 2020 2061 6666 5b64 696d 325d 5b2d 315d     aff[dim2][-1]
-00007890: 203d 2066 6c6f 6174 2873 656c 662e 696d   = float(self.im
-000078a0: 6167 655f 7369 7a65 5b64 696d 325d 290a  age_size[dim2]).
-000078b0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-000078c0: 6666 2e75 6e73 7175 6565 7a65 285b 5d29  ff.unsqueeze([])
-000078d0: 0a0a 2020 2020 6465 6620 696e 7628 7365  ..    def inv(se
-000078e0: 6c66 293a 2072 6574 7572 6e20 526f 7461  lf): return Rota
-000078f0: 7469 6f6e 3138 3028 7365 6c66 2e64 696d  tion180(self.dim
-00007900: 312c 2073 656c 662e 6469 6d32 2c20 696d  1, self.dim2, im
-00007910: 6167 655f 7369 7a65 203d 2073 656c 662e  age_size = self.
-00007920: 696d 6167 655f 7369 7a65 292e 6261 636b  image_size).back
-00007930: 7761 7264 5f28 7365 6c66 2e62 6163 6b77  ward_(self.backw
-00007940: 6172 6429 0a0a 4061 6c69 6173 2822 5265  ard)..@alias("Re
-00007950: 666c 6563 7422 290a 636c 6173 7320 5265  flect").class Re
-00007960: 666c 6563 7469 6f6e 2853 7061 7469 616c  flection(Spatial
-00007970: 5472 616e 7366 6f72 6d61 7469 6f6e 293a  Transformation):
-00007980: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00007990: 5f28 7365 6c66 2c20 2a64 696d 2c20 696d  _(self, *dim, im
-000079a0: 6167 655f 7369 7a65 3d4e 6f6e 6529 3a0a  age_size=None):.
-000079b0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000079c0: 2020 2020 5472 616e 7366 6f72 6d61 7469      Transformati
-000079d0: 6f6e 2074 6861 7420 7265 666c 6563 7473  on that reflects
-000079e0: 2061 6e20 696d 6167 6520 616c 6f6e 6720   an image along 
-000079f0: 6469 6d65 6e73 696f 6e20 6469 6d2e 0a20  dimension dim.. 
-00007a00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007a10: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
-00007a20: 2020 2020 6469 6d20 5b69 6e74 5d3a 2054      dim [int]: T
-00007a30: 6865 2064 696d 656e 7369 6f6e 2077 6520  he dimension we 
-00007a40: 7265 666c 6563 7420 7468 6520 696d 6167  reflect the imag
-00007a50: 6520 616c 6f6e 672e 200a 2020 2020 2020  e along. .      
-00007a60: 2020 2020 2020 2020 2020 692e 652e 2072            i.e. r
-00007a70: 6566 6c65 6374 696f 6e20 6f6e 2064 696d  eflection on dim
-00007a80: 3a20 5b64 696d 5d20 636f 6f72 6469 6e61  : [dim] coordina
-00007a90: 7465 2078 2062 6563 6f6d 6573 2078 6d61  te x becomes xma
-00007aa0: 782d 782e 0a20 2020 2020 2020 2020 2020  x-x..           
-00007ab0: 2069 6d61 6765 5f73 697a 6520 5b74 7570   image_size [tup
-00007ac0: 6c65 206f 7220 6274 2e54 656e 736f 725d  le or bt.Tensor]
-00007ad0: 3a20 5468 6520 7369 7a65 206f 6620 7468  : The size of th
-00007ae0: 6520 696d 6167 652c 206f 7220 7468 6520  e image, or the 
-00007af0: 696d 6167 6520 6974 7365 6c66 2e20 0a20  image itself. . 
-00007b00: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00007b10: 2020 2020 5768 656e 2069 7420 6973 2063      When it is c
-00007b20: 616c 6c65 643a 0a20 2020 2020 2020 2020  alled:.         
-00007b30: 2020 2058 205b 6274 2e54 656e 736f 725d     X [bt.Tensor]
-00007b40: 3a20 436f 6f72 6469 6e61 7465 7320 746f  : Coordinates to
-00007b50: 2062 6520 7472 616e 7366 6f72 6d65 642e   be transformed.
-00007b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b70: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-00007b80: 3a6f 7074 696f 6e61 6c5d 2c20 7b6e 5f64  :optional], {n_d
-00007b90: 696d 7d2c 206e 5f31 2c20 6e5f 322c 202e  im}, n_1, n_2, .
-00007ba0: 2e2e 2c20 6e5f 7229 0a20 2020 2020 2020  .., n_r).       
-00007bb0: 2020 2020 206f 7574 7075 7420 5b62 742e       output [bt.
-00007bc0: 5465 6e73 6f72 5d3a 2054 6865 2074 7261  Tensor]: The tra
-00007bd0: 6e73 666f 726d 6564 2063 6f6f 7264 696e  nsformed coordin
-00007be0: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
-00007bf0: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
-00007c00: 6261 7463 685d 2c20 7b6e 5f64 696d 7d2c  batch], {n_dim},
-00007c10: 206e 5f31 2c20 6e5f 322c 202e 2e2e 2c20   n_1, n_2, ..., 
-00007c20: 6e5f 7229 0a20 2020 2020 2020 2027 2727  n_r).        '''
-00007c30: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00007c40: 2e5f 5f69 6e69 745f 5f28 6469 6d73 3d64  .__init__(dims=d
-00007c50: 696d 2c20 696d 6167 655f 7369 7a65 3d69  im, image_size=i
-00007c60: 6d61 6765 5f73 697a 6529 0a0a 2020 2020  mage_size)..    
-00007c70: 2020 2020 6966 206c 656e 2864 696d 2920      if len(dim) 
-00007c80: 3d3d 2031 2061 6e64 2069 7369 6e73 7461  == 1 and isinsta
-00007c90: 6e63 6528 6469 6d5b 305d 2c20 286c 6973  nce(dim[0], (lis
-00007ca0: 742c 2074 7570 6c65 2929 3a20 6469 6d20  t, tuple)): dim 
-00007cb0: 3d20 6469 6d5b 305d 0a20 2020 2020 2020  = dim[0].       
-00007cc0: 2073 656c 662e 6469 6d73 203d 2064 696d   self.dims = dim
-00007cd0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00007ce0: 7374 616e 6365 2869 6d61 6765 5f73 697a  stance(image_siz
-00007cf0: 652c 2062 742e 746f 7263 682e 5465 6e73  e, bt.torch.Tens
-00007d00: 6f72 293a 2069 6d61 6765 5f73 697a 6520  or): image_size 
-00007d10: 3d20 696d 6167 655f 7369 7a65 2e73 6861  = image_size.sha
-00007d20: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
-00007d30: 696d 6167 655f 7369 7a65 203d 2069 6d61  image_size = ima
-00007d40: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
-00007d50: 6966 2069 6d61 6765 5f73 697a 6520 6973  if image_size is
-00007d60: 206e 6f74 204e 6f6e 653a 2073 656c 662e   not None: self.
-00007d70: 6e5f 6469 6d20 3d20 6c65 6e28 696d 6167  n_dim = len(imag
-00007d80: 655f 7369 7a65 290a 0a20 2020 2064 6566  e_size)..    def
-00007d90: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-00007da0: 5829 3a0a 2020 2020 2020 2020 5820 3d20  X):.        X = 
-00007db0: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
-00007dc0: 2858 290a 2020 2020 2020 2020 6469 6d73  (X).        dims
-00007dd0: 203d 2073 656c 662e 6469 6d73 0a20 2020   = self.dims.   
-00007de0: 2020 2020 2066 6f72 2064 696d 2069 6e20       for dim in 
-00007df0: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
-00007e00: 2020 7365 6c65 6374 203d 2028 736c 6963    select = (slic
-00007e10: 6528 4e6f 6e65 292c 2920 2a20 582e 6368  e(None),) * X.ch
-00007e20: 616e 6e65 6c5f 6469 6d20 2b20 2864 696d  annel_dim + (dim
-00007e30: 2c29 0a20 2020 2020 2020 2020 2020 2069  ,).            i
-00007e40: 6620 7365 6c66 2e69 6d61 6765 5f73 697a  f self.image_siz
-00007e50: 6520 6973 204e 6f6e 653a 206d 6178 5f72  e is None: max_r
-00007e60: 616e 6765 203d 2058 5b73 656c 6563 745d  ange = X[select]
-00007e70: 2e6d 6178 2829 0a20 2020 2020 2020 2020  .max().         
-00007e80: 2020 2065 6c73 653a 206d 6178 5f72 616e     else: max_ran
-00007e90: 6765 203d 2073 656c 662e 696d 6167 655f  ge = self.image_
-00007ea0: 7369 7a65 5b64 696d 5d0a 2020 2020 2020  size[dim].      
-00007eb0: 2020 2020 2020 585b 7365 6c65 6374 5d20        X[select] 
-00007ec0: 3d20 6d61 785f 7261 6e67 6520 2d20 585b  = max_range - X[
-00007ed0: 7365 6c65 6374 5d0a 2020 2020 2020 2020  select].        
-00007ee0: 7265 7475 726e 2058 0a20 2020 2020 2020  return X.       
-00007ef0: 200a 2020 2020 6465 6620 6166 6669 6e65   .    def affine
-00007f00: 2873 656c 662c 206e 5f64 696d 3d4e 6f6e  (self, n_dim=Non
-00007f10: 6529 3a0a 2020 2020 2020 2020 6966 2073  e):.        if s
-00007f20: 656c 662e 696d 6167 655f 7369 7a65 2069  elf.image_size i
-00007f30: 7320 4e6f 6e65 3a20 7265 7475 726e 0a20  s None: return. 
-00007f40: 2020 2020 2020 2069 6620 6e5f 6469 6d20         if n_dim 
-00007f50: 6973 204e 6f6e 6520 616e 6420 7365 6c66  is None and self
-00007f60: 2e6e 5f64 696d 2069 7320 4e6f 6e65 3a20  .n_dim is None: 
-00007f70: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-00007f80: 6620 6e5f 6469 6d20 6973 204e 6f6e 653a  f n_dim is None:
-00007f90: 206e 5f64 696d 203d 2073 656c 662e 6e5f   n_dim = self.n_
-00007fa0: 6469 6d0a 2020 2020 2020 2020 6176 6f75  dim.        avou
-00007fb0: 6368 2873 656c 662e 6e5f 6469 6d20 6973  ch(self.n_dim is
-00007fc0: 204e 6f6e 6520 6f72 2073 656c 662e 6e5f   None or self.n_
-00007fd0: 6469 6d20 3d3d 206e 5f64 696d 290a 2020  dim == n_dim).  
-00007fe0: 2020 2020 2020 6166 6620 3d20 6274 2e65        aff = bt.e
-00007ff0: 7965 286e 5f64 696d 202b 2031 290a 2020  ye(n_dim + 1).  
-00008000: 2020 2020 2020 666f 7220 6469 6d20 696e        for dim in
-00008010: 2073 656c 662e 6469 6d73 3a0a 2020 2020   self.dims:.    
-00008020: 2020 2020 2020 2020 6166 665b 6469 6d5d          aff[dim]
-00008030: 5b64 696d 5d20 3d20 2d31 2e0a 2020 2020  [dim] = -1..    
-00008040: 2020 2020 2020 2020 6166 665b 6469 6d5d          aff[dim]
-00008050: 5b2d 315d 203d 2066 6c6f 6174 2873 656c  [-1] = float(sel
-00008060: 662e 696d 6167 655f 7369 7a65 5b64 696d  f.image_size[dim
-00008070: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-00008080: 6e20 6166 662e 756e 7371 7565 657a 6528  n aff.unsqueeze(
-00008090: 5b5d 290a 0a20 2020 2064 6566 2069 6e76  [])..    def inv
-000080a0: 2873 656c 6629 3a20 7265 7475 726e 2052  (self): return R
-000080b0: 6566 6c65 6374 282a 7365 6c66 2e64 696d  eflect(*self.dim
-000080c0: 732c 2069 6d61 6765 5f73 697a 6520 3d20  s, image_size = 
-000080d0: 7365 6c66 2e69 6d61 6765 5f73 697a 6529  self.image_size)
-000080e0: 2e62 6163 6b77 6172 645f 2873 656c 662e  .backward_(self.
-000080f0: 6261 636b 7761 7264 290a 0a40 616c 6961  backward)..@alia
-00008100: 7328 2250 6572 6d75 7465 6469 6d22 290a  s("Permutedim").
-00008110: 636c 6173 7320 4469 6d50 6572 6d75 7461  class DimPermuta
-00008120: 7469 6f6e 2853 7061 7469 616c 5472 616e  tion(SpatialTran
-00008130: 7366 6f72 6d61 7469 6f6e 293a 0a20 2020  sformation):.   
-00008140: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00008150: 6c66 2c20 2a64 696d 732c 2072 6573 697a  lf, *dims, resiz
-00008160: 655f 696d 6167 653d 5472 7565 293a 0a20  e_image=True):. 
-00008170: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00008180: 2020 2050 6572 6d75 7465 2074 6865 2064     Permute the d
-00008190: 696d 656e 7369 6f6e 7320 666f 7220 616e  imensions for an
-000081a0: 2069 6d61 6765 2c20 7369 6d69 6c61 7220   image, similar 
-000081b0: 746f 206e 702e 7472 616e 7370 6f73 6520  to np.transpose 
-000081c0: 6f72 2074 6f72 6368 2f62 6174 6f72 6368  or torch/batorch
-000081d0: 2e70 6572 6d75 7465 2e0a 2020 2020 2020  .permute..      
-000081e0: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
-000081f0: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-00008200: 696d 7320 5b6c 6973 7420 6f72 2074 7570  ims [list or tup
-00008210: 6c65 206f 7220 6274 2e54 656e 736f 725d  le or bt.Tensor]
-00008220: 3a20 5468 6520 6469 6d65 6e73 696f 6e20  : The dimension 
-00008230: 7065 726d 7561 7469 6f6e 2e20 0a20 2020  permuation. .   
-00008240: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-00008250: 653a 206c 656e 6774 6828 6e5f 6469 6d29  e: length(n_dim)
-00008260: 206f 7220 285b 6e5f 6261 7463 683a 6f70   or ([n_batch:op
-00008270: 7469 6f6e 616c 5d2c 207b 6e5f 6469 6d7d  tional], {n_dim}
-00008280: 292e 0a0a 2020 2020 2020 2020 5768 656e  )...        When
-00008290: 2069 7420 6973 2063 616c 6c65 643a 0a20   it is called:. 
-000082a0: 2020 2020 2020 2020 2020 2058 205b 6274             X [bt
-000082b0: 2e54 656e 736f 725d 3a20 436f 6f72 6469  .Tensor]: Coordi
-000082c0: 6e61 7465 7320 746f 2062 6520 7472 616e  nates to be tran
-000082d0: 7366 6f72 6d65 642e 0a20 2020 2020 2020  sformed..       
-000082e0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-000082f0: 5b6e 5f62 6174 6368 3a6f 7074 696f 6e61  [n_batch:optiona
-00008300: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 5f31  l], {n_dim}, n_1
-00008310: 2c20 6e5f 322c 202e 2e2e 2c20 6e5f 7229  , n_2, ..., n_r)
-00008320: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-00008330: 7075 7420 5b62 742e 5465 6e73 6f72 5d3a  put [bt.Tensor]:
-00008340: 2054 6865 2074 7261 6e73 666f 726d 6564   The transformed
-00008350: 2063 6f6f 7264 696e 6174 6573 2e0a 2020   coordinates..  
-00008360: 2020 2020 2020 2020 2020 2020 2020 7369                si
-00008370: 7a65 3a20 285b 6e5f 6261 7463 685d 2c20  ze: ([n_batch], 
-00008380: 7b6e 5f64 696d 7d2c 206e 5f31 2c20 6e5f  {n_dim}, n_1, n_
-00008390: 322c 202e 2e2e 2c20 6e5f 7229 0a20 2020  2, ..., n_r).   
-000083a0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-000083b0: 2069 6620 6c65 6e28 6469 6d73 2920 3d3d   if len(dims) ==
-000083c0: 2031 3a20 6469 6d73 203d 2064 696d 735b   1: dims = dims[
-000083d0: 305d 0a20 2020 2020 2020 2064 696d 7320  0].        dims 
-000083e0: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
-000083f0: 286c 6973 7428 6469 6d73 2929 2e73 7175  (list(dims)).squ
-00008400: 6565 7a65 2829 0a20 2020 2020 2020 2064  eeze().        d
-00008410: 696d 7320 3d20 6469 6d73 2e6c 6f6e 6728  ims = dims.long(
-00008420: 290a 2020 2020 2020 2020 6966 2064 696d  ).        if dim
-00008430: 732e 6e5f 6469 6d20 3c3d 2031 3a20 6469  s.n_dim <= 1: di
-00008440: 6d73 203d 2064 696d 732e 756e 7371 7565  ms = dims.unsque
-00008450: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
-00008460: 6966 2064 696d 732e 6e5f 6469 6d20 3d3d  if dims.n_dim ==
-00008470: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00008480: 6966 206e 6f74 2064 696d 732e 6861 735f  if not dims.has_
-00008490: 6261 7463 683a 2064 696d 732e 6261 7463  batch: dims.batc
-000084a0: 685f 6469 6d65 6e73 696f 6e20 3d20 300a  h_dimension = 0.
-000084b0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000084c0: 6f74 2064 696d 732e 6861 735f 6368 616e  ot dims.has_chan
-000084d0: 6e65 6c3a 2064 696d 732e 6368 616e 6e65  nel: dims.channe
-000084e0: 6c5f 6469 6d65 6e73 696f 6e20 3d20 3020  l_dimension = 0 
-000084f0: 6966 2064 696d 732e 6261 7463 685f 6469  if dims.batch_di
-00008500: 6d65 6e73 696f 6e20 3e20 3020 656c 7365  mension > 0 else
-00008510: 2031 0a20 2020 2020 2020 2061 766f 7563   1.        avouc
-00008520: 6828 6469 6d73 2e68 6173 5f62 6174 6368  h(dims.has_batch
-00008530: 2061 6e64 2064 696d 732e 6861 735f 6368   and dims.has_ch
-00008540: 616e 6e65 6c2c 2066 2250 6c65 6173 6520  annel, f"Please 
-00008550: 7573 6520 6261 746f 7263 6820 7465 6e73  use batorch tens
-00008560: 6f72 206f 6620 7369 7a65 205c 0a20 2020  or of size \.   
-00008570: 2020 2020 2020 2020 2028 5b6e 5f62 6174           ([n_bat
-00008580: 6368 3a6f 7074 696f 6e61 6c5d 2c20 7b7b  ch:optional], {{
-00008590: 6e5f 6469 6d7d 7d29 2066 6f72 2054 7261  n_dim}}) for Tra
-000085a0: 6e73 6c61 7469 6f6e 2070 6172 616d 6574  nslation paramet
-000085b0: 6572 732c 2069 6e73 7465 6164 206f 6620  ers, instead of 
-000085c0: 7b64 696d 732e 7368 6170 657d 2e20 2229  {dims.shape}. ")
-000085d0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-000085e0: 2e5f 5f69 6e69 745f 5f28 6469 6d73 2c20  .__init__(dims, 
-000085f0: 7265 7369 7a65 5f69 6d61 6765 3d72 6573  resize_image=res
-00008600: 697a 655f 696d 6167 6529 0a0a 2020 2020  ize_image)..    
-00008610: 2020 2020 7365 6c66 2e64 696d 7320 3d20      self.dims = 
-00008620: 6469 6d73 0a20 2020 2020 2020 2073 656c  dims.        sel
-00008630: 662e 6e5f 6469 6d20 3d20 6469 6d73 2e6e  f.n_dim = dims.n
-00008640: 5f63 6861 6e6e 656c 0a20 2020 2020 2020  _channel.       
-00008650: 2073 656c 662e 7265 7369 7a65 5f69 6d61   self.resize_ima
-00008660: 6765 203d 2072 6573 697a 655f 696d 6167  ge = resize_imag
-00008670: 650a 2020 2020 2020 2020 6966 2072 6573  e.        if res
-00008680: 697a 655f 696d 6167 653a 0a20 2020 2020  ize_image:.     
-00008690: 2020 2020 2020 2069 6620 6469 6d73 2e6e         if dims.n
-000086a0: 5f62 6174 6368 203e 2031 3a0a 2020 2020  _batch > 1:.    
-000086b0: 2020 2020 2020 2020 2020 2020 6469 6d73              dims
-000086c0: 5f63 6170 203d 2064 696d 732e 7361 6d70  _cap = dims.samp
-000086d0: 6c65 2872 616e 646f 6d3d 4661 6c73 652c  le(random=False,
-000086e0: 2064 696d 3d5b 5d29 0a20 2020 2020 2020   dim=[]).       
-000086f0: 2020 2020 2020 2020 2061 766f 7563 6828           avouch(
-00008700: 6274 2e6e 6f72 6d28 6469 6d73 202d 2064  bt.norm(dims - d
-00008710: 696d 735f 6361 7029 2e73 756d 2829 203c  ims_cap).sum() <
-00008720: 2031 652d 342c 2022 4361 6e6e 6f74 2072   1e-4, "Cannot r
-00008730: 6573 697a 6520 696d 6167 6520 7768 656e  esize image when
-00008740: 2064 6966 6665 7265 6e74 2070 6572 6d75   different permu
-00008750: 7461 7469 6f6e 2064 6f6e 6520 666f 7220  tation done for 
-00008760: 6469 6666 6572 656e 7420 6261 7463 6820  different batch 
-00008770: 6d65 6d62 6572 732e 2022 290a 2020 2020  members. ").    
-00008780: 2020 2020 2020 2020 6469 6d73 203d 2064          dims = d
-00008790: 696d 732e 7069 636b 2830 2c20 5b5d 292e  ims.pick(0, []).
-000087a0: 746f 6c69 7374 2829 0a20 2020 2020 2020  tolist().       
-000087b0: 2020 2020 2076 6973 6974 6564 203d 205b       visited = [
-000087c0: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
-000087d0: 6c66 2e72 6573 6861 7065 203d 205b 2831  lf.reshape = [(1
-000087e0: 2c29 5d0a 2020 2020 2020 2020 2020 2020  ,)].            
-000087f0: 666f 7220 7020 696e 2072 616e 6765 2873  for p in range(s
-00008800: 656c 662e 6e5f 6469 6d29 3a0a 2020 2020  elf.n_dim):.    
-00008810: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-00008820: 2069 6e20 7669 7369 7465 643a 2063 6f6e   in visited: con
-00008830: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00008840: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00008850: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008860: 2020 2020 2020 7669 7369 7465 642e 6170        visited.ap
-00008870: 7065 6e64 2870 290a 2020 2020 2020 2020  pend(p).        
-00008880: 2020 2020 2020 2020 2020 2020 7120 3d20              q = 
-00008890: 6469 6d73 5b70 5d0a 2020 2020 2020 2020  dims[p].        
-000088a0: 2020 2020 2020 2020 2020 2020 6966 2071              if q
-000088b0: 2069 6e20 7669 7369 7465 643a 2062 7265   in visited: bre
-000088c0: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
-000088d0: 2020 2020 2020 2073 656c 662e 7265 7368         self.resh
-000088e0: 6170 652e 6170 7065 6e64 2828 702c 2071  ape.append((p, q
-000088f0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00008900: 2020 2020 2020 2070 203d 2071 0a0a 2020         p = q..  
-00008910: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
-00008920: 656c 662c 2058 293a 0a20 2020 2020 2020  elf, X):.       
-00008930: 2058 203d 2073 7570 6572 2829 2e5f 5f63   X = super().__c
-00008940: 616c 6c5f 5f28 5829 0a20 2020 2020 2020  all__(X).       
-00008950: 2072 6574 7572 6e20 582e 6761 7468 6572   return X.gather
-00008960: 2858 2e63 6861 6e6e 656c 5f64 696d 656e  (X.channel_dimen
-00008970: 7369 6f6e 2c20 7365 6c66 2e64 696d 732e  sion, self.dims.
-00008980: 6578 7061 6e64 5f74 6f28 5829 290a 2020  expand_to(X)).  
-00008990: 2020 2020 2020 0a20 2020 2064 6566 2061        .    def a
-000089a0: 6666 696e 6528 7365 6c66 2c20 6e5f 6469  ffine(self, n_di
-000089b0: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-000089c0: 2061 766f 7563 6828 6e5f 6469 6d20 6973   avouch(n_dim is
-000089d0: 204e 6f6e 6520 6f72 2073 656c 662e 6e5f   None or self.n_
-000089e0: 6469 6d20 3d3d 206e 5f64 696d 290a 2020  dim == n_dim).  
-000089f0: 2020 2020 2020 6966 206e 5f64 696d 2069        if n_dim i
-00008a00: 7320 4e6f 6e65 3a20 6e5f 6469 6d20 3d20  s None: n_dim = 
-00008a10: 7365 6c66 2e6e 5f64 696d 0a20 2020 2020  self.n_dim.     
-00008a20: 2020 206e 5f62 6174 6368 203d 2073 656c     n_batch = sel
-00008a30: 662e 6e5f 6261 7463 680a 2020 2020 2020  f.n_batch.      
-00008a40: 2020 6966 206e 5f62 6174 6368 2069 7320    if n_batch is 
-00008a50: 4e6f 6e65 3a20 6e5f 6261 7463 6820 3d20  None: n_batch = 
-00008a60: 310a 2020 2020 2020 2020 6166 6620 3d20  1.        aff = 
-00008a70: 6274 2e64 6961 6728 6274 2e6f 6e65 5f68  bt.diag(bt.one_h
-00008a80: 6f74 282d 312c 206e 5f64 696d 202b 2031  ot(-1, n_dim + 1
-00008a90: 292e 666c 6f61 7428 292e 6d75 6c74 6970  ).float().multip
-00008aa0: 6c79 286e 5f62 6174 6368 2c20 5b5d 2929  ly(n_batch, []))
-00008ab0: 0a20 2020 2020 2020 2062 203d 2062 742e  .        b = bt.
-00008ac0: 6261 7463 685f 7465 6e73 6f72 2862 742e  batch_tensor(bt.
-00008ad0: 6172 616e 6765 286e 5f62 6174 6368 2929  arange(n_batch))
-00008ae0: 2e65 7870 616e 645f 746f 2873 656c 662e  .expand_to(self.
-00008af0: 6469 6d73 290a 2020 2020 2020 2020 6920  dims).        i 
-00008b00: 3d20 6274 2e61 7261 6e67 6528 6e5f 6469  = bt.arange(n_di
-00008b10: 6d29 2e6d 756c 7469 706c 7928 6e5f 6261  m).multiply(n_ba
-00008b20: 7463 682c 205b 5d29 0a20 2020 2020 2020  tch, []).       
-00008b30: 2061 6666 5b62 2c20 692c 2073 656c 662e   aff[b, i, self.
-00008b40: 6469 6d73 5d20 3d20 312e 0a20 2020 2020  dims] = 1..     
-00008b50: 2020 2072 6574 7572 6e20 6166 660a 0a20     return aff.. 
-00008b60: 2020 2064 6566 2069 6e76 2873 656c 6629     def inv(self)
-00008b70: 3a0a 2020 2020 2020 2020 6e5f 6469 6d20  :.        n_dim 
-00008b80: 3d20 7365 6c66 2e6e 5f64 696d 0a20 2020  = self.n_dim.   
-00008b90: 2020 2020 206e 6577 5f70 6572 6d75 7465       new_permute
-00008ba0: 203d 2028 7365 6c66 2e64 696d 7320 3d3d   = (self.dims ==
-00008bb0: 2062 742e 6172 616e 6765 286e 5f64 696d   bt.arange(n_dim
-00008bc0: 292e 7669 6577 285b 315d 2c20 6e5f 6469  ).view([1], n_di
-00008bd0: 6d2c 207b 317d 2929 2e66 6c6f 6174 2829  m, {1})).float()
-00008be0: 2e61 7267 6d61 7828 2d31 292e 6368 616e  .argmax(-1).chan
-00008bf0: 6e65 6c5f 6469 6d65 6e73 696f 6e5f 282d  nel_dimension_(-
-00008c00: 3129 0a20 2020 2020 2020 2072 6574 7572  1).        retur
-00008c10: 6e20 5065 726d 7574 6564 696d 286e 6577  n Permutedim(new
-00008c20: 5f70 6572 6d75 7465 2c20 7265 7369 7a65  _permute, resize
-00008c30: 5f69 6d61 6765 203d 2073 656c 662e 7265  _image = self.re
-00008c40: 7369 7a65 5f69 6d61 6765 292e 6261 636b  size_image).back
-00008c50: 7761 7264 5f28 7365 6c66 2e62 6163 6b77  ward_(self.backw
-00008c60: 6172 6429 0a0a 4061 6c69 6173 2822 5265  ard)..@alias("Re
-00008c70: 7363 616c 6522 290a 636c 6173 7320 5265  scale").class Re
-00008c80: 7363 616c 696e 6728 5370 6174 6961 6c54  scaling(SpatialT
-00008c90: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
-00008ca0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00008cb0: 2873 656c 662c 202a 7363 616c 652c 2072  (self, *scale, r
-00008cc0: 6573 697a 655f 696d 6167 653d 5472 7565  esize_image=True
-00008cd0: 293a 0a20 2020 2020 2020 2027 2727 0a20  ):.        '''. 
-00008ce0: 2020 2020 2020 2053 6361 6c65 2061 6e20         Scale an 
-00008cf0: 696d 6167 652e 0a20 2020 2020 2020 200a  image..        .
-00008d00: 2020 2020 2020 2020 4e6f 7465 3a20 5468          Note: Th
-00008d10: 6520 7363 616c 696e 6720 6973 2066 6f72  e scaling is for
-00008d20: 2063 6f6f 7264 696e 6174 6573 2c20 6865   coordinates, he
-00008d30: 6e63 6520 7468 6520 696d 6167 6520 776f  nce the image wo
-00008d40: 756c 6420 7368 7269 6e6b 2069 6620 7363  uld shrink if sc
-00008d50: 616c 6520 3e20 312e 200a 2020 2020 2020  ale > 1. .      
-00008d60: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
-00008d70: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00008d80: 6361 6c65 205b 666c 6f61 7420 6f72 2074  cale [float or t
-00008d90: 7570 6c65 206f 7220 6274 2e54 656e 736f  uple or bt.Tenso
-00008da0: 725d 3a20 5468 6520 7363 616c 696e 6720  r]: The scaling 
-00008db0: 666f 7220 616c 6c20 6469 6d65 6e73 696f  for all dimensio
-00008dc0: 6e73 2028 666c 6f61 7429 200a 2020 2020  ns (float) .    
-00008dd0: 2020 2020 2020 2020 2020 2020 6f72 2066              or f
-00008de0: 6f72 2065 6163 6820 6469 6d65 6e73 696f  or each dimensio
-00008df0: 6e20 2874 7570 6c65 292e 203e 3120 6d65  n (tuple). >1 me
-00008e00: 616e 7320 656e 6c61 7267 696e 6720 7468  ans enlarging th
-00008e10: 6520 636f 6f72 6469 6e61 7465 732e 0a20  e coordinates.. 
-00008e20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008e30: 697a 653a 2028 5b6e 5f62 6174 6368 3a6f  ize: ([n_batch:o
-00008e40: 7074 696f 6e61 6c5d 2c20 7b6e 5f64 696d  ptional], {n_dim
-00008e50: 7d29 2066 6f72 2062 742e 5465 6e73 6f72  }) for bt.Tensor
-00008e60: 2e0a 2020 2020 2020 2020 2020 2020 0a20  ..            . 
-00008e70: 2020 2020 2020 2057 6865 6e20 6974 2069         When it i
-00008e80: 7320 6361 6c6c 6564 3a0a 2020 2020 2020  s called:.      
-00008e90: 2020 2020 2020 5820 5b62 742e 5465 6e73        X [bt.Tens
-00008ea0: 6f72 5d3a 2043 6f6f 7264 696e 6174 6573  or]: Coordinates
-00008eb0: 2074 6f20 6265 2074 7261 6e73 666f 726d   to be transform
-00008ec0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00008ed0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00008ee0: 7463 683a 6f70 7469 6f6e 616c 5d2c 207b  tch:optional], {
-00008ef0: 6e5f 6469 6d7d 2c20 6e5f 312c 206e 5f32  n_dim}, n_1, n_2
-00008f00: 2c20 2e2e 2e2c 206e 5f72 290a 2020 2020  , ..., n_r).    
-00008f10: 2020 2020 2020 2020 6f75 7470 7574 205b          output [
-00008f20: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
-00008f30: 7472 616e 7366 6f72 6d65 6420 636f 6f72  transformed coor
-00008f40: 6469 6e61 7465 732e 0a20 2020 2020 2020  dinates..       
-00008f50: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-00008f60: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-00008f70: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
-00008f80: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
-00008f90: 2727 270a 2020 2020 2020 2020 6966 206c  '''.        if l
-00008fa0: 656e 2873 6361 6c65 2920 3d3d 2031 2061  en(scale) == 1 a
-00008fb0: 6e64 2069 7369 6e73 7461 6e63 6528 7363  nd isinstance(sc
-00008fc0: 616c 655b 305d 2c20 2869 6e74 2c20 666c  ale[0], (int, fl
-00008fd0: 6f61 7429 293a 2073 6361 6c65 203d 2073  oat)): scale = s
-00008fe0: 6361 6c65 5b30 5d20 2a20 6274 2e6f 6e65  cale[0] * bt.one
-00008ff0: 7328 5b31 5d2c 207b 317d 290a 2020 2020  s([1], {1}).    
-00009000: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00009010: 2020 2020 2020 6966 206c 656e 2873 6361        if len(sca
-00009020: 6c65 2920 3d3d 2031 3a20 7363 616c 6520  le) == 1: scale 
-00009030: 3d20 7363 616c 655b 305d 0a20 2020 2020  = scale[0].     
-00009040: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-00009050: 696e 7374 616e 6365 2873 6361 6c65 2c20  instance(scale, 
-00009060: 6274 2e54 656e 736f 7229 3a20 7363 616c  bt.Tensor): scal
-00009070: 6520 3d20 6261 746f 7263 685f 7465 6e73  e = batorch_tens
-00009080: 6f72 286c 6973 7428 7363 616c 6529 292e  or(list(scale)).
-00009090: 7371 7565 657a 6528 290a 2020 2020 2020  squeeze().      
-000090a0: 2020 2020 2020 6966 2073 6361 6c65 2e6e        if scale.n
-000090b0: 5f64 696d 203c 3d20 313a 2073 6361 6c65  _dim <= 1: scale
-000090c0: 203d 2073 6361 6c65 2e75 6e73 7175 6565   = scale.unsquee
-000090d0: 7a65 285b 5d29 0a20 2020 2020 2020 2020  ze([]).         
-000090e0: 2020 2069 6620 7363 616c 652e 6e5f 6469     if scale.n_di
-000090f0: 6d20 3d3d 2032 3a0a 2020 2020 2020 2020  m == 2:.        
-00009100: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00009110: 6361 6c65 2e68 6173 5f62 6174 6368 3a20  cale.has_batch: 
-00009120: 7363 616c 652e 6261 7463 685f 6469 6d65  scale.batch_dime
-00009130: 6e73 696f 6e20 3d20 300a 2020 2020 2020  nsion = 0.      
-00009140: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00009150: 2073 6361 6c65 2e68 6173 5f63 6861 6e6e   scale.has_chann
-00009160: 656c 3a20 7363 616c 652e 6368 616e 6e65  el: scale.channe
-00009170: 6c5f 6469 6d65 6e73 696f 6e20 3d20 3020  l_dimension = 0 
-00009180: 6966 2073 6361 6c65 2e62 6174 6368 5f64  if scale.batch_d
-00009190: 696d 656e 7369 6f6e 203e 2030 2065 6c73  imension > 0 els
-000091a0: 6520 310a 2020 2020 2020 2020 6176 6f75  e 1.        avou
-000091b0: 6368 2873 6361 6c65 2e68 6173 5f62 6174  ch(scale.has_bat
-000091c0: 6368 2061 6e64 2073 6361 6c65 2e68 6173  ch and scale.has
-000091d0: 5f63 6861 6e6e 656c 2c20 6622 506c 6561  _channel, f"Plea
-000091e0: 7365 2075 7365 2062 6174 6f72 6368 2074  se use batorch t
-000091f0: 656e 736f 7220 6f66 2073 697a 6520 5c0a  ensor of size \.
-00009200: 2020 2020 2020 2020 2020 2020 285b 6e5f              ([n_
-00009210: 6261 7463 683a 6f70 7469 6f6e 616c 5d2c  batch:optional],
-00009220: 207b 7b6e 5f64 696d 7d7d 2920 666f 7220   {{n_dim}}) for 
-00009230: 5363 616c 696e 6720 7061 7261 6d65 7465  Scaling paramete
-00009240: 7273 2c20 696e 7374 6561 6420 6f66 207b  rs, instead of {
-00009250: 7363 616c 652e 7368 6170 657d 2e20 2229  scale.shape}. ")
-00009260: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00009270: 2e5f 5f69 6e69 745f 5f28 7363 616c 652c  .__init__(scale,
-00009280: 2072 6573 697a 655f 696d 6167 653d 7265   resize_image=re
-00009290: 7369 7a65 5f69 6d61 6765 290a 0a20 2020  size_image)..   
-000092a0: 2020 2020 2073 656c 662e 7363 616c 6520       self.scale 
-000092b0: 3d20 7363 616c 650a 2020 2020 2020 2020  = scale.        
-000092c0: 6966 2073 656c 662e 7363 616c 652e 6e5f  if self.scale.n_
-000092d0: 6368 616e 6e65 6c20 3e20 313a 2073 656c  channel > 1: sel
-000092e0: 662e 6e5f 6469 6d20 3d20 7365 6c66 2e73  f.n_dim = self.s
-000092f0: 6361 6c65 2e6e 5f63 6861 6e6e 656c 0a20  cale.n_channel. 
-00009300: 2020 2020 2020 2069 6620 7265 7369 7a65         if resize
-00009310: 5f69 6d61 6765 3a0a 2020 2020 2020 2020  _image:.        
-00009320: 2020 2020 7363 616c 6520 3d20 7363 616c      scale = scal
-00009330: 652e 7371 7565 657a 6528 5b5d 290a 2020  e.squeeze([]).  
-00009340: 2020 2020 2020 2020 2020 6176 6f75 6368            avouch
-00009350: 2873 6361 6c65 2e6e 6469 6d20 3d3d 2031  (scale.ndim == 1
-00009360: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00009370: 6c66 2e72 6573 6861 7065 203d 205b 7475  lf.reshape = [tu
-00009380: 706c 6528 2831 2f73 6361 6c65 292e 746f  ple((1/scale).to
-00009390: 6c69 7374 2829 295d 0a20 2020 2020 2020  list())].       
-000093a0: 2073 656c 662e 7265 7369 7a65 5f69 6d61   self.resize_ima
-000093b0: 6765 203d 2072 6573 697a 655f 696d 6167  ge = resize_imag
-000093c0: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
-000093d0: 6174 6368 5f70 6172 616d 2e61 7070 656e  atch_param.appen
-000093e0: 6428 2773 6361 6c65 2729 0a0a 2020 2020  d('scale')..    
-000093f0: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-00009400: 662c 2058 293a 0a20 2020 2020 2020 2058  f, X):.        X
-00009410: 203d 2073 7570 6572 2829 2e5f 5f63 616c   = super().__cal
-00009420: 6c5f 5f28 5829 0a20 2020 2020 2020 2073  l__(X).        s
-00009430: 6361 6c65 203d 2073 656c 662e 7363 616c  cale = self.scal
-00009440: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00009450: 2058 202a 2073 6361 6c65 0a20 2020 200a   X * scale.    .
-00009460: 2020 2020 6465 6620 6166 6669 6e65 2873      def affine(s
-00009470: 656c 662c 206e 5f64 696d 3d4e 6f6e 6529  elf, n_dim=None)
-00009480: 3a0a 2020 2020 2020 2020 6966 206e 5f64  :.        if n_d
-00009490: 696d 2069 7320 4e6f 6e65 2061 6e64 2073  im is None and s
-000094a0: 656c 662e 6e5f 6469 6d20 6973 204e 6f6e  elf.n_dim is Non
-000094b0: 653a 2072 6574 7572 6e0a 2020 2020 2020  e: return.      
-000094c0: 2020 6966 206e 5f64 696d 2069 7320 4e6f    if n_dim is No
-000094d0: 6e65 3a20 6e5f 6469 6d20 3d20 7365 6c66  ne: n_dim = self
-000094e0: 2e6e 5f64 696d 0a20 2020 2020 2020 2061  .n_dim.        a
-000094f0: 766f 7563 6828 7365 6c66 2e6e 5f64 696d  vouch(self.n_dim
-00009500: 2069 7320 4e6f 6e65 206f 7220 7365 6c66   is None or self
-00009510: 2e6e 5f64 696d 203d 3d20 6e5f 6469 6d29  .n_dim == n_dim)
-00009520: 0a20 2020 2020 2020 2073 6361 6c65 203d  .        scale =
-00009530: 2073 656c 662e 7363 616c 650a 2020 2020   self.scale.    
-00009540: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00009550: 6528 7363 616c 652c 2028 696e 742c 2066  e(scale, (int, f
-00009560: 6c6f 6174 2929 3a20 7265 7475 726e 2073  loat)): return s
-00009570: 6361 6c65 202a 2062 742e 6579 6528 6e5f  cale * bt.eye(n_
-00009580: 6469 6d20 2b20 3129 0a20 2020 2020 2020  dim + 1).       
-00009590: 2072 6574 7572 6e20 6274 2e64 6961 6728   return bt.diag(
-000095a0: 6274 2e63 6174 2873 6361 6c65 2c20 6274  bt.cat(scale, bt
-000095b0: 2e6f 6e65 7328 5b73 6361 6c65 2e6e 5f62  .ones([scale.n_b
-000095c0: 6174 6368 5d2c 2031 292c 2031 2929 0a0a  atch], 1), 1))..
-000095d0: 2020 2020 6465 6620 696e 7628 7365 6c66      def inv(self
-000095e0: 293a 2072 6574 7572 6e20 5265 7363 616c  ): return Rescal
-000095f0: 6528 312f 7365 6c66 2e73 6361 6c65 2c20  e(1/self.scale, 
-00009600: 7265 7369 7a65 5f69 6d61 6765 203d 2073  resize_image = s
-00009610: 656c 662e 7265 7369 7a65 5f69 6d61 6765  elf.resize_image
-00009620: 292e 6261 636b 7761 7264 5f28 7365 6c66  ).backward_(self
-00009630: 2e62 6163 6b77 6172 6429 0a0a 4061 6c69  .backward)..@ali
-00009640: 6173 2822 5472 616e 736c 6174 6522 290a  as("Translate").
-00009650: 636c 6173 7320 5472 616e 736c 6174 696f  class Translatio
-00009660: 6e28 5370 6174 6961 6c54 7261 6e73 666f  n(SpatialTransfo
-00009670: 726d 6174 696f 6e29 3a0a 2020 2020 6465  rmation):.    de
-00009680: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00009690: 202a 7472 616e 736c 6174 696f 6e29 3a0a   *translation):.
-000096a0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000096b0: 2020 2020 5472 616e 736c 6174 6520 616e      Translate an
-000096c0: 2069 6d61 6765 2e0a 2020 2020 2020 2020   image..        
-000096d0: 0a20 2020 2020 2020 204e 6f74 653a 2054  .        Note: T
-000096e0: 6865 2074 7261 6e73 6c61 7469 6f6e 2069  he translation i
-000096f0: 7320 666f 7220 636f 6f72 6469 6e61 7465  s for coordinate
-00009700: 732c 2068 656e 6365 2074 6865 2069 6d61  s, hence the ima
-00009710: 6765 2077 6f75 6c64 2067 6f20 696e 2074  ge would go in t
-00009720: 6865 206f 7070 6f73 6974 6520 6469 7265  he opposite dire
-00009730: 6374 696f 6e2e 200a 2020 2020 2020 2020  ction. .        
-00009740: 0a20 2020 2020 2020 2050 6172 616d 733a  .        Params:
-00009750: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00009760: 6e73 6c61 7469 6f6e 205b 7475 706c 6520  nslation [tuple 
-00009770: 6f72 2062 742e 5465 6e73 6f72 5d3a 2054  or bt.Tensor]: T
-00009780: 6865 2074 7261 6e73 6c61 7469 6f6e 206f  he translation o
-00009790: 6620 7468 6520 636f 6f72 6469 6e61 7465  f the coordinate
-000097a0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-000097b0: 2020 2073 697a 653a 206c 656e 6774 6828     size: length(
-000097c0: 6e5f 6469 6d29 206f 7220 285b 6e5f 6261  n_dim) or ([n_ba
-000097d0: 7463 683a 6f70 7469 6f6e 616c 5d2c 207b  tch:optional], {
-000097e0: 6e5f 6469 6d7d 290a 2020 2020 2020 2020  n_dim}).        
-000097f0: 2020 2020 0a20 2020 2020 2020 2057 6865      .        Whe
-00009800: 6e20 6974 2069 7320 6361 6c6c 6564 3a0a  n it is called:.
-00009810: 2020 2020 2020 2020 2020 2020 5820 5b62              X [b
-00009820: 742e 5465 6e73 6f72 5d3a 2043 6f6f 7264  t.Tensor]: Coord
-00009830: 696e 6174 6573 2074 6f20 6265 2074 7261  inates to be tra
-00009840: 6e73 666f 726d 6564 2e0a 2020 2020 2020  nsformed..      
-00009850: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00009860: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
-00009870: 616c 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f  al], {n_dim}, n_
-00009880: 312c 206e 5f32 2c20 2e2e 2e2c 206e 5f72  1, n_2, ..., n_r
-00009890: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
-000098a0: 7470 7574 205b 6274 2e54 656e 736f 725d  tput [bt.Tensor]
-000098b0: 3a20 5468 6520 7472 616e 7366 6f72 6d65  : The transforme
-000098c0: 6420 636f 6f72 6469 6e61 7465 732e 0a20  d coordinates.. 
-000098d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000098e0: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
-000098f0: 207b 6e5f 6469 6d7d 2c20 6e5f 312c 206e   {n_dim}, n_1, n
-00009900: 5f32 2c20 2e2e 2e2c 206e 5f72 290a 2020  _2, ..., n_r).  
-00009910: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00009920: 2020 6966 206c 656e 2874 7261 6e73 6c61    if len(transla
-00009930: 7469 6f6e 2920 3d3d 2031 3a20 7472 616e  tion) == 1: tran
-00009940: 736c 6174 696f 6e20 3d20 7472 616e 736c  slation = transl
-00009950: 6174 696f 6e5b 305d 0a20 2020 2020 2020  ation[0].       
-00009960: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
-00009970: 7261 6e73 6c61 7469 6f6e 2c20 7475 706c  ranslation, tupl
-00009980: 6529 3a20 7472 616e 736c 6174 696f 6e20  e): translation 
-00009990: 3d20 6c69 7374 2874 7261 6e73 6c61 7469  = list(translati
-000099a0: 6f6e 290a 2020 2020 2020 2020 7472 616e  on).        tran
-000099b0: 736c 6174 696f 6e20 3d20 6261 746f 7263  slation = batorc
-000099c0: 685f 7465 6e73 6f72 2874 7261 6e73 6c61  h_tensor(transla
-000099d0: 7469 6f6e 292e 7371 7565 657a 6528 290a  tion).squeeze().
-000099e0: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
-000099f0: 6c61 7469 6f6e 2e6e 5f64 696d 203c 3d20  lation.n_dim <= 
-00009a00: 313a 2074 7261 6e73 6c61 7469 6f6e 203d  1: translation =
-00009a10: 2074 7261 6e73 6c61 7469 6f6e 2e75 6e73   translation.uns
-00009a20: 7175 6565 7a65 285b 5d29 0a20 2020 2020  queeze([]).     
-00009a30: 2020 2069 6620 7472 616e 736c 6174 696f     if translatio
-00009a40: 6e2e 6e5f 6469 6d20 3d3d 2032 3a0a 2020  n.n_dim == 2:.  
-00009a50: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00009a60: 2074 7261 6e73 6c61 7469 6f6e 2e68 6173   translation.has
-00009a70: 5f62 6174 6368 3a20 7472 616e 736c 6174  _batch: translat
-00009a80: 696f 6e2e 6261 7463 685f 6469 6d65 6e73  ion.batch_dimens
-00009a90: 696f 6e20 3d20 300a 2020 2020 2020 2020  ion = 0.        
-00009aa0: 2020 2020 6966 206e 6f74 2074 7261 6e73      if not trans
-00009ab0: 6c61 7469 6f6e 2e68 6173 5f63 6861 6e6e  lation.has_chann
-00009ac0: 656c 3a20 7472 616e 736c 6174 696f 6e2e  el: translation.
-00009ad0: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
-00009ae0: 6e20 3d20 3020 6966 2074 7261 6e73 6c61  n = 0 if transla
-00009af0: 7469 6f6e 2e62 6174 6368 5f64 696d 656e  tion.batch_dimen
-00009b00: 7369 6f6e 203e 2030 2065 6c73 6520 310a  sion > 0 else 1.
-00009b10: 2020 2020 2020 2020 6176 6f75 6368 2874          avouch(t
-00009b20: 7261 6e73 6c61 7469 6f6e 2e68 6173 5f62  ranslation.has_b
-00009b30: 6174 6368 2061 6e64 2074 7261 6e73 6c61  atch and transla
-00009b40: 7469 6f6e 2e68 6173 5f63 6861 6e6e 656c  tion.has_channel
-00009b50: 2c20 6622 506c 6561 7365 2075 7365 2062  , f"Please use b
-00009b60: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
-00009b70: 2073 697a 6520 5c0a 2020 2020 2020 2020   size \.        
-00009b80: 2020 2020 285b 6e5f 6261 7463 683a 6f70      ([n_batch:op
-00009b90: 7469 6f6e 616c 5d2c 207b 7b6e 5f64 696d  tional], {{n_dim
-00009ba0: 7d7d 2920 666f 7220 5472 616e 736c 6174  }}) for Translat
-00009bb0: 696f 6e20 7061 7261 6d65 7465 7273 2c20  ion parameters, 
-00009bc0: 696e 7374 6561 6420 6f66 207b 7472 616e  instead of {tran
-00009bd0: 736c 6174 696f 6e2e 7368 6170 657d 2e20  slation.shape}. 
-00009be0: 2229 0a20 2020 2020 2020 2073 7570 6572  ").        super
-00009bf0: 2829 2e5f 5f69 6e69 745f 5f28 7472 616e  ().__init__(tran
-00009c00: 736c 6174 696f 6e29 0a0a 2020 2020 2020  slation)..      
-00009c10: 2020 7365 6c66 2e74 7261 6e73 6c61 7469    self.translati
-00009c20: 6f6e 203d 2074 7261 6e73 6c61 7469 6f6e  on = translation
-00009c30: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
-00009c40: 6469 6d20 3d20 7365 6c66 2e74 7261 6e73  dim = self.trans
-00009c50: 6c61 7469 6f6e 2e6e 5f63 6861 6e6e 656c  lation.n_channel
-00009c60: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
-00009c70: 7463 685f 7061 7261 6d2e 6170 7065 6e64  tch_param.append
-00009c80: 2827 7472 616e 736c 6174 696f 6e27 290a  ('translation').
-00009c90: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
-00009ca0: 5f28 7365 6c66 2c20 5829 3a0a 2020 2020  _(self, X):.    
-00009cb0: 2020 2020 5820 3d20 7375 7065 7228 292e      X = super().
-00009cc0: 5f5f 6361 6c6c 5f5f 2858 290a 2020 2020  __call__(X).    
-00009cd0: 2020 2020 7265 7475 726e 2058 202b 2073      return X + s
-00009ce0: 656c 662e 7472 616e 736c 6174 696f 6e0a  elf.translation.
-00009cf0: 2020 2020 0a20 2020 2064 6566 2061 6666      .    def aff
-00009d00: 696e 6528 7365 6c66 2c20 6e5f 6469 6d3d  ine(self, n_dim=
-00009d10: 4e6f 6e65 293a 0a20 2020 2020 2020 2061  None):.        a
-00009d20: 766f 7563 6828 6e5f 6469 6d20 6973 204e  vouch(n_dim is N
-00009d30: 6f6e 6520 6f72 2073 656c 662e 6e5f 6469  one or self.n_di
-00009d40: 6d20 3d3d 206e 5f64 696d 290a 2020 2020  m == n_dim).    
-00009d50: 2020 2020 6966 206e 5f64 696d 2069 7320      if n_dim is 
-00009d60: 4e6f 6e65 3a20 6e5f 6469 6d20 3d20 7365  None: n_dim = se
-00009d70: 6c66 2e6e 5f64 696d 0a20 2020 2020 2020  lf.n_dim.       
-00009d80: 206e 5f62 6174 6368 203d 2073 656c 662e   n_batch = self.
-00009d90: 7472 616e 736c 6174 696f 6e2e 6e5f 6261  translation.n_ba
-00009da0: 7463 680a 2020 2020 2020 2020 7265 7475  tch.        retu
-00009db0: 726e 2062 742e 6361 7428 6274 2e63 6174  rn bt.cat(bt.cat
-00009dc0: 2862 742e 6579 6528 7365 6c66 2e6e 5f64  (bt.eye(self.n_d
-00009dd0: 696d 292e 6d75 6c74 6970 6c79 286e 5f62  im).multiply(n_b
-00009de0: 6174 6368 2c20 5b5d 292c 2073 656c 662e  atch, []), self.
-00009df0: 7472 616e 736c 6174 696f 6e2e 7769 7468  translation.with
-00009e00: 5f63 6861 6e6e 656c 6469 6d28 4e6f 6e65  _channeldim(None
-00009e10: 292e 756e 7371 7565 657a 6528 2d31 292c  ).unsqueeze(-1),
-00009e20: 202d 3129 2c20 6274 2e6f 6e65 5f68 6f74   -1), bt.one_hot
-00009e30: 282d 312c 206e 5f64 696d 2b31 292e 756e  (-1, n_dim+1).un
-00009e40: 7371 7565 657a 6528 3029 2e6d 756c 7469  squeeze(0).multi
-00009e50: 706c 7928 6e5f 6261 7463 682c 205b 5d29  ply(n_batch, [])
-00009e60: 2c20 3129 0a0a 2020 2020 6465 6620 696e  , 1)..    def in
-00009e70: 7628 7365 6c66 293a 2072 6574 7572 6e20  v(self): return 
-00009e80: 5472 616e 736c 6174 6528 2d73 656c 662e  Translate(-self.
-00009e90: 7472 616e 736c 6174 696f 6e29 2e62 6163  translation).bac
-00009ea0: 6b77 6172 645f 2873 656c 662e 6261 636b  kward_(self.back
-00009eb0: 7761 7264 290a 0a40 616c 6961 7328 2252  ward)..@alias("R
-00009ec0: 6967 2229 0a63 6c61 7373 2052 6967 6964  ig").class Rigid
-00009ed0: 2853 7061 7469 616c 5472 616e 7366 6f72  (SpatialTransfor
-00009ee0: 6d61 7469 6f6e 293a 0a20 2020 2064 6566  mation):.    def
-00009ef0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00009f00: 616e 676c 652c 2061 7869 733d 4e6f 6e65  angle, axis=None
-00009f10: 2c20 7472 616e 736c 6174 696f 6e3d 4e6f  , translation=No
-00009f20: 6e65 2c20 6365 6e74 6572 3d4e 6f6e 652c  ne, center=None,
-00009f30: 2074 7261 6e73 5f73 7472 6574 6368 3d4e   trans_stretch=N
-00009f40: 6f6e 652c 2073 7061 6369 6e67 3d31 293a  one, spacing=1):
-00009f50: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00009f60: 2020 2020 2052 6967 6964 2074 7261 6e73       Rigid trans
-00009f70: 666f 726d 6174 696f 6e20 7769 7468 2072  formation with r
-00009f80: 6573 7065 6374 2074 6f20 7061 7261 6d65  espect to parame
-00009f90: 7465 7273 2e0a 2020 2020 2020 2020 0a20  ters..        . 
-00009fa0: 2020 2020 2020 2050 6172 616d 7320 5365         Params Se
-00009fb0: 7420 313a 0a20 2020 2020 2020 2020 2020  t 1:.           
-00009fc0: 2061 6e67 6c65 205b 6274 2e54 656e 736f   angle [bt.Tenso
-00009fd0: 7220 6f72 206e 702e 6e75 6d70 795d 3a20  r or np.numpy]: 
-00009fe0: 7468 6520 5b63 6c6f 636b 7769 7365 5d20  the [clockwise] 
-00009ff0: 726f 7461 7469 6f6e 2061 6e67 6c65 7320  rotation angles 
-0000a000: 6162 6f75 7420 7468 6520 6178 6973 6573  about the axises
-0000a010: 2028 6f72 207a 2064 6972 6563 7469 6f6e   (or z direction
-0000a020: 2066 6f72 2032 4429 2e20 4974 2069 7320   for 2D). It is 
-0000a030: 636f 756e 7465 722d 636c 6f63 6b77 6973  counter-clockwis
-0000a040: 6520 666f 7220 696d 6167 652e 0a20 2020  e for image..   
-0000a050: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-0000a060: 653a 2028 5b6e 5f62 6174 6368 5d2c 290a  e: ([n_batch],).
-0000a070: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-0000a080: 205b 6274 2e54 656e 736f 7220 6f72 206e   [bt.Tensor or n
-0000a090: 702e 6e75 6d70 795d 3a20 7468 6520 726f  p.numpy]: the ro
-0000a0a0: 7461 7469 6f6e 2061 7869 7365 732c 206e  tation axises, n
-0000a0b0: 6f72 6d61 6c69 7a65 6420 7665 6374 6f72  ormalized vector
-0000a0c0: 732c 204e 6f6e 6520 666f 7220 3244 2e20  s, None for 2D. 
-0000a0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a0e0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-0000a0f0: 5d2c 207b 6e5f 6469 6d7d 290a 2020 2020  ], {n_dim}).    
-0000a100: 2020 2020 2020 2020 7472 616e 736c 6174          translat
-0000a110: 696f 6e20 5b62 742e 5465 6e73 6f72 206f  ion [bt.Tensor o
-0000a120: 7220 6e70 2e6e 756d 7079 5d3a 2074 6865  r np.numpy]: the
-0000a130: 2074 7261 6e73 6c61 7469 6f6e 7320 6166   translations af
-0000a140: 7465 7220 7468 6520 726f 7461 7469 6f6e  ter the rotation
-0000a150: 2c20 7a65 726f 7320 6279 2064 6566 6175  , zeros by defau
-0000a160: 6c74 2e20 0a20 2020 2020 2020 2020 2020  lt. .           
-0000a170: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
-0000a180: 6174 6368 5d2c 207b 6e5f 6469 6d7d 290a  atch], {n_dim}).
-0000a190: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
-0000a1a0: 6572 205b 6274 2e54 656e 736f 7220 6f72  er [bt.Tensor or
-0000a1b0: 206e 702e 6e75 6d70 795d 3a20 7468 6520   np.numpy]: the 
-0000a1c0: 6365 6e74 6572 2066 6f72 2074 6865 2072  center for the r
-0000a1d0: 6f74 6174 696f 6e73 2c20 7a65 726f 7320  otations, zeros 
-0000a1e0: 6279 2064 6566 6175 6c74 2e20 0a20 2020  by default. .   
-0000a1f0: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-0000a200: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
-0000a210: 6e5f 6469 6d7d 290a 2020 2020 2020 2020  n_dim}).        
-0000a220: 2020 2020 7472 616e 735f 7374 7265 7463      trans_stretc
-0000a230: 6820 5b69 6e74 5d3a 206f 6e6c 7920 7573  h [int]: only us
-0000a240: 6564 2066 6f72 2069 7465 7261 7469 7665  ed for iterative
-0000a250: 2070 6172 616d 6574 6572 2074 7261 696e   parameter train
-0000a260: 696e 672c 2031 2062 7920 6465 6661 756c  ing, 1 by defaul
-0000a270: 742e 2032 3020 7365 656d 7320 746f 2062  t. 20 seems to b
-0000a280: 6520 6120 676f 6f64 2063 686f 6963 652e  e a good choice.
-0000a290: 200a 2020 2020 2020 2020 2020 2020 7370   .            sp
-0000a2a0: 6163 696e 6720 5b74 7570 6c65 5d3a 2074  acing [tuple]: t
-0000a2b0: 6865 2073 7061 6369 6e67 206f 6620 7468  he spacing of th
-0000a2c0: 6520 7472 616e 7366 6f72 6d65 6420 0a20  e transformed . 
-0000a2d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000a2e0: 5061 7261 6d73 2053 6574 2032 3a0a 2020  Params Set 2:.  
-0000a2f0: 2020 2020 2020 2020 2020 6d61 7472 6978            matrix
-0000a300: 205b 6274 2e54 656e 736f 7220 6f72 206e   [bt.Tensor or n
-0000a310: 702e 6e75 6d70 795d 3a20 7468 6520 6166  p.numpy]: the af
-0000a320: 6669 6e65 206d 6174 7269 782c 2069 7420  fine matrix, it 
-0000a330: 7368 6f75 6c64 2062 6520 6f72 7468 6f67  should be orthog
-0000a340: 6f6e 616c 206f 7220 7769 6c6c 2062 6520  onal or will be 
-0000a350: 7072 6f6a 6563 7465 6420 6279 2050 726f  projected by Pro
-0000a360: 6372 7573 7465 7320 5072 6f62 6c65 6d2e  crustes Problem.
-0000a370: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000a380: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-0000a390: 685d 2c20 6e5f 6469 6d20 2b20 312c 206e  h], n_dim + 1, n
-0000a3a0: 5f64 696d 202b 2031 290a 2020 2020 2020  _dim + 1).      
-0000a3b0: 2020 2020 2020 7472 616e 735f 7374 7265        trans_stre
-0000a3c0: 7463 6820 5b69 6e74 5d3a 206f 6e6c 7920  tch [int]: only 
-0000a3d0: 7573 6564 2066 6f72 2069 7465 7261 7469  used for iterati
-0000a3e0: 7665 2070 6172 616d 6574 6572 2074 7261  ve parameter tra
-0000a3f0: 696e 696e 672c 2031 2062 7920 6465 6661  ining, 1 by defa
-0000a400: 756c 742e 2032 3020 7365 656d 7320 746f  ult. 20 seems to
-0000a410: 2062 6520 6120 676f 6f64 2063 686f 6963   be a good choic
-0000a420: 652e 200a 2020 2020 2020 2020 2020 2020  e. .            
-0000a430: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
-0000a440: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
-0000a450: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
-0000a460: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
-0000a470: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
-0000a480: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
-0000a490: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
-0000a4a0: 6261 7463 683a 206f 7074 696f 6e61 6c5d  batch: optional]
-0000a4b0: 2c20 7b6e 5f64 696d 7d2c 206e 5f31 2c20  , {n_dim}, n_1, 
-0000a4c0: 6e5f 322c 202e 2e2e 2c20 6e5f 7229 0a20  n_2, ..., n_r). 
-0000a4d0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-0000a4e0: 7420 5b62 742e 5465 6e73 6f72 5d3a 2054  t [bt.Tensor]: T
-0000a4f0: 6865 2074 7261 6e73 666f 726d 6564 2063  he transformed c
-0000a500: 6f6f 7264 696e 6174 6573 2e0a 2020 2020  oordinates..    
-0000a510: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-0000a520: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
-0000a530: 5f64 696d 7d2c 206e 5f31 2c20 6e5f 322c  _dim}, n_1, n_2,
-0000a540: 202e 2e2e 2c20 6e5f 7229 0a20 2020 2020   ..., n_r).     
-0000a550: 2020 2027 2727 0a20 2020 2020 2020 2061     '''.        a
-0000a560: 6e67 6c65 203d 2062 6174 6f72 6368 5f74  ngle = batorch_t
-0000a570: 656e 736f 7228 616e 676c 6529 0a20 2020  ensor(angle).   
-0000a580: 2020 2020 2069 6620 616e 676c 652e 6e5f       if angle.n_
-0000a590: 6469 6d20 3c3d 2030 2061 6e64 206e 6f74  dim <= 0 and not
-0000a5a0: 2061 6e67 6c65 2e68 6173 5f62 6174 6368   angle.has_batch
-0000a5b0: 3a20 616e 676c 6520 3d20 616e 676c 652e  : angle = angle.
-0000a5c0: 756e 7371 7565 657a 6528 5b5d 290a 2020  unsqueeze([]).  
-0000a5d0: 2020 2020 2020 6966 2061 6e67 6c65 2e6e        if angle.n
-0000a5e0: 5f64 696d 203d 3d20 3120 616e 6420 6e6f  _dim == 1 and no
-0000a5f0: 7420 616e 676c 652e 6861 735f 6261 7463  t angle.has_batc
-0000a600: 683a 2061 6e67 6c65 203d 2061 6e67 6c65  h: angle = angle
-0000a610: 2e77 6974 685f 6261 7463 6864 696d 2830  .with_batchdim(0
-0000a620: 290a 2020 2020 2020 2020 6966 2061 6e67  ).        if ang
-0000a630: 6c65 2e6e 5f64 696d 203d 3d20 3220 616e  le.n_dim == 2 an
-0000a640: 6420 6e6f 7420 616e 676c 652e 6861 735f  d not angle.has_
-0000a650: 6261 7463 683a 2061 6e67 6c65 203d 2061  batch: angle = a
-0000a660: 6e67 6c65 2e75 6e73 7175 6565 7a65 285b  ngle.unsqueeze([
-0000a670: 5d29 0a20 2020 2020 2020 2069 6620 616e  ]).        if an
-0000a680: 676c 652e 6e5f 6469 6d20 3d3d 2033 2061  gle.n_dim == 3 a
-0000a690: 6e64 206e 6f74 2061 6e67 6c65 2e68 6173  nd not angle.has
-0000a6a0: 5f62 6174 6368 2061 6e64 2061 6e67 6c65  _batch and angle
-0000a6b0: 2e73 6861 7065 5b31 5d20 3d3d 2061 6e67  .shape[1] == ang
-0000a6c0: 6c65 2e73 6861 7065 5b32 5d3a 2061 6e67  le.shape[2]: ang
-0000a6d0: 6c65 2e62 6174 6368 5f64 696d 656e 7369  le.batch_dimensi
-0000a6e0: 6f6e 203d 2030 0a20 2020 2020 2020 2061  on = 0.        a
-0000a6f0: 766f 7563 6828 616e 676c 652e 6861 735f  vouch(angle.has_
-0000a700: 6261 7463 682c 2066 2250 6c65 6173 6520  batch, f"Please 
-0000a710: 7573 6520 6261 746f 7263 6820 7465 6e73  use batorch tens
-0000a720: 6f72 206f 6620 7369 7a65 2028 5b6e 5f62  or of size ([n_b
-0000a730: 6174 6368 5d2c 2920 666f 7220 5269 6769  atch],) for Rigi
-0000a740: 6420 726f 7461 7469 6f6e 2061 6e67 6c65  d rotation angle
-0000a750: 732c 2069 6e73 7465 6164 206f 6620 7b61  s, instead of {a
-0000a760: 6e67 6c65 2e73 6861 7065 7d2e 2022 290a  ngle.shape}. ").
-0000a770: 2020 2020 2020 2020 6e5f 6261 7463 6820          n_batch 
-0000a780: 3d20 616e 676c 652e 6e5f 6261 7463 680a  = angle.n_batch.
-0000a790: 2020 2020 2020 2020 6e5f 6469 6d20 3d20          n_dim = 
-0000a7a0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-0000a7b0: 616e 676c 652e 6e5f 6469 6d20 3e3d 2032  angle.n_dim >= 2
-0000a7c0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-0000a7d0: 7472 6978 203d 2061 6e67 6c65 0a20 2020  trix = angle.   
-0000a7e0: 2020 2020 2020 2020 206e 5f64 696d 203d           n_dim =
-0000a7f0: 206d 6174 7269 782e 7369 7a65 282d 3129   matrix.size(-1)
-0000a800: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
-0000a810: 2063 656e 7465 7220 3d20 6274 2e7a 6572   center = bt.zer
-0000a820: 6f73 285b 6e5f 6261 7463 685d 2c20 7b6e  os([n_batch], {n
-0000a830: 5f64 696d 7d29 0a20 2020 2020 2020 2020  _dim}).         
-0000a840: 2020 2074 7261 6e73 6c61 7469 6f6e 203d     translation =
-0000a850: 206d 6174 7269 785b 2e2e 2e2c 203a 2d31   matrix[..., :-1
-0000a860: 2c20 2d31 5d2e 7769 7468 5f63 6861 6e6e  , -1].with_chann
-0000a870: 656c 6469 6d28 3129 0a20 2020 2020 2020  eldim(1).       
-0000a880: 2020 2020 2041 203d 206d 6174 7269 785b       A = matrix[
-0000a890: 2e2e 2e2c 203a 2d31 2c20 3a2d 315d 0a20  ..., :-1, :-1]. 
-0000a8a0: 2020 2020 2020 2020 2020 2061 766f 7563             avouc
-0000a8b0: 6828 6274 2e6e 6f72 6d28 412e 5420 4020  h(bt.norm(A.T @ 
-0000a8c0: 4120 2d20 6274 2e65 7965 2841 2929 2e73  A - bt.eye(A)).s
-0000a8d0: 756d 2829 203c 2031 652d 342c 2022 506c  um() < 1e-4, "Pl
-0000a8e0: 6561 7365 206d 616b 6520 7375 7265 2074  ease make sure t
-0000a8f0: 6861 7420 6d61 7472 6978 2069 6e70 7574  hat matrix input
-0000a900: 2066 6f72 2052 6967 6964 2069 7320 6f72   for Rigid is or
-0000a910: 7468 6f67 6f6e 616c 2e20 5573 6520 4166  thogonal. Use Af
-0000a920: 6669 6e65 2069 6e73 7465 6164 2069 6620  fine instead if 
-0000a930: 6974 2069 7320 6e6f 742e 2022 290a 2020  it is not. ").  
-0000a940: 2020 2020 2020 2020 2020 2320 4920 3d20            # I = 
-0000a950: 6274 2e65 7965 2841 290a 2020 2020 2020  bt.eye(A).      
-0000a960: 2020 2020 2020 2320 5a5f 6c65 6674 203d        # Z_left =
-0000a970: 2028 4120 2d20 4929 5b2e 2e2e 2c20 3a2d   (A - I)[..., :-
-0000a980: 315d 2023 2028 5b6e 5f62 6174 6368 5d2c  1] # ([n_batch],
-0000a990: 206e 5f64 696d 2c20 6e5f 6469 6d2d 3129   n_dim, n_dim-1)
-0000a9a0: 0a20 2020 2020 2020 2020 2020 2023 205a  .            # Z
-0000a9b0: 5f72 6967 6874 203d 2028 4120 2d20 4929  _right = (A - I)
-0000a9c0: 5b2e 2e2e 2c20 2d31 5d20 2320 285b 6e5f  [..., -1] # ([n_
-0000a9d0: 6261 7463 685d 2c20 6e5f 6469 6d29 0a20  batch], n_dim). 
-0000a9e0: 2020 2020 2020 2020 2020 2023 205a 545a             # ZTZ
-0000a9f0: 203d 205a 5f6c 6566 742e 5420 4020 5a5f   = Z_left.T @ Z_
-0000aa00: 6c65 6674 0a20 2020 2020 2020 2020 2020  left.           
-0000aa10: 2023 2069 6620 6e5f 6469 6d20 3d3d 2032   # if n_dim == 2
-0000aa20: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000aa30: 2020 2020 6178 6973 203d 204e 6f6e 650a      axis = None.
-0000aa40: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000aa50: 2020 616e 676c 6520 3d20 6274 2e77 6865    angle = bt.whe
-0000aa60: 7265 2862 742e 6162 7328 6274 2e64 6574  re(bt.abs(bt.det
-0000aa70: 285a 545a 2929 203c 2031 652d 362c 2062  (ZTZ)) < 1e-6, b
-0000aa80: 742e 7a65 726f 7328 5b6e 5f62 6174 6368  t.zeros([n_batch
-0000aa90: 5d29 2c20 6274 2e61 636f 7328 3120 2d20  ]), bt.acos(1 - 
-0000aaa0: 5a54 5a20 2f20 3229 2e73 7175 6565 7a65  ZTZ / 2).squeeze
-0000aab0: 282d 312c 202d 3129 290a 2020 2020 2020  (-1, -1)).      
-0000aac0: 2020 2020 2020 2320 656c 6966 206e 5f64        # elif n_d
-0000aad0: 696d 203d 3d20 333a 0a20 2020 2020 2020  im == 3:.       
-0000aae0: 2020 2020 2023 2020 2020 2069 6e76 5a54       #     invZT
-0000aaf0: 5a20 3d20 6274 2e69 6e76 2862 742e 7768  Z = bt.inv(bt.wh
-0000ab00: 6572 6528 6274 2e61 6273 2862 742e 6465  ere(bt.abs(bt.de
-0000ab10: 7428 5a54 5a29 292e 756e 7371 7565 657a  t(ZTZ)).unsqueez
-0000ab20: 6528 2d31 2c20 2d31 2920 3c20 3165 2d36  e(-1, -1) < 1e-6
-0000ab30: 2c20 6274 2e65 7965 285a 545a 292c 205a  , bt.eye(ZTZ), Z
-0000ab40: 545a 2929 0a20 2020 2020 2020 2020 2020  TZ)).           
-0000ab50: 2023 2020 2020 2076 6563 746f 7220 3d20   #     vector = 
-0000ab60: 6274 2e63 6174 282d 2069 6e76 5a54 5a20  bt.cat(- invZTZ 
-0000ab70: 4020 5a5f 6c65 6674 2e54 2040 205a 5f72  @ Z_left.T @ Z_r
-0000ab80: 6967 6874 2c20 6274 2e6f 6e65 7328 5b6e  ight, bt.ones([n
-0000ab90: 5f62 6174 6368 5d2c 2031 292c 2031 292e  _batch], 1), 1).
-0000aba0: 7769 7468 5f63 6861 6e6e 656c 6469 6d28  with_channeldim(
-0000abb0: 3129 0a20 2020 2020 2020 2020 2020 2023  1).            #
-0000abc0: 2020 2020 2061 6e67 6c65 203d 2062 742e       angle = bt.
-0000abd0: 7768 6572 6528 6274 2e61 6273 2862 742e  where(bt.abs(bt.
-0000abe0: 6465 7428 5a54 5a29 2920 3c20 3165 2d36  det(ZTZ)) < 1e-6
-0000abf0: 2c20 6274 2e7a 6572 6f73 285b 6e5f 6261  , bt.zeros([n_ba
-0000ac00: 7463 685d 292c 2076 6563 746f 722e 6e6f  tch]), vector.no
-0000ac10: 726d 2829 290a 2020 2020 2020 2020 2020  rm()).          
-0000ac20: 2020 2320 2020 2020 6178 6973 203d 2062    #     axis = b
-0000ac30: 742e 7768 6572 6528 2862 742e 6162 7328  t.where((bt.abs(
-0000ac40: 6274 2e64 6574 285a 545a 2929 203c 2031  bt.det(ZTZ)) < 1
-0000ac50: 652d 3629 2e6d 756c 7469 706c 7928 6e5f  e-6).multiply(n_
-0000ac60: 6469 6d2c 207b 7d29 2c20 6274 2e63 6861  dim, {}), bt.cha
-0000ac70: 6e6e 656c 5f74 656e 736f 7228 6274 2e6f  nnel_tensor(bt.o
-0000ac80: 6e65 5f68 6f74 2830 2c20 6e5f 6469 6d29  ne_hot(0, n_dim)
-0000ac90: 292e 6d75 6c74 6970 6c79 286e 5f62 6174  ).multiply(n_bat
-0000aca0: 6368 2c20 5b5d 292c 2076 6563 746f 7220  ch, []), vector 
-0000acb0: 2f20 616e 676c 6529 0a20 2020 2020 2020  / angle).       
-0000acc0: 2020 2020 2069 6620 6e5f 6469 6d20 3d3d       if n_dim ==
-0000acd0: 2032 3a20 6178 6973 203d 204e 6f6e 653b   2: axis = None;
-0000ace0: 2061 6e67 6c65 203d 2062 742e 6163 6f73   angle = bt.acos
-0000acf0: 2841 5b2e 2e2e 2c20 302c 2030 5d29 0a20  (A[..., 0, 0]). 
-0000ad00: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000ad10: 6e5f 6469 6d20 3d3d 2033 3a0a 2020 2020  n_dim == 3:.    
-0000ad20: 2020 2020 2020 2020 2020 2020 616e 7469              anti
-0000ad30: 5f73 796d 203d 2028 4120 2d20 412e 5429  _sym = (A - A.T)
-0000ad40: 202f 2032 0a20 2020 2020 2020 2020 2020   / 2.           
-0000ad50: 2020 2020 2073 796d 203d 2028 4120 2b20       sym = (A + 
-0000ad60: 412e 5429 202f 2032 202d 2062 742e 6579  A.T) / 2 - bt.ey
-0000ad70: 6528 4129 0a20 2020 2020 2020 2020 2020  e(A).           
-0000ad80: 2020 2020 2061 6e67 6c65 203d 2062 742e       angle = bt.
-0000ad90: 6163 6f73 2828 2861 6e74 695f 7379 6d20  acos(((anti_sym 
-0000ada0: 4020 616e 7469 5f73 796d 2920 2f20 7379  @ anti_sym) / sy
-0000adb0: 6d29 2e6d 6561 6e28 2920 2d20 3129 0a20  m).mean() - 1). 
-0000adc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000add0: 7869 7320 3d20 6274 2e75 6e63 726f 7373  xis = bt.uncross
-0000ade0: 5f6d 6174 7269 7828 616e 7469 5f73 796d  _matrix(anti_sym
-0000adf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ae00: 2020 6178 6973 202f 3d20 6274 2e73 696e    axis /= bt.sin
-0000ae10: 2861 6e67 6c65 290a 2020 2020 2020 2020  (angle).        
-0000ae20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000ae30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000ae40: 4572 726f 7228 224e 6f74 496d 706c 656d  Error("NotImplem
-0000ae50: 656e 7465 6422 2928 6622 5269 6769 6420  ented")(f"Rigid 
-0000ae60: 7472 616e 7366 6f72 6d61 7469 6f6e 2069  transformation i
-0000ae70: 6e20 6d69 636f 6d70 7574 696e 6720 646f  n micomputing do
-0000ae80: 6573 206e 6f74 2073 7570 706f 7274 207b  es not support {
-0000ae90: 6e5f 6469 6d7d 2064 696d 656e 7369 6f6e  n_dim} dimension
-0000aea0: 616c 2074 7261 6e73 666f 726d 7320 2832  al transforms (2
-0000aeb0: 2026 2033 4420 6f6e 6c79 292e 2022 202b   & 3D only). " +
-0000aec0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aee0: 2020 2020 2020 2020 2020 2020 2020 2250                "P
-0000aef0: 6c65 6173 6520 636f 6e74 6163 7420 7468  lease contact th
-0000af00: 6520 6465 7665 6c6f 7065 7273 2069 6620  e developers if 
-0000af10: 7468 6572 6520 6172 6520 6665 6173 6962  there are feasib
-0000af20: 6c65 2061 6c67 6f72 6974 686d 7320 2845  le algorithms (E
-0000af30: 7272 6f72 2043 6f64 653a 2054 3333 3329  rror Code: T333)
-0000af40: 2e20 5468 616e 6b20 796f 752e 2022 290a  . Thank you. ").
-0000af50: 0a20 2020 2020 2020 2069 6620 7472 616e  .        if tran
-0000af60: 736c 6174 696f 6e20 6973 206e 6f74 204e  slation is not N
-0000af70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000af80: 2074 7261 6e73 6c61 7469 6f6e 203d 2062   translation = b
-0000af90: 6174 6f72 6368 5f74 656e 736f 7228 7472  atorch_tensor(tr
-0000afa0: 616e 736c 6174 696f 6e29 0a20 2020 2020  anslation).     
-0000afb0: 2020 2020 2020 2069 6620 7472 616e 736c         if transl
-0000afc0: 6174 696f 6e2e 6e5f 6469 6d20 3c3d 2031  ation.n_dim <= 1
-0000afd0: 2061 6e64 206e 6f74 2074 7261 6e73 6c61   and not transla
-0000afe0: 7469 6f6e 2e68 6173 5f62 6174 6368 3a20  tion.has_batch: 
-0000aff0: 7472 616e 736c 6174 696f 6e20 3d20 7472  translation = tr
-0000b000: 616e 736c 6174 696f 6e2e 756e 7371 7565  anslation.unsque
-0000b010: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
-0000b020: 2020 2020 6966 2074 7261 6e73 6c61 7469      if translati
-0000b030: 6f6e 2e6e 5f64 696d 203d 3d20 3220 616e  on.n_dim == 2 an
-0000b040: 6420 6e6f 7420 7472 616e 736c 6174 696f  d not translatio
-0000b050: 6e2e 6861 735f 6261 7463 683a 2074 7261  n.has_batch: tra
-0000b060: 6e73 6c61 7469 6f6e 203d 2074 7261 6e73  nslation = trans
-0000b070: 6c61 7469 6f6e 2e77 6974 685f 6261 7463  lation.with_batc
-0000b080: 6864 696d 2828 3120 2d20 7472 616e 736c  hdim((1 - transl
-0000b090: 6174 696f 6e2e 6368 616e 6e65 6c5f 6469  ation.channel_di
-0000b0a0: 6d65 6e73 696f 6e29 2069 6620 7472 616e  mension) if tran
-0000b0b0: 736c 6174 696f 6e2e 6861 735f 6368 616e  slation.has_chan
-0000b0c0: 6e65 6c20 656c 7365 2030 290a 2020 2020  nel else 0).    
-0000b0d0: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
-0000b0e0: 6c61 7469 6f6e 2e6e 5f64 696d 203d 3d20  lation.n_dim == 
-0000b0f0: 3220 616e 6420 6e6f 7420 7472 616e 736c  2 and not transl
-0000b100: 6174 696f 6e2e 6861 735f 6368 616e 6e65  ation.has_channe
-0000b110: 6c3a 2074 7261 6e73 6c61 7469 6f6e 203d  l: translation =
-0000b120: 2074 7261 6e73 6c61 7469 6f6e 2e77 6974   translation.wit
-0000b130: 685f 6368 616e 6e65 6c64 696d 2831 202d  h_channeldim(1 -
-0000b140: 2074 7261 6e73 6c61 7469 6f6e 2e62 6174   translation.bat
-0000b150: 6368 5f64 696d 656e 7369 6f6e 290a 2020  ch_dimension).  
-0000b160: 2020 2020 2020 2020 2020 6176 6f75 6368            avouch
-0000b170: 2874 7261 6e73 6c61 7469 6f6e 2e68 6173  (translation.has
-0000b180: 5f62 6174 6368 2061 6e64 2074 7261 6e73  _batch and trans
-0000b190: 6c61 7469 6f6e 2e68 6173 5f63 6861 6e6e  lation.has_chann
-0000b1a0: 656c 2c20 6622 506c 6561 7365 2075 7365  el, f"Please use
-0000b1b0: 2062 6174 6f72 6368 2074 656e 736f 7220   batorch tensor 
-0000b1c0: 6f66 2073 697a 6520 285b 6e5f 6261 7463  of size ([n_batc
-0000b1d0: 685d 2c20 7b7b 6e5f 6469 6d7d 7d29 2066  h], {{n_dim}}) f
-0000b1e0: 6f72 2052 6967 6964 2074 7261 6e73 6c61  or Rigid transla
-0000b1f0: 7469 6f6e 2c20 696e 7374 6561 6420 6f66  tion, instead of
-0000b200: 207b 7472 616e 736c 6174 696f 6e2e 7368   {translation.sh
-0000b210: 6170 657d 2e20 2229 0a20 2020 2020 2020  ape}. ").       
-0000b220: 2020 2020 2069 6620 6e5f 6261 7463 6820       if n_batch 
-0000b230: 3d3d 2031 2061 6e64 2074 7261 6e73 6c61  == 1 and transla
-0000b240: 7469 6f6e 2e6e 5f62 6174 6368 203e 2031  tion.n_batch > 1
-0000b250: 3a20 6e5f 6261 7463 6820 3d20 7472 616e  : n_batch = tran
-0000b260: 736c 6174 696f 6e2e 6e5f 6261 7463 680a  slation.n_batch.
-0000b270: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000b280: 5f64 696d 2069 7320 4e6f 6e65 3a20 6e5f  _dim is None: n_
-0000b290: 6469 6d20 3d20 7472 616e 736c 6174 696f  dim = translatio
-0000b2a0: 6e2e 6e5f 6368 616e 6e65 6c0a 2020 2020  n.n_channel.    
-0000b2b0: 2020 2020 2020 2020 656c 7365 3a20 6176          else: av
-0000b2c0: 6f75 6368 286e 5f64 696d 203d 3d20 7472  ouch(n_dim == tr
-0000b2d0: 616e 736c 6174 696f 6e2e 6e5f 6368 616e  anslation.n_chan
-0000b2e0: 6e65 6c2c 2022 5379 7374 656d 6174 6963  nel, "Systematic
-0000b2f0: 2065 7272 6f72 2e20 506c 6561 7365 2063   error. Please c
-0000b300: 6f6e 7461 6374 2074 6865 2064 6576 656c  ontact the devel
-0000b310: 6f70 6572 7320 666f 7220 6465 7461 696c  opers for detail
-0000b320: 7320 2845 7272 6f72 2043 6f64 653a 2054  s (Error Code: T
-0000b330: 3333 3229 2e20 2229 0a20 2020 2020 2020  332). ").       
-0000b340: 2020 2020 206e 5f64 696d 203d 2074 7261       n_dim = tra
-0000b350: 6e73 6c61 7469 6f6e 2e6e 5f63 6861 6e6e  nslation.n_chann
-0000b360: 656c 0a20 2020 2020 2020 2069 6620 6365  el.        if ce
-0000b370: 6e74 6572 2069 7320 6e6f 7420 4e6f 6e65  nter is not None
-0000b380: 3a0a 2020 2020 2020 2020 2020 2020 6365  :.            ce
-0000b390: 6e74 6572 203d 2062 6174 6f72 6368 5f74  nter = batorch_t
-0000b3a0: 656e 736f 7228 6365 6e74 6572 290a 2020  ensor(center).  
-0000b3b0: 2020 2020 2020 2020 2020 6966 2063 656e            if cen
-0000b3c0: 7465 722e 6e5f 6469 6d20 3c3d 2031 2061  ter.n_dim <= 1 a
-0000b3d0: 6e64 206e 6f74 2063 656e 7465 722e 6861  nd not center.ha
-0000b3e0: 735f 6261 7463 683a 2063 656e 7465 7220  s_batch: center 
-0000b3f0: 3d20 6365 6e74 6572 2e75 6e73 7175 6565  = center.unsquee
-0000b400: 7a65 285b 5d29 0a20 2020 2020 2020 2020  ze([]).         
-0000b410: 2020 2069 6620 6365 6e74 6572 2e6e 5f64     if center.n_d
-0000b420: 696d 203d 3d20 3220 616e 6420 6e6f 7420  im == 2 and not 
-0000b430: 6365 6e74 6572 2e68 6173 5f62 6174 6368  center.has_batch
-0000b440: 3a20 6365 6e74 6572 203d 2063 656e 7465  : center = cente
-0000b450: 722e 7769 7468 5f62 6174 6368 6469 6d28  r.with_batchdim(
-0000b460: 2831 202d 2063 656e 7465 722e 6368 616e  (1 - center.chan
-0000b470: 6e65 6c5f 6469 6d65 6e73 696f 6e29 2069  nel_dimension) i
-0000b480: 6620 6365 6e74 6572 2e68 6173 5f63 6861  f center.has_cha
-0000b490: 6e6e 656c 2065 6c73 6520 3029 0a20 2020  nnel else 0).   
-0000b4a0: 2020 2020 2020 2020 2069 6620 6365 6e74           if cent
-0000b4b0: 6572 2e6e 5f64 696d 203d 3d20 3220 616e  er.n_dim == 2 an
-0000b4c0: 6420 6e6f 7420 6365 6e74 6572 2e68 6173  d not center.has
-0000b4d0: 5f63 6861 6e6e 656c 3a20 6365 6e74 6572  _channel: center
-0000b4e0: 203d 2063 656e 7465 722e 7769 7468 5f63   = center.with_c
-0000b4f0: 6861 6e6e 656c 6469 6d28 3120 2d20 6365  hanneldim(1 - ce
-0000b500: 6e74 6572 2e62 6174 6368 5f64 696d 656e  nter.batch_dimen
-0000b510: 7369 6f6e 290a 2020 2020 2020 2020 2020  sion).          
-0000b520: 2020 6176 6f75 6368 2863 656e 7465 722e    avouch(center.
-0000b530: 6861 735f 6261 7463 6820 616e 6420 6365  has_batch and ce
-0000b540: 6e74 6572 2e68 6173 5f63 6861 6e6e 656c  nter.has_channel
-0000b550: 2c20 6622 506c 6561 7365 2075 7365 2062  , f"Please use b
-0000b560: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
-0000b570: 2073 697a 6520 285b 6e5f 6261 7463 685d   size ([n_batch]
-0000b580: 2c20 7b7b 6e5f 6469 6d7d 7d29 2066 6f72  , {{n_dim}}) for
-0000b590: 2052 6967 6964 2063 656e 7465 722c 2069   Rigid center, i
-0000b5a0: 6e73 7465 6164 206f 6620 7b63 656e 7465  nstead of {cente
-0000b5b0: 722e 7368 6170 657d 2e20 2229 0a20 2020  r.shape}. ").   
-0000b5c0: 2020 2020 2020 2020 2069 6620 6e5f 6261           if n_ba
-0000b5d0: 7463 6820 3d3d 2031 2061 6e64 2063 656e  tch == 1 and cen
-0000b5e0: 7465 722e 6e5f 6261 7463 6820 3e20 313a  ter.n_batch > 1:
-0000b5f0: 206e 5f62 6174 6368 203d 2063 656e 7465   n_batch = cente
-0000b600: 722e 6e5f 6261 7463 680a 2020 2020 2020  r.n_batch.      
-0000b610: 2020 2020 2020 6966 206e 5f64 696d 2069        if n_dim i
-0000b620: 7320 4e6f 6e65 3a20 6e5f 6469 6d20 3d20  s None: n_dim = 
-0000b630: 6365 6e74 6572 2e6e 5f63 6861 6e6e 656c  center.n_channel
-0000b640: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000b650: 653a 2061 766f 7563 6828 6e5f 6469 6d20  e: avouch(n_dim 
-0000b660: 3d3d 2063 656e 7465 722e 6e5f 6368 616e  == center.n_chan
-0000b670: 6e65 6c2c 2066 2243 656e 7465 7228 7b63  nel, f"Center({c
-0000b680: 656e 7465 722e 6e5f 6368 616e 6e65 6c7d  enter.n_channel}
-0000b690: 4429 2061 6e64 2074 7261 6e73 6c61 7469  D) and translati
-0000b6a0: 6f6e 287b 6e5f 6469 6d7d 4429 2069 6e20  on({n_dim}D) in 
-0000b6b0: 7472 616e 732e 5269 6769 6420 7368 6f75  trans.Rigid shou
-0000b6c0: 6c64 2068 6176 6520 7468 6520 7361 6d65  ld have the same
-0000b6d0: 2064 696d 656e 7369 6f6e 2e20 2229 0a20   dimension. "). 
-0000b6e0: 2020 2020 2020 2020 2020 206e 5f64 696d             n_dim
-0000b6f0: 203d 2063 656e 7465 722e 6e5f 6368 616e   = center.n_chan
-0000b700: 6e65 6c0a 2020 2020 2020 2020 6966 2061  nel.        if a
-0000b710: 7869 7320 6973 206e 6f74 204e 6f6e 653a  xis is not None:
-0000b720: 0a20 2020 2020 2020 2020 2020 2061 7869  .            axi
-0000b730: 7320 3d20 6261 746f 7263 685f 7465 6e73  s = batorch_tens
-0000b740: 6f72 2861 7869 7329 0a20 2020 2020 2020  or(axis).       
-0000b750: 2020 2020 2069 6620 6178 6973 2e6e 5f64       if axis.n_d
-0000b760: 696d 203c 3d20 3120 616e 6420 6e6f 7420  im <= 1 and not 
-0000b770: 6178 6973 2e68 6173 5f62 6174 6368 3a20  axis.has_batch: 
-0000b780: 6178 6973 203d 2061 7869 732e 756e 7371  axis = axis.unsq
-0000b790: 7565 657a 6528 5b5d 290a 2020 2020 2020  ueeze([]).      
-0000b7a0: 2020 2020 2020 6966 2061 7869 732e 6e5f        if axis.n_
-0000b7b0: 6469 6d20 3d3d 2032 2061 6e64 206e 6f74  dim == 2 and not
-0000b7c0: 2061 7869 732e 6861 735f 6261 7463 683a   axis.has_batch:
-0000b7d0: 2061 7869 7320 3d20 6178 6973 2e77 6974   axis = axis.wit
-0000b7e0: 685f 6261 7463 6864 696d 2828 3120 2d20  h_batchdim((1 - 
-0000b7f0: 6178 6973 2e63 6861 6e6e 656c 5f64 696d  axis.channel_dim
-0000b800: 656e 7369 6f6e 2920 6966 2061 7869 732e  ension) if axis.
-0000b810: 6861 735f 6368 616e 6e65 6c20 656c 7365  has_channel else
-0000b820: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
-0000b830: 6966 2061 7869 732e 6e5f 6469 6d20 3d3d  if axis.n_dim ==
-0000b840: 2032 2061 6e64 206e 6f74 2061 7869 732e   2 and not axis.
-0000b850: 6861 735f 6368 616e 6e65 6c3a 2061 7869  has_channel: axi
-0000b860: 7320 3d20 6178 6973 2e77 6974 685f 6368  s = axis.with_ch
-0000b870: 616e 6e65 6c64 696d 2831 202d 2061 7869  anneldim(1 - axi
-0000b880: 732e 6261 7463 685f 6469 6d65 6e73 696f  s.batch_dimensio
-0000b890: 6e29 0a20 2020 2020 2020 2020 2020 2061  n).            a
-0000b8a0: 766f 7563 6828 6178 6973 2e68 6173 5f62  vouch(axis.has_b
-0000b8b0: 6174 6368 2061 6e64 2061 7869 732e 6861  atch and axis.ha
-0000b8c0: 735f 6368 616e 6e65 6c2c 2066 2250 6c65  s_channel, f"Ple
-0000b8d0: 6173 6520 7573 6520 6261 746f 7263 6820  ase use batorch 
-0000b8e0: 7465 6e73 6f72 206f 6620 7369 7a65 2028  tensor of size (
-0000b8f0: 5b6e 5f62 6174 6368 5d2c 207b 7b6e 5f64  [n_batch], {{n_d
-0000b900: 696d 7d7d 2920 666f 7220 5269 6769 6420  im}}) for Rigid 
-0000b910: 6178 6973 6573 2c20 696e 7374 6561 6420  axises, instead 
-0000b920: 6f66 207b 6178 6973 2e73 6861 7065 7d2e  of {axis.shape}.
-0000b930: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
-0000b940: 6966 2028 2861 7869 732e 6e6f 726d 2829  if ((axis.norm()
-0000b950: 202d 2031 2920 2a2a 2032 292e 7375 6d28   - 1) ** 2).sum(
-0000b960: 292e 7375 6d28 2920 3e3d 2031 652d 343a  ).sum() >= 1e-4:
-0000b970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b980: 2070 7269 6e74 2822 7761 726e 696e 673a   print("warning:
-0000b990: 2070 6172 616d 2e20 6178 6973 6573 2066   param. axises f
-0000b9a0: 6f72 2027 5269 6769 6427 2074 7261 6e73  or 'Rigid' trans
-0000b9b0: 666f 726d 6174 696f 6e20 7368 6f75 6c64  formation should
-0000b9c0: 2062 6520 6e6f 726d 2d31 2076 6563 746f   be norm-1 vecto
-0000b9d0: 7273 2c20 6175 746f 2d6e 6f72 6d61 6c69  rs, auto-normali
-0000b9e0: 7a61 7469 6f6e 2077 6f75 6c64 2062 6520  zation would be 
-0000b9f0: 7065 7266 6f72 6d65 642e 2050 6c65 6173  performed. Pleas
-0000ba00: 6520 636f 6e74 6163 7420 7468 6520 6465  e contact the de
-0000ba10: 7665 6c6f 7065 7273 2069 6620 6e65 6365  velopers if nece
-0000ba20: 7373 6172 7920 2845 7272 6f72 2043 6f64  ssary (Error Cod
-0000ba30: 653a 2054 3333 3129 2e20 2229 0a20 2020  e: T331). ").   
-0000ba40: 2020 2020 2020 2020 2020 2020 2061 7869               axi
-0000ba50: 7320 3d20 6178 6973 202f 2061 7869 732e  s = axis / axis.
-0000ba60: 6e6f 726d 2829 0a20 2020 2020 2020 2020  norm().         
-0000ba70: 2020 2069 6620 6e5f 6261 7463 6820 3d3d     if n_batch ==
-0000ba80: 2031 2061 6e64 2061 7869 732e 6e5f 6261   1 and axis.n_ba
-0000ba90: 7463 6820 3e20 313a 206e 5f62 6174 6368  tch > 1: n_batch
-0000baa0: 203d 2061 7869 732e 6e5f 6261 7463 680a   = axis.n_batch.
-0000bab0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000bac0: 5f64 696d 2069 7320 4e6f 6e65 3a20 6e5f  _dim is None: n_
-0000bad0: 6469 6d20 3d20 6178 6973 2e6e 5f63 6861  dim = axis.n_cha
-0000bae0: 6e6e 656c 0a20 2020 2020 2020 2020 2020  nnel.           
-0000baf0: 2065 6c73 653a 2061 766f 7563 6828 6e5f   else: avouch(n_
-0000bb00: 6469 6d20 3d3d 2061 7869 732e 6e5f 6368  dim == axis.n_ch
-0000bb10: 616e 6e65 6c2c 2066 2254 7261 6e73 6c61  annel, f"Transla
-0000bb20: 7469 6f6e 287b 6e5f 6469 6d7d 4429 2061  tion({n_dim}D) a
-0000bb30: 6e64 2061 7869 7365 7328 7b61 7869 732e  nd axises({axis.
-0000bb40: 6e5f 6368 616e 6e65 6c7d 4429 2920 696e  n_channel}D)) in
-0000bb50: 2074 7261 6e73 2e52 6967 6964 2073 686f   trans.Rigid sho
-0000bb60: 756c 6420 6861 7665 2074 6865 2073 616d  uld have the sam
-0000bb70: 6520 6469 6d65 6e73 696f 6e2e 2022 290a  e dimension. ").
-0000bb80: 2020 2020 2020 2020 6966 206e 5f64 696d          if n_dim
-0000bb90: 2069 7320 4e6f 6e65 3a20 6e5f 6469 6d20   is None: n_dim 
-0000bba0: 3d20 3220 6966 2061 7869 7320 6973 204e  = 2 if axis is N
-0000bbb0: 6f6e 6520 656c 7365 2033 0a20 2020 2020  one else 3.     
-0000bbc0: 2020 2069 6620 7472 616e 736c 6174 696f     if translatio
-0000bbd0: 6e20 6973 204e 6f6e 653a 2074 7261 6e73  n is None: trans
-0000bbe0: 6c61 7469 6f6e 203d 2062 742e 7a65 726f  lation = bt.zero
-0000bbf0: 7328 5b6e 5f62 6174 6368 5d2c 207b 6e5f  s([n_batch], {n_
-0000bc00: 6469 6d7d 290a 2020 2020 2020 2020 6966  dim}).        if
-0000bc10: 2063 656e 7465 7220 6973 204e 6f6e 653a   center is None:
-0000bc20: 2063 656e 7465 7220 3d20 6274 2e7a 6572   center = bt.zer
-0000bc30: 6f73 285b 6e5f 6261 7463 685d 2c20 7b6e  os([n_batch], {n
-0000bc40: 5f64 696d 7d29 0a20 2020 2020 2020 200a  _dim}).        .
-0000bc50: 2020 2020 2020 2020 2320 4e6f 7720 7765          # Now we
-0000bc60: 2063 7265 6174 6520 7468 6520 6d61 7472   create the matr
-0000bc70: 6978 0a20 2020 2020 2020 2061 6e67 6c65  ix.        angle
-0000bc80: 203d 2061 6e67 6c65 2e66 6c6f 6174 2829   = angle.float()
-0000bc90: 0a20 2020 2020 2020 2063 656e 7465 7220  .        center 
-0000bca0: 3d20 6365 6e74 6572 2e66 6c6f 6174 2829  = center.float()
-0000bcb0: 0a20 2020 2020 2020 2074 7261 6e73 6c61  .        transla
-0000bcc0: 7469 6f6e 203d 2074 7261 6e73 6c61 7469  tion = translati
-0000bcd0: 6f6e 2e66 6c6f 6174 2829 0a20 2020 2020  on.float().     
-0000bce0: 2020 2069 6620 6e5f 6469 6d20 3d3d 2032     if n_dim == 2
-0000bcf0: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
-0000bd00: 3d20 6274 2e73 7461 636b 2862 742e 636f  = bt.stack(bt.co
-0000bd10: 7328 616e 676c 6529 2c20 6274 2e73 696e  s(angle), bt.sin
-0000bd20: 2861 6e67 6c65 292c 202d 6274 2e73 696e  (angle), -bt.sin
-0000bd30: 2861 6e67 6c65 292c 2062 742e 636f 7328  (angle), bt.cos(
-0000bd40: 616e 676c 6529 2c20 2d31 292e 7370 6c69  angle), -1).spli
-0000bd50: 7464 696d 282d 312c 2032 2c20 3229 0a20  tdim(-1, 2, 2). 
-0000bd60: 2020 2020 2020 2065 6c69 6620 6e5f 6469         elif n_di
-0000bd70: 6d20 3d3d 2033 3a0a 2020 2020 2020 2020  m == 3:.        
-0000bd80: 2020 2020 6178 6973 203d 2061 7869 732e      axis = axis.
-0000bd90: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
-0000bda0: 2020 2020 4120 3d20 6274 2e65 7965 285b      A = bt.eye([
-0000bdb0: 6e5f 6261 7463 685d 2c20 6e5f 6469 6d29  n_batch], n_dim)
-0000bdc0: 202b 2028 3120 2d20 6274 2e63 6f73 2861   + (1 - bt.cos(a
-0000bdd0: 6e67 6c65 2929 202a 2062 742e 6372 6f73  ngle)) * bt.cros
-0000bde0: 735f 6d61 7472 6978 2861 7869 7329 2040  s_matrix(axis) @
-0000bdf0: 2062 742e 6372 6f73 735f 6d61 7472 6978   bt.cross_matrix
-0000be00: 2861 7869 7329 202b 2062 742e 7369 6e28  (axis) + bt.sin(
-0000be10: 616e 676c 6529 202a 2062 742e 6372 6f73  angle) * bt.cros
-0000be20: 735f 6d61 7472 6978 2861 7869 7329 0a20  s_matrix(axis). 
-0000be30: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000be40: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
-0000be50: 7272 6f72 2822 4e6f 7449 6d70 6c65 6d65  rror("NotImpleme
-0000be60: 6e74 6564 2229 2866 2252 6967 6964 2074  nted")(f"Rigid t
-0000be70: 7261 6e73 666f 726d 6174 696f 6e20 696e  ransformation in
-0000be80: 206d 6963 6f6d 7075 7469 6e67 2064 6f65   micomputing doe
-0000be90: 7320 6e6f 7420 7375 7070 6f72 7420 7b6e  s not support {n
-0000bea0: 5f64 696d 7d20 6469 6d65 6e73 696f 6e61  _dim} dimensiona
-0000beb0: 6c20 7472 616e 7366 6f72 6d73 2028 3220  l transforms (2 
-0000bec0: 2620 3344 206f 6e6c 7929 2e20 2220 2b20  & 3D only). " + 
-0000bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bef0: 2020 2020 2020 2020 2022 506c 6561 7365           "Please
-0000bf00: 2063 6f6e 7461 6374 2074 6865 2064 6576   contact the dev
-0000bf10: 656c 6f70 6572 7320 6966 2074 6865 7265  elopers if there
-0000bf20: 2061 7265 2066 6561 7369 626c 6520 616c   are feasible al
-0000bf30: 676f 7269 7468 6d73 2028 4572 726f 7220  gorithms (Error 
-0000bf40: 436f 6465 3a20 5433 3333 292e 2054 6861  Code: T333). Tha
-0000bf50: 6e6b 2079 6f75 2e20 2229 0a20 2020 2020  nk you. ").     
-0000bf60: 2020 206d 6174 7269 7820 3d20 6274 2e63     matrix = bt.c
-0000bf70: 6174 2862 742e 6361 7428 412c 2028 2874  at(bt.cat(A, ((t
-0000bf80: 7261 6e73 6c61 7469 6f6e 202b 2063 656e  ranslation + cen
-0000bf90: 7465 7229 2e77 6974 685f 6368 616e 6e65  ter).with_channe
-0000bfa0: 6c64 696d 284e 6f6e 6529 202d 2041 2040  ldim(None) - A @
-0000bfb0: 2063 656e 7465 722e 7769 7468 5f63 6861   center.with_cha
-0000bfc0: 6e6e 656c 6469 6d28 4e6f 6e65 2929 2e75  nneldim(None)).u
-0000bfd0: 6e73 7175 6565 7a65 282d 3129 2c20 2d31  nsqueeze(-1), -1
-0000bfe0: 292c 200a 2020 2020 2020 2020 2020 2020  ), .            
-0000bff0: 2020 2020 2020 2020 2020 2020 6274 2e63              bt.c
-0000c000: 6174 2862 742e 7a65 726f 7328 6e5f 6469  at(bt.zeros(n_di
-0000c010: 6d29 2c20 6274 2e6f 6e65 7328 3129 292e  m), bt.ones(1)).
-0000c020: 756e 7371 7565 657a 6528 5b5d 2c20 3129  unsqueeze([], 1)
-0000c030: 2c20 3129 0a20 2020 2020 2020 2069 6620  , 1).        if 
-0000c040: 7472 616e 735f 7374 7265 7463 6820 6973  trans_stretch is
-0000c050: 206e 6f74 204e 6f6e 653a 206d 6174 7269   not None: matri
-0000c060: 785b 2e2e 2e2c 203a 6e5f 6469 6d2c 202d  x[..., :n_dim, -
-0000c070: 315d 202a 3d20 7472 616e 735f 7374 7265  1] *= trans_stre
-0000c080: 7463 680a 2020 2020 2020 2020 6966 206e  tch.        if n
-0000c090: 6f74 2069 7369 6e73 7461 6e63 6528 7370  ot isinstance(sp
-0000c0a0: 6163 696e 672c 2074 7570 6c65 293a 2073  acing, tuple): s
-0000c0b0: 7061 6369 6e67 203d 2074 6f5f 7475 706c  pacing = to_tupl
-0000c0c0: 6528 7370 6163 696e 6729 0a20 2020 2020  e(spacing).     
-0000c0d0: 2020 2069 6620 6c65 6e28 7370 6163 696e     if len(spacin
-0000c0e0: 6729 203d 3d20 313a 2073 7061 6369 6e67  g) == 1: spacing
-0000c0f0: 203d 2073 7061 6369 6e67 202a 206e 5f64   = spacing * n_d
-0000c100: 696d 0a20 2020 2020 2020 2041 203d 2062  im.        A = b
-0000c110: 742e 6469 6167 2862 6174 6f72 6368 5f74  t.diag(batorch_t
-0000c120: 656e 736f 7228 6c69 7374 2873 7061 6369  ensor(list(spaci
-0000c130: 6e67 2920 2b20 5b31 2e5d 2929 2e75 6e73  ng) + [1.])).uns
-0000c140: 7175 6565 7a65 285b 5d29 2e61 7374 7970  queeze([]).astyp
-0000c150: 6528 6d61 7472 6978 290a 2020 2020 2020  e(matrix).      
-0000c160: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-0000c170: 5f5f 2861 6e67 6c65 2c20 6178 6973 2c20  __(angle, axis, 
-0000c180: 7472 616e 736c 6174 696f 6e2c 2063 656e  translation, cen
-0000c190: 7465 723d 6365 6e74 6572 2c20 7472 616e  ter=center, tran
-0000c1a0: 735f 7374 7265 7463 683d 7472 616e 735f  s_stretch=trans_
-0000c1b0: 7374 7265 7463 682c 2073 7061 6369 6e67  stretch, spacing
-0000c1c0: 3d73 7061 6369 6e67 290a 0a20 2020 2020  =spacing)..     
-0000c1d0: 2020 2073 656c 662e 6e5f 6469 6d20 3d20     self.n_dim = 
-0000c1e0: 6e5f 6469 6d0a 2020 2020 2020 2020 7365  n_dim.        se
-0000c1f0: 6c66 2e74 7261 6e73 5f73 7472 6574 6368  lf.trans_stretch
-0000c200: 203d 2074 7261 6e73 5f73 7472 6574 6368   = trans_stretch
-0000c210: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
-0000c220: 6163 696e 6720 3d20 7370 6163 696e 670a  acing = spacing.
-0000c230: 2020 2020 2020 2020 7365 6c66 2e6d 6174          self.mat
-0000c240: 7269 7820 3d20 412e 696e 7628 2920 4020  rix = A.inv() @ 
-0000c250: 6d61 7472 6978 2040 2041 0a20 2020 2020  matrix @ A.     
-0000c260: 2020 2073 656c 662e 6261 7463 685f 7061     self.batch_pa
-0000c270: 7261 6d2e 6170 7065 6e64 2827 6d61 7472  ram.append('matr
-0000c280: 6978 2729 0a0a 2020 2020 6465 6620 5f5f  ix')..    def __
-0000c290: 6361 6c6c 5f5f 2873 656c 662c 2058 293a  call__(self, X):
-0000c2a0: 0a20 2020 2020 2020 2058 203d 2073 7570  .        X = sup
-0000c2b0: 6572 2829 2e5f 5f63 616c 6c5f 5f28 5829  er().__call__(X)
-0000c2c0: 0a20 2020 2020 2020 206d 6174 7269 7820  .        matrix 
-0000c2d0: 3d20 7365 6c66 2e6d 6174 7269 780a 2020  = self.matrix.  
-0000c2e0: 2020 2020 2020 6e5f 6469 6d20 3d20 7365        n_dim = se
-0000c2f0: 6c66 2e6e 5f64 696d 0a20 2020 2020 2020  lf.n_dim.       
-0000c300: 2041 203d 206d 6174 7269 785b 3a2c 203a   A = matrix[:, :
-0000c310: 6e5f 6469 6d2c 203a 6e5f 6469 6d5d 0a20  n_dim, :n_dim]. 
-0000c320: 2020 2020 2020 2062 203d 206d 6174 7269         b = matri
-0000c330: 785b 3a2c 203a 6e5f 6469 6d2c 206e 5f64  x[:, :n_dim, n_d
-0000c340: 696d 5d0a 2020 2020 2020 2020 7368 6170  im].        shap
-0000c350: 6520 3d20 582e 7368 6170 650a 2020 2020  e = X.shape.    
-0000c360: 2020 2020 5920 3d20 2841 2040 2058 2e66      Y = (A @ X.f
-0000c370: 6c61 7474 656e 2829 2e63 6861 6e6e 656c  latten().channel
-0000c380: 5f64 696d 5f28 4e6f 6e65 2920 2b20 622e  _dim_(None) + b.
-0000c390: 756e 7371 7565 657a 6528 2d31 2929 2e76  unsqueeze(-1)).v
-0000c3a0: 6965 7728 7368 6170 6529 0a20 2020 2020  iew(shape).     
-0000c3b0: 2020 2072 6574 7572 6e20 590a 2020 2020     return Y.    
-0000c3c0: 0a20 2020 2064 6566 2061 6666 696e 6528  .    def affine(
-0000c3d0: 7365 6c66 2c20 6e5f 6469 6d3d 4e6f 6e65  self, n_dim=None
-0000c3e0: 293a 0a20 2020 2020 2020 2061 766f 7563  ):.        avouc
-0000c3f0: 6828 6e5f 6469 6d20 6973 204e 6f6e 6520  h(n_dim is None 
-0000c400: 6f72 2073 656c 662e 6e5f 6469 6d20 3d3d  or self.n_dim ==
-0000c410: 206e 5f64 696d 290a 2020 2020 2020 2020   n_dim).        
-0000c420: 7265 7475 726e 2073 656c 662e 6d61 7472  return self.matr
-0000c430: 6978 0a0a 2020 2020 6465 6620 696e 7628  ix..    def inv(
-0000c440: 7365 6c66 293a 0a20 2020 2020 2020 2041  self):.        A
-0000c450: 203d 2062 742e 6469 6167 2862 6174 6f72   = bt.diag(bator
-0000c460: 6368 5f74 656e 736f 7228 6c69 7374 2873  ch_tensor(list(s
-0000c470: 656c 662e 7370 6163 696e 6729 202b 205b  elf.spacing) + [
-0000c480: 312e 5d29 292e 756e 7371 7565 657a 6528  1.])).unsqueeze(
-0000c490: 5b5d 292e 6173 7479 7065 2873 656c 662e  []).astype(self.
-0000c4a0: 6d61 7472 6978 290a 2020 2020 2020 2020  matrix).        
-0000c4b0: 7265 7475 726e 2052 6967 6964 2841 2040  return Rigid(A @
-0000c4c0: 2062 742e 696e 7628 7365 6c66 2e6d 6174   bt.inv(self.mat
-0000c4d0: 7269 7829 2040 2041 2e69 6e76 2829 2c20  rix) @ A.inv(), 
-0000c4e0: 7472 616e 735f 7374 7265 7463 6820 3d20  trans_stretch = 
-0000c4f0: 312c 2073 7061 6369 6e67 3d73 656c 662e  1, spacing=self.
-0000c500: 7370 6163 696e 6729 2e62 6163 6b77 6172  spacing).backwar
-0000c510: 645f 2873 656c 662e 6261 636b 7761 7264  d_(self.backward
-0000c520: 290a 0a40 616c 6961 7328 2241 6666 2229  )..@alias("Aff")
-0000c530: 0a63 6c61 7373 2041 6666 696e 6528 5370  .class Affine(Sp
-0000c540: 6174 6961 6c54 7261 6e73 666f 726d 6174  atialTransformat
-0000c550: 696f 6e29 3a0a 2020 2020 6465 6620 5f5f  ion):.    def __
-0000c560: 696e 6974 5f5f 2873 656c 662c 206d 6174  init__(self, mat
-0000c570: 7269 782c 2074 7261 6e73 5f73 7472 6574  rix, trans_stret
-0000c580: 6368 3d4e 6f6e 652c 2073 7061 6369 6e67  ch=None, spacing
-0000c590: 3d31 293a 0a20 2020 2020 2020 2027 2727  =1):.        '''
-0000c5a0: 0a20 2020 2020 2020 2041 6666 696e 6520  .        Affine 
-0000c5b0: 7472 616e 7366 6f72 6d61 7469 6f6e 2077  transformation w
-0000c5c0: 6974 6820 7265 7370 6563 7420 746f 2074  ith respect to t
-0000c5d0: 7261 6e73 666f 726d 6174 696f 6e20 6d61  ransformation ma
-0000c5e0: 7472 6978 2e0a 2020 2020 2020 2020 0a20  trix..        . 
-0000c5f0: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
-0000c600: 2020 2020 2020 2020 2020 206d 6174 7269             matri
-0000c610: 7820 5b62 742e 5465 6e73 6f72 206f 7220  x [bt.Tensor or 
-0000c620: 6e70 2e6e 756d 7079 5d3a 2074 6865 2061  np.numpy]: the a
-0000c630: 6666 696e 6520 6d61 7472 6978 2e20 0a20  ffine matrix. . 
-0000c640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c650: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
-0000c660: 206e 5f64 696d 202b 2031 2c20 6e5f 6469   n_dim + 1, n_di
-0000c670: 6d20 2b20 3129 0a20 2020 2020 2020 2020  m + 1).         
-0000c680: 2020 2074 7261 6e73 5f73 7472 6574 6368     trans_stretch
-0000c690: 205b 696e 745d 3a20 6f6e 6c79 2075 7365   [int]: only use
-0000c6a0: 6420 666f 7220 6974 6572 6174 6976 6520  d for iterative 
-0000c6b0: 7061 7261 6d65 7465 7220 7472 6169 6e69  parameter traini
-0000c6c0: 6e67 2c20 3120 6279 2064 6566 6175 6c74  ng, 1 by default
-0000c6d0: 2e20 3230 2073 6565 6d73 2074 6f20 6265  . 20 seems to be
-0000c6e0: 2061 2067 6f6f 6420 6368 6f69 6365 2e20   a good choice. 
-0000c6f0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-0000c700: 2020 2020 2020 5768 656e 2069 7420 6973        When it is
-0000c710: 2063 616c 6c65 643a 0a20 2020 2020 2020   called:.       
-0000c720: 2020 2020 2058 205b 6274 2e54 656e 736f       X [bt.Tenso
-0000c730: 725d 3a20 436f 6f72 6469 6e61 7465 7320  r]: Coordinates 
-0000c740: 746f 2062 6520 7472 616e 7366 6f72 6d65  to be transforme
-0000c750: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
-0000c760: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
-0000c770: 6368 3a20 6f70 7469 6f6e 616c 5d2c 207b  ch: optional], {
-0000c780: 6e5f 6469 6d7d 2c20 6e5f 312c 206e 5f32  n_dim}, n_1, n_2
-0000c790: 2c20 2e2e 2e2c 206e 5f72 290a 2020 2020  , ..., n_r).    
-0000c7a0: 2020 2020 2020 2020 6f75 7470 7574 205b          output [
-0000c7b0: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
-0000c7c0: 7472 616e 7366 6f72 6d65 6420 636f 6f72  transformed coor
-0000c7d0: 6469 6e61 7465 732e 0a20 2020 2020 2020  dinates..       
-0000c7e0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-0000c7f0: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-0000c800: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
-0000c810: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
-0000c820: 2727 270a 2020 2020 2020 2020 6d61 7472  '''.        matr
-0000c830: 6978 203d 2062 6174 6f72 6368 5f74 656e  ix = batorch_ten
-0000c840: 736f 7228 6d61 7472 6978 290a 2020 2020  sor(matrix).    
-0000c850: 2020 2020 6e5f 6469 6d20 3d20 6d61 7472      n_dim = matr
-0000c860: 6978 2e73 697a 6528 2d31 2920 2d20 310a  ix.size(-1) - 1.
-0000c870: 2020 2020 2020 2020 6966 206d 6174 7269          if matri
-0000c880: 782e 6e5f 6469 6d20 3c3d 2032 2061 6e64  x.n_dim <= 2 and
-0000c890: 206e 6f74 206d 6174 7269 782e 6861 735f   not matrix.has_
-0000c8a0: 6261 7463 683a 206d 6174 7269 7820 3d20  batch: matrix = 
-0000c8b0: 6d61 7472 6978 2e75 6e73 7175 6565 7a65  matrix.unsqueeze
-0000c8c0: 285b 5d29 0a20 2020 2020 2020 2069 6620  ([]).        if 
-0000c8d0: 6d61 7472 6978 2e6e 5f64 696d 203d 3d20  matrix.n_dim == 
-0000c8e0: 3320 616e 6420 6e6f 7420 6d61 7472 6978  3 and not matrix
-0000c8f0: 2e68 6173 5f62 6174 6368 2061 6e64 206d  .has_batch and m
-0000c900: 6174 7269 782e 7368 6170 655b 315d 203d  atrix.shape[1] =
-0000c910: 3d20 6d61 7472 6978 2e73 6861 7065 5b32  = matrix.shape[2
-0000c920: 5d3a 206d 6174 7269 782e 6261 7463 685f  ]: matrix.batch_
-0000c930: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
-0000c940: 2020 2020 2020 6176 6f75 6368 286d 6174        avouch(mat
-0000c950: 7269 782e 6861 735f 6261 7463 682c 2066  rix.has_batch, f
-0000c960: 2250 6c65 6173 6520 7573 6520 6261 746f  "Please use bato
-0000c970: 7263 6820 7465 6e73 6f72 206f 6620 7369  rch tensor of si
-0000c980: 7a65 2028 5b6e 5f62 6174 6368 5d2c 206e  ze ([n_batch], n
-0000c990: 5f64 696d 202b 2031 2c20 6e5f 6469 6d20  _dim + 1, n_dim 
-0000c9a0: 2b20 3129 2066 6f72 2041 6666 696e 6520  + 1) for Affine 
-0000c9b0: 7061 7261 6d65 7465 7273 2c20 696e 7374  parameters, inst
-0000c9c0: 6561 6420 6f66 207b 6d61 7472 6978 2e73  ead of {matrix.s
-0000c9d0: 6861 7065 7d2e 2022 290a 2020 2020 2020  hape}. ").      
-0000c9e0: 2020 6966 2074 7261 6e73 5f73 7472 6574    if trans_stret
-0000c9f0: 6368 2069 7320 6e6f 7420 4e6f 6e65 3a20  ch is not None: 
-0000ca00: 6d61 7472 6978 5b2e 2e2e 2c20 3a6e 5f64  matrix[..., :n_d
-0000ca10: 696d 2c20 2d31 5d20 2a3d 2074 7261 6e73  im, -1] *= trans
-0000ca20: 5f73 7472 6574 6368 0a20 2020 2020 2020  _stretch.       
-0000ca30: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-0000ca40: 6365 2873 7061 6369 6e67 2c20 7475 706c  ce(spacing, tupl
-0000ca50: 6529 3a20 7370 6163 696e 6720 3d20 746f  e): spacing = to
-0000ca60: 5f74 7570 6c65 2873 7061 6369 6e67 290a  _tuple(spacing).
-0000ca70: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
-0000ca80: 7061 6369 6e67 2920 3d3d 2031 3a20 7370  pacing) == 1: sp
-0000ca90: 6163 696e 6720 3d20 7370 6163 696e 6720  acing = spacing 
-0000caa0: 2a20 6e5f 6469 6d0a 2020 2020 2020 2020  * n_dim.        
-0000cab0: 4120 3d20 6274 2e64 6961 6728 6261 746f  A = bt.diag(bato
-0000cac0: 7263 685f 7465 6e73 6f72 286c 6973 7428  rch_tensor(list(
-0000cad0: 7370 6163 696e 6729 202b 205b 312e 5d29  spacing) + [1.])
-0000cae0: 292e 756e 7371 7565 657a 6528 5b5d 292e  ).unsqueeze([]).
-0000caf0: 6173 7479 7065 286d 6174 7269 7829 0a20  astype(matrix). 
-0000cb00: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-0000cb10: 5f69 6e69 745f 5f28 6d61 7472 6978 2c20  _init__(matrix, 
-0000cb20: 7472 616e 735f 7374 7265 7463 683d 7472  trans_stretch=tr
-0000cb30: 616e 735f 7374 7265 7463 682c 2073 7061  ans_stretch, spa
-0000cb40: 6369 6e67 3d73 7061 6369 6e67 290a 0a20  cing=spacing).. 
-0000cb50: 2020 2020 2020 2073 656c 662e 6e5f 6469         self.n_di
-0000cb60: 6d20 3d20 6d61 7472 6978 2e73 697a 6528  m = matrix.size(
-0000cb70: 2d31 2920 2d20 310a 2020 2020 2020 2020  -1) - 1.        
-0000cb80: 7365 6c66 2e74 7261 6e73 5f73 7472 6574  self.trans_stret
-0000cb90: 6368 203d 2074 7261 6e73 5f73 7472 6574  ch = trans_stret
-0000cba0: 6368 0a20 2020 2020 2020 2073 656c 662e  ch.        self.
-0000cbb0: 7370 6163 696e 6720 3d20 7370 6163 696e  spacing = spacin
-0000cbc0: 670a 2020 2020 2020 2020 7365 6c66 2e6d  g.        self.m
-0000cbd0: 6174 7269 7820 3d20 412e 696e 7628 2920  atrix = A.inv() 
-0000cbe0: 4020 6d61 7472 6978 2040 2041 0a20 2020  @ matrix @ A.   
-0000cbf0: 2020 2020 2073 656c 662e 6261 7463 685f       self.batch_
-0000cc00: 7061 7261 6d2e 6170 7065 6e64 2827 6d61  param.append('ma
-0000cc10: 7472 6978 2729 0a0a 2020 2020 6465 6620  trix')..    def 
-0000cc20: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2058  __call__(self, X
-0000cc30: 293a 0a20 2020 2020 2020 2058 203d 2073  ):.        X = s
-0000cc40: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
-0000cc50: 5829 0a20 2020 2020 2020 206d 6174 7269  X).        matri
-0000cc60: 7820 3d20 7365 6c66 2e6d 6174 7269 782e  x = self.matrix.
-0000cc70: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
-0000cc80: 6e5f 6469 6d20 3d20 7365 6c66 2e6e 5f64  n_dim = self.n_d
-0000cc90: 696d 0a20 2020 2020 2020 2041 203d 206d  im.        A = m
-0000cca0: 6174 7269 785b 3a2c 203a 6e5f 6469 6d2c  atrix[:, :n_dim,
-0000ccb0: 203a 6e5f 6469 6d5d 0a20 2020 2020 2020   :n_dim].       
-0000ccc0: 2062 203d 206d 6174 7269 785b 3a2c 203a   b = matrix[:, :
-0000ccd0: 6e5f 6469 6d2c 206e 5f64 696d 5d0a 2020  n_dim, n_dim].  
-0000cce0: 2020 2020 2020 7368 6170 6520 3d20 582e        shape = X.
-0000ccf0: 7368 6170 650a 2020 2020 2020 2020 5920  shape.        Y 
-0000cd00: 3d20 2841 2040 2058 2e66 6c61 7474 656e  = (A @ X.flatten
-0000cd10: 2829 2e63 6861 6e6e 656c 5f64 696d 5f28  ().channel_dim_(
-0000cd20: 4e6f 6e65 2920 2b20 622e 756e 7371 7565  None) + b.unsque
-0000cd30: 657a 6528 2d31 2929 2e76 6965 7728 7368  eze(-1)).view(sh
-0000cd40: 6170 6529 0a20 2020 2020 2020 2072 6574  ape).        ret
-0000cd50: 7572 6e20 590a 2020 2020 0a20 2020 2064  urn Y.    .    d
-0000cd60: 6566 2061 6666 696e 6528 7365 6c66 2c20  ef affine(self, 
-0000cd70: 6e5f 6469 6d3d 4e6f 6e65 293a 0a20 2020  n_dim=None):.   
-0000cd80: 2020 2020 2061 766f 7563 6828 6e5f 6469       avouch(n_di
-0000cd90: 6d20 6973 204e 6f6e 6520 6f72 2073 656c  m is None or sel
-0000cda0: 662e 6e5f 6469 6d20 3d3d 206e 5f64 696d  f.n_dim == n_dim
-0000cdb0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000cdc0: 2073 656c 662e 6d61 7472 6978 0a0a 2020   self.matrix..  
-0000cdd0: 2020 6465 6620 696e 7628 7365 6c66 293a    def inv(self):
-0000cde0: 0a20 2020 2020 2020 2041 203d 2062 742e  .        A = bt.
-0000cdf0: 6469 6167 2862 6174 6f72 6368 5f74 656e  diag(batorch_ten
-0000ce00: 736f 7228 6c69 7374 2873 656c 662e 7370  sor(list(self.sp
-0000ce10: 6163 696e 6729 202b 205b 312e 5d29 292e  acing) + [1.])).
-0000ce20: 756e 7371 7565 657a 6528 5b5d 292e 6173  unsqueeze([]).as
-0000ce30: 7479 7065 2873 656c 662e 6d61 7472 6978  type(self.matrix
-0000ce40: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000ce50: 2041 6666 696e 6528 4120 4020 6274 2e69   Affine(A @ bt.i
-0000ce60: 6e76 2873 656c 662e 6d61 7472 6978 2920  nv(self.matrix) 
-0000ce70: 4020 412e 696e 7628 292c 2074 7261 6e73  @ A.inv(), trans
-0000ce80: 5f73 7472 6574 6368 203d 2031 2c20 7370  _stretch = 1, sp
-0000ce90: 6163 696e 673d 7365 6c66 2e73 7061 6369  acing=self.spaci
-0000cea0: 6e67 292e 6261 636b 7761 7264 5f28 7365  ng).backward_(se
-0000ceb0: 6c66 2e62 6163 6b77 6172 6429 0a0a 4061  lf.backward)..@a
-0000cec0: 6c69 6173 2822 6c6f 6745 7522 290a 636c  lias("logEu").cl
-0000ced0: 6173 7320 506f 6c79 4166 6669 6e65 2853  ass PolyAffine(S
-0000cee0: 7061 7469 616c 5472 616e 7366 6f72 6d61  patialTransforma
-0000cef0: 7469 6f6e 293a 0a20 2020 2064 6566 205f  tion):.    def _
-0000cf00: 5f69 6e69 745f 5f28 7365 6c66 2c20 646d  _init__(self, dm
-0000cf10: 6174 7269 6365 732c 206d 6173 6b73 2c20  atrices, masks, 
-0000cf20: 6f72 6465 723d 322c 2069 735f 696e 763d  order=2, is_inv=
-0000cf30: 4661 6c73 652c 2074 7261 6e73 5f73 7472  False, trans_str
-0000cf40: 6574 6368 3d4e 6f6e 6529 3a0a 2020 2020  etch=None):.    
-0000cf50: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0000cf60: 506f 6c79 2061 6666 696e 6520 7472 616e  Poly affine tran
-0000cf70: 7366 6f72 6d61 7469 6f6e 2077 6974 6820  sformation with 
-0000cf80: 7265 7370 6563 7420 746f 2074 7261 6e73  respect to trans
-0000cf90: 666f 726d 6174 696f 6e20 6d61 7472 6963  formation matric
-0000cfa0: 6573 205b 315d 2e0a 2020 2020 2020 2020  es [1]..        
-0000cfb0: 4e6f 7465 2074 6861 7420 646d 6174 7269  Note that dmatri
-0000cfc0: 6365 7320 666f 7220 7468 6973 2074 7261  ces for this tra
-0000cfd0: 6e66 6f72 6d61 7469 6f6e 2049 5320 4e4f  nformation IS NO
-0000cfe0: 5420 7468 6520 6163 7475 616c 2061 6666  T the actual aff
-0000cff0: 696e 6520 6d61 7472 6963 6573 2c20 6275  ine matrices, bu
-0000d000: 7420 4953 2061 2064 6966 6665 7265 6e74  t IS a different
-0000d010: 6961 7469 6f6e 2069 6e73 7465 6164 2e0a  iation instead..
-0000d020: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000d030: 2050 6172 616d 733a 0a20 2020 2020 2020   Params:.       
-0000d040: 2020 2020 2064 6d61 7472 6963 6573 205b       dmatrices [
-0000d050: 6274 2e54 656e 736f 7220 6f72 206e 702e  bt.Tensor or np.
-0000d060: 6e75 6d70 795d 3a20 4f6e 6520 6166 6669  numpy]: One affi
-0000d070: 6e65 206d 6174 7269 7820 666f 7220 6561  ne matrix for ea
-0000d080: 6368 2072 6567 696f 6e2e 200a 2020 2020  ch region. .    
-0000d090: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-0000d0a0: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
-0000d0b0: 5f72 6567 696f 6e7d 2c20 6e5f 6469 6d20  _region}, n_dim 
-0000d0c0: 2b20 312c 206e 5f64 696d 202b 2031 290a  + 1, n_dim + 1).
-0000d0d0: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
-0000d0e0: 7320 5b62 742e 5465 6e73 6f72 206f 7220  s [bt.Tensor or 
-0000d0f0: 6e70 2e6e 756d 7079 5d3a 204f 6e65 2030  np.numpy]: One 0
-0000d100: 2d31 206d 6173 6b20 666f 7220 6561 6368  -1 mask for each
-0000d110: 2072 6567 696f 6e2e 200a 2020 2020 2020   region. .      
-0000d120: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-0000d130: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
-0000d140: 6567 696f 6e7d 2c20 6e40 312c 206e 4032  egion}, n@1, n@2
-0000d150: 2c20 2e2e 2e2c 206e 406e 5f64 696d 290a  , ..., n@n_dim).
-0000d160: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-0000d170: 7220 5b69 6e74 5d3a 2074 6865 206f 7264  r [int]: the ord
-0000d180: 6572 206f 6620 696e 7465 7270 6f6c 6174  er of interpolat
-0000d190: 696f 6e20 636f 6566 6669 6369 656e 742e  ion coefficient.
-0000d1a0: 2054 6865 2069 6e66 6c75 656e 6365 206f   The influence o
-0000d1b0: 6620 616e 2061 6666 696e 6520 6465 6361  f an affine deca
-0000d1c0: 7973 2061 7420 6120 7261 7465 206f 6620  ys at a rate of 
-0000d1d0: 3120 2f20 6469 7374 616e 6365 5e6f 7264  1 / distance^ord
-0000d1e0: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-0000d1f0: 7472 616e 735f 7374 7265 7463 6820 5b69  trans_stretch [i
-0000d200: 6e74 5d3a 206f 6e6c 7920 7573 6564 2066  nt]: only used f
-0000d210: 6f72 2069 7465 7261 7469 7665 2070 6172  or iterative par
-0000d220: 616d 6574 6572 2074 7261 696e 696e 672c  ameter training,
-0000d230: 2031 2062 7920 6465 6661 756c 742e 2032   1 by default. 2
-0000d240: 3020 7365 656d 7320 746f 2062 6520 6120  0 seems to be a 
-0000d250: 676f 6f64 2063 686f 6963 652e 2020 0a20  good choice.  . 
-0000d260: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-0000d270: 2020 2020 5768 656e 2069 7420 6973 2063      When it is c
-0000d280: 616c 6c65 643a 0a20 2020 2020 2020 2020  alled:.         
-0000d290: 2020 2058 205b 6274 2e54 656e 736f 725d     X [bt.Tensor]
-0000d2a0: 3a20 436f 6f72 6469 6e61 7465 7320 746f  : Coordinates to
-0000d2b0: 2062 6520 7472 616e 7366 6f72 6d65 642e   be transformed.
-0000d2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d2d0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-0000d2e0: 3a20 6f70 7469 6f6e 616c 5d2c 207b 6e5f  : optional], {n_
-0000d2f0: 6469 6d7d 2c20 6e40 312c 206e 4032 2c20  dim}, n@1, n@2, 
-0000d300: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
-0000d310: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-0000d320: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
-0000d330: 6520 7472 616e 7366 6f72 6d65 6420 636f  e transformed co
-0000d340: 6f72 6469 6e61 7465 732e 0a20 2020 2020  ordinates..     
-0000d350: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-0000d360: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
-0000d370: 6469 6d7d 2c20 6e40 312c 206e 4032 2c20  dim}, n@1, n@2, 
-0000d380: 2e2e 2e2c 206e 406e 5f64 696d 290a 0a20  ..., n@n_dim).. 
-0000d390: 2020 2020 2020 205b 315d 2041 7273 6967         [1] Arsig
-0000d3a0: 6e79 2056 202c 2043 6f6d 6d6f 7769 636b  ny V , Commowick
-0000d3b0: 204f 202c 2041 7961 6368 6520 4e20 2c20   O , Ayache N , 
-0000d3c0: 6574 2061 6c2e 2041 2046 6173 7420 616e  et al. A Fast an
-0000d3d0: 6420 4c6f 672d 4575 636c 6964 6561 6e20  d Log-Euclidean 
-0000d3e0: 506f 6c79 6166 6669 6e65 2046 7261 6d65  Polyaffine Frame
-0000d3f0: 776f 726b 2066 6f72 204c 6f63 616c 6c79  work for Locally
-0000d400: 200a 2020 2020 2020 2020 2020 2020 4c69   .            Li
-0000d410: 6e65 6172 2052 6567 6973 7472 6174 696f  near Registratio
-0000d420: 6e5b 4a5d 2e20 4a6f 7572 6e61 6c20 6f66  n[J]. Journal of
-0000d430: 204d 6174 6865 6d61 7469 6361 6c20 496d   Mathematical Im
-0000d440: 6167 696e 6720 2620 5669 7369 6f6e 2c20  aging & Vision, 
-0000d450: 3230 3039 2c20 3333 2832 293a 3232 322d  2009, 33(2):222-
-0000d460: 3233 382e 0a20 2020 2020 2020 2027 2727  238..        '''
-0000d470: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-0000d480: 5369 6d70 6c65 4954 4b20 6173 2073 6974  SimpleITK as sit
-0000d490: 6b0a 2020 2020 2020 2020 6672 6f6d 202e  k.        from .
-0000d4a0: 6675 6e63 7320 696d 706f 7274 2064 696c  funcs import dil
-0000d4b0: 6174 652c 2064 6973 7461 6e63 655f 6d61  ate, distance_ma
-0000d4c0: 700a 2020 2020 2020 2020 6966 206e 6f74  p.        if not
-0000d4d0: 2069 7369 6e73 7461 6e63 6528 646d 6174   isinstance(dmat
-0000d4e0: 7269 6365 732c 2062 742e 5465 6e73 6f72  rices, bt.Tensor
-0000d4f0: 293a 2064 6d61 7472 6963 6573 203d 2062  ): dmatrices = b
-0000d500: 742e 7465 6e73 6f72 2864 6d61 7472 6963  t.tensor(dmatric
-0000d510: 6573 290a 2020 2020 2020 2020 6966 2064  es).        if d
-0000d520: 6d61 7472 6963 6573 2e6e 5f64 696d 203c  matrices.n_dim <
-0000d530: 3d20 3320 616e 6420 6e6f 7420 646d 6174  = 3 and not dmat
-0000d540: 7269 6365 732e 6861 735f 6261 7463 683a  rices.has_batch:
-0000d550: 2064 6d61 7472 6963 6573 203d 2064 6d61   dmatrices = dma
-0000d560: 7472 6963 6573 2e75 6e73 7175 6565 7a65  trices.unsqueeze
-0000d570: 285b 5d29 0a20 2020 2020 2020 2069 6620  ([]).        if 
-0000d580: 646d 6174 7269 6365 732e 6e5f 6469 6d20  dmatrices.n_dim 
-0000d590: 3c3d 2033 2061 6e64 206e 6f74 2064 6d61  <= 3 and not dma
-0000d5a0: 7472 6963 6573 2e68 6173 5f63 6861 6e6e  trices.has_chann
-0000d5b0: 656c 3a20 646d 6174 7269 6365 7320 3d20  el: dmatrices = 
-0000d5c0: 646d 6174 7269 6365 732e 756e 7371 7565  dmatrices.unsque
-0000d5d0: 657a 6528 7b7d 290a 2020 2020 2020 2020  eze({}).        
-0000d5e0: 6966 2064 6d61 7472 6963 6573 2e6e 5f64  if dmatrices.n_d
-0000d5f0: 696d 203d 3d20 3420 616e 6420 646d 6174  im == 4 and dmat
-0000d600: 7269 6365 732e 7368 6170 655b 325d 203d  rices.shape[2] =
-0000d610: 3d20 646d 6174 7269 6365 732e 7368 6170  = dmatrices.shap
-0000d620: 655b 335d 3a0a 2020 2020 2020 2020 2020  e[3]:.          
-0000d630: 2020 6966 206e 6f74 2064 6d61 7472 6963    if not dmatric
-0000d640: 6573 2e68 6173 5f62 6174 6368 3a20 646d  es.has_batch: dm
-0000d650: 6174 7269 6365 732e 6261 7463 685f 6469  atrices.batch_di
-0000d660: 6d65 6e73 696f 6e20 3d20 300a 2020 2020  mension = 0.    
-0000d670: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
-0000d680: 6d61 7472 6963 6573 2e68 6173 5f63 6861  matrices.has_cha
-0000d690: 6e6e 656c 3a20 646d 6174 7269 6365 732e  nnel: dmatrices.
-0000d6a0: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
-0000d6b0: 6e20 3d20 310a 2020 2020 2020 2020 6176  n = 1.        av
-0000d6c0: 6f75 6368 2864 6d61 7472 6963 6573 2e68  ouch(dmatrices.h
-0000d6d0: 6173 5f62 6174 6368 2061 6e64 2064 6d61  as_batch and dma
-0000d6e0: 7472 6963 6573 2e68 6173 5f63 6861 6e6e  trices.has_chann
-0000d6f0: 656c 2c20 2250 6c65 6173 6520 7573 6520  el, "Please use 
-0000d700: 6261 746f 7263 6820 7465 6e73 6f72 206f  batorch tensor o
-0000d710: 6620 7369 7a65 2028 5b6e 5f62 6174 6368  f size ([n_batch
-0000d720: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 2220  ], {n_region}," 
-0000d730: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
-0000d740: 2066 226e 5f64 696d 202b 2031 2c20 6e5f   f"n_dim + 1, n_
-0000d750: 6469 6d20 2b20 3129 2066 6f72 2050 6f6c  dim + 1) for Pol
-0000d760: 7941 6666 696e 6520 7061 7261 6d65 7465  yAffine paramete
-0000d770: 7273 2c20 696e 7374 6561 6420 6f66 207b  rs, instead of {
-0000d780: 646d 6174 7269 6365 732e 7368 6170 657d  dmatrices.shape}
-0000d790: 2e20 2229 0a20 2020 2020 2020 2069 6620  . ").        if 
-0000d7a0: 7472 616e 735f 7374 7265 7463 6820 6973  trans_stretch is
-0000d7b0: 206e 6f74 204e 6f6e 653a 2064 6d61 7472   not None: dmatr
-0000d7c0: 6963 6573 5b2e 2e2e 2c20 3a6e 5f64 696d  ices[..., :n_dim
-0000d7d0: 2c20 2d31 5d20 2a3d 2074 7261 6e73 5f73  , -1] *= trans_s
-0000d7e0: 7472 6574 6368 0a20 2020 2020 2020 206e  tretch.        n
-0000d7f0: 5f64 696d 203d 2064 6d61 7472 6963 6573  _dim = dmatrices
-0000d800: 2e73 697a 6528 2d31 2920 2d20 310a 2020  .size(-1) - 1.  
-0000d810: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-0000d820: 6e73 7461 6e63 6528 6d61 736b 732c 2062  nstance(masks, b
-0000d830: 742e 5465 6e73 6f72 293a 206d 6173 6b73  t.Tensor): masks
-0000d840: 203d 2062 742e 7465 6e73 6f72 286d 6173   = bt.tensor(mas
-0000d850: 6b73 290a 2020 2020 2020 2020 6966 206d  ks).        if m
-0000d860: 6173 6b73 2e6e 5f64 696d 203c 3d20 6e5f  asks.n_dim <= n_
-0000d870: 6469 6d20 2b20 3120 616e 6420 6e6f 7420  dim + 1 and not 
-0000d880: 6d61 736b 732e 6861 735f 6261 7463 683a  masks.has_batch:
-0000d890: 206d 6173 6b73 203d 206d 6173 6b73 2e75   masks = masks.u
-0000d8a0: 6e73 7175 6565 7a65 285b 5d29 0a20 2020  nsqueeze([]).   
-0000d8b0: 2020 2020 2069 6620 6d61 736b 732e 6e5f       if masks.n_
-0000d8c0: 6469 6d20 3c3d 206e 5f64 696d 202b 2031  dim <= n_dim + 1
-0000d8d0: 2061 6e64 206e 6f74 206d 6173 6b73 2e68   and not masks.h
-0000d8e0: 6173 5f63 6861 6e6e 656c 3a20 6d61 736b  as_channel: mask
-0000d8f0: 7320 3d20 6d61 736b 732e 756e 7371 7565  s = masks.unsque
-0000d900: 657a 6528 7b7d 290a 2020 2020 2020 2020  eze({}).        
-0000d910: 6966 206d 6173 6b73 2e6e 5f64 696d 203d  if masks.n_dim =
-0000d920: 3d20 6e5f 6469 6d20 2b20 3220 616e 6420  = n_dim + 2 and 
-0000d930: 6e6f 7420 6d61 736b 732e 6861 735f 6261  not masks.has_ba
-0000d940: 7463 683a 206d 6173 6b73 2e62 6174 6368  tch: masks.batch
-0000d950: 5f64 696d 656e 7369 6f6e 203d 2030 0a20  _dimension = 0. 
-0000d960: 2020 2020 2020 2069 6620 6d61 736b 732e         if masks.
-0000d970: 6e5f 6469 6d20 3d3d 206e 5f64 696d 202b  n_dim == n_dim +
-0000d980: 2032 2061 6e64 206e 6f74 206d 6173 6b73   2 and not masks
-0000d990: 2e68 6173 5f63 6861 6e6e 656c 3a20 6d61  .has_channel: ma
-0000d9a0: 736b 732e 6368 616e 6e65 6c5f 6469 6d65  sks.channel_dime
-0000d9b0: 6e73 696f 6e20 3d20 310a 2020 2020 2020  nsion = 1.      
-0000d9c0: 2020 6176 6f75 6368 286d 6173 6b73 2e68    avouch(masks.h
-0000d9d0: 6173 5f62 6174 6368 2061 6e64 206d 6173  as_batch and mas
-0000d9e0: 6b73 2e68 6173 5f63 6861 6e6e 656c 2c20  ks.has_channel, 
-0000d9f0: 2250 6c65 6173 6520 7573 6520 6261 746f  "Please use bato
-0000da00: 7263 6820 7465 6e73 6f72 206f 6620 7369  rch tensor of si
-0000da10: 7a65 2028 5b6e 5f62 6174 6368 5d2c 207b  ze ([n_batch], {
-0000da20: 6e5f 7265 6769 6f6e 7d2c 2220 2b0a 2020  n_region}," +.  
-0000da30: 2020 2020 2020 2020 2020 2020 2066 226e               f"n
-0000da40: 4031 2c20 6e40 322c 202e 2e2e 2c20 6e40  @1, n@2, ..., n@
-0000da50: 6e5f 6469 6d29 2066 6f72 2050 6f6c 7941  n_dim) for PolyA
-0000da60: 6666 696e 6520 7061 7261 6d65 7465 7273  ffine parameters
-0000da70: 2c20 696e 7374 6561 6420 6f66 207b 6d61  , instead of {ma
-0000da80: 736b 732e 7368 6170 657d 2e20 2229 0a0a  sks.shape}. ")..
-0000da90: 2020 2020 2020 2020 2320 7072 6570 726f          # prepro
-0000daa0: 6365 7373 206d 6173 6b73 2028 5b6e 5f62  cess masks ([n_b
-0000dab0: 6174 6368 5d2c 207b 6e5f 7265 6769 6f6e  atch], {n_region
-0000dac0: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
-0000dad0: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
-0000dae0: 2020 206e 5f62 6174 6368 203d 206d 6173     n_batch = mas
-0000daf0: 6b73 2e6e 5f62 6174 6368 0a20 2020 2020  ks.n_batch.     
-0000db00: 2020 206e 5f72 6567 696f 6e20 3d20 6d61     n_region = ma
-0000db10: 736b 732e 6e5f 6368 616e 6e65 6c0a 2020  sks.n_channel.  
-0000db20: 2020 2020 2020 6469 7320 3d20 6469 7374        dis = dist
-0000db30: 616e 6365 5f6d 6170 286d 6173 6b73 290a  ance_map(masks).
-0000db40: 2020 2020 2020 2020 6469 7320 3d20 2864          dis = (d
-0000db50: 6973 202b 2031 292e 636c 616d 7028 3029  is + 1).clamp(0)
-0000db60: 0a20 2020 2020 2020 2023 2069 6d70 6f72  .        # impor
-0000db70: 7420 6d69 636f 6d70 7574 696e 672e 706c  t micomputing.pl
-0000db80: 6f74 2061 7320 706c 740a 2020 2020 2020  ot as plt.      
-0000db90: 2020 2320 706c 742e 7375 6270 6c6f 7473    # plt.subplots
-0000dba0: 2832 290a 2020 2020 2020 2020 2320 706c  (2).        # pl
-0000dbb0: 742e 696d 7373 686f 7728 6469 735b 302c  t.imsshow(dis[0,
-0000dbc0: 2030 5d2c 2064 6973 5b30 2c20 315d 290a   0], dis[0, 1]).
-0000dbd0: 2020 2020 2020 2020 2320 706c 742e 7368          # plt.sh
-0000dbe0: 6f77 2829 0a20 2020 2020 2020 2077 6569  ow().        wei
-0000dbf0: 6768 7473 203d 2031 202f 2028 6469 7320  ghts = 1 / (dis 
-0000dc00: 2a2a 206f 7264 6572 202b 2031 652d 3529  ** order + 1e-5)
-0000dc10: 0a20 2020 2020 2020 2077 6569 6768 7473  .        weights
-0000dc20: 203d 2077 6569 6768 7473 202f 2077 6569   = weights / wei
-0000dc30: 6768 7473 2e73 756d 287b 7d29 2023 2028  ghts.sum({}) # (
-0000dc40: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 7265  [n_batch], {n_re
-0000dc50: 6769 6f6e 7d2c 206e 4031 2c20 6e40 322c  gion}, n@1, n@2,
-0000dc60: 202e 2e2e 2c20 6e40 6e5f 6469 6d29 0a20   ..., n@n_dim). 
-0000dc70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000dc80: 2320 2320 6465 7072 6563 6174 6564 2070  # # deprecated p
-0000dc90: 7265 7072 6f63 6573 7320 6f66 206d 6173  reprocess of mas
-0000dca0: 6b73 0a20 2020 2020 2020 2023 206d 6173  ks.        # mas
-0000dcb0: 6b73 203d 206d 6173 6b73 2e6e 756d 7079  ks = masks.numpy
-0000dcc0: 2829 2e61 7374 7970 6528 6e70 2e69 6e74  ().astype(np.int
-0000dcd0: 290a 2020 2020 2020 2020 2320 6e5f 6261  ).        # n_ba
-0000dce0: 7463 682c 206e 5f72 6567 696f 6e2c 202a  tch, n_region, *
-0000dcf0: 5f20 3d20 6d61 736b 732e 7368 6170 650a  _ = masks.shape.
-0000dd00: 2020 2020 2020 2020 2320 5f64 6973 5f6d          # _dis_m
-0000dd10: 6170 203d 2062 742e 7a65 726f 7328 2a6d  ap = bt.zeros(*m
-0000dd20: 6173 6b73 2e73 6861 7065 290a 2020 2020  asks.shape).    
-0000dd30: 2020 2020 2320 666f 7220 6920 696e 2072      # for i in r
-0000dd40: 616e 6765 286e 5f62 6174 6368 293a 0a20  ange(n_batch):. 
-0000dd50: 2020 2020 2020 2023 2020 2020 2066 6f72         #     for
-0000dd60: 206a 2069 6e20 7261 6e67 6528 6e5f 7265   j in range(n_re
-0000dd70: 6769 6f6e 293a 0a20 2020 2020 2020 2023  gion):.        #
-0000dd80: 2020 2020 2020 2020 206d 6173 6b5f 696d           mask_im
-0000dd90: 6167 6520 3d20 7369 746b 2e47 6574 496d  age = sitk.GetIm
-0000dda0: 6167 6546 726f 6d41 7272 6179 286d 6173  ageFromArray(mas
-0000ddb0: 6b73 5b69 2c20 6a5d 2c20 6973 5665 6374  ks[i, j], isVect
-0000ddc0: 6f72 203d 2046 616c 7365 290a 2020 2020  or = False).    
-0000ddd0: 2020 2020 2320 2020 2020 2020 2020 6469      #         di
-0000dde0: 735f 6d61 7020 3d20 7369 746b 2e47 6574  s_map = sitk.Get
-0000ddf0: 4172 7261 7956 6965 7746 726f 6d49 6d61  ArrayViewFromIma
-0000de00: 6765 2873 6974 6b2e 5369 676e 6564 4d61  ge(sitk.SignedMa
-0000de10: 7572 6572 4469 7374 616e 6365 4d61 7028  urerDistanceMap(
-0000de20: 6d61 736b 5f69 6d61 6765 2c20 7371 7561  mask_image, squa
-0000de30: 7265 6444 6973 7461 6e63 6520 3d20 4661  redDistance = Fa
-0000de40: 6c73 652c 2075 7365 496d 6167 6553 7061  lse, useImageSpa
-0000de50: 6369 6e67 203d 2046 616c 7365 2929 0a20  cing = False)). 
-0000de60: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0000de70: 2064 6973 5f6d 6170 203d 206e 702e 6172   dis_map = np.ar
-0000de80: 7261 7928 6469 735f 6d61 7029 2e61 7374  ray(dis_map).ast
-0000de90: 7970 6528 6e70 2e66 6c6f 6174 290a 2020  ype(np.float).  
-0000dea0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0000deb0: 5f64 6973 5f6d 6170 5b69 2c20 6a5d 203d  _dis_map[i, j] =
-0000dec0: 2062 742e 7465 6e73 6f72 2864 6973 5f6d   bt.tensor(dis_m
-0000ded0: 6170 202a 2028 6469 735f 6d61 7020 3e20  ap * (dis_map > 
-0000dee0: 3029 2e61 7374 7970 6528 6e70 2e66 6c6f  0).astype(np.flo
-0000def0: 6174 2929 0a20 2020 2020 2020 2023 206b  at)).        # k
-0000df00: 203d 2032 0a20 2020 2020 2020 2023 2069   = 2.        # i
-0000df10: 6e76 706f 776b 5f64 6973 5f6d 6170 203d  nvpowk_dis_map =
-0000df20: 2031 202f 2028 5f64 6973 5f6d 6170 202a   1 / (_dis_map *
-0000df30: 2a20 6b20 2b20 3165 2d35 290a 2020 2020  * k + 1e-5).    
-0000df40: 2020 2020 2320 7375 6d5f 6469 735f 6d61      # sum_dis_ma
-0000df50: 7020 3d20 696e 7670 6f77 6b5f 6469 735f  p = invpowk_dis_
-0000df60: 6d61 702e 7375 6d28 312c 206b 6565 7064  map.sum(1, keepd
-0000df70: 696d 203d 2054 7275 6529 0a20 2020 2020  im = True).     
-0000df80: 2020 2023 2077 6569 6768 7473 203d 2069     # weights = i
-0000df90: 6e76 706f 776b 5f64 6973 5f6d 6170 202f  nvpowk_dis_map /
-0000dfa0: 2073 756d 5f64 6973 5f6d 6170 0a20 2020   sum_dis_map.   
-0000dfb0: 2020 2020 2023 2066 726f 6d20 6d61 7470       # from matp
-0000dfc0: 6c6f 746c 6962 2069 6d70 6f72 7420 7079  lotlib import py
-0000dfd0: 706c 6f74 2061 7320 706c 740a 2020 2020  plot as plt.    
-0000dfe0: 2020 2020 2320 706c 742e 7375 6270 6c6f      # plt.subplo
-0000dff0: 7428 3132 3129 3b20 706c 742e 696d 7368  t(121); plt.imsh
-0000e000: 6f77 2877 6569 6768 7473 5b30 2c20 305d  ow(weights[0, 0]
-0000e010: 290a 2020 2020 2020 2020 2320 706c 742e  ).        # plt.
-0000e020: 7375 6270 6c6f 7428 3132 3229 3b20 706c  subplot(122); pl
-0000e030: 742e 696d 7368 6f77 2877 6569 6768 7473  t.imshow(weights
-0000e040: 5b30 2c20 315d 290a 2020 2020 2020 2020  [0, 1]).        
-0000e050: 2320 706c 742e 7368 6f77 2829 0a20 2020  # plt.show().   
-0000e060: 2020 2020 2023 2069 6620 7472 616e 735f       # if trans_
-0000e070: 7374 7265 7463 6820 6973 206e 6f74 204e  stretch is not N
-0000e080: 6f6e 653a 2064 6d61 7472 6963 6573 203d  one: dmatrices =
-0000e090: 2064 6d61 7472 6963 6573 202a 2062 742e   dmatrices * bt.
-0000e0a0: 7465 6e73 6f72 285b 312e 5d20 2a20 6e5f  tensor([1.] * n_
-0000e0b0: 6469 6d20 2b20 5b74 7261 6e73 5f73 7472  dim + [trans_str
-0000e0c0: 6574 6368 5d29 2e75 6e73 7175 6565 7a65  etch]).unsqueeze
-0000e0d0: 2830 2c20 302c 2030 290a 0a20 2020 2020  (0, 0, 0)..     
-0000e0e0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-0000e0f0: 745f 5f28 646d 6174 7269 6365 732c 206d  t__(dmatrices, m
-0000e100: 6173 6b73 3d6d 6173 6b73 2c20 6f72 6465  asks=masks, orde
-0000e110: 723d 6f72 6465 722c 2069 735f 696e 763d  r=order, is_inv=
-0000e120: 6973 5f69 6e76 2c20 7472 616e 735f 7374  is_inv, trans_st
-0000e130: 7265 7463 683d 7472 616e 735f 7374 7265  retch=trans_stre
-0000e140: 7463 6829 0a20 2020 2020 2020 2073 656c  tch).        sel
-0000e150: 662e 6e5f 6261 7463 6820 3d20 6e5f 6261  f.n_batch = n_ba
-0000e160: 7463 680a 2020 2020 2020 2020 7365 6c66  tch.        self
-0000e170: 2e6e 5f64 696d 203d 206e 5f64 696d 0a20  .n_dim = n_dim. 
-0000e180: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
-0000e190: 7320 3d20 6d61 736b 730a 2020 2020 2020  s = masks.      
-0000e1a0: 2020 7365 6c66 2e77 6569 6768 7473 203d    self.weights =
-0000e1b0: 2077 6569 6768 7473 0a20 2020 2020 2020   weights.       
-0000e1c0: 2073 656c 662e 7472 616e 735f 7374 7265   self.trans_stre
-0000e1d0: 7463 6820 3d20 7472 616e 735f 7374 7265  tch = trans_stre
-0000e1e0: 7463 680a 2020 2020 2020 2020 7365 6c66  tch.        self
-0000e1f0: 2e64 6d61 7472 6963 6573 203d 2064 6d61  .dmatrices = dma
-0000e200: 7472 6963 6573 0a20 2020 2020 2020 2073  trices.        s
-0000e210: 656c 662e 6973 5f69 6e76 203d 2069 735f  elf.is_inv = is_
-0000e220: 696e 760a 2020 2020 2020 2020 7365 6c66  inv.        self
-0000e230: 2e6f 7264 6572 203d 206f 7264 6572 0a0a  .order = order..
-0000e240: 2020 2020 6465 6620 5f5f 6361 6c6c 5f5f      def __call__
-0000e250: 2873 656c 662c 2058 293a 0a20 2020 2020  (self, X):.     
-0000e260: 2020 2058 203d 2073 7570 6572 2829 2e5f     X = super()._
-0000e270: 5f63 616c 6c5f 5f28 5829 0a20 2020 2020  _call__(X).     
-0000e280: 2020 2064 6d61 7472 6963 6573 203d 2073     dmatrices = s
-0000e290: 656c 662e 646d 6174 7269 6365 7320 2320  elf.dmatrices # 
-0000e2a0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
-0000e2b0: 6567 696f 6e7d 2c20 6e5f 6469 6d20 2b20  egion}, n_dim + 
-0000e2c0: 312c 206e 5f64 696d 202b 2031 290a 2020  1, n_dim + 1).  
-0000e2d0: 2020 2020 2020 7765 6967 6874 7320 3d20        weights = 
-0000e2e0: 7365 6c66 2e77 6569 6768 7473 2023 2028  self.weights # (
-0000e2f0: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 7265  [n_batch], {n_re
-0000e300: 6769 6f6e 7d2c 206e 4031 2c20 6e40 322c  gion}, n@1, n@2,
-0000e310: 202e 2e2e 2c20 6e40 6e5f 6469 6d29 0a20   ..., n@n_dim). 
-0000e320: 2020 2020 2020 206e 5f64 696d 203d 2073         n_dim = s
-0000e330: 656c 662e 6e5f 6469 6d0a 2020 2020 2020  elf.n_dim.      
-0000e340: 2020 6e5f 7265 6769 6f6e 203d 2064 6d61    n_region = dma
-0000e350: 7472 6963 6573 2e6e 5f63 6861 6e6e 656c  trices.n_channel
-0000e360: 0a20 2020 2020 2020 2058 7320 3d20 582e  .        Xs = X.
-0000e370: 6d75 6c74 6970 6c79 286e 5f72 6567 696f  multiply(n_regio
-0000e380: 6e2c 207b 7d29 2023 2028 5b6e 5f62 6174  n, {}) # ([n_bat
-0000e390: 6368 5d2c 207b 6e5f 7265 6769 6f6e 7d2c  ch], {n_region},
-0000e3a0: 206e 5f64 696d 2c20 6e40 312c 206e 4032   n_dim, n@1, n@2
-0000e3b0: 2c20 2e2e 2e2c 206e 406e 5f64 696d 290a  , ..., n@n_dim).
-0000e3c0: 2020 2020 2020 2020 4120 3d20 646d 6174          A = dmat
-0000e3d0: 7269 6365 735b 2e2e 2e2c 203a 6e5f 6469  rices[..., :n_di
-0000e3e0: 6d2c 203a 6e5f 6469 6d5d 0a20 2020 2020  m, :n_dim].     
-0000e3f0: 2020 2062 203d 2064 6d61 7472 6963 6573     b = dmatrices
-0000e400: 5b2e 2e2e 2c20 3a6e 5f64 696d 2c20 6e5f  [..., :n_dim, n_
-0000e410: 6469 6d3a 5d0a 2020 2020 2020 2020 5920  dim:].        Y 
-0000e420: 3d20 2841 2040 2058 732e 666c 6174 7465  = (A @ Xs.flatte
-0000e430: 6e28 3329 202b 2062 292e 7669 6577 5f61  n(3) + b).view_a
-0000e440: 7328 5873 290a 2020 2020 2020 2020 4420  s(Xs).        D 
-0000e450: 3d20 2859 202a 2077 6569 6768 7473 2e75  = (Y * weights.u
-0000e460: 6e73 7175 6565 7a65 2829 292e 7375 6d28  nsqueeze()).sum(
-0000e470: 7b7d 292e 7769 7468 5f63 6861 6e6e 656c  {}).with_channel
-0000e480: 6469 6d28 3129 202d 2058 0a20 2020 2020  dim(1) - X.     
-0000e490: 2020 2069 6620 7365 6c66 2e69 735f 696e     if self.is_in
-0000e4a0: 763a 2044 203d 202d 440a 2020 2020 2020  v: D = -D.      
-0000e4b0: 2020 7472 616e 7320 3d20 4465 6e73 6544    trans = DenseD
-0000e4c0: 6973 706c 6163 656d 656e 7446 6965 6c64  isplacementField
-0000e4d0: 2844 290a 2020 2020 2020 2020 7472 616e  (D).        tran
-0000e4e0: 7332 203d 2044 656e 7365 4469 7370 6c61  s2 = DenseDispla
-0000e4f0: 6365 6d65 6e74 4669 656c 6428 7472 616e  cementField(tran
-0000e500: 7328 7472 616e 7328 5829 2920 2d20 5829  s(trans(X)) - X)
-0000e510: 0a20 2020 2020 2020 2074 7261 6e73 3420  .        trans4 
-0000e520: 3d20 4465 6e73 6544 6973 706c 6163 656d  = DenseDisplacem
-0000e530: 656e 7446 6965 6c64 2874 7261 6e73 3228  entField(trans2(
-0000e540: 7472 616e 7332 2858 2929 202d 2058 290a  trans2(X)) - X).
-0000e550: 2020 2020 2020 2020 7472 616e 7338 203d          trans8 =
-0000e560: 2044 656e 7365 4469 7370 6c61 6365 6d65   DenseDisplaceme
-0000e570: 6e74 4669 656c 6428 7472 616e 7334 2874  ntField(trans4(t
-0000e580: 7261 6e73 3428 5829 2920 2d20 5829 0a20  rans4(X)) - X). 
-0000e590: 2020 2020 2020 2074 7261 6e73 3136 203d         trans16 =
-0000e5a0: 2044 656e 7365 4469 7370 6c61 6365 6d65   DenseDisplaceme
-0000e5b0: 6e74 4669 656c 6428 7472 616e 7338 2874  ntField(trans8(t
-0000e5c0: 7261 6e73 3828 5829 2920 2d20 5829 0a20  rans8(X)) - X). 
-0000e5d0: 2020 2020 2020 2074 7261 6e73 3332 203d         trans32 =
-0000e5e0: 2044 656e 7365 4469 7370 6c61 6365 6d65   DenseDisplaceme
-0000e5f0: 6e74 4669 656c 6428 7472 616e 7331 3628  ntField(trans16(
-0000e600: 7472 616e 7331 3628 5829 2920 2d20 5829  trans16(X)) - X)
-0000e610: 0a20 2020 2020 2020 2074 7261 6e73 3634  .        trans64
-0000e620: 203d 2044 656e 7365 4469 7370 6c61 6365   = DenseDisplace
-0000e630: 6d65 6e74 4669 656c 6428 7472 616e 7333  mentField(trans3
-0000e640: 3228 7472 616e 7333 3228 5829 2920 2d20  2(trans32(X)) - 
-0000e650: 5829 0a20 2020 2020 2020 2072 6574 7572  X).        retur
-0000e660: 6e20 7472 616e 7336 3428 5829 0a0a 2020  n trans64(X)..  
-0000e670: 2020 6465 6620 696e 7628 7365 6c66 293a    def inv(self):
-0000e680: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e690: 506f 6c79 4166 6669 6e65 2873 656c 662e  PolyAffine(self.
-0000e6a0: 646d 6174 7269 6365 732c 2073 656c 662e  dmatrices, self.
-0000e6b0: 6d61 736b 732c 206f 7264 6572 3d73 656c  masks, order=sel
-0000e6c0: 662e 6f72 6465 722c 2069 735f 696e 763d  f.order, is_inv=
-0000e6d0: 6e6f 7420 7365 6c66 2e69 735f 696e 762c  not self.is_inv,
-0000e6e0: 2074 7261 6e73 5f73 7472 6574 6368 203d   trans_stretch =
-0000e6f0: 2031 292e 6261 636b 7761 7264 5f28 7365   1).backward_(se
-0000e700: 6c66 2e62 6163 6b77 6172 6429 0a20 2020  lf.backward).   
-0000e710: 2020 2020 2023 206e 5f62 6174 6368 203d       # n_batch =
-0000e720: 2073 656c 662e 646d 6174 7269 6365 732e   self.dmatrices.
-0000e730: 6e5f 6261 7463 680a 2020 2020 2020 2020  n_batch.        
-0000e740: 2320 6166 6673 203d 2062 742e 696e 7628  # affs = bt.inv(
-0000e750: 7365 6c66 2e64 6d61 7472 6963 6573 290a  self.dmatrices).
-0000e760: 2020 2020 2020 2020 2320 6d61 736b 7320          # masks 
-0000e770: 3d20 696e 7465 7270 6f6c 6174 696f 6e28  = interpolation(
-0000e780: 7365 6c66 2e6d 6173 6b73 2e6d 6572 6765  self.masks.merge
-0000e790: 6469 6d73 285b 5d2c 207b 7d29 2c20 4166  dims([], {}), Af
-0000e7a0: 6669 6e65 2862 742e 6d61 7470 6f77 2861  fine(bt.matpow(a
-0000e7b0: 6666 732e 6d65 7267 6564 696d 7328 5b5d  ffs.mergedims([]
-0000e7c0: 2c20 7b7d 292c 2036 3429 2929 2e73 706c  , {}), 64))).spl
-0000e7d0: 6974 6469 6d28 5b5d 2c20 5b6e 5f62 6174  itdim([], [n_bat
-0000e7e0: 6368 5d2c 207b 2d31 7d29 0a20 2020 2020  ch], {-1}).     
-0000e7f0: 2020 2023 2072 6574 7572 6e20 506f 6c79     # return Poly
-0000e800: 4166 6669 6e65 2861 6666 732c 206d 6173  Affine(affs, mas
-0000e810: 6b73 203d 206d 6173 6b73 2c20 7472 616e  ks = masks, tran
-0000e820: 735f 7374 7265 7463 6820 3d20 7365 6c66  s_stretch = self
-0000e830: 2e74 7261 6e73 5f73 7472 6574 6368 292e  .trans_stretch).
-0000e840: 6261 636b 7761 7264 5f28 7365 6c66 2e62  backward_(self.b
-0000e850: 6163 6b77 6172 6429 0a0a 4061 6c69 6173  ackward)..@alias
-0000e860: 2822 4c41 524d 2229 0a63 6c61 7373 204c  ("LARM").class L
-0000e870: 6f63 616c 6c79 4166 6669 6e65 2853 7061  ocallyAffine(Spa
-0000e880: 7469 616c 5472 616e 7366 6f72 6d61 7469  tialTransformati
-0000e890: 6f6e 293a 0a20 2020 2064 6566 205f 5f69  on):.    def __i
-0000e8a0: 6e69 745f 5f28 7365 6c66 2c20 6d61 7472  nit__(self, matr
-0000e8b0: 6963 6573 2c20 6d61 736b 732c 206f 7264  ices, masks, ord
-0000e8c0: 6572 3d32 2c20 7472 616e 735f 7374 7265  er=2, trans_stre
-0000e8d0: 7463 683d 4e6f 6e65 2c20 6176 6f69 645f  tch=None, avoid_
-0000e8e0: 636f 6e66 6c69 6374 3d54 7275 6529 3a0a  conflict=True):.
-0000e8f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0000e900: 2020 2020 4c6f 6361 6c6c 7920 6166 6669      Locally affi
-0000e910: 6e65 2074 7261 6e73 666f 726d 6174 696f  ne transformatio
-0000e920: 6e20 7769 7468 2072 6573 7065 6374 2074  n with respect t
-0000e930: 6f20 7472 616e 7366 6f72 6d61 7469 6f6e  o transformation
-0000e940: 206d 6174 7269 6365 7320 5b31 5d2e 0a20   matrices [1].. 
-0000e950: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000e960: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
-0000e970: 2020 2020 6d61 7472 6963 6573 205b 6274      matrices [bt
-0000e980: 2e54 656e 736f 7220 6f72 206e 702e 6e75  .Tensor or np.nu
-0000e990: 6d70 795d 3a20 4f6e 6520 6166 6669 6e65  mpy]: One affine
-0000e9a0: 206d 6174 7269 7820 666f 7220 6561 6368   matrix for each
-0000e9b0: 2072 6567 696f 6e2e 200a 2020 2020 2020   region. .      
-0000e9c0: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-0000e9d0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
-0000e9e0: 6567 696f 6e7d 2c20 6e5f 6469 6d20 2b20  egion}, n_dim + 
-0000e9f0: 312c 206e 5f64 696d 202b 2031 290a 2020  1, n_dim + 1).  
-0000ea00: 2020 2020 2020 2020 2020 6d61 736b 7320            masks 
-0000ea10: 5b62 742e 5465 6e73 6f72 206f 7220 6e70  [bt.Tensor or np
-0000ea20: 2e6e 756d 7079 5d3a 204f 6e65 2030 2d31  .numpy]: One 0-1
-0000ea30: 206d 6173 6b20 666f 7220 6561 6368 2072   mask for each r
-0000ea40: 6567 696f 6e2e 200a 2020 2020 2020 2020  egion. .        
-0000ea50: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
-0000ea60: 6e5f 6261 7463 685d 2c20 7b6e 5f72 6567  n_batch], {n_reg
-0000ea70: 696f 6e7d 2c20 6e40 312c 206e 4032 2c20  ion}, n@1, n@2, 
-0000ea80: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
-0000ea90: 2020 2020 2020 2020 2020 6f72 6465 7220            order 
-0000eaa0: 5b69 6e74 5d3a 2074 6865 206f 7264 6572  [int]: the order
-0000eab0: 206f 6620 696e 7465 7270 6f6c 6174 696f   of interpolatio
-0000eac0: 6e20 636f 6566 6669 6369 656e 742e 2054  n coefficient. T
-0000ead0: 6865 2069 6e66 6c75 656e 6365 206f 6620  he influence of 
-0000eae0: 616e 2061 6666 696e 6520 6465 6361 7973  an affine decays
-0000eaf0: 2061 7420 6120 7261 7465 206f 6620 3120   at a rate of 1 
-0000eb00: 2f20 6469 7374 616e 6365 5e6f 7264 6572  / distance^order
-0000eb10: 2e0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-0000eb20: 616e 735f 7374 7265 7463 6820 5b69 6e74  ans_stretch [int
-0000eb30: 5d3a 206f 6e6c 7920 7573 6564 2066 6f72  ]: only used for
-0000eb40: 2069 7465 7261 7469 7665 2070 6172 616d   iterative param
-0000eb50: 6574 6572 2074 7261 696e 696e 672c 2031  eter training, 1
-0000eb60: 2062 7920 6465 6661 756c 742e 2032 3020   by default. 20 
-0000eb70: 7365 656d 7320 746f 2062 6520 6120 676f  seems to be a go
-0000eb80: 6f64 2063 686f 6963 652e 2020 0a20 2020  od choice.  .   
-0000eb90: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-0000eba0: 2020 5768 656e 2069 7420 6973 2063 616c    When it is cal
-0000ebb0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-0000ebc0: 2058 205b 6274 2e54 656e 736f 725d 3a20   X [bt.Tensor]: 
-0000ebd0: 436f 6f72 6469 6e61 7465 7320 746f 2062  Coordinates to b
-0000ebe0: 6520 7472 616e 7366 6f72 6d65 642e 0a20  e transformed.. 
-0000ebf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ec00: 697a 653a 2028 5b6e 5f62 6174 6368 3a20  ize: ([n_batch: 
-0000ec10: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
-0000ec20: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
-0000ec30: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
-0000ec40: 2020 2020 2020 2020 6f75 7470 7574 205b          output [
-0000ec50: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
-0000ec60: 7472 616e 7366 6f72 6d65 6420 636f 6f72  transformed coor
-0000ec70: 6469 6e61 7465 732e 0a20 2020 2020 2020  dinates..       
-0000ec80: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-0000ec90: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-0000eca0: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
-0000ecb0: 2e2c 206e 406e 5f64 696d 290a 0a20 2020  ., n@n_dim)..   
-0000ecc0: 2020 2020 205b 315d 205a 6875 616e 6720       [1] Zhuang 
-0000ecd0: 5820 2c20 5268 6f64 6520 4b20 2c20 4172  X , Rhode K , Ar
-0000ece0: 7269 6467 6520 5320 2c20 6574 2061 6c2e  ridge S , et al.
-0000ecf0: 2041 6e20 4174 6c61 732d 4261 7365 6420   An Atlas-Based 
-0000ed00: 5365 676d 656e 7461 7469 6f6e 2050 726f  Segmentation Pro
-0000ed10: 7061 6761 7469 6f6e 2046 7261 6d65 776f  pagation Framewo
-0000ed20: 726b 2055 7369 6e67 204c 6f63 616c 6c79  rk Using Locally
-0000ed30: 2041 6666 696e 6520 0a20 2020 2020 2020   Affine .       
-0000ed40: 2020 2020 2052 6567 6973 7472 6174 696f       Registratio
-0000ed50: 6e20 2d20 4170 706c 6963 6174 696f 6e20  n - Application 
-0000ed60: 746f 2041 7574 6f6d 6174 6963 2057 686f  to Automatic Who
-0000ed70: 6c65 2048 6561 7274 2053 6567 6d65 6e74  le Heart Segment
-0000ed80: 6174 696f 6e5b 4a5d 2e20 5370 7269 6e67  ation[J]. Spring
-0000ed90: 6572 2c20 4265 726c 696e 2c20 4865 6964  er, Berlin, Heid
-0000eda0: 656c 6265 7267 2c20 3230 3038 2e0a 2020  elberg, 2008..  
-0000edb0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0000edc0: 2020 696d 706f 7274 2053 696d 706c 6549    import SimpleI
-0000edd0: 544b 2061 7320 7369 746b 0a20 2020 2020  TK as sitk.     
-0000ede0: 2020 2066 726f 6d20 2e66 756e 6373 2069     from .funcs i
-0000edf0: 6d70 6f72 7420 6469 6c61 7465 2c20 6469  mport dilate, di
-0000ee00: 7374 616e 6365 5f6d 6170 0a20 2020 2020  stance_map.     
-0000ee10: 2020 206d 6174 7269 6365 7320 3d20 6261     matrices = ba
-0000ee20: 746f 7263 685f 7465 6e73 6f72 286d 6174  torch_tensor(mat
-0000ee30: 7269 6365 7329 0a20 2020 2020 2020 2069  rices).        i
-0000ee40: 6620 6d61 7472 6963 6573 2e6e 5f64 696d  f matrices.n_dim
-0000ee50: 203c 3d20 3320 616e 6420 6e6f 7420 6d61   <= 3 and not ma
-0000ee60: 7472 6963 6573 2e68 6173 5f62 6174 6368  trices.has_batch
-0000ee70: 3a20 6d61 7472 6963 6573 203d 206d 6174  : matrices = mat
-0000ee80: 7269 6365 732e 756e 7371 7565 657a 6528  rices.unsqueeze(
-0000ee90: 5b5d 290a 2020 2020 2020 2020 6966 206d  []).        if m
-0000eea0: 6174 7269 6365 732e 6e5f 6469 6d20 3c3d  atrices.n_dim <=
-0000eeb0: 2033 2061 6e64 206e 6f74 206d 6174 7269   3 and not matri
-0000eec0: 6365 732e 6861 735f 6368 616e 6e65 6c3a  ces.has_channel:
-0000eed0: 206d 6174 7269 6365 7320 3d20 6d61 7472   matrices = matr
-0000eee0: 6963 6573 2e75 6e73 7175 6565 7a65 287b  ices.unsqueeze({
-0000eef0: 7d29 0a20 2020 2020 2020 2069 6620 6d61  }).        if ma
-0000ef00: 7472 6963 6573 2e6e 5f64 696d 203d 3d20  trices.n_dim == 
-0000ef10: 3420 616e 6420 6d61 7472 6963 6573 2e73  4 and matrices.s
-0000ef20: 6861 7065 5b32 5d20 3d3d 206d 6174 7269  hape[2] == matri
-0000ef30: 6365 732e 7368 6170 655b 335d 3a0a 2020  ces.shape[3]:.  
-0000ef40: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000ef50: 206d 6174 7269 6365 732e 6861 735f 6261   matrices.has_ba
-0000ef60: 7463 683a 206d 6174 7269 6365 732e 6261  tch: matrices.ba
-0000ef70: 7463 685f 6469 6d65 6e73 696f 6e20 3d20  tch_dimension = 
-0000ef80: 300a 2020 2020 2020 2020 2020 2020 6966  0.            if
-0000ef90: 206e 6f74 206d 6174 7269 6365 732e 6861   not matrices.ha
-0000efa0: 735f 6368 616e 6e65 6c3a 206d 6174 7269  s_channel: matri
-0000efb0: 6365 732e 6368 616e 6e65 6c5f 6469 6d65  ces.channel_dime
-0000efc0: 6e73 696f 6e20 3d20 310a 2020 2020 2020  nsion = 1.      
-0000efd0: 2020 6176 6f75 6368 286d 6174 7269 6365    avouch(matrice
-0000efe0: 732e 6861 735f 6261 7463 6820 616e 6420  s.has_batch and 
-0000eff0: 6d61 7472 6963 6573 2e68 6173 5f63 6861  matrices.has_cha
-0000f000: 6e6e 656c 2c20 2250 6c65 6173 6520 7573  nnel, "Please us
-0000f010: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
-0000f020: 206f 6620 7369 7a65 2028 5b6e 5f62 6174   of size ([n_bat
-0000f030: 6368 5d2c 207b 6e5f 7265 6769 6f6e 7d2c  ch], {n_region},
-0000f040: 2220 2b0a 2020 2020 2020 2020 2020 2020  " +.            
-0000f050: 2020 2066 226e 5f64 696d 202b 2031 2c20     f"n_dim + 1, 
-0000f060: 6e5f 6469 6d20 2b20 3129 2066 6f72 204c  n_dim + 1) for L
-0000f070: 6f63 616c 6c79 4166 6669 6e65 2070 6172  ocallyAffine par
-0000f080: 616d 6574 6572 732c 2069 6e73 7465 6164  ameters, instead
-0000f090: 206f 6620 7b6d 6174 7269 6365 732e 7368   of {matrices.sh
-0000f0a0: 6170 657d 2e20 2229 0a20 2020 2020 2020  ape}. ").       
-0000f0b0: 2069 6620 7472 616e 735f 7374 7265 7463   if trans_stretc
-0000f0c0: 6820 6973 206e 6f74 204e 6f6e 653a 206d  h is not None: m
-0000f0d0: 6174 7269 6365 735b 2e2e 2e2c 203a 6e5f  atrices[..., :n_
-0000f0e0: 6469 6d2c 202d 315d 202a 3d20 7472 616e  dim, -1] *= tran
-0000f0f0: 735f 7374 7265 7463 680a 2020 2020 2020  s_stretch.      
-0000f100: 2020 6e5f 6469 6d20 3d20 6d61 7472 6963    n_dim = matric
-0000f110: 6573 2e73 697a 6528 2d31 2920 2d20 310a  es.size(-1) - 1.
-0000f120: 2020 2020 2020 2020 6d61 736b 7320 3d20          masks = 
-0000f130: 6261 746f 7263 685f 7465 6e73 6f72 286d  batorch_tensor(m
-0000f140: 6173 6b73 290a 2020 2020 2020 2020 6966  asks).        if
-0000f150: 206d 6173 6b73 2e6e 5f64 696d 203c 3d20   masks.n_dim <= 
-0000f160: 6e5f 6469 6d20 2b20 3120 616e 6420 6e6f  n_dim + 1 and no
-0000f170: 7420 6d61 736b 732e 6861 735f 6261 7463  t masks.has_batc
-0000f180: 683a 206d 6173 6b73 203d 206d 6173 6b73  h: masks = masks
-0000f190: 2e75 6e73 7175 6565 7a65 285b 5d29 0a20  .unsqueeze([]). 
-0000f1a0: 2020 2020 2020 2069 6620 6d61 736b 732e         if masks.
-0000f1b0: 6e5f 6469 6d20 3c3d 206e 5f64 696d 202b  n_dim <= n_dim +
-0000f1c0: 2031 2061 6e64 206e 6f74 206d 6173 6b73   1 and not masks
-0000f1d0: 2e68 6173 5f63 6861 6e6e 656c 3a20 6d61  .has_channel: ma
-0000f1e0: 736b 7320 3d20 6d61 736b 732e 756e 7371  sks = masks.unsq
-0000f1f0: 7565 657a 6528 7b7d 290a 2020 2020 2020  ueeze({}).      
-0000f200: 2020 6966 206d 6173 6b73 2e6e 5f64 696d    if masks.n_dim
-0000f210: 203d 3d20 6e5f 6469 6d20 2b20 3220 616e   == n_dim + 2 an
-0000f220: 6420 6e6f 7420 6d61 736b 732e 6861 735f  d not masks.has_
-0000f230: 6261 7463 683a 206d 6173 6b73 2e62 6174  batch: masks.bat
-0000f240: 6368 5f64 696d 656e 7369 6f6e 203d 2030  ch_dimension = 0
-0000f250: 0a20 2020 2020 2020 2069 6620 6d61 736b  .        if mask
-0000f260: 732e 6e5f 6469 6d20 3d3d 206e 5f64 696d  s.n_dim == n_dim
-0000f270: 202b 2032 2061 6e64 206e 6f74 206d 6173   + 2 and not mas
-0000f280: 6b73 2e68 6173 5f63 6861 6e6e 656c 3a20  ks.has_channel: 
-0000f290: 6d61 736b 732e 6368 616e 6e65 6c5f 6469  masks.channel_di
-0000f2a0: 6d65 6e73 696f 6e20 3d20 310a 2020 2020  mension = 1.    
-0000f2b0: 2020 2020 6176 6f75 6368 286d 6173 6b73      avouch(masks
-0000f2c0: 2e68 6173 5f62 6174 6368 2061 6e64 206d  .has_batch and m
-0000f2d0: 6173 6b73 2e68 6173 5f63 6861 6e6e 656c  asks.has_channel
-0000f2e0: 2c20 2250 6c65 6173 6520 7573 6520 6261  , "Please use ba
-0000f2f0: 746f 7263 6820 7465 6e73 6f72 206f 6620  torch tensor of 
-0000f300: 7369 7a65 2028 5b6e 5f62 6174 6368 5d2c  size ([n_batch],
-0000f310: 207b 6e5f 7265 6769 6f6e 7d2c 2220 2b20   {n_region}," + 
-0000f320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f330: 6622 6e40 312c 206e 4032 2c20 2e2e 2e2c  f"n@1, n@2, ...,
-0000f340: 206e 406e 5f64 696d 2920 666f 7220 4c6f   n@n_dim) for Lo
-0000f350: 6361 6c6c 7941 6666 696e 6520 7061 7261  callyAffine para
-0000f360: 6d65 7465 7273 2c20 696e 7374 6561 6420  meters, instead 
-0000f370: 6f66 207b 6d61 736b 732e 7368 6170 657d  of {masks.shape}
-0000f380: 2e20 2229 0a0a 2020 2020 2020 2020 2320  . ")..        # 
-0000f390: 7072 6570 726f 6365 7373 206d 6173 6b73  preprocess masks
-0000f3a0: 0a20 2020 2020 2020 206e 5f62 6174 6368  .        n_batch
-0000f3b0: 203d 206d 6174 7269 6365 732e 6e5f 6261   = matrices.n_ba
-0000f3c0: 7463 680a 2020 2020 2020 2020 6e5f 7265  tch.        n_re
-0000f3d0: 6769 6f6e 203d 206d 6174 7269 6365 732e  gion = matrices.
-0000f3e0: 6e5f 6368 616e 6e65 6c0a 2020 2020 2020  n_channel.      
-0000f3f0: 2020 6966 2061 766f 6964 5f63 6f6e 666c    if avoid_confl
-0000f400: 6963 743a 0a20 2020 2020 2020 2020 2020  ict:.           
-0000f410: 2047 6920 3d20 4166 6669 6e65 286d 6174   Gi = Affine(mat
-0000f420: 7269 6365 732e 6d65 7267 6564 696d 7328  rices.mergedims(
-0000f430: 7b7d 2c20 5b5d 2929 0a20 2020 2020 2020  {}, [])).       
-0000f440: 2020 2020 2047 6956 6920 3d20 696e 7465       GiVi = inte
-0000f450: 7270 6f6c 6174 696f 6e28 6d61 736b 732e  rpolation(masks.
-0000f460: 6d65 7267 6564 696d 7328 7b7d 2c20 5b5d  mergedims({}, []
-0000f470: 292c 2047 692e 696e 7628 292c 206d 6574  ), Gi.inv(), met
-0000f480: 686f 643d 274e 6561 7265 7374 2729 2e73  hod='Nearest').s
-0000f490: 706c 6974 6469 6d28 5b5d 2c20 5b6e 5f62  plitdim([], [n_b
-0000f4a0: 6174 6368 5d2c 206e 5f72 6567 696f 6e29  atch], n_region)
-0000f4b0: 2023 2028 5b6e 5f62 6174 6368 5d2c 206e   # ([n_batch], n
-0000f4c0: 5f72 6567 696f 6e2c 206e 4031 2c20 6e40  _region, n@1, n@
-0000f4d0: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
-0000f4e0: 0a20 2020 2020 2020 2020 2020 2047 6956  .            GiV
-0000f4f0: 696a 6f69 6e47 6b56 6b20 3d20 2847 6956  ijoinGkVk = (GiV
-0000f500: 692e 756e 7371 7565 657a 6528 3129 202a  i.unsqueeze(1) *
-0000f510: 2047 6956 692e 756e 7371 7565 657a 6528   GiVi.unsqueeze(
-0000f520: 3229 292e 6d65 7267 6564 696d 7328 312c  2)).mergedims(1,
-0000f530: 205b 5d29 2e77 6974 685f 6368 616e 6e65   []).with_channe
-0000f540: 6c64 696d 2831 2920 2320 285b 6e5f 6261  ldim(1) # ([n_ba
-0000f550: 7463 6820 7820 6e5f 7265 6769 6f6e 5d2c  tch x n_region],
-0000f560: 207b 6e5f 7265 6769 6f6e 7d2c 206e 4031   {n_region}, n@1
-0000f570: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-0000f580: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-0000f590: 2052 696b 203d 2069 6e74 6572 706f 6c61   Rik = interpola
-0000f5a0: 7469 6f6e 2847 6956 696a 6f69 6e47 6b56  tion(GiVijoinGkV
-0000f5b0: 6b2c 2047 692c 206d 6574 686f 643d 274e  k, Gi, method='N
-0000f5c0: 6561 7265 7374 2729 2e73 706c 6974 6469  earest').splitdi
-0000f5d0: 6d28 5b5d 2c20 5b6e 5f62 6174 6368 5d2c  m([], [n_batch],
-0000f5e0: 206e 5f72 6567 696f 6e29 2023 2028 5b6e   n_region) # ([n
-0000f5f0: 5f62 6174 6368 5d2c 206e 5f72 6567 696f  _batch], n_regio
-0000f600: 6e2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  n, {n_region}, n
-0000f610: 4031 2c20 6e40 322c 202e 2e2e 2c20 6e40  @1, n@2, ..., n@
-0000f620: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
-0000f630: 2020 2055 5269 6b20 3d20 2852 696b 2e73     URik = (Rik.s
-0000f640: 756d 287b 7d29 2e77 6974 685f 6368 616e  um({}).with_chan
-0000f650: 6e65 6c64 696d 2831 2920 2d20 6d61 736b  neldim(1) - mask
-0000f660: 7320 3e20 302e 3129 2e66 6c6f 6174 2829  s > 0.1).float()
-0000f670: 2023 2028 5b6e 5f62 6174 6368 5d2c 207b   # ([n_batch], {
-0000f680: 6e5f 7265 6769 6f6e 7d2c 206e 4031 2c20  n_region}, n@1, 
-0000f690: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-0000f6a0: 6d29 0a20 2020 2020 2020 2020 2020 2055  m).            U
-0000f6b0: 5269 6b5f 706c 7573 203d 2064 696c 6174  Rik_plus = dilat
-0000f6c0: 6528 5552 696b 2e6d 6572 6765 6469 6d73  e(URik.mergedims
-0000f6d0: 287b 7d2c 205b 5d29 2c20 3129 2e73 706c  ({}, []), 1).spl
-0000f6e0: 6974 6469 6d28 5b5d 2c20 5b6e 5f62 6174  itdim([], [n_bat
-0000f6f0: 6368 5d2c 206e 5f72 6567 696f 6e29 2023  ch], n_region) #
-0000f700: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
-0000f710: 7265 6769 6f6e 7d2c 206e 4031 2c20 6e40  region}, n@1, n@
-0000f720: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
-0000f730: 0a20 2020 2020 2020 2020 2020 206d 6173  .            mas
-0000f740: 6b73 203d 2028 6d61 736b 7320 2d20 5552  ks = (masks - UR
-0000f750: 696b 5f70 6c75 7320 3e20 302e 3129 2e66  ik_plus > 0.1).f
-0000f760: 6c6f 6174 2829 2023 2028 5b6e 5f62 6174  loat() # ([n_bat
-0000f770: 6368 5d2c 207b 6e5f 7265 6769 6f6e 7d2c  ch], {n_region},
-0000f780: 206e 4031 2c20 6e40 322c 202e 2e2e 2c20   n@1, n@2, ..., 
-0000f790: 6e40 6e5f 6469 6d29 0a0a 2020 2020 2020  n@n_dim)..      
-0000f7a0: 2020 7765 6967 6874 7320 3d20 3120 2f20    weights = 1 / 
-0000f7b0: 2864 6973 7461 6e63 655f 6d61 7028 6d61  (distance_map(ma
-0000f7c0: 736b 7329 202a 2a20 6f72 6465 7220 2b20  sks) ** order + 
-0000f7d0: 3165 2d35 290a 2020 2020 2020 2020 7765  1e-5).        we
-0000f7e0: 6967 6874 7320 3d20 7765 6967 6874 7320  ights = weights 
-0000f7f0: 2f20 7765 6967 6874 732e 7375 6d28 7b7d  / weights.sum({}
-0000f800: 2920 2320 285b 6e5f 6261 7463 685d 2c20  ) # ([n_batch], 
-0000f810: 7b6e 5f72 6567 696f 6e7d 2c20 6e40 312c  {n_region}, n@1,
-0000f820: 206e 4032 2c20 2e2e 2e2c 206e 406e 5f64   n@2, ..., n@n_d
-0000f830: 696d 290a 2020 2020 2020 2020 2320 6966  im).        # if
-0000f840: 2074 7261 6e73 5f73 7472 6574 6368 2069   trans_stretch i
-0000f850: 7320 6e6f 7420 4e6f 6e65 3a20 6d61 7472  s not None: matr
-0000f860: 6963 6573 203d 206d 6174 7269 6365 7320  ices = matrices 
-0000f870: 2a20 6261 746f 7263 685f 7465 6e73 6f72  * batorch_tensor
-0000f880: 285b 312e 5d20 2a20 6e5f 6469 6d20 2b20  ([1.] * n_dim + 
-0000f890: 5b74 7261 6e73 5f73 7472 6574 6368 5d29  [trans_stretch])
-0000f8a0: 2e75 6e73 7175 6565 7a65 2830 2c20 302c  .unsqueeze(0, 0,
-0000f8b0: 2030 290a 0a20 2020 2020 2020 2073 7570   0)..        sup
-0000f8c0: 6572 2829 2e5f 5f69 6e69 745f 5f28 6d61  er().__init__(ma
-0000f8d0: 7472 6963 6573 2c20 6d61 736b 733d 6d61  trices, masks=ma
-0000f8e0: 736b 732c 206f 7264 6572 3d6f 7264 6572  sks, order=order
-0000f8f0: 2c20 7472 616e 735f 7374 7265 7463 683d  , trans_stretch=
-0000f900: 7472 616e 735f 7374 7265 7463 6829 0a20  trans_stretch). 
-0000f910: 2020 2020 2020 2073 656c 662e 6e5f 6261         self.n_ba
-0000f920: 7463 6820 3d20 6e5f 6261 7463 680a 2020  tch = n_batch.  
-0000f930: 2020 2020 2020 7365 6c66 2e6e 5f64 696d        self.n_dim
-0000f940: 203d 206e 5f64 696d 0a20 2020 2020 2020   = n_dim.       
-0000f950: 2073 656c 662e 6d61 736b 7320 3d20 6d61   self.masks = ma
-0000f960: 736b 730a 2020 2020 2020 2020 7365 6c66  sks.        self
-0000f970: 2e77 6569 6768 7473 203d 2077 6569 6768  .weights = weigh
-0000f980: 7473 0a20 2020 2020 2020 2073 656c 662e  ts.        self.
-0000f990: 7472 616e 735f 7374 7265 7463 6820 3d20  trans_stretch = 
-0000f9a0: 7472 616e 735f 7374 7265 7463 680a 2020  trans_stretch.  
-0000f9b0: 2020 2020 2020 7365 6c66 2e6d 6174 7269        self.matri
-0000f9c0: 6365 7320 3d20 6d61 7472 6963 6573 0a20  ces = matrices. 
-0000f9d0: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
-0000f9e0: 685f 7061 7261 6d2e 6578 7465 6e64 285b  h_param.extend([
-0000f9f0: 276d 6174 7269 6365 7327 2c20 2777 6569  'matrices', 'wei
-0000fa00: 6768 7473 272c 2027 6d61 736b 7327 5d29  ghts', 'masks'])
-0000fa10: 0a0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
-0000fa20: 5f5f 2873 656c 662c 2058 293a 0a20 2020  __(self, X):.   
-0000fa30: 2020 2020 2058 203d 2073 7570 6572 2829       X = super()
-0000fa40: 2e5f 5f63 616c 6c5f 5f28 5829 0a20 2020  .__call__(X).   
-0000fa50: 2020 2020 206d 6174 7269 6365 7320 3d20       matrices = 
-0000fa60: 7365 6c66 2e6d 6174 7269 6365 730a 2020  self.matrices.  
-0000fa70: 2020 2020 2020 6d61 736b 7320 3d20 7365        masks = se
-0000fa80: 6c66 2e6d 6173 6b73 2023 2028 5b6e 5f62  lf.masks # ([n_b
-0000fa90: 6174 6368 5d2c 207b 6e5f 7265 6769 6f6e  atch], {n_region
-0000faa0: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
-0000fab0: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
-0000fac0: 2020 2077 6569 6768 7473 203d 2073 656c     weights = sel
-0000fad0: 662e 7765 6967 6874 7320 2320 285b 6e5f  f.weights # ([n_
-0000fae0: 6261 7463 685d 2c20 7b6e 5f72 6567 696f  batch], {n_regio
-0000faf0: 6e7d 2c20 6e40 312c 206e 4032 2c20 2e2e  n}, n@1, n@2, ..
-0000fb00: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
-0000fb10: 2020 2020 6e5f 6469 6d20 3d20 7365 6c66      n_dim = self
-0000fb20: 2e6e 5f64 696d 0a20 2020 2020 2020 206e  .n_dim.        n
-0000fb30: 5f72 6567 696f 6e20 3d20 6d61 7472 6963  _region = matric
-0000fb40: 6573 2e6e 5f63 6861 6e6e 656c 0a20 2020  es.n_channel.   
-0000fb50: 2020 2020 2058 7320 3d20 582e 6d75 6c74       Xs = X.mult
-0000fb60: 6970 6c79 286e 5f72 6567 696f 6e2c 207b  iply(n_region, {
-0000fb70: 7d29 2023 2028 5b6e 5f62 6174 6368 5d2c  }) # ([n_batch],
-0000fb80: 207b 6e5f 7265 6769 6f6e 7d2c 206e 5f64   {n_region}, n_d
-0000fb90: 696d 2c20 6e40 312c 206e 4032 2c20 2e2e  im, n@1, n@2, ..
-0000fba0: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
-0000fbb0: 2020 2020 4120 3d20 6d61 7472 6963 6573      A = matrices
-0000fbc0: 5b2e 2e2e 2c20 3a6e 5f64 696d 2c20 3a6e  [..., :n_dim, :n
-0000fbd0: 5f64 696d 5d0a 2020 2020 2020 2020 6220  _dim].        b 
-0000fbe0: 3d20 6d61 7472 6963 6573 5b2e 2e2e 2c20  = matrices[..., 
-0000fbf0: 3a6e 5f64 696d 2c20 6e5f 6469 6d3a 5d0a  :n_dim, n_dim:].
-0000fc00: 2020 2020 2020 2020 5920 3d20 2841 2040          Y = (A @
-0000fc10: 2058 732e 666c 6174 7465 6e28 3329 202b   Xs.flatten(3) +
-0000fc20: 2062 292e 7669 6577 5f61 7328 5873 290a   b).view_as(Xs).
-0000fc30: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-0000fc40: 7765 6967 6874 732e 756e 7371 7565 657a  weights.unsqueez
-0000fc50: 6528 2920 2a20 5929 2e73 756d 287b 7d29  e() * Y).sum({})
-0000fc60: 2e77 6974 685f 6368 616e 6e65 6c64 696d  .with_channeldim
-0000fc70: 2831 2920 2a20 2831 202d 206d 6173 6b73  (1) * (1 - masks
-0000fc80: 2e73 756d 287b 7d29 2e75 6e73 7175 6565  .sum({}).unsquee
-0000fc90: 7a65 287b 7d29 2920 2b20 2859 202a 206d  ze({})) + (Y * m
-0000fca0: 6173 6b73 2e75 6e73 7175 6565 7a65 2829  asks.unsqueeze()
-0000fcb0: 292e 7375 6d28 7b7d 292e 7769 7468 5f63  ).sum({}).with_c
-0000fcc0: 6861 6e6e 656c 6469 6d28 3129 0a0a 2020  hanneldim(1)..  
-0000fcd0: 2020 6465 6620 696e 7628 7365 6c66 293a    def inv(self):
-0000fce0: 0a20 2020 2020 2020 206e 5f62 6174 6368  .        n_batch
-0000fcf0: 203d 2073 656c 662e 6d61 7472 6963 6573   = self.matrices
-0000fd00: 2e6e 5f62 6174 6368 0a20 2020 2020 2020  .n_batch.       
-0000fd10: 2061 6666 7320 3d20 6274 2e69 6e76 2873   affs = bt.inv(s
-0000fd20: 656c 662e 6d61 7472 6963 6573 290a 2020  elf.matrices).  
-0000fd30: 2020 2020 2020 6d61 736b 7320 3d20 696e        masks = in
-0000fd40: 7465 7270 6f6c 6174 696f 6e28 7365 6c66  terpolation(self
-0000fd50: 2e6d 6173 6b73 2e6d 6572 6765 6469 6d73  .masks.mergedims
-0000fd60: 285b 5d2c 207b 7d29 2c20 4166 6669 6e65  ([], {}), Affine
-0000fd70: 2861 6666 732e 6d65 7267 6564 696d 7328  (affs.mergedims(
-0000fd80: 5b5d 2c20 7b7d 2929 292e 7370 6c69 7464  [], {}))).splitd
-0000fd90: 696d 285b 5d2c 205b 6e5f 6261 7463 685d  im([], [n_batch]
-0000fda0: 2c20 7b2d 317d 290a 2020 2020 2020 2020  , {-1}).        
-0000fdb0: 7265 7475 726e 2050 6f6c 7941 6666 696e  return PolyAffin
-0000fdc0: 6528 6166 6673 2c20 6d61 736b 7320 3d20  e(affs, masks = 
-0000fdd0: 6d61 736b 732c 2074 7261 6e73 5f73 7472  masks, trans_str
-0000fde0: 6574 6368 203d 2031 292e 6261 636b 7761  etch = 1).backwa
-0000fdf0: 7264 5f28 7365 6c66 2e62 6163 6b77 6172  rd_(self.backwar
-0000fe00: 6429 0a0a 4061 6c69 6173 2822 4646 4422  d)..@alias("FFD"
-0000fe10: 290a 636c 6173 7320 4672 6565 466f 726d  ).class FreeForm
-0000fe20: 4465 666f 726d 6174 696f 6e28 5370 6174  Deformation(Spat
-0000fe30: 6961 6c54 7261 6e73 666f 726d 6174 696f  ialTransformatio
-0000fe40: 6e29 3a0a 0a20 2020 2064 6566 205f 5f69  n):..    def __i
-0000fe50: 6e69 745f 5f28 7365 6c66 2c20 6f66 6673  nit__(self, offs
-0000fe60: 6574 732c 2073 7061 6369 6e67 3d31 2c20  ets, spacing=1, 
-0000fe70: 6f72 6967 696e 3d30 293a 0a20 2020 2020  origin=0):.     
-0000fe80: 2020 2027 2727 0a20 2020 2020 2020 2046     '''.        F
-0000fe90: 7265 6520 466f 726d 2044 6566 6f72 6d61  ree Form Deforma
-0000fea0: 7469 6f6e 2028 4646 4429 2074 7261 6e73  tion (FFD) trans
-0000feb0: 666f 726d 6174 696f 6e20 5b31 5d2e 0a20  formation [1].. 
-0000fec0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000fed0: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
-0000fee0: 2020 2020 6f66 6673 6574 7320 5b62 742e      offsets [bt.
-0000fef0: 5465 6e73 6f72 5d3a 2074 6865 2046 4644  Tensor]: the FFD
-0000ff00: 206f 6666 7365 7473 2e20 0a20 2020 2020   offsets. .     
-0000ff10: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-0000ff20: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
-0000ff30: 6469 6d7d 2c20 6d40 312c 206d 4032 2c20  dim}, m@1, m@2, 
-0000ff40: 2e2e 2e2c 206d 406e 5f64 696d 290a 2020  ..., m@n_dim).  
-0000ff50: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000ff60: 7220 6d40 3120 7820 6d40 3220 7820 2e2e  r m@1 x m@2 x ..
-0000ff70: 2e20 7820 6d40 6e5f 6469 6d20 6772 6964  . x m@n_dim grid
-0000ff80: 206f 6620 ce94 636f 6e74 726f 6c20 706f   of ..control po
-0000ff90: 696e 7473 0a20 2020 2020 2020 2020 2020  ints.           
-0000ffa0: 2073 7061 6369 6e67 205b 696e 7420 6f72   spacing [int or
-0000ffb0: 2074 7570 6c65 5d3a 2046 4644 2073 7061   tuple]: FFD spa
-0000ffc0: 6369 6e67 3b20 7370 6163 696e 6720 6265  cing; spacing be
-0000ffd0: 7477 6565 6e20 4646 4420 636f 6e74 726f  tween FFD contro
-0000ffe0: 6c20 706f 696e 7473 2e20 0a20 2020 2020  l points. .     
-0000fff0: 2020 2020 2020 206f 7269 6769 6e20 5b69         origin [i
-00010000: 6e74 206f 7220 7475 706c 655d 3a20 4646  nt or tuple]: FF
-00010010: 4420 6f72 6967 696e 3b20 636f 6f72 6469  D origin; coordi
-00010020: 6e61 7465 2066 6f72 2074 6865 2028 302c  nate for the (0,
-00010030: 2030 2c20 3029 2063 6f6e 7472 6f6c 2070   0, 0) control p
-00010040: 6f69 6e74 2e20 0a20 2020 2020 2020 2020  oint. .         
-00010050: 2020 200a 2020 2020 2020 2020 5768 656e     .        When
-00010060: 2069 7420 6973 2063 616c 6c65 643a 0a20   it is called:. 
-00010070: 2020 2020 2020 2020 2020 2058 205b 6274             X [bt
-00010080: 2e54 656e 736f 725d 3a20 436f 6f72 6469  .Tensor]: Coordi
-00010090: 6e61 7465 7320 746f 2062 6520 7472 616e  nates to be tran
-000100a0: 7366 6f72 6d65 642e 0a20 2020 2020 2020  sformed..       
-000100b0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-000100c0: 5b6e 5f62 6174 6368 3a20 6f70 7469 6f6e  [n_batch: option
-000100d0: 616c 5d2c 207b 6e5f 6469 6d7d 2c20 6e40  al], {n_dim}, n@
-000100e0: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-000100f0: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
-00010100: 2020 6f75 7470 7574 205b 6274 2e54 656e    output [bt.Ten
-00010110: 736f 725d 3a20 5468 6520 7472 616e 7366  sor]: The transf
-00010120: 6f72 6d65 6420 636f 6f72 6469 6e61 7465  ormed coordinate
-00010130: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-00010140: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
-00010150: 6368 5d2c 207b 6e5f 6469 6d7d 2c20 6e40  ch], {n_dim}, n@
-00010160: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-00010170: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
-00010180: 2020 2020 2020 0a20 2020 2020 2020 205b        .        [
-00010190: 315d 2052 7565 636b 6572 7420 4420 2c20  1] Rueckert D , 
-000101a0: 536f 6e6f 6461 204c 2049 202c 2048 6179  Sonoda L I , Hay
-000101b0: 6573 2043 202c 2065 7420 616c 2e20 4e6f  es C , et al. No
-000101c0: 6e72 6967 6964 2072 6567 6973 7472 6174  nrigid registrat
-000101d0: 696f 6e20 7573 696e 6720 6672 6565 2d66  ion using free-f
-000101e0: 6f72 6d20 6465 666f 726d 6174 696f 6e73  orm deformations
-000101f0: 3a20 0a20 2020 2020 2020 2020 2020 2061  : .            a
-00010200: 7070 6c69 6361 7469 6f6e 2074 6f20 6272  pplication to br
-00010210: 6561 7374 204d 5220 696d 6167 6573 5b4a  east MR images[J
-00010220: 5d2e 2049 4545 4520 5472 616e 7361 6374  ]. IEEE Transact
-00010230: 696f 6e73 206f 6e20 4d65 6469 6361 6c20  ions on Medical 
-00010240: 496d 6167 696e 672c 2031 3939 3928 3829  Imaging, 1999(8)
-00010250: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00010260: 2020 2020 2020 6f66 6673 6574 7320 3d20        offsets = 
-00010270: 6261 746f 7263 685f 7465 6e73 6f72 286f  batorch_tensor(o
-00010280: 6666 7365 7473 290a 2020 2020 2020 2020  ffsets).        
-00010290: 6966 206e 6f74 206f 6666 7365 7473 2e68  if not offsets.h
-000102a0: 6173 5f63 6861 6e6e 656c 3a0a 2020 2020  as_channel:.    
-000102b0: 2020 2020 2020 2020 6966 206f 6666 7365          if offse
-000102c0: 7473 2e73 697a 6528 3029 203d 3d20 6f66  ts.size(0) == of
-000102d0: 6673 6574 732e 6e5f 6469 6d20 2d20 313a  fsets.n_dim - 1:
-000102e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000102f0: 206e 5f64 696d 203d 206f 6666 7365 7473   n_dim = offsets
-00010300: 2e73 697a 6528 3029 0a20 2020 2020 2020  .size(0).       
-00010310: 2020 2020 2020 2020 206f 6666 7365 7473           offsets
-00010320: 2e63 6861 6e6e 656c 5f64 696d 656e 7369  .channel_dimensi
-00010330: 6f6e 203d 2030 0a20 2020 2020 2020 2020  on = 0.         
-00010340: 2020 2020 2020 206f 6666 7365 7473 203d         offsets =
-00010350: 206f 6666 7365 7473 2e75 6e73 7175 6565   offsets.unsquee
-00010360: 7a65 285b 5d29 0a20 2020 2020 2020 2020  ze([]).         
-00010370: 2020 2065 6c69 6620 6f66 6673 6574 732e     elif offsets.
-00010380: 7369 7a65 2831 2920 3d3d 206f 6666 7365  size(1) == offse
-00010390: 7473 2e6e 5f64 696d 202d 2032 3a0a 2020  ts.n_dim - 2:.  
-000103a0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
-000103b0: 6469 6d20 3d20 6f66 6673 6574 732e 7369  dim = offsets.si
-000103c0: 7a65 2831 290a 2020 2020 2020 2020 2020  ze(1).          
-000103d0: 2020 2020 2020 6f66 6673 6574 732e 6368        offsets.ch
-000103e0: 616e 6e65 6c5f 6469 6d65 6e73 696f 6e20  annel_dimension 
-000103f0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00010400: 656c 7365 3a20 7261 6973 6520 5479 7065  else: raise Type
-00010410: 4572 726f 7228 6622 4646 4420 7061 7261  Error(f"FFD para
-00010420: 6d65 7465 7273 2077 6974 6820 7369 7a65  meters with size
-00010430: 207b 6f66 6673 6574 732e 7368 6170 657d   {offsets.shape}
-00010440: 2064 6f6e 6f74 206d 6174 6368 2028 5b6e   donot match ([n
-00010450: 5f62 6174 6368 5d2c 207b 7b6e 5f64 696d  _batch], {{n_dim
-00010460: 7d7d 2c20 6d5f 312c 206d 5f32 2c20 2e2e  }}, m_1, m_2, ..
-00010470: 2e2c 206d 5f72 2920 5b72 3d6e 5f64 696d  ., m_r) [r=n_dim
-00010480: 5d2e 2022 290a 2020 2020 2020 2020 6966  ]. ").        if
-00010490: 206e 6f74 206f 6666 7365 7473 2e68 6173   not offsets.has
-000104a0: 5f62 6174 6368 3a0a 2020 2020 2020 2020  _batch:.        
-000104b0: 2020 2020 6e5f 6469 6d20 3d20 6f66 6673      n_dim = offs
-000104c0: 6574 732e 6e5f 6368 616e 6e65 6c0a 2020  ets.n_channel.  
-000104d0: 2020 2020 2020 2020 2020 6966 206f 6666            if off
-000104e0: 7365 7473 2e6e 5f64 696d 203c 3d20 6e5f  sets.n_dim <= n_
-000104f0: 6469 6d20 2b20 313a 206f 6666 7365 7473  dim + 1: offsets
-00010500: 203d 206f 6666 7365 7473 2e75 6e73 7175   = offsets.unsqu
-00010510: 6565 7a65 285b 5d29 0a20 2020 2020 2020  eeze([]).       
-00010520: 2020 2020 2065 6c73 653a 206f 6666 7365       else: offse
-00010530: 7473 2e62 6174 6368 5f64 696d 656e 7369  ts.batch_dimensi
-00010540: 6f6e 203d 2030 0a20 2020 2020 2020 2061  on = 0.        a
-00010550: 766f 7563 6828 6f66 6673 6574 732e 6861  vouch(offsets.ha
-00010560: 735f 6261 7463 6820 616e 6420 6f66 6673  s_batch and offs
-00010570: 6574 732e 6861 735f 6368 616e 6e65 6c2c  ets.has_channel,
-00010580: 2066 2250 6c65 6173 6520 7573 6520 6261   f"Please use ba
-00010590: 746f 7263 6820 7465 6e73 6f72 206f 6620  torch tensor of 
-000105a0: 7369 7a65 205c 0a20 2020 2020 2020 2020  size \.         
-000105b0: 2020 2028 5b6e 5f62 6174 6368 5d2c 207b     ([n_batch], {
-000105c0: 7b6e 5f64 696d 7d7d 2c20 6d5f 312c 206d  {n_dim}}, m_1, m
-000105d0: 5f32 2c20 2e2e 2e2c 206d 5f72 2920 5b72  _2, ..., m_r) [r
-000105e0: 3d6e 5f64 696d 5d20 666f 7220 4646 4420  =n_dim] for FFD 
-000105f0: 7061 7261 6d65 7465 7273 2c20 696e 7374  parameters, inst
-00010600: 6561 6420 6f66 207b 6f66 6673 6574 732e  ead of {offsets.
-00010610: 7368 6170 657d 2e20 2229 0a20 2020 2020  shape}. ").     
-00010620: 2020 206e 5f64 696d 203d 206f 6666 7365     n_dim = offse
-00010630: 7473 2e6e 5f63 6861 6e6e 656c 0a20 2020  ts.n_channel.   
-00010640: 2020 2020 2073 7061 6369 6e67 203d 2074       spacing = t
-00010650: 6f5f 7475 706c 6528 7370 6163 696e 6729  o_tuple(spacing)
-00010660: 0a20 2020 2020 2020 206f 7269 6769 6e20  .        origin 
-00010670: 3d20 746f 5f74 7570 6c65 286f 7269 6769  = to_tuple(origi
-00010680: 6e29 0a20 2020 2020 2020 2069 6620 6c65  n).        if le
-00010690: 6e28 7370 6163 696e 6729 203d 3d20 313a  n(spacing) == 1:
-000106a0: 2073 7061 6369 6e67 202a 3d20 6e5f 6469   spacing *= n_di
-000106b0: 6d0a 2020 2020 2020 2020 6966 206c 656e  m.        if len
-000106c0: 286f 7269 6769 6e29 203d 3d20 313a 206f  (origin) == 1: o
-000106d0: 7269 6769 6e20 2a3d 206e 5f64 696d 0a20  rigin *= n_dim. 
-000106e0: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-000106f0: 5f69 6e69 745f 5f28 6f66 6673 6574 732c  _init__(offsets,
-00010700: 2073 7061 6369 6e67 3d73 7061 6369 6e67   spacing=spacing
-00010710: 2c20 6f72 6967 696e 3d6f 7269 6769 6e29  , origin=origin)
-00010720: 0a0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-00010730: 5f64 696d 203d 206e 5f64 696d 0a20 2020  _dim = n_dim.   
-00010740: 2020 2020 2073 656c 662e 6f66 6673 6574       self.offset
-00010750: 7320 3d20 6f66 6673 6574 730a 2020 2020  s = offsets.    
-00010760: 2020 2020 7365 6c66 2e73 7061 6369 6e67      self.spacing
-00010770: 203d 2073 7061 6369 6e67 0a20 2020 2020   = spacing.     
-00010780: 2020 2073 656c 662e 6f72 6967 696e 203d     self.origin =
-00010790: 206f 7269 6769 6e0a 2020 2020 2020 2020   origin.        
-000107a0: 7365 6c66 2e62 6174 6368 5f70 6172 616d  self.batch_param
-000107b0: 2e61 7070 656e 6428 276f 6666 7365 7473  .append('offsets
-000107c0: 2729 0a20 2020 200a 2020 2020 6465 6620  ').    .    def 
-000107d0: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2058  __call__(self, X
-000107e0: 293a 0a20 2020 2020 2020 2058 203d 2073  ):.        X = s
-000107f0: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
-00010800: 5829 0a20 2020 2020 2020 2073 6861 7065  X).        shape
-00010810: 203d 2058 2e73 6861 7065 0a20 2020 2020   = X.shape.     
-00010820: 2020 206e 5f64 696d 203d 2073 656c 662e     n_dim = self.
-00010830: 6e5f 6469 6d0a 2020 2020 2020 2020 6f66  n_dim.        of
-00010840: 6673 6574 7320 3d20 7365 6c66 2e6f 6666  fsets = self.off
-00010850: 7365 7473 2e66 6c6f 6174 2829 0a20 2020  sets.float().   
-00010860: 2020 2020 2073 7061 6369 6e67 203d 2073       spacing = s
-00010870: 656c 662e 7370 6163 696e 670a 2020 2020  elf.spacing.    
-00010880: 2020 2020 6e5f 6261 7463 6820 3d20 6f66      n_batch = of
-00010890: 6673 6574 732e 6e5f 6261 7463 680a 2020  fsets.n_batch.  
-000108a0: 2020 2020 2020 2320 583a 2028 5b6e 5f62        # X: ([n_b
-000108b0: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
-000108c0: 6e5f 6461 7461 203d 206e 5f31 2078 206e  n_data = n_1 x n
-000108d0: 5f32 2078 202e 2e2e 2078 206e 5f72 290a  _2 x ... x n_r).
-000108e0: 2020 2020 2020 2020 5820 3d20 582e 666c          X = X.fl
-000108f0: 6174 7465 6e28 290a 2020 2020 2020 2020  atten().        
-00010900: 5820 2d3d 2062 742e 6368 616e 6e65 6c5f  X -= bt.channel_
-00010910: 7465 6e73 6f72 2873 656c 662e 6f72 6967  tensor(self.orig
-00010920: 696e 290a 2020 2020 2020 2020 6e5f 6461  in).        n_da
-00010930: 7461 203d 2058 2e73 697a 6528 2d31 290a  ta = X.size(-1).
-00010940: 2020 2020 2020 2020 7369 7a65 203d 2062          size = b
-00010950: 742e 6368 616e 6e65 6c5f 7465 6e73 6f72  t.channel_tensor
-00010960: 286f 6666 7365 7473 2e73 7061 6365 290a  (offsets.space).
-00010970: 2020 2020 2020 2020 2320 4e6f 726d 616c          # Normal
-00010980: 697a 6520 5820 696e 2074 6865 2064 6f6d  ize X in the dom
-00010990: 6169 6e20 286d 5f31 2c20 6d5f 322c 202e  ain (m_1, m_2, .
-000109a0: 2e2e 2c20 6d5f 7b6e 5f64 696d 7d29 2e0a  .., m_{n_dim})..
-000109b0: 2020 2020 2020 2020 4646 4458 203d 2058          FFDX = X
-000109c0: 202f 2062 742e 6368 616e 6e65 6c5f 7465   / bt.channel_te
-000109d0: 6e73 6f72 2873 7061 6369 6e67 292e 666c  nsor(spacing).fl
-000109e0: 6f61 7428 290a 2020 2020 2020 2020 6958  oat().        iX
-000109f0: 203d 2062 742e 666c 6f6f 7228 4646 4458   = bt.floor(FFDX
-00010a00: 292e 666c 6f61 7428 293b 2075 5820 3d20  ).float(); uX = 
-00010a10: 4646 4458 202d 2069 580a 2020 2020 2020  FFDX - iX.      
-00010a20: 2020 2320 436f 6d70 7574 6520 7468 6520    # Compute the 
-00010a30: 7765 6967 6874 732e 2057 3a20 2834 2c20  weights. W: (4, 
-00010a40: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-00010a50: 6d7d 2c20 6e5f 6461 7461 203d 206e 5f31  m}, n_data = n_1
-00010a60: 2078 206e 5f32 2078 202e 2e2e 2078 206e   x n_2 x ... x n
-00010a70: 5f72 290a 2020 2020 2020 2020 6920 3d20  _r).        i = 
-00010a80: 6274 2e61 7261 6e67 6528 2d31 2c20 3329  bt.arange(-1, 3)
-00010a90: 2e65 7870 616e 645f 746f 2834 2c20 5b6e  .expand_to(4, [n
-00010aa0: 5f62 6174 6368 5d2c 207b 6e5f 6469 6d7d  _batch], {n_dim}
-00010ab0: 2c20 6e5f 6461 7461 2c20 6178 6973 3d30  , n_data, axis=0
-00010ac0: 290a 2020 2020 2020 2020 5720 3d20 4273  ).        W = Bs
-00010ad0: 706c 696e 6528 692c 2075 582e 6d75 6c74  pline(i, uX.mult
-00010ae0: 6970 6c79 2834 2c20 3029 290a 2020 2020  iply(4, 0)).    
-00010af0: 2020 2020 2243 6f6d 7075 7465 2046 4644      "Compute FFD
-00010b00: 2054 7261 6e73 666f 726d 6174 696f 6e22   Transformation"
-00010b10: 0a20 2020 2020 2020 206f 7574 7075 7420  .        output 
-00010b20: 3d20 6274 2e7a 6572 6f73 5f6c 696b 6528  = bt.zeros_like(
-00010b30: 5829 0a20 2020 2020 2020 2023 204c 6f6f  X).        # Loo
-00010b40: 7020 696e 2074 6865 2073 7061 6365 207b  p in the space {
-00010b50: 2d31 2c20 302c 2031 2c20 327d 205e 206e  -1, 0, 1, 2} ^ n
-00010b60: 5f64 696d 3b20 4720 6973 2069 6e20 2830  _dim; G is in (0
-00010b70: 2c20 312c 2032 2c20 3329 0a20 2020 2020  , 1, 2, 3).     
-00010b80: 2020 2066 6f72 2047 2069 6e20 6274 2e69     for G in bt.i
-00010b90: 6d61 6765 5f67 7269 6428 5b34 5d2a 6e5f  mage_grid([4]*n_
-00010ba0: 6469 6d29 2e66 6c61 7474 656e 2829 2e74  dim).flatten().t
-00010bb0: 7261 6e73 706f 7365 2830 2c20 3129 3a0a  ranspose(0, 1):.
-00010bc0: 2020 2020 2020 2020 2020 2020 4720 3d20              G = 
-00010bd0: 6274 2e63 6861 6e6e 656c 5f74 656e 736f  bt.channel_tenso
-00010be0: 7228 4729 0a20 2020 2020 2020 2020 2020  r(G).           
-00010bf0: 2023 2057 6569 6768 7473 2066 6f72 2065   # Weights for e
-00010c00: 6163 6820 706f 696e 743a 205b 7072 6f64  ach point: [prod
-00010c10: 7563 7420 6f66 2057 5b47 5b44 5d2c 2074  uct of W[G[D], t
-00010c20: 2c20 442c 2078 5d20 666f 7220 4420 696e  , D, x] for D in
-00010c30: 2072 616e 6765 286e 5f64 696d 295d 2066   range(n_dim)] f
-00010c40: 6f72 2070 6f69 6e74 2078 2061 6e64 2062  or point x and b
-00010c50: 6174 6368 2074 2e0a 2020 2020 2020 2020  atch t..        
-00010c60: 2020 2020 2320 5767 3a20 285b 6e5f 6261      # Wg: ([n_ba
-00010c70: 7463 685d 2c20 7b31 7d2c 206e 5f64 6174  tch], {1}, n_dat
-00010c80: 6120 3d20 6e5f 3120 7820 6e5f 3220 7820  a = n_1 x n_2 x 
-00010c90: 2e2e 2e20 7820 6e5f 7229 0a20 2020 2020  ... x n_r).     
-00010ca0: 2020 2020 2020 2057 6720 3d20 572e 6761         Wg = W.ga
-00010cb0: 7468 6572 2830 2c20 472e 6578 7061 6e64  ther(0, G.expand
-00010cc0: 5f74 6f28 2831 2c29 202b 2057 2e73 6861  _to((1,) + W.sha
-00010cd0: 7065 5b31 3a5d 2929 2e73 7175 6565 7a65  pe[1:])).squeeze
-00010ce0: 2830 292e 7072 6f64 287b 7d2c 206b 6565  (0).prod({}, kee
-00010cf0: 7064 696d 3d54 7275 6529 0a20 2020 2020  pdim=True).     
-00010d00: 2020 2020 2020 2023 2043 6f6d 7075 7465         # Compute
-00010d10: 2074 6865 2069 6e64 6963 6573 206f 6620   the indices of 
-00010d20: 7265 6c61 7465 6420 636f 6e74 726f 6c20  related control 
-00010d30: 706f 696e 7473 2e20 496e 643a 2028 5b6e  points. Ind: ([n
-00010d40: 5f62 6174 6368 5d2c 207b 6e5f 6469 6d7d  _batch], {n_dim}
-00010d50: 2c20 6e5f 6461 7461 203d 206e 5f31 2078  , n_data = n_1 x
-00010d60: 206e 5f32 2078 202e 2e2e 2078 206e 5f72   n_2 x ... x n_r
-00010d70: 290a 2020 2020 2020 2020 2020 2020 496e  ).            In
-00010d80: 6420 3d20 6274 2e63 6c61 6d70 2869 582e  d = bt.clamp(iX.
-00010d90: 6c6f 6e67 2829 202b 2047 202d 2031 2c20  long() + G - 1, 
-00010da0: 6d69 6e3d 3029 0a20 2020 2020 2020 2020  min=0).         
-00010db0: 2020 2049 6e64 203d 2062 742e 6d69 6e28     Ind = bt.min(
-00010dc0: 496e 642c 2028 7369 7a65 202d 2031 292e  Ind, (size - 1).
-00010dd0: 6578 7061 6e64 5f74 6f28 496e 6429 290a  expand_to(Ind)).
-00010de0: 2020 2020 2020 2020 2020 2020 2320 436f              # Co
-00010df0: 6e76 6572 7420 7468 6520 696e 6469 6365  nvert the indice
-00010e00: 7320 746f 2031 2064 696d 656e 7369 6f6e  s to 1 dimension
-00010e10: 616c 2e20 446f 743a 2028 5b6e 5f62 6174  al. Dot: ([n_bat
-00010e20: 6368 5d2c 206e 5f64 6174 6120 3d20 6e5f  ch], n_data = n_
-00010e30: 3120 7820 6e5f 3220 7820 2e2e 2e20 7820  1 x n_2 x ... x 
-00010e40: 6e5f 7229 0a20 2020 2020 2020 2020 2020  n_r).           
-00010e50: 2044 6f74 203d 2049 6e64 5b3a 2c20 305d   Dot = Ind[:, 0]
-00010e60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00010e70: 2072 2069 6e20 7261 6e67 6528 312c 206e   r in range(1, n
-00010e80: 5f64 696d 293a 2044 6f74 202a 3d20 7369  _dim): Dot *= si
-00010e90: 7a65 5b72 5d3b 2044 6f74 202b 3d20 496e  ze[r]; Dot += In
-00010ea0: 645b 3a2c 2072 5d0a 2020 2020 2020 2020  d[:, r].        
-00010eb0: 2020 2020 2320 4f62 7461 696e 2074 6865      # Obtain the
-00010ec0: 2063 6f6f 7264 696e 6174 6573 206f 6620   coordinates of 
-00010ed0: 7468 6520 636f 6e74 726f 6c20 706f 696e  the control poin
-00010ee0: 7473 2e20 4350 6f69 6e74 733a 2028 5b6e  ts. CPoints: ([n
-00010ef0: 5f62 6174 6368 5d2c 207b 6e5f 6469 6d7d  _batch], {n_dim}
-00010f00: 2c20 6e5f 6461 7461 203d 206e 5f31 2078  , n_data = n_1 x
-00010f10: 206e 5f32 2078 202e 2e2e 2078 206e 5f72   n_2 x ... x n_r
-00010f20: 290a 2020 2020 2020 2020 2020 2020 4350  ).            CP
-00010f30: 6f69 6e74 7320 3d20 6f66 6673 6574 732e  oints = offsets.
-00010f40: 666c 6174 7465 6e28 292e 6761 7468 6572  flatten().gather
-00010f50: 282d 312c 2044 6f74 2e6c 6f6e 6728 292e  (-1, Dot.long().
-00010f60: 6578 7061 6e64 5f74 6f28 496e 6429 292e  expand_to(Ind)).
-00010f70: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
-00010f80: 2020 2020 2320 4164 6420 7468 6520 7765      # Add the we
-00010f90: 6967 6874 6564 2063 6f6e 7472 6f6c 2063  ighted control c
-00010fa0: 6f6f 7264 696e 6174 6573 2074 6f20 7468  oordinates to th
-00010fb0: 6520 6f75 7470 7574 2063 6f6f 7264 696e  e output coordin
-00010fc0: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
-00010fd0: 2020 6f75 7470 7574 202b 3d20 2857 6720    output += (Wg 
-00010fe0: 2a20 4350 6f69 6e74 7329 2e76 6965 775f  * CPoints).view_
-00010ff0: 6173 2858 290a 2020 2020 2020 2020 2320  as(X).        # 
-00011000: 4465 6e6f 726d 616c 697a 6520 7468 6520  Denormalize the 
-00011010: 6f75 7470 7574 732e 0a20 2020 2020 2020  outputs..       
-00011020: 206f 7574 7075 7420 2b3d 2058 0a20 2020   output += X.   
-00011030: 2020 2020 206f 7574 7075 7420 2b3d 2062       output += b
-00011040: 742e 6368 616e 6e65 6c5f 7465 6e73 6f72  t.channel_tensor
-00011050: 2873 656c 662e 6f72 6967 696e 290a 2020  (self.origin).  
-00011060: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-00011070: 7075 742e 7669 6577 2873 6861 7065 290a  put.view(shape).
-00011080: 0a40 616c 6961 7328 2244 4446 2229 0a63  .@alias("DDF").c
-00011090: 6c61 7373 2044 656e 7365 4469 7370 6c61  lass DenseDispla
-000110a0: 6365 6d65 6e74 4669 656c 6428 5370 6174  cementField(Spat
-000110b0: 6961 6c54 7261 6e73 666f 726d 6174 696f  ialTransformatio
-000110c0: 6e29 3a0a 2020 2020 6465 6620 5f5f 696e  n):.    def __in
-000110d0: 6974 5f5f 2873 656c 662c 2064 6973 706c  it__(self, displ
-000110e0: 6163 656d 656e 7473 2c20 7368 6170 653d  acements, shape=
-000110f0: 4e6f 6e65 2c20 696e 7465 7270 6f6c 6174  None, interpolat
-00011100: 653d 4661 6c73 6529 3a0a 2020 2020 2020  e=False):.      
-00011110: 2020 2727 270a 2020 2020 2020 2020 4465    '''.        De
-00011120: 6e73 6520 4469 7370 6c61 6365 6d65 6e74  nse Displacement
-00011130: 2046 6965 6c64 2028 4444 4629 2074 7261   Field (DDF) tra
-00011140: 6e73 666f 726d 6174 696f 6e2e 0a20 2020  nsformation..   
-00011150: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
-00011160: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
-00011170: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
-00011180: 5b62 742e 5465 6e73 6f72 5d3a 2074 6865  [bt.Tensor]: the
-00011190: 2064 6973 706c 6163 656d 656e 7420 6f66   displacement of
-000111a0: 2065 6163 6820 766f 7865 6c2e 200a 2020   each voxel. .  
-000111b0: 2020 2020 2020 2020 2020 2020 2020 7369                si
-000111c0: 7a65 3a20 285b 6e5f 6261 7463 685d 2c20  ze: ([n_batch], 
-000111d0: 7b6e 5f64 696d 7d2c 206e 4031 2c20 6e40  {n_dim}, n@1, n@
-000111e0: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
-000111f0: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
-00011200: 7065 205b 6274 2e53 697a 6520 6f72 2074  pe [bt.Size or t
-00011210: 7570 6c65 5d3a 2074 6865 2073 6861 7065  uple]: the shape
-00011220: 206f 6620 6469 7370 6c61 6365 6d65 6e74   of displacement
-00011230: 2028 6e65 6564 6564 2069 6620 696e 7075   (needed if inpu
-00011240: 7420 6469 7370 6c61 6365 6d65 6e74 2069  t displacement i
-00011250: 7320 6120 7472 616e 7366 6f72 6d61 7469  s a transformati
-00011260: 6f6e 292e 200a 2020 2020 2020 2020 2020  on). .          
-00011270: 2020 696e 7465 7270 6f6c 6174 6520 5b62    interpolate [b
-00011280: 6f6f 6c5d 3a20 5768 6574 6865 7220 746f  ool]: Whether to
-00011290: 2066 6f72 6365 2069 6e74 6572 706f 6c61   force interpola
-000112a0: 7469 6f6e 2069 6e20 6170 706c 792e 200a  tion in apply. .
-000112b0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-000112c0: 2020 2020 2057 6865 6e20 6974 2069 7320       When it is 
-000112d0: 6361 6c6c 6564 3a0a 2020 2020 2020 2020  called:.        
-000112e0: 2020 2020 5820 5b62 742e 5465 6e73 6f72      X [bt.Tensor
-000112f0: 5d3a 2043 6f6f 7264 696e 6174 6573 2074  ]: Coordinates t
-00011300: 6f20 6265 2074 7261 6e73 666f 726d 6564  o be transformed
-00011310: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011320: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-00011330: 683a 206f 7074 696f 6e61 6c5d 2c20 7b6e  h: optional], {n
-00011340: 5f64 696d 7d2c 206e 4031 2c20 6e40 322c  _dim}, n@1, n@2,
-00011350: 202e 2e2e 2c20 6e40 6e5f 6469 6d29 0a20   ..., n@n_dim). 
-00011360: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00011370: 7420 5b62 742e 5465 6e73 6f72 5d3a 2054  t [bt.Tensor]: T
-00011380: 6865 2074 7261 6e73 666f 726d 6564 2063  he transformed c
-00011390: 6f6f 7264 696e 6174 6573 2e0a 2020 2020  oordinates..    
-000113a0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-000113b0: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
-000113c0: 5f64 696d 7d2c 206e 4031 2c20 6e40 322c  _dim}, n@1, n@2,
-000113d0: 202e 2e2e 2c20 6e40 6e5f 6469 6d29 0a20   ..., n@n_dim). 
-000113e0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-000113f0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00011400: 2864 6973 706c 6163 656d 656e 7473 2c20  (displacements, 
-00011410: 5370 6174 6961 6c54 7261 6e73 666f 726d  SpatialTransform
-00011420: 6174 696f 6e29 3a20 6469 7370 6c61 6365  ation): displace
-00011430: 6d65 6e74 7320 3d20 6469 7370 6c61 6365  ments = displace
-00011440: 6d65 6e74 732e 746f 4444 4628 7368 6170  ments.toDDF(shap
-00011450: 6529 0a20 2020 2020 2020 2064 6973 706c  e).        displ
-00011460: 6163 656d 656e 7473 203d 2062 6174 6f72  acements = bator
-00011470: 6368 5f74 656e 736f 7228 6469 7370 6c61  ch_tensor(displa
-00011480: 6365 6d65 6e74 7329 0a20 2020 2020 2020  cements).       
-00011490: 2069 6620 6e6f 7420 6469 7370 6c61 6365   if not displace
-000114a0: 6d65 6e74 732e 6861 735f 6368 616e 6e65  ments.has_channe
-000114b0: 6c3a 0a20 2020 2020 2020 2020 2020 2069  l:.            i
-000114c0: 6620 6469 7370 6c61 6365 6d65 6e74 732e  f displacements.
-000114d0: 7369 7a65 2830 2920 3d3d 2064 6973 706c  size(0) == displ
-000114e0: 6163 656d 656e 7473 2e6e 5f64 696d 202d  acements.n_dim -
-000114f0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00011500: 2020 2020 6e5f 6469 6d20 3d20 6469 7370      n_dim = disp
-00011510: 6c61 6365 6d65 6e74 732e 7369 7a65 2830  lacements.size(0
-00011520: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011530: 2020 6469 7370 6c61 6365 6d65 6e74 732e    displacements.
-00011540: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
-00011550: 6e20 3d20 300a 2020 2020 2020 2020 2020  n = 0.          
-00011560: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
-00011570: 6e74 7320 3d20 6469 7370 6c61 6365 6d65  nts = displaceme
-00011580: 6e74 732e 756e 7371 7565 657a 6528 5b5d  nts.unsqueeze([]
-00011590: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000115a0: 6966 2064 6973 706c 6163 656d 656e 7473  if displacements
-000115b0: 2e73 697a 6528 3129 203d 3d20 6469 7370  .size(1) == disp
-000115c0: 6c61 6365 6d65 6e74 732e 6e5f 6469 6d20  lacements.n_dim 
-000115d0: 2d20 323a 0a20 2020 2020 2020 2020 2020  - 2:.           
-000115e0: 2020 2020 206e 5f64 696d 203d 2064 6973       n_dim = dis
-000115f0: 706c 6163 656d 656e 7473 2e73 697a 6528  placements.size(
-00011600: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-00011610: 2020 2064 6973 706c 6163 656d 656e 7473     displacements
-00011620: 2e63 6861 6e6e 656c 5f64 696d 656e 7369  .channel_dimensi
-00011630: 6f6e 203d 2031 0a20 2020 2020 2020 2020  on = 1.         
-00011640: 2020 2065 6c73 653a 2072 6169 7365 2054     else: raise T
-00011650: 7970 6545 7272 6f72 2866 2244 4446 2070  ypeError(f"DDF p
-00011660: 6172 616d 6574 6572 7320 7769 7468 2073  arameters with s
-00011670: 697a 6520 7b64 6973 706c 6163 656d 656e  ize {displacemen
-00011680: 7473 2e73 6861 7065 7d20 646f 6e6f 7420  ts.shape} donot 
-00011690: 6d61 7463 6820 285b 6e5f 6261 7463 685d  match ([n_batch]
-000116a0: 2c20 7b7b 6e5f 6469 6d7d 7d2c 206e 4031  , {{n_dim}}, n@1
-000116b0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-000116c0: 6469 6d29 2e20 2229 0a20 2020 2020 2020  dim). ").       
-000116d0: 2069 6620 6e6f 7420 6469 7370 6c61 6365   if not displace
-000116e0: 6d65 6e74 732e 6861 735f 6261 7463 683a  ments.has_batch:
-000116f0: 0a20 2020 2020 2020 2020 2020 206e 5f64  .            n_d
-00011700: 696d 203d 2064 6973 706c 6163 656d 656e  im = displacemen
-00011710: 7473 2e6e 5f63 6861 6e6e 656c 0a20 2020  ts.n_channel.   
-00011720: 2020 2020 2020 2020 2069 6620 6469 7370           if disp
-00011730: 6c61 6365 6d65 6e74 732e 6e5f 6469 6d20  lacements.n_dim 
-00011740: 3c3d 206e 5f64 696d 202b 2031 3a20 6469  <= n_dim + 1: di
-00011750: 7370 6c61 6365 6d65 6e74 7320 3d20 6469  splacements = di
-00011760: 7370 6c61 6365 6d65 6e74 732e 756e 7371  splacements.unsq
-00011770: 7565 657a 6528 5b5d 290a 2020 2020 2020  ueeze([]).      
-00011780: 2020 2020 2020 656c 7365 3a20 6469 7370        else: disp
-00011790: 6c61 6365 6d65 6e74 732e 6261 7463 685f  lacements.batch_
-000117a0: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
-000117b0: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
-000117c0: 6e74 7320 3d20 6469 7370 6c61 6365 6d65  nts = displaceme
-000117d0: 6e74 732e 666c 6f61 7428 290a 2020 2020  nts.float().    
-000117e0: 2020 2020 6176 6f75 6368 2864 6973 706c      avouch(displ
-000117f0: 6163 656d 656e 7473 2e68 6173 5f62 6174  acements.has_bat
-00011800: 6368 2061 6e64 2064 6973 706c 6163 656d  ch and displacem
-00011810: 656e 7473 2e68 6173 5f63 6861 6e6e 656c  ents.has_channel
-00011820: 2c20 6622 506c 6561 7365 2075 7365 2062  , f"Please use b
-00011830: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
-00011840: 2073 697a 6520 5c0a 2020 2020 2020 2020   size \.        
-00011850: 2020 2020 285b 6e5f 6261 7463 685d 2c20      ([n_batch], 
-00011860: 7b7b 6e5f 6469 6d7d 7d2c 206e 4031 2c20  {{n_dim}}, n@1, 
-00011870: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-00011880: 6d29 2066 6f72 2044 4446 2070 6172 616d  m) for DDF param
-00011890: 6574 6572 732c 2069 6e73 7465 6164 206f  eters, instead o
-000118a0: 6620 7b64 6973 706c 6163 656d 656e 7473  f {displacements
-000118b0: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-000118c0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-000118d0: 6974 5f5f 2864 6973 706c 6163 656d 656e  it__(displacemen
-000118e0: 7473 2c20 7368 6170 653d 7368 6170 652c  ts, shape=shape,
-000118f0: 2069 6e74 6572 706f 6c61 7465 3d69 6e74   interpolate=int
-00011900: 6572 706f 6c61 7465 290a 2020 2020 2020  erpolate).      
-00011910: 2020 7365 6c66 2e6e 5f64 696d 203d 2064    self.n_dim = d
-00011920: 6973 706c 6163 656d 656e 7473 2e6e 5f63  isplacements.n_c
-00011930: 6861 6e6e 656c 0a20 2020 2020 2020 2073  hannel.        s
-00011940: 656c 662e 6469 7370 6c61 6365 6d65 6e74  elf.displacement
-00011950: 7320 3d20 6469 7370 6c61 6365 6d65 6e74  s = displacement
-00011960: 730a 2020 2020 2020 2020 7365 6c66 2e69  s.        self.i
-00011970: 6e74 6572 706f 6c61 7465 203d 2069 6e74  nterpolate = int
-00011980: 6572 706f 6c61 7465 0a20 2020 2020 2020  erpolate.       
-00011990: 2073 656c 662e 6261 7463 685f 7061 7261   self.batch_para
-000119a0: 6d2e 6170 7065 6e64 2827 6469 7370 6c61  m.append('displa
-000119b0: 6365 6d65 6e74 7327 290a 2020 2020 0a20  cements').    . 
-000119c0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-000119d0: 7365 6c66 2c20 5829 3a0a 2020 2020 2020  self, X):.      
-000119e0: 2020 5820 3d20 7375 7065 7228 292e 5f5f    X = super().__
-000119f0: 6361 6c6c 5f5f 2858 290a 2020 2020 2020  call__(X).      
-00011a00: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
-00011a10: 3d20 7365 6c66 2e64 6973 706c 6163 656d  = self.displacem
-00011a20: 656e 7473 0a20 2020 2020 2020 206e 5f64  ents.        n_d
-00011a30: 696d 203d 2073 656c 662e 6e5f 6469 6d0a  im = self.n_dim.
-00011a40: 2020 2020 2020 2020 6966 2058 2e6e 5f73          if X.n_s
-00011a50: 7061 6365 203d 3d20 303a 2058 203d 2058  pace == 0: X = X
-00011a60: 2e75 6e73 7175 6565 7a65 282d 3129 0a20  .unsqueeze(-1). 
-00011a70: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00011a80: 6c66 2e69 6e74 6572 706f 6c61 7465 2061  lf.interpolate a
-00011a90: 6e64 2058 2e73 7061 6365 203d 3d20 6469  nd X.space == di
-00011aa0: 7370 6c61 6365 6d65 6e74 732e 7370 6163  splacements.spac
-00011ab0: 6520 616e 6420 582e 6e5f 6368 616e 6e65  e and X.n_channe
-00011ac0: 6c20 3d3d 2064 6973 706c 6163 656d 656e  l == displacemen
-00011ad0: 7473 2e6e 5f63 6861 6e6e 656c 3a20 7265  ts.n_channel: re
-00011ae0: 7475 726e 2058 202b 2064 6973 706c 6163  turn X + displac
-00011af0: 656d 656e 7473 0a20 2020 2020 2020 2065  ements.        e
-00011b00: 6c73 653a 2072 6574 7572 6e20 5820 2b20  lse: return X + 
-00011b10: 696e 7465 7270 6f6c 6174 696f 6e28 6469  interpolation(di
-00011b20: 7370 6c61 6365 6d65 6e74 732c 2074 6172  splacements, tar
-00011b30: 6765 745f 7370 6163 653d 5829 2e63 6861  get_space=X).cha
-00011b40: 6e6e 656c 5f64 696d 656e 7369 6f6e 5f28  nnel_dimension_(
-00011b50: 3129 0a0a 4061 6c69 6173 2822 4d4c 5022  1)..@alias("MLP"
-00011b60: 290a 636c 6173 7320 4d75 6c74 694c 6179  ).class MultiLay
-00011b70: 6572 5065 7263 6570 7469 6f6e 2853 7061  erPerception(Spa
-00011b80: 7469 616c 5472 616e 7366 6f72 6d61 7469  tialTransformati
-00011b90: 6f6e 293a 0a20 2020 2064 6566 205f 5f69  on):.    def __i
-00011ba0: 6e69 745f 5f28 7365 6c66 2c20 7765 6967  nit__(self, weig
-00011bb0: 6874 732c 2068 6964 6465 6e5f 6c61 7965  hts, hidden_laye
-00011bc0: 7273 3d5b 5d2c 2061 6374 6976 655f 6675  rs=[], active_fu
-00011bd0: 6e63 7469 6f6e 3d4e 6f6e 652c 2074 7261  nction=None, tra
-00011be0: 6e73 5f73 7472 6574 6368 3d31 293a 0a20  ns_stretch=1):. 
-00011bf0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00011c00: 2020 2041 2074 7261 6e73 666f 726d 6174     A transformat
-00011c10: 696f 6e20 6465 6669 6e65 6420 6279 2061  ion defined by a
-00011c20: 204d 4c50 2e20 0a20 2020 2020 2020 200a   MLP. .        .
-00011c30: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
-00011c40: 2020 2020 2020 2020 2020 2020 7765 6967              weig
-00011c50: 6874 7320 5b62 742e 5465 6e73 6f72 5d3a  hts [bt.Tensor]:
-00011c60: 2074 6865 2077 6569 6768 7473 2066 6f72   the weights for
-00011c70: 2074 6865 2070 6572 6365 7074 696f 6e20   the perception 
-00011c80: 6e65 7477 6f72 6b2e 200a 2020 2020 2020  network. .      
-00011c90: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00011ca0: 285b 6e5f 6261 7463 685d 2c20 6e5f 6469  ([n_batch], n_di
-00011cb0: 6d20 2a20 6e5f 686c 5f31 202b 206e 5f68  m * n_hl_1 + n_h
-00011cc0: 6c5f 3120 2b20 7375 6d28 693d 312e 2e6b  l_1 + sum(i=1..k
-00011cd0: 2d31 297b 6e5f 686c 5f69 202a 206e 5f68  -1){n_hl_i * n_h
-00011ce0: 6c5f 7b69 2b31 7d20 2b20 6e5f 686c 5f7b  l_{i+1} + n_hl_{
-00011cf0: 692b 317d 7d20 2b20 6e5f 686c 5f6b 202a  i+1}} + n_hl_k *
-00011d00: 206e 5f64 696d 202b 206e 5f64 696d 290a   n_dim + n_dim).
-00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d20: 7768 6572 6520 6b20 6973 2074 6865 206e  where k is the n
-00011d30: 756d 6265 7220 6f66 2068 6964 6465 6e20  umber of hidden 
-00011d40: 6c61 7965 7273 2061 6e64 206e 5f68 6c5f  layers and n_hl_
-00011d50: 6920 6973 2074 6865 206c 656e 6774 6820  i is the length 
-00011d60: 6f66 2074 6865 2069 2d74 6820 6869 6464  of the i-th hidd
-00011d70: 656e 206c 6179 6572 2e20 0a20 2020 2020  en layer. .     
-00011d80: 2020 2020 2020 2068 6964 6465 6e5f 6c61         hidden_la
-00011d90: 7965 7273 205b 6c69 7374 206f 6620 696e  yers [list of in
-00011da0: 745d 3a20 7468 6520 6c65 6e67 7468 7320  t]: the lengths 
-00011db0: 666f 7220 7468 6520 6869 6464 656e 206c  for the hidden l
-00011dc0: 6179 6572 732c 2069 2e65 2e20 5b6e 5f68  ayers, i.e. [n_h
-00011dd0: 6c5f 312c 206e 5f68 6c5f 322c 202e 2e2e  l_1, n_hl_2, ...
-00011de0: 2c20 6e5f 686c 5f6b 5d0a 2020 2020 2020  , n_hl_k].      
-00011df0: 2020 2020 2020 2020 2020 4974 2069 7320            It is 
-00011e00: 6279 2064 6566 6175 6c74 2027 5b5d 2720  by default '[]' 
-00011e10: 736f 2074 6861 7420 7468 6520 6465 6661  so that the defa
-00011e20: 756c 7420 4d4c 5020 6973 2061 6e20 6166  ult MLP is an af
-00011e30: 6669 6e65 2074 7261 6e73 666f 726d 6174  fine transformat
-00011e40: 696f 6e2e 200a 2020 2020 2020 2020 2020  ion. .          
-00011e50: 2020 6163 7469 7665 5f66 756e 6374 696f    active_functio
-00011e60: 6e20 5b63 6c61 7373 5d3a 2074 6865 2061  n [class]: the a
-00011e70: 6374 6976 655f 6675 6e63 7469 6f6e 2e20  ctive_function. 
-00011e80: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00011e90: 6e73 5f73 7472 6574 6368 205b 696e 745d  ns_stretch [int]
-00011ea0: 3a20 3120 6279 2064 6566 6175 6c74 2e20  : 1 by default. 
-00011eb0: 3230 2073 6565 6d73 2074 6f20 6265 2061  20 seems to be a
-00011ec0: 2067 6f6f 6420 6368 6f69 6365 2e20 0a20   good choice. . 
-00011ed0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00011ee0: 2020 2020 5768 656e 2069 7420 6973 2063      When it is c
-00011ef0: 616c 6c65 643a 0a20 2020 2020 2020 2020  alled:.         
-00011f00: 2020 2058 205b 6274 2e54 656e 736f 725d     X [bt.Tensor]
-00011f10: 3a20 436f 6f72 6469 6e61 7465 7320 746f  : Coordinates to
-00011f20: 2062 6520 7472 616e 7366 6f72 6d65 642e   be transformed.
-00011f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011f40: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-00011f50: 3a20 6f70 7469 6f6e 616c 5d2c 207b 6e5f  : optional], {n_
-00011f60: 6469 6d7d 2c20 6e40 312c 206e 4032 2c20  dim}, n@1, n@2, 
-00011f70: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
-00011f80: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00011f90: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
-00011fa0: 6520 7472 616e 7366 6f72 6d65 6420 636f  e transformed co
-00011fb0: 6f72 6469 6e61 7465 732e 0a20 2020 2020  ordinates..     
-00011fc0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-00011fd0: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
-00011fe0: 6469 6d7d 2c20 6e40 312c 206e 4032 2c20  dim}, n@1, n@2, 
-00011ff0: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
-00012000: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00012010: 2020 7365 6c66 2e68 6964 6465 6e5f 6c61    self.hidden_la
-00012020: 7965 7273 203d 2068 6964 6465 6e5f 6c61  yers = hidden_la
-00012030: 7965 7273 0a20 2020 2020 2020 2069 6620  yers.        if 
-00012040: 6e6f 7420 7765 6967 6874 732e 6861 735f  not weights.has_
-00012050: 6261 7463 683a 0a20 2020 2020 2020 2020  batch:.         
-00012060: 2020 2069 6620 7765 6967 6874 732e 6e5f     if weights.n_
-00012070: 6469 6d20 3d3d 2032 3a20 7765 6967 6874  dim == 2: weight
-00012080: 732e 6261 7463 685f 6469 6d20 3d20 300a  s.batch_dim = 0.
-00012090: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000120a0: 3a20 7765 6967 6874 7320 3d20 7765 6967  : weights = weig
-000120b0: 6874 732e 756e 7371 7565 657a 6528 5b5d  hts.unsqueeze([]
-000120c0: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
-000120d0: 6569 6768 7473 203d 2077 6569 6768 7473  eights = weights
-000120e0: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
-000120f0: 616e 735f 7374 7265 7463 6820 3d20 7472  ans_stretch = tr
-00012100: 616e 735f 7374 7265 7463 680a 2020 2020  ans_stretch.    
-00012110: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00012120: 6974 5f5f 2877 6569 6768 7473 2c20 6869  it__(weights, hi
-00012130: 6464 656e 5f6c 6179 6572 7320 3d20 6869  dden_layers = hi
-00012140: 6464 656e 5f6c 6179 6572 732c 2074 7261  dden_layers, tra
-00012150: 6e73 5f73 7472 6574 6368 203d 2074 7261  ns_stretch = tra
-00012160: 6e73 5f73 7472 6574 6368 290a 2020 2020  ns_stretch).    
-00012170: 2020 2020 6469 6d5f 636f 6e73 7420 3d20      dim_const = 
-00012180: 7765 6967 6874 732e 7369 7a65 282d 3129  weights.size(-1)
-00012190: 202d 2073 756d 2868 6964 6465 6e5f 6c61   - sum(hidden_la
-000121a0: 7965 7273 2920 2d20 7375 6d28 7820 2a20  yers) - sum(x * 
-000121b0: 7920 666f 7220 782c 2079 2069 6e20 7a69  y for x, y in zi
-000121c0: 7028 6869 6464 656e 5f6c 6179 6572 735b  p(hidden_layers[
-000121d0: 3a2d 315d 2c20 6869 6464 656e 5f6c 6179  :-1], hidden_lay
-000121e0: 6572 735b 313a 5d29 290a 2020 2020 2020  ers[1:])).      
-000121f0: 2020 6469 6d5f 636f 6566 6620 3d20 6869    dim_coeff = hi
-00012200: 6464 656e 5f6c 6179 6572 735b 305d 202b  dden_layers[0] +
-00012210: 2068 6964 6465 6e5f 6c61 7965 7273 5b2d   hidden_layers[-
-00012220: 315d 202b 2031 0a20 2020 2020 2020 2061  1] + 1.        a
-00012230: 766f 7563 6828 6469 6d5f 636f 6e73 7420  vouch(dim_const 
-00012240: 2520 6469 6d5f 636f 6566 6620 3d3d 2030  % dim_coeff == 0
-00012250: 2c20 6622 5772 6f6e 6720 7765 6967 6874  , f"Wrong weight
-00012260: 206c 656e 6774 6820 666f 7220 6869 6464   length for hidd
-00012270: 656e 206c 6179 6572 7320 6f66 2073 697a  en layers of siz
-00012280: 6573 207b 6869 6464 656e 5f6c 6179 6572  es {hidden_layer
-00012290: 737d 2c20 7b64 696d 5f63 6f65 6666 7d20  s}, {dim_coeff} 
-000122a0: 7820 6e5f 6469 6d20 2b20 7b64 696d 5f63  x n_dim + {dim_c
-000122b0: 6f6e 7374 7d20 6578 7065 6374 6564 2c20  onst} expected, 
-000122c0: 6275 7420 676f 7420 7b77 6569 6768 7473  but got {weights
-000122d0: 2e73 697a 6528 2d31 297d 2e22 290a 2020  .size(-1)}.").  
-000122e0: 2020 2020 2020 7365 6c66 2e6e 5f64 696d        self.n_dim
-000122f0: 203d 2064 696d 5f63 6f6e 7374 202f 2f20   = dim_const // 
-00012300: 6469 6d5f 636f 6566 660a 2020 2020 2020  dim_coeff.      
-00012310: 2020 7365 6c66 2e6e 5f62 6174 6368 203d    self.n_batch =
-00012320: 2077 6569 6768 7473 2e6e 5f62 6174 6368   weights.n_batch
-00012330: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
-00012340: 7965 7273 203d 205b 5d0a 2020 2020 2020  yers = [].      
-00012350: 2020 7020 3d20 300a 2020 2020 2020 2020    p = 0.        
-00012360: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00012370: 656e 2868 6964 6465 6e5f 6c61 7965 7273  en(hidden_layers
-00012380: 2920 2b20 3129 3a0a 2020 2020 2020 2020  ) + 1):.        
-00012390: 2020 2020 696e 5f66 6561 7475 7265 7320      in_features 
-000123a0: 3d20 7365 6c66 2e6e 5f64 696d 2069 6620  = self.n_dim if 
-000123b0: 6920 3d3d 2030 2065 6c73 6520 6869 6464  i == 0 else hidd
-000123c0: 656e 5f6c 6179 6572 735b 6920 2d20 315d  en_layers[i - 1]
-000123d0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-000123e0: 5f66 6561 7475 7265 7320 3d20 7365 6c66  _features = self
-000123f0: 2e6e 5f64 696d 2069 6620 6920 3d3d 206c  .n_dim if i == l
-00012400: 656e 2868 6964 6465 6e5f 6c61 7965 7273  en(hidden_layers
-00012410: 2920 656c 7365 2068 6964 6465 6e5f 6c61  ) else hidden_la
-00012420: 7965 7273 5b69 5d0a 2020 2020 2020 2020  yers[i].        
-00012430: 2020 2020 6c61 7965 725f 7765 6967 6874      layer_weight
-00012440: 7320 3d20 7765 6967 6874 735b 2e2e 2e2c  s = weights[...,
-00012450: 2070 3a70 2b6f 7574 5f66 6561 7475 7265   p:p+out_feature
-00012460: 732a 696e 5f66 6561 7475 7265 735d 2e76  s*in_features].v
-00012470: 6965 7728 5b73 656c 662e 6e5f 6261 7463  iew([self.n_batc
-00012480: 685d 2c20 6f75 745f 6665 6174 7572 6573  h], out_features
-00012490: 2c20 696e 5f66 6561 7475 7265 7329 0a20  , in_features). 
-000124a0: 2020 2020 2020 2020 2020 2070 202b 3d20             p += 
-000124b0: 6f75 745f 6665 6174 7572 6573 202a 2069  out_features * i
-000124c0: 6e5f 6665 6174 7572 6573 0a20 2020 2020  n_features.     
-000124d0: 2020 2020 2020 206c 6179 6572 5f62 6961         layer_bia
-000124e0: 7320 3d20 7765 6967 6874 735b 2e2e 2e2c  s = weights[...,
-000124f0: 2070 3a70 2b6f 7574 5f66 6561 7475 7265   p:p+out_feature
-00012500: 735d 2e76 6965 7728 5b73 656c 662e 6e5f  s].view([self.n_
-00012510: 6261 7463 685d 2c20 6f75 745f 6665 6174  batch], out_feat
+00004390: 2020 2020 2061 766f 7563 6828 6c65 6e28       avouch(len(
+000043a0: 636f 6d70 2920 3d3d 2031 2c20 2245 7272  comp) == 1, "Err
+000043b0: 6f72 2069 6e20 6361 6c6c 696e 6720 6061  or in calling `a
+000043c0: 6666 696e 6560 3a20 4f6e 6c79 2074 6865  ffine`: Only the
+000043d0: 2063 6f6d 706f 7369 7469 6f6e 206f 6620   composition of 
+000043e0: 6c69 6e65 6172 2074 7261 6e73 666f 726d  linear transform
+000043f0: 6174 696f 6e73 2063 616e 2072 6573 756c  ations can resul
+00004400: 7420 696e 2061 6e20 6166 6669 6e65 206d  t in an affine m
+00004410: 6174 7269 782e 2229 0a20 2020 2020 2020  atrix.").       
+00004420: 2074 7261 6e73 203d 2063 6f6d 702e 7472   trans = comp.tr
+00004430: 616e 735f 6c69 7374 5b30 5d0a 2020 2020  ans_list[0].    
+00004440: 2020 2020 7265 7475 726e 2074 7261 6e73      return trans
+00004450: 2e61 6666 696e 6528 6e5f 6469 6d29 0a0a  .affine(n_dim)..
+00004460: 2020 2020 6465 6620 636f 6d70 6f73 6528      def compose(
+00004470: 7365 6c66 293a 0a20 2020 2020 2020 206f  self):.        o
+00004480: 7574 5f6c 6973 7420 3d20 5b5d 0a20 2020  ut_list = [].   
+00004490: 2020 2020 206e 5f64 696d 203d 2073 656c       n_dim = sel
+000044a0: 662e 6e5f 6469 6d0a 2020 2020 2020 2020  f.n_dim.        
+000044b0: 6375 725f 6166 6669 6e65 203d 204e 6f6e  cur_affine = Non
+000044c0: 650a 2020 2020 2020 2020 666f 7220 7420  e.        for t 
+000044d0: 696e 2073 656c 662e 7472 616e 735f 6c69  in self.trans_li
+000044e0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+000044f0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00004500: 6528 742c 2053 7061 7469 616c 5472 616e  e(t, SpatialTran
+00004510: 7366 6f72 6d61 7469 6f6e 293a 206f 7574  sformation): out
+00004520: 5f6c 6973 742e 6170 7065 6e64 2874 290a  _list.append(t).
+00004530: 2020 2020 2020 2020 2020 2020 6166 6620              aff 
+00004540: 3d20 742e 6166 6669 6e65 286e 5f64 696d  = t.affine(n_dim
+00004550: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00004560: 2061 6666 2069 7320 4e6f 6e65 2061 6e64   aff is None and
+00004570: 2063 7572 5f61 6666 696e 6520 6973 206e   cur_affine is n
+00004580: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00004590: 2020 2020 2020 2020 206f 7574 5f6c 6973           out_lis
+000045a0: 742e 6578 7465 6e64 285b 4166 6669 6e65  t.extend([Affine
+000045b0: 2863 7572 5f61 6666 696e 6529 2c20 745d  (cur_affine), t]
+000045c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000045d0: 2020 6375 725f 6166 6669 6e65 203d 204e    cur_affine = N
+000045e0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000045f0: 656c 6966 2061 6666 2069 7320 4e6f 6e65  elif aff is None
+00004600: 3a20 6f75 745f 6c69 7374 2e61 7070 656e  : out_list.appen
+00004610: 6428 7429 0a20 2020 2020 2020 2020 2020  d(t).           
+00004620: 2065 6c69 6620 6166 662e 7370 6163 6520   elif aff.space 
+00004630: 213d 2028 6e5f 6469 6d2b 312c 206e 5f64  != (n_dim+1, n_d
+00004640: 696d 2b31 293a 0a20 2020 2020 2020 2020  im+1):.         
+00004650: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+00004660: 6545 7272 6f72 2866 2255 6e63 6f6e 7369  eError(f"Unconsi
+00004670: 7374 656e 7420 7472 616e 7366 6f72 6d61  stent transforma
+00004680: 7469 6f6e 2077 6974 6820 6166 6669 6e65  tion with affine
+00004690: 206f 6620 7369 7a65 207b 6166 662e 7370   of size {aff.sp
+000046a0: 6163 657d 2069 6e20 436f 6d70 6f73 6564  ace} in Composed
+000046b0: 5472 616e 7366 6f72 6d61 7469 6f6e 2e20  Transformation. 
+000046c0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+000046d0: 6c69 6620 6375 725f 6166 6669 6e65 2069  lif cur_affine i
+000046e0: 7320 4e6f 6e65 3a20 6375 725f 6166 6669  s None: cur_affi
+000046f0: 6e65 203d 2061 6666 0a20 2020 2020 2020  ne = aff.       
+00004700: 2020 2020 2065 6c73 653a 2063 7572 5f61       else: cur_a
+00004710: 6666 696e 6520 3d20 6375 725f 6166 6669  ffine = cur_affi
+00004720: 6e65 2040 2061 6666 0a20 2020 2020 2020  ne @ aff.       
+00004730: 2069 6620 6375 725f 6166 6669 6e65 2069   if cur_affine i
+00004740: 7320 6e6f 7420 4e6f 6e65 3a20 6f75 745f  s not None: out_
+00004750: 6c69 7374 2e61 7070 656e 6428 4166 6669  list.append(Affi
+00004760: 6e65 2863 7572 5f61 6666 696e 6529 290a  ne(cur_affine)).
+00004770: 2020 2020 2020 2020 7265 7475 726e 2043          return C
+00004780: 6f6d 706f 7365 6454 7261 6e73 666f 726d  omposedTransform
+00004790: 6174 696f 6e28 2a6f 7574 5f6c 6973 742c  ation(*out_list,
+000047a0: 206d 6f64 6520 3d20 7365 6c66 2e6d 6f64   mode = self.mod
+000047b0: 6529 0a0a 2020 2020 6465 6620 746f 5f64  e)..    def to_d
+000047c0: 6963 7428 7365 6c66 293a 0a20 2020 2020  ict(self):.     
+000047d0: 2020 2064 6963 203d 2073 7570 6572 2829     dic = super()
+000047e0: 2e74 6f5f 6469 6374 2829 0a20 2020 2020  .to_dict().     
+000047f0: 2020 2064 6963 5b27 7472 616e 735f 6c69     dic['trans_li
+00004800: 7374 275d 203d 205b 742e 746f 5f64 6963  st'] = [t.to_dic
+00004810: 7428 2920 666f 7220 7420 696e 2073 656c  t() for t in sel
+00004820: 662e 7472 616e 735f 6c69 7374 5d0a 2020  f.trans_list].  
+00004830: 2020 2020 2020 7265 7475 726e 2064 6963        return dic
+00004840: 0a0a 2323 2323 2323 2323 2323 2320 5370  ..########### Sp
+00004850: 6174 6961 6c20 5472 616e 7366 6f72 6d61  atial Transforma
+00004860: 7469 6f6e 7320 2323 2323 2323 2323 2323  tions ##########
+00004870: 230a 0a63 6c61 7373 2053 7061 7469 616c  #..class Spatial
+00004880: 5472 616e 7366 6f72 6d61 7469 6f6e 2854  Transformation(T
+00004890: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
+000048a0: 2020 2020 0a20 2020 2064 6566 205f 5f69      .    def __i
+000048b0: 6e69 745f 5f28 7365 6c66 2c20 2a70 6172  nit__(self, *par
+000048c0: 616d 732c 202a 2a6b 7770 6172 616d 7329  ams, **kwparams)
+000048d0: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
+000048e0: 292e 5f5f 696e 6974 5f5f 282a 7061 7261  ).__init__(*para
+000048f0: 6d73 2c20 2a2a 6b77 7061 7261 6d73 290a  ms, **kwparams).
+00004900: 2020 2020 2020 2020 7365 6c66 2e62 6163          self.bac
+00004910: 6b77 6172 6420 3d20 5472 7565 0a20 2020  kward = True.   
+00004920: 2020 2020 200a 2020 2020 6465 6620 5f5f       .    def __
+00004930: 6361 6c6c 5f5f 2873 656c 662c 2058 293a  call__(self, X):
+00004940: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004950: 2020 2020 2058 205b 6274 2e54 656e 736f       X [bt.Tenso
+00004960: 725d 3a20 436f 6f72 6469 6e61 7465 7320  r]: Coordinates 
+00004970: 746f 2062 6520 7472 616e 7366 6f72 6d65  to be transforme
+00004980: 642e 0a20 2020 2020 2020 2020 2020 2073  d..            s
+00004990: 697a 653a 2028 5b6e 5f62 6174 6368 3a20  ize: ([n_batch: 
+000049a0: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
+000049b0: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
+000049c0: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
+000049d0: 6f75 7470 7574 205b 6274 2e54 656e 736f  output [bt.Tenso
+000049e0: 725d 3a20 5468 6520 7472 616e 7366 6f72  r]: The transfor
+000049f0: 6d65 6420 636f 6f72 6469 6e61 7465 732e  med coordinates.
+00004a00: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00004a10: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
+00004a20: 6e5f 6469 6d7d 2c20 6e5f 312c 206e 5f32  n_dim}, n_1, n_2
+00004a30: 2c20 2e2e 2e2c 206e 5f72 290a 2020 2020  , ..., n_r).    
+00004a40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004a50: 6176 6f75 6368 2858 2e68 6173 5f63 6861  avouch(X.has_cha
+00004a60: 6e6e 656c 2c20 6622 506c 6561 7365 2075  nnel, f"Please u
+00004a70: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
+00004a80: 7220 6f66 2073 697a 6520 5c0a 2020 2020  r of size \.    
+00004a90: 2020 2020 2020 2020 285b 6e5f 6261 7463          ([n_batc
+00004aa0: 683a 6f70 7469 6f6e 616c 5d2c 207b 7b6e  h:optional], {{n
+00004ab0: 5f64 696d 7d7d 2c20 6e5f 312c 206e 5f32  _dim}}, n_1, n_2
+00004ac0: 2c20 2e2e 2e2c 206e 5f72 2920 5c0a 2020  , ..., n_r) \.  
+00004ad0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00004ae0: 7220 7b73 656c 662e 5f5f 636c 6173 735f  r {self.__class_
+00004af0: 5f2e 5f5f 6e61 6d65 5f5f 2e73 706c 6974  _.__name__.split
+00004b00: 2827 2e27 295b 2d31 5d7d 2054 7261 6e73  ('.')[-1]} Trans
+00004b10: 666f 726d 6174 696f 6e2c 2069 6e73 7465  formation, inste
+00004b20: 6164 206f 6620 7b58 2e73 6861 7065 7d2e  ad of {X.shape}.
+00004b30: 2022 290a 2020 2020 2020 2020 6966 2073   ").        if s
+00004b40: 656c 662e 6e5f 6469 6d20 6973 206e 6f74  elf.n_dim is not
+00004b50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00004b60: 2020 2061 766f 7563 6828 582e 6e5f 6368     avouch(X.n_ch
+00004b70: 616e 6e65 6c20 3d3d 2073 656c 662e 6e5f  annel == self.n_
+00004b80: 6469 6d2c 2066 227b 7365 6c66 2e6e 5f64  dim, f"{self.n_d
+00004b90: 696d 7d44 207b 7365 6c66 2e5f 5f63 6c61  im}D {self.__cla
+00004ba0: 7373 5f5f 2e5f 5f6e 616d 655f 5f2e 7370  ss__.__name__.sp
+00004bb0: 6c69 7428 272e 2729 5b2d 315d 7d20 5472  lit('.')[-1]} Tr
+00004bc0: 616e 7366 6f72 6d61 7469 6f6e 205c 0a20  ansformation \. 
+00004bd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00004be0: 6f65 7320 6e6f 7420 7461 6b65 2063 6f6f  oes not take coo
+00004bf0: 7264 696e 6174 6573 206f 6620 7369 7a65  rdinates of size
+00004c00: 207b 582e 7368 6170 657d 2229 0a20 2020   {X.shape}").   
+00004c10: 2020 2020 2069 6620 582e 6861 735f 6261       if X.has_ba
+00004c20: 7463 683a 2061 766f 7563 6828 7365 6c66  tch: avouch(self
+00004c30: 2e6e 5f62 6174 6368 2069 7320 4e6f 6e65  .n_batch is None
+00004c40: 206f 7220 7365 6c66 2e6e 5f62 6174 6368   or self.n_batch
+00004c50: 203d 3d20 3120 6f72 2058 2e6e 5f62 6174   == 1 or X.n_bat
+00004c60: 6368 203d 3d20 3120 6f72 2058 2e6e 5f62  ch == 1 or X.n_b
+00004c70: 6174 6368 203d 3d20 7365 6c66 2e6e 5f62  atch == self.n_b
+00004c80: 6174 6368 2c20 0a20 2020 2020 2020 2020  atch, .         
+00004c90: 2020 2066 227b 7365 6c66 2e6e 5f64 696d     f"{self.n_dim
+00004ca0: 7d44 207b 7365 6c66 2e5f 5f63 6c61 7373  }D {self.__class
+00004cb0: 5f5f 2e5f 5f6e 616d 655f 5f2e 7370 6c69  __.__name__.spli
+00004cc0: 7428 272e 2729 5b2d 315d 7d20 5472 616e  t('.')[-1]} Tran
+00004cd0: 7366 6f72 6d61 7469 6f6e 2077 6974 6820  sformation with 
+00004ce0: 6261 7463 6820 7369 7a65 207b 7365 6c66  batch size {self
+00004cf0: 2e6e 5f62 6174 6368 7d20 5c0a 2020 2020  .n_batch} \.    
+00004d00: 2020 2020 2020 2020 2020 2020 646f 6573              does
+00004d10: 206e 6f74 2074 616b 6520 636f 6f72 6469   not take coordi
+00004d20: 6e61 7465 7320 7769 7468 2077 726f 6e67  nates with wrong
+00004d30: 2062 6174 6368 2073 697a 652e 2043 7572   batch size. Cur
+00004d40: 7265 6e74 2073 697a 653a 207b 582e 7368  rent size: {X.sh
+00004d50: 6170 657d 2e22 290a 2020 2020 2020 2020  ape}.").        
+00004d60: 5920 3d20 582e 666c 6f61 7428 292e 636c  Y = X.float().cl
+00004d70: 6f6e 6528 290a 2020 2020 2020 2020 6966  one().        if
+00004d80: 206e 6f74 2059 2e68 6173 5f62 6174 6368   not Y.has_batch
+00004d90: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00004da0: 2073 656c 662e 6e5f 6261 7463 6820 6973   self.n_batch is
+00004db0: 206e 6f74 204e 6f6e 653a 2059 203d 2059   not None: Y = Y
+00004dc0: 2e6d 756c 7469 706c 7928 7365 6c66 2e6e  .multiply(self.n
+00004dd0: 5f62 6174 6368 2c20 5b5d 290a 2020 2020  _batch, []).    
+00004de0: 2020 2020 2020 2020 656c 7365 3a20 5920          else: Y 
+00004df0: 3d20 592e 756e 7371 7565 657a 6528 5b5d  = Y.unsqueeze([]
+00004e00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00004e10: 2059 0a0a 2020 2020 6465 6620 5f5f 6d61   Y..    def __ma
+00004e20: 746d 756c 5f5f 2878 2c20 7929 3a0a 2020  tmul__(x, y):.  
+00004e30: 2020 2020 2020 6966 2069 735f 7370 6174        if is_spat
+00004e40: 6961 6c5f 7472 616e 7366 6f72 6d61 7469  ial_transformati
+00004e50: 6f6e 2878 2920 616e 6420 6973 5f73 7061  on(x) and is_spa
+00004e60: 7469 616c 5f74 7261 6e73 666f 726d 6174  tial_transformat
+00004e70: 696f 6e28 7929 3a0a 2020 2020 2020 2020  ion(y):.        
+00004e80: 2020 2020 7265 7475 726e 2043 6f6d 706f      return Compo
+00004e90: 7365 6454 7261 6e73 666f 726d 6174 696f  sedTransformatio
+00004ea0: 6e28 782c 2079 2c20 6d6f 6465 3d22 7370  n(x, y, mode="sp
+00004eb0: 6174 6961 6c22 290a 2020 2020 2020 2020  atial").        
+00004ec0: 7265 7475 726e 2043 6f6d 706f 7365 6454  return ComposedT
+00004ed0: 7261 6e73 666f 726d 6174 696f 6e28 782c  ransformation(x,
+00004ee0: 2079 290a 2020 2020 0a20 2020 2064 6566   y).    .    def
+00004ef0: 2061 6666 696e 6528 7365 6c66 2c20 6e5f   affine(self, n_
+00004f00: 6469 6d3d 4e6f 6e65 293a 0a20 2020 2020  dim=None):.     
+00004f10: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00004f20: 2020 200a 2020 2020 4061 6c69 6173 2827     .    @alias('
+00004f30: 746f 4444 4627 290a 2020 2020 6465 6620  toDDF').    def 
+00004f40: 746f 5f44 4446 2873 656c 662c 202a 7368  to_DDF(self, *sh
+00004f50: 6170 6529 3a0a 2020 2020 2020 2020 7368  ape):.        sh
+00004f60: 6170 6520 3d20 6172 675f 7475 706c 6528  ape = arg_tuple(
+00004f70: 7368 6170 6529 0a20 2020 2020 2020 2067  shape).        g
+00004f80: 7269 6420 3d20 6274 2e69 6d61 6765 5f67  rid = bt.image_g
+00004f90: 7269 6428 2a73 6861 7065 292e 756e 7371  rid(*shape).unsq
+00004fa0: 7565 657a 6528 5b5d 292e 666c 6f61 7428  ueeze([]).float(
+00004fb0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00004fc0: 2073 656c 6628 6772 6964 2920 2d20 6772   self(grid) - gr
+00004fd0: 6964 0a0a 2020 2020 6465 6620 746f 5f69  id..    def to_i
+00004fe0: 6d61 6765 5f73 7061 6365 2873 656c 662c  mage_space(self,
+00004ff0: 2073 6f75 7263 652c 2074 6172 6765 7429   source, target)
+00005000: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
+00005010: 6e73 7461 6e63 6528 736f 7572 6365 2c20  nstance(source, 
+00005020: 7374 7229 3a20 736f 7572 6365 203d 2049  str): source = I
+00005030: 4d47 2873 6f75 7263 6529 0a20 2020 2020  MG(source).     
+00005040: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00005050: 2874 6172 6765 742c 2073 7472 293a 2074  (target, str): t
+00005060: 6172 6765 7420 3d20 494d 4728 7461 7267  arget = IMG(targ
+00005070: 6574 290a 2020 2020 2020 2020 6966 2069  et).        if i
+00005080: 7369 6e73 7461 6e63 6528 736f 7572 6365  sinstance(source
+00005090: 2c20 494d 4729 3a20 736f 7572 6365 203d  , IMG): source =
+000050a0: 2073 6f75 7263 652e 6166 6669 6e65 0a20   source.affine. 
+000050b0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+000050c0: 616e 6365 2874 6172 6765 742c 2049 4d47  ance(target, IMG
+000050d0: 293a 2074 6172 6765 7420 3d20 7461 7267  ): target = targ
+000050e0: 6574 2e61 6666 696e 650a 2020 2020 2020  et.affine.      
+000050f0: 2020 7265 7475 726e 2073 656c 662e 746f    return self.to
+00005100: 2827 696d 6167 6527 2c20 736f 7572 6365  ('image', source
+00005110: 5f61 6666 696e 653d 736f 7572 6365 2c20  _affine=source, 
+00005120: 7461 7267 6574 5f61 6666 696e 653d 7461  target_affine=ta
+00005130: 7267 6574 290a 0a20 2020 2064 6566 2074  rget)..    def t
+00005140: 6f5f 776f 726c 645f 7370 6163 6528 7365  o_world_space(se
+00005150: 6c66 2c20 736f 7572 6365 2c20 7461 7267  lf, source, targ
+00005160: 6574 293a 0a20 2020 2020 2020 2069 6620  et):.        if 
+00005170: 6973 696e 7374 616e 6365 2873 6f75 7263  isinstance(sourc
+00005180: 652c 2073 7472 293a 2073 6f75 7263 6520  e, str): source 
+00005190: 3d20 494d 4728 736f 7572 6365 290a 2020  = IMG(source).  
+000051a0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+000051b0: 6e63 6528 7461 7267 6574 2c20 7374 7229  nce(target, str)
+000051c0: 3a20 7461 7267 6574 203d 2049 4d47 2874  : target = IMG(t
+000051d0: 6172 6765 7429 0a20 2020 2020 2020 2069  arget).        i
+000051e0: 6620 6973 696e 7374 616e 6365 2873 6f75  f isinstance(sou
+000051f0: 7263 652c 2049 4d47 293a 2073 6f75 7263  rce, IMG): sourc
+00005200: 6520 3d20 736f 7572 6365 2e61 6666 696e  e = source.affin
+00005210: 650a 2020 2020 2020 2020 6966 2069 7369  e.        if isi
+00005220: 6e73 7461 6e63 6528 7461 7267 6574 2c20  nstance(target, 
+00005230: 494d 4729 3a20 7461 7267 6574 203d 2074  IMG): target = t
+00005240: 6172 6765 742e 6166 6669 6e65 0a20 2020  arget.affine.   
+00005250: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00005260: 2e74 6f28 2777 6f72 6c64 272c 2073 6f75  .to('world', sou
+00005270: 7263 655f 6166 6669 6e65 3d73 6f75 7263  rce_affine=sourc
+00005280: 652c 2074 6172 6765 745f 6166 6669 6e65  e, target_affine
+00005290: 3d74 6172 6765 7429 0a0a 2020 2020 6465  =target)..    de
+000052a0: 6620 746f 2873 656c 662c 2073 7061 6365  f to(self, space
+000052b0: 203d 2022 776f 726c 6422 2c20 736f 7572   = "world", sour
+000052c0: 6365 5f61 6666 696e 6520 3d20 6274 2e65  ce_affine = bt.e
+000052d0: 7965 2834 292c 2074 6172 6765 745f 6166  ye(4), target_af
+000052e0: 6669 6e65 203d 2062 742e 6579 6528 3429  fine = bt.eye(4)
+000052f0: 293a 0a20 2020 2020 2020 2074 6172 6765  ):.        targe
+00005300: 745f 6166 6669 6e65 203d 2062 6174 6f72  t_affine = bator
+00005310: 6368 5f74 656e 736f 7228 7461 7267 6574  ch_tensor(target
+00005320: 5f61 6666 696e 6529 2e66 6c6f 6174 2829  _affine).float()
+00005330: 0a20 2020 2020 2020 2073 6f75 7263 655f  .        source_
+00005340: 6166 6669 6e65 203d 2062 6174 6f72 6368  affine = batorch
+00005350: 5f74 656e 736f 7228 736f 7572 6365 5f61  _tensor(source_a
+00005360: 6666 696e 6529 2e66 6c6f 6174 2829 0a20  ffine).float(). 
+00005370: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+00005380: 5f61 6666 696e 652e 6e64 696d 203c 3d20  _affine.ndim <= 
+00005390: 323a 2074 6172 6765 745f 6166 6669 6e65  2: target_affine
+000053a0: 203d 2062 742e 756e 7371 7565 657a 6528   = bt.unsqueeze(
+000053b0: 7461 7267 6574 5f61 6666 696e 6529 0a20  target_affine). 
+000053c0: 2020 2020 2020 2069 6620 736f 7572 6365         if source
+000053d0: 5f61 6666 696e 652e 6e64 696d 203c 3d20  _affine.ndim <= 
+000053e0: 323a 2073 6f75 7263 655f 6166 6669 6e65  2: source_affine
+000053f0: 203d 2062 742e 756e 7371 7565 657a 6528   = bt.unsqueeze(
+00005400: 736f 7572 6365 5f61 6666 696e 6529 0a20  source_affine). 
+00005410: 2020 2020 2020 2069 6620 7370 6163 652e         if space.
+00005420: 6c6f 7765 7228 2920 3d3d 2022 776f 726c  lower() == "worl
+00005430: 6422 206f 7220 7370 6163 652e 6c6f 7765  d" or space.lowe
+00005440: 7228 2920 3d3d 2022 7068 7973 6963 616c  r() == "physical
+00005450: 223a 2074 6166 6669 6e65 203d 2062 742e  ": taffine = bt.
+00005460: 696e 7628 7461 7267 6574 5f61 6666 696e  inv(target_affin
+00005470: 6529 3b20 7361 6666 696e 6520 3d20 736f  e); saffine = so
+00005480: 7572 6365 5f61 6666 696e 650a 2020 2020  urce_affine.    
+00005490: 2020 2020 656c 6966 2073 7061 6365 2e6c      elif space.l
+000054a0: 6f77 6572 2829 203d 3d20 2269 6d61 6765  ower() == "image
+000054b0: 2220 6f72 2073 7061 6365 2e6c 6f77 6572  " or space.lower
+000054c0: 2829 203d 3d20 2269 6e64 6578 223a 2074  () == "index": t
+000054d0: 6166 6669 6e65 203d 2074 6172 6765 745f  affine = target_
+000054e0: 6166 6669 6e65 3b20 7361 6666 696e 6520  affine; saffine 
+000054f0: 3d20 6274 2e69 6e76 2873 6f75 7263 655f  = bt.inv(source_
+00005500: 6166 6669 6e65 290a 2020 2020 2020 2020  affine).        
+00005510: 656c 7365 3a20 7261 6973 6520 5479 7065  else: raise Type
+00005520: 4572 726f 7228 2249 6e76 616c 6964 2073  Error("Invalid s
+00005530: 7061 6365 2066 6f72 206d 6574 686f 6420  pace for method 
+00005540: 2774 6f27 2c20 7573 6520 2777 6f72 6c64  'to', use 'world
+00005550: 272f 2770 6879 7369 6361 6c27 206f 7220  '/'physical' or 
+00005560: 2769 6d61 6765 272f 2769 6e64 6578 2720  'image'/'index' 
+00005570: 696e 7374 6561 642e 2229 0a20 2020 2020  instead.").     
+00005580: 2020 2072 6574 7572 6e20 436f 6d70 6f73     return Compos
+00005590: 6564 5472 616e 7366 6f72 6d61 7469 6f6e  edTransformation
+000055a0: 2841 6666 696e 6528 7361 6666 696e 6529  (Affine(saffine)
+000055b0: 2c20 7365 6c66 2c20 4166 6669 6e65 2874  , self, Affine(t
+000055c0: 6166 6669 6e65 292c 206d 6f64 653d 2773  affine), mode='s
+000055d0: 7061 7469 616c 2729 0a20 2020 200a 2020  patial').    .  
+000055e0: 2020 6465 6620 6e75 6d5f 696e 7628 7365    def num_inv(se
+000055f0: 6c66 2c20 2a73 697a 652c 2076 6572 626f  lf, *size, verbo
+00005600: 7365 3d46 616c 7365 293a 0a20 2020 2020  se=False):.     
+00005610: 2020 2066 726f 6d20 2e66 756e 6373 2069     from .funcs i
+00005620: 6d70 6f72 7420 6265 6e64 696e 670a 2020  mport bending.  
+00005630: 2020 2020 2020 7369 7a65 203d 2061 7267        size = arg
+00005640: 5f74 7570 6c65 2873 697a 6529 0a20 2020  _tuple(size).   
+00005650: 2020 2020 2058 203d 2062 742e 696d 6167       X = bt.imag
+00005660: 655f 6772 6964 282a 7369 7a65 292e 756e  e_grid(*size).un
+00005670: 7371 7565 657a 6528 5b5d 292e 666c 6f61  squeeze([]).floa
+00005680: 7428 290a 2020 2020 2020 2020 696e 765f  t().        inv_
+00005690: 6469 7370 203d 202d 2073 656c 662e 746f  disp = - self.to
+000056a0: 5f44 4446 282a 7369 7a65 292e 636c 6f6e  _DDF(*size).clon
+000056b0: 6528 292e 6465 7461 6368 2829 0a20 2020  e().detach().   
+000056c0: 2020 2020 2069 6e76 5f64 6973 702e 7265       inv_disp.re
+000056d0: 7175 6972 6573 5f67 7261 6420 3d20 5472  quires_grad = Tr
+000056e0: 7565 0a20 2020 2020 2020 206f 7074 696d  ue.        optim
+000056f0: 697a 6572 203d 2062 742e 4341 4441 4d28  izer = bt.CADAM(
+00005700: 5b69 6e76 5f64 6973 705d 2c20 6c72 203d  [inv_disp], lr =
+00005710: 2031 652d 3229 0a20 2020 2020 2020 2070   1e-2).        p
+00005720: 7265 765f 6c6f 7373 203d 204e 6f6e 650a  rev_loss = None.
+00005730: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00005740: 2072 616e 6765 2834 3030 293a 0a20 2020   range(400):.   
+00005750: 2020 2020 2020 2020 2069 7472 616e 7320           itrans 
+00005760: 3d20 4465 6e73 6544 6973 706c 6163 656d  = DenseDisplacem
+00005770: 656e 7446 6965 6c64 2869 6e76 5f64 6973  entField(inv_dis
+00005780: 7029 0a20 2020 2020 2020 2020 2020 206c  p).            l
+00005790: 6f73 7320 3d20 2869 7472 616e 7328 7365  oss = (itrans(se
+000057a0: 6c66 2858 2929 202d 2058 292e 6e6f 726d  lf(X)) - X).norm
+000057b0: 3228 292e 6d65 616e 2829 202b 2031 652d  2().mean() + 1e-
+000057c0: 3120 2a20 6265 6e64 696e 6728 696e 765f  1 * bending(inv_
+000057d0: 6469 7370 290a 2020 2020 2020 2020 2020  disp).          
+000057e0: 2020 6f70 7469 6d69 7a65 722e 6d69 6e69    optimizer.mini
+000057f0: 6d69 7a65 286c 6f73 7329 2e73 7465 7028  mize(loss).step(
+00005800: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00005810: 2076 6572 626f 7365 3a20 7072 696e 7428   verbose: print(
+00005820: 6622 6974 6572 6174 696f 6e20 7b69 2b31  f"iteration {i+1
+00005830: 7d3a 206c 6f73 7320 3d20 7b6c 6f73 732e  }: loss = {loss.
+00005840: 6974 656d 2829 7d22 290a 2020 2020 2020  item()}").      
+00005850: 2020 2020 2020 6966 2070 7265 765f 6c6f        if prev_lo
+00005860: 7373 2069 7320 6e6f 7420 4e6f 6e65 2061  ss is not None a
+00005870: 6e64 206c 6f73 732e 6974 656d 2829 203e  nd loss.item() >
+00005880: 3d20 7072 6576 5f6c 6f73 733a 206e 6f64  = prev_loss: nod
+00005890: 726f 705f 636f 756e 7420 2b3d 2031 0a20  rop_count += 1. 
+000058a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000058b0: 206e 6f64 726f 705f 636f 756e 7420 3d20   nodrop_count = 
+000058c0: 300a 2020 2020 2020 2020 2020 2020 6966  0.            if
+000058d0: 206e 6f64 726f 705f 636f 756e 7420 3e3d   nodrop_count >=
+000058e0: 2036 3a0a 2020 2020 2020 2020 2020 2020   6:.            
+000058f0: 2020 2020 6966 2076 6572 626f 7365 3a20      if verbose: 
+00005900: 7072 696e 7428 6622 5374 6f70 2061 7420  print(f"Stop at 
+00005910: 6974 6572 6174 696f 6e20 7b69 2b31 7d20  iteration {i+1} 
+00005920: 6475 6520 746f 206e 6f20 6472 6f70 7069  due to no droppi
+00005930: 6e67 2e20 2229 0a20 2020 2020 2020 2020  ng. ").         
+00005940: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00005950: 2020 2020 2020 2020 2069 6620 6c6f 7373           if loss
+00005960: 2e69 7465 6d28 2920 3c20 3165 2d33 3a0a  .item() < 1e-3:.
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 6966 2076 6572 626f 7365 3a20 7072 696e  if verbose: prin
+00005990: 7428 6622 5374 6f70 2061 7420 6974 6572  t(f"Stop at iter
+000059a0: 6174 696f 6e20 7b69 2b31 7d20 6475 6520  ation {i+1} due 
+000059b0: 746f 2073 6d61 6c6c 206c 6f73 732e 2022  to small loss. "
+000059c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000059d0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+000059e0: 7265 7475 726e 2044 656e 7365 4469 7370  return DenseDisp
+000059f0: 6c61 6365 6d65 6e74 4669 656c 6428 696e  lacementField(in
+00005a00: 765f 6469 7370 290a 2020 2020 0a20 2020  v_disp).    .   
+00005a10: 2064 6566 2066 6f72 6365 5f69 6e76 2873   def force_inv(s
+00005a20: 656c 662c 202a 7369 7a65 293a 0a20 2020  elf, *size):.   
+00005a30: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+00005a40: 7365 6c66 2c20 2769 6e76 2729 3a20 7265  self, 'inv'): re
+00005a50: 7475 726e 2073 656c 662e 696e 7628 290a  turn self.inv().
+00005a60: 2020 2020 2020 2020 656c 7365 3a20 7265          else: re
+00005a70: 7475 726e 2073 656c 662e 6e75 6d5f 696e  turn self.num_in
+00005a80: 7628 2a73 697a 6529 0a0a 4061 6c69 6173  v(*size)..@alias
+00005a90: 2822 4964 2229 0a63 6c61 7373 2049 6465  ("Id").class Ide
+00005aa0: 6e74 6974 7928 5370 6174 6961 6c54 7261  ntity(SpatialTra
+00005ab0: 6e73 666f 726d 6174 696f 6e29 3a0a 0a20  nsformation):.. 
+00005ac0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00005ad0: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
+00005ae0: 2727 0a20 2020 2020 2020 2049 6465 6e74  ''.        Ident
+00005af0: 6974 7920 7472 616e 7366 6f72 6d61 7469  ity transformati
+00005b00: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+00005b10: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
+00005b20: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
+00005b30: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
+00005b40: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
+00005b50: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
+00005b60: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
+00005b70: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
+00005b80: 6261 7463 683a 6f70 7469 6f6e 616c 5d2c  batch:optional],
+00005b90: 207b 6e5f 6469 6d7d 2c20 6e5f 312c 206e   {n_dim}, n_1, n
+00005ba0: 5f32 2c20 2e2e 2e2c 206e 5f72 290a 2020  _2, ..., n_r).  
+00005bb0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00005bc0: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
+00005bd0: 6520 7472 616e 7366 6f72 6d65 6420 636f  e transformed co
+00005be0: 6f72 6469 6e61 7465 732e 2028 5361 6d65  ordinates. (Same
+00005bf0: 2061 7320 5820 666f 7220 4964 656e 7469   as X for Identi
+00005c00: 7479 290a 2020 2020 2020 2020 2020 2020  ty).            
+00005c10: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+00005c20: 7463 685d 2c20 7b6e 5f64 696d 7d2c 206e  tch], {n_dim}, n
+00005c30: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
+00005c40: 7229 0a20 2020 2020 2020 2027 2727 0a20  r).        '''. 
+00005c50: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+00005c60: 5f69 6e69 745f 5f28 290a 2020 2020 2020  _init__().      
+00005c70: 2020 0a20 2020 2064 6566 2061 6666 696e    .    def affin
+00005c80: 6528 7365 6c66 2c20 6e5f 6469 6d3d 4e6f  e(self, n_dim=No
+00005c90: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
+00005ca0: 6e5f 6469 6d20 6973 204e 6f6e 653a 2072  n_dim is None: r
+00005cb0: 6574 7572 6e0a 2020 2020 2020 2020 7265  eturn.        re
+00005cc0: 7475 726e 2062 742e 6579 6528 6e5f 6469  turn bt.eye(n_di
+00005cd0: 6d20 2b20 3129 2e75 6e73 7175 6565 7a65  m + 1).unsqueeze
+00005ce0: 285b 5d29 0a0a 2020 2020 6465 6620 696e  ([])..    def in
+00005cf0: 7628 7365 6c66 293a 2072 6574 7572 6e20  v(self): return 
+00005d00: 4964 656e 7469 7479 2829 2e62 6163 6b77  Identity().backw
+00005d10: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
+00005d20: 7264 290a 0a63 6c61 7373 2052 6f74 6174  rd)..class Rotat
+00005d30: 696f 6e39 3028 5370 6174 6961 6c54 7261  ion90(SpatialTra
+00005d40: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
+00005d50: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00005d60: 656c 662c 2064 696d 312c 2064 696d 322c  elf, dim1, dim2,
+00005d70: 2069 6d61 6765 5f73 697a 653d 4e6f 6e65   image_size=None
+00005d80: 2c20 7265 7369 7a65 5f69 6d61 6765 3d54  , resize_image=T
+00005d90: 7275 6529 3a0a 2020 2020 2020 2020 2727  rue):.        ''
+00005da0: 270a 2020 2020 2020 2020 5472 616e 7366  '.        Transf
+00005db0: 6f72 6d61 7469 6f6e 2074 6861 7420 726f  ormation that ro
+00005dc0: 7461 7465 7320 616e 2069 6d61 6765 206f  tates an image o
+00005dd0: 6620 6069 6d61 6765 5f73 697a 6560 2062  f `image_size` b
+00005de0: 7920 3930 2064 6567 7265 6573 2e0a 2020  y 90 degrees..  
+00005df0: 2020 2020 2020 0a20 2020 2020 2020 204e        .        N
+00005e00: 6f74 653a 2054 6865 2072 6f74 6174 696f  ote: The rotatio
+00005e10: 6e20 6973 2066 6f72 2063 6f6f 7264 696e  n is for coordin
+00005e20: 6174 6573 2c20 6865 6e63 6520 7468 6520  ates, hence the 
+00005e30: 696d 6167 6520 726f 7461 7465 7320 636c  image rotates cl
+00005e40: 6f63 6b77 6973 652e 200a 2020 2020 2020  ockwise. .      
+00005e50: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
+00005e60: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+00005e70: 696d 312c 2064 696d 3220 5b69 6e74 5d3a  im1, dim2 [int]:
+00005e80: 2054 6865 2070 6c61 6e65 2077 6520 726f   The plane we ro
+00005e90: 7461 7465 206f 6e2e 2044 6972 6563 7469  tate on. Directi
+00005ea0: 6f6e 206f 6620 7468 6520 726f 7461 7469  on of the rotati
+00005eb0: 6f6e 2069 7320 6672 6f6d 2060 6469 6d31  on is from `dim1
+00005ec0: 6020 746f 2060 6469 6d32 602e 0a20 2020  ` to `dim2`..   
+00005ed0: 2020 2020 2020 2020 2020 2020 2069 2e65               i.e
+00005ee0: 2e20 636f 756e 7465 722d 636c 6f63 6b77  . counter-clockw
+00005ef0: 6973 6520 726f 7461 7469 6f6e 2077 6974  ise rotation wit
+00005f00: 6820 6469 6d31 2061 7320 782d 6178 6973  h dim1 as x-axis
+00005f10: 2061 6e64 2064 696d 3220 6173 2079 2d61   and dim2 as y-a
+00005f20: 7869 733a 205b 6469 6d31 2c20 6469 6d32  xis: [dim1, dim2
+00005f30: 5d20 636f 6f72 6469 6e61 7465 7320 2878  ] coordinates (x
+00005f40: 2c20 7929 2062 6563 6f6d 6573 2028 796d  , y) becomes (ym
+00005f50: 6178 2d79 2c20 7829 2e0a 2020 2020 2020  ax-y, x)..      
+00005f60: 2020 2020 2020 696d 6167 655f 7369 7a65        image_size
+00005f70: 205b 7475 706c 6520 6f72 2062 742e 5465   [tuple or bt.Te
+00005f80: 6e73 6f72 5d3a 2054 6865 2073 697a 6520  nsor]: The size 
+00005f90: 6f66 2074 6865 2069 6d61 6765 2c20 6f72  of the image, or
+00005fa0: 2074 6865 2069 6d61 6765 2069 7473 656c   the image itsel
+00005fb0: 662e 200a 2020 2020 2020 2020 2020 2020  f. .            
+00005fc0: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
+00005fd0: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
+00005fe0: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
+00005ff0: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
+00006000: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
+00006010: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
+00006020: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
+00006030: 6261 7463 683a 6f70 7469 6f6e 616c 5d2c  batch:optional],
+00006040: 207b 6e5f 6469 6d7d 2c20 6e5f 312c 206e   {n_dim}, n_1, n
+00006050: 5f32 2c20 2e2e 2e2c 206e 5f72 290a 2020  _2, ..., n_r).  
+00006060: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00006070: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
+00006080: 6520 7472 616e 7366 6f72 6d65 6420 636f  e transformed co
+00006090: 6f72 6469 6e61 7465 732e 0a20 2020 2020  ordinates..     
+000060a0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
+000060b0: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
+000060c0: 6469 6d7d 2c20 6e5f 312c 206e 5f32 2c20  dim}, n_1, n_2, 
+000060d0: 2e2e 2e2c 206e 5f72 290a 2020 2020 2020  ..., n_r).      
+000060e0: 2020 2727 270a 2020 2020 2020 2020 7375    '''.        su
+000060f0: 7065 7228 292e 5f5f 696e 6974 5f5f 2864  per().__init__(d
+00006100: 696d 313d 6469 6d31 2c20 6469 6d32 3d64  im1=dim1, dim2=d
+00006110: 696d 322c 2069 6d61 6765 5f73 697a 653d  im2, image_size=
+00006120: 696d 6167 655f 7369 7a65 2c20 7265 7369  image_size, resi
+00006130: 7a65 5f69 6d61 6765 3d72 6573 697a 655f  ze_image=resize_
+00006140: 696d 6167 6529 0a0a 2020 2020 2020 2020  image)..        
+00006150: 7365 6c66 2e64 696d 312c 2073 656c 662e  self.dim1, self.
+00006160: 6469 6d32 203d 2064 696d 312c 2064 696d  dim2 = dim1, dim
+00006170: 320a 2020 2020 2020 2020 6966 2069 7369  2.        if isi
+00006180: 6e73 7461 6e63 6528 696d 6167 655f 7369  nstance(image_si
+00006190: 7a65 2c20 6274 2e74 6f72 6368 2e54 656e  ze, bt.torch.Ten
+000061a0: 736f 7229 3a20 696d 6167 655f 7369 7a65  sor): image_size
+000061b0: 203d 2069 6d61 6765 5f73 697a 652e 7368   = image_size.sh
+000061c0: 6170 650a 2020 2020 2020 2020 7365 6c66  ape.        self
+000061d0: 2e69 6d61 6765 5f73 697a 6520 3d20 696d  .image_size = im
+000061e0: 6167 655f 7369 7a65 0a20 2020 2020 2020  age_size.       
+000061f0: 2069 6620 696d 6167 655f 7369 7a65 2069   if image_size i
+00006200: 7320 6e6f 7420 4e6f 6e65 3a20 7365 6c66  s not None: self
+00006210: 2e6e 5f64 696d 203d 206c 656e 2869 6d61  .n_dim = len(ima
+00006220: 6765 5f73 697a 6529 0a20 2020 2020 2020  ge_size).       
+00006230: 2069 6620 7265 7369 7a65 5f69 6d61 6765   if resize_image
+00006240: 3a20 7365 6c66 2e72 6573 6861 7065 203d  : self.reshape =
+00006250: 205b 2831 2c29 2c20 2864 696d 312c 2064   [(1,), (dim1, d
+00006260: 696d 3229 5d0a 0a20 2020 2064 6566 205f  im2)]..    def _
+00006270: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
+00006280: 3a0a 2020 2020 2020 2020 5820 3d20 7375  :.        X = su
+00006290: 7065 7228 292e 5f5f 6361 6c6c 5f5f 2858  per().__call__(X
+000062a0: 290a 2020 2020 2020 2020 6469 6d31 2c20  ).        dim1, 
+000062b0: 6469 6d32 203d 2073 656c 662e 6469 6d31  dim2 = self.dim1
+000062c0: 2c20 7365 6c66 2e64 696d 320a 2020 2020  , self.dim2.    
+000062d0: 2020 2020 7365 6c65 6374 3120 3d20 2873      select1 = (s
+000062e0: 6c69 6365 284e 6f6e 6529 2c29 202a 2058  lice(None),) * X
+000062f0: 2e63 6861 6e6e 656c 5f64 696d 202b 2028  .channel_dim + (
+00006300: 6469 6d31 2c29 0a20 2020 2020 2020 2073  dim1,).        s
+00006310: 656c 6563 7432 203d 2028 736c 6963 6528  elect2 = (slice(
+00006320: 4e6f 6e65 292c 2920 2a20 582e 6368 616e  None),) * X.chan
+00006330: 6e65 6c5f 6469 6d20 2b20 2864 696d 322c  nel_dim + (dim2,
+00006340: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00006350: 662e 696d 6167 655f 7369 7a65 2069 7320  f.image_size is 
+00006360: 4e6f 6e65 3a20 6d61 785f 7261 6e67 6520  None: max_range 
+00006370: 3d20 585b 7365 6c65 6374 325d 2e6d 6178  = X[select2].max
+00006380: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+00006390: 206d 6178 5f72 616e 6765 203d 2073 656c   max_range = sel
+000063a0: 662e 696d 6167 655f 7369 7a65 5b64 696d  f.image_size[dim
+000063b0: 325d 0a20 2020 2020 2020 2058 5b73 656c  2].        X[sel
+000063c0: 6563 7431 5d20 3d20 585b 7365 6c65 6374  ect1] = X[select
+000063d0: 315d 202b 206d 6178 5f72 616e 6765 202d  1] + max_range -
+000063e0: 2058 5b73 656c 6563 7432 5d0a 2020 2020   X[select2].    
+000063f0: 2020 2020 585b 7365 6c65 6374 325d 203d      X[select2] =
+00006400: 2058 5b73 656c 6563 7431 5d20 2b20 585b   X[select1] + X[
+00006410: 7365 6c65 6374 325d 202d 206d 6178 5f72  select2] - max_r
+00006420: 616e 6765 0a20 2020 2020 2020 2058 5b73  ange.        X[s
+00006430: 656c 6563 7431 5d20 3d20 585b 7365 6c65  elect1] = X[sele
+00006440: 6374 315d 202d 2058 5b73 656c 6563 7432  ct1] - X[select2
+00006450: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
+00006460: 2058 0a20 2020 2020 2020 200a 2020 2020   X.        .    
+00006470: 6465 6620 6166 6669 6e65 2873 656c 662c  def affine(self,
+00006480: 206e 5f64 696d 3d4e 6f6e 6529 3a0a 2020   n_dim=None):.  
+00006490: 2020 2020 2020 6966 2073 656c 662e 696d        if self.im
+000064a0: 6167 655f 7369 7a65 2069 7320 4e6f 6e65  age_size is None
+000064b0: 3a20 7265 7475 726e 0a20 2020 2020 2020  : return.       
+000064c0: 2069 6620 6e5f 6469 6d20 6973 204e 6f6e   if n_dim is Non
+000064d0: 6520 616e 6420 7365 6c66 2e6e 5f64 696d  e and self.n_dim
+000064e0: 2069 7320 4e6f 6e65 3a20 7265 7475 726e   is None: return
+000064f0: 0a20 2020 2020 2020 2069 6620 6e5f 6469  .        if n_di
+00006500: 6d20 6973 204e 6f6e 653a 206e 5f64 696d  m is None: n_dim
+00006510: 203d 2073 656c 662e 6e5f 6469 6d0a 2020   = self.n_dim.  
+00006520: 2020 2020 2020 6176 6f75 6368 2873 656c        avouch(sel
+00006530: 662e 6e5f 6469 6d20 6973 204e 6f6e 6520  f.n_dim is None 
+00006540: 6f72 2073 656c 662e 6e5f 6469 6d20 3d3d  or self.n_dim ==
+00006550: 206e 5f64 696d 290a 2020 2020 2020 2020   n_dim).        
+00006560: 6469 6d31 2c20 6469 6d32 203d 2073 656c  dim1, dim2 = sel
+00006570: 662e 6469 6d31 2c20 7365 6c66 2e64 696d  f.dim1, self.dim
+00006580: 320a 2020 2020 2020 2020 6166 6620 3d20  2.        aff = 
+00006590: 6274 2e65 7965 286e 5f64 696d 202b 2031  bt.eye(n_dim + 1
+000065a0: 290a 2020 2020 2020 2020 6166 665b 6469  ).        aff[di
+000065b0: 6d31 5d5b 6469 6d31 5d20 3d20 302e 0a20  m1][dim1] = 0.. 
+000065c0: 2020 2020 2020 2061 6666 5b64 696d 315d         aff[dim1]
+000065d0: 5b64 696d 325d 203d 202d 312e 0a20 2020  [dim2] = -1..   
+000065e0: 2020 2020 2061 6666 5b64 696d 315d 5b2d       aff[dim1][-
+000065f0: 315d 203d 2066 6c6f 6174 2873 656c 662e  1] = float(self.
+00006600: 696d 6167 655f 7369 7a65 5b64 696d 325d  image_size[dim2]
+00006610: 290a 2020 2020 2020 2020 6166 665b 6469  ).        aff[di
+00006620: 6d32 5d5b 6469 6d32 5d20 3d20 302e 0a20  m2][dim2] = 0.. 
+00006630: 2020 2020 2020 2061 6666 5b64 696d 325d         aff[dim2]
+00006640: 5b64 696d 315d 203d 2031 2e0a 2020 2020  [dim1] = 1..    
+00006650: 2020 2020 7265 7475 726e 2061 6666 2e75      return aff.u
+00006660: 6e73 7175 6565 7a65 285b 5d29 0a20 2020  nsqueeze([]).   
+00006670: 200a 2020 2020 6465 6620 696e 7628 7365   .    def inv(se
+00006680: 6c66 293a 2072 6574 7572 6e20 526f 7461  lf): return Rota
+00006690: 7469 6f6e 3237 3028 7365 6c66 2e64 696d  tion270(self.dim
+000066a0: 312c 2073 656c 662e 6469 6d32 2c20 696d  1, self.dim2, im
+000066b0: 6167 655f 7369 7a65 203d 2073 656c 662e  age_size = self.
+000066c0: 696d 6167 655f 7369 7a65 2c20 7265 7369  image_size, resi
+000066d0: 7a65 5f69 6d61 6765 203d 2073 656c 662e  ze_image = self.
+000066e0: 7265 7369 7a65 5f69 6d61 6765 292e 6261  resize_image).ba
+000066f0: 636b 7761 7264 5f28 7365 6c66 2e62 6163  ckward_(self.bac
+00006700: 6b77 6172 6429 0a0a 636c 6173 7320 526f  kward)..class Ro
+00006710: 7461 7469 6f6e 3237 3028 5370 6174 6961  tation270(Spatia
+00006720: 6c54 7261 6e73 666f 726d 6174 696f 6e29  lTransformation)
+00006730: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00006740: 5f5f 2873 656c 662c 2064 696d 312c 2064  __(self, dim1, d
+00006750: 696d 322c 2069 6d61 6765 5f73 697a 653d  im2, image_size=
+00006760: 4e6f 6e65 2c20 7265 7369 7a65 5f69 6d61  None, resize_ima
+00006770: 6765 3d54 7275 6529 3a0a 2020 2020 2020  ge=True):.      
+00006780: 2020 2727 270a 2020 2020 2020 2020 5472    '''.        Tr
+00006790: 616e 7366 6f72 6d61 7469 6f6e 2074 6861  ansformation tha
+000067a0: 7420 726f 7461 7465 7320 616e 2069 6d61  t rotates an ima
+000067b0: 6765 2062 7920 3237 3020 6465 6772 6565  ge by 270 degree
+000067c0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+000067d0: 2020 2020 4e6f 7465 3a20 5468 6520 726f      Note: The ro
+000067e0: 7461 7469 6f6e 2069 7320 666f 7220 636f  tation is for co
+000067f0: 6f72 6469 6e61 7465 732c 2068 656e 6365  ordinates, hence
+00006800: 2074 6865 2069 6d61 6765 2072 6f74 6174   the image rotat
+00006810: 6573 2063 6c6f 636b 7769 7365 2e20 0a20  es clockwise. . 
+00006820: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006830: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
+00006840: 2020 2020 6469 6d31 2c20 6469 6d32 205b      dim1, dim2 [
+00006850: 696e 745d 3a20 5468 6520 706c 616e 6520  int]: The plane 
+00006860: 7765 2072 6f74 6174 6520 6f6e 2e20 4469  we rotate on. Di
+00006870: 7265 6374 696f 6e20 6f66 2074 6865 2072  rection of the r
+00006880: 6f74 6174 696f 6e20 6973 2066 726f 6d20  otation is from 
+00006890: 6064 696d 3160 2074 6f20 6064 696d 3260  `dim1` to `dim2`
+000068a0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000068b0: 2020 692e 652e 2063 6f75 6e74 6572 2d63    i.e. counter-c
+000068c0: 6c6f 636b 7769 7365 2072 6f74 6174 696f  lockwise rotatio
+000068d0: 6e20 7769 7468 2064 696d 3120 6173 2078  n with dim1 as x
+000068e0: 2d61 7869 7320 616e 6420 6469 6d32 2061  -axis and dim2 a
+000068f0: 7320 792d 6178 6973 3a20 5b64 696d 312c  s y-axis: [dim1,
+00006900: 2064 696d 325d 2063 6f6f 7264 696e 6174   dim2] coordinat
+00006910: 6573 2028 782c 2079 2920 6265 636f 6d65  es (x, y) become
+00006920: 7320 2879 2c20 786d 6178 2d78 292e 0a20  s (y, xmax-x).. 
+00006930: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+00006940: 5f73 697a 6520 5b74 7570 6c65 206f 7220  _size [tuple or 
+00006950: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
+00006960: 7369 7a65 206f 6620 7468 6520 696d 6167  size of the imag
+00006970: 652c 206f 7220 7468 6520 696d 6167 6520  e, or the image 
+00006980: 6974 7365 6c66 2e20 0a20 2020 2020 2020  itself. .       
+00006990: 2020 2020 200a 2020 2020 2020 2020 5768       .        Wh
+000069a0: 656e 2069 7420 6973 2063 616c 6c65 643a  en it is called:
+000069b0: 0a20 2020 2020 2020 2020 2020 2058 205b  .            X [
+000069c0: 6274 2e54 656e 736f 725d 3a20 436f 6f72  bt.Tensor]: Coor
+000069d0: 6469 6e61 7465 7320 746f 2062 6520 7472  dinates to be tr
+000069e0: 616e 7366 6f72 6d65 642e 0a20 2020 2020  ansformed..     
+000069f0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
+00006a00: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
+00006a10: 6e61 6c5d 2c20 7b6e 5f64 696d 7d2c 206e  nal], {n_dim}, n
+00006a20: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
+00006a30: 7229 0a20 2020 2020 2020 2020 2020 206f  r).            o
+00006a40: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
+00006a50: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
+00006a60: 6564 2063 6f6f 7264 696e 6174 6573 2e0a  ed coordinates..
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
+00006a90: 2c20 7b6e 5f64 696d 7d2c 206e 5f31 2c20  , {n_dim}, n_1, 
+00006aa0: 6e5f 322c 202e 2e2e 2c20 6e5f 7229 0a20  n_2, ..., n_r). 
+00006ab0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00006ac0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00006ad0: 745f 5f28 6469 6d31 3d64 696d 312c 2064  t__(dim1=dim1, d
+00006ae0: 696d 323d 6469 6d32 2c20 696d 6167 655f  im2=dim2, image_
+00006af0: 7369 7a65 3d69 6d61 6765 5f73 697a 652c  size=image_size,
+00006b00: 2072 6573 697a 655f 696d 6167 653d 7265   resize_image=re
+00006b10: 7369 7a65 5f69 6d61 6765 290a 0a20 2020  size_image)..   
+00006b20: 2020 2020 2073 656c 662e 6469 6d31 2c20       self.dim1, 
+00006b30: 7365 6c66 2e64 696d 3220 3d20 6469 6d31  self.dim2 = dim1
+00006b40: 2c20 6469 6d32 0a20 2020 2020 2020 2069  , dim2.        i
+00006b50: 6620 6973 696e 7374 616e 6365 2869 6d61  f isinstance(ima
+00006b60: 6765 5f73 697a 652c 2062 742e 746f 7263  ge_size, bt.torc
+00006b70: 682e 5465 6e73 6f72 293a 2069 6d61 6765  h.Tensor): image
+00006b80: 5f73 697a 6520 3d20 696d 6167 655f 7369  _size = image_si
+00006b90: 7a65 2e73 6861 7065 0a20 2020 2020 2020  ze.shape.       
+00006ba0: 2073 656c 662e 696d 6167 655f 7369 7a65   self.image_size
+00006bb0: 203d 2069 6d61 6765 5f73 697a 650a 2020   = image_size.  
+00006bc0: 2020 2020 2020 6966 2069 6d61 6765 5f73        if image_s
+00006bd0: 697a 6520 6973 206e 6f74 204e 6f6e 653a  ize is not None:
+00006be0: 2073 656c 662e 6e5f 6469 6d20 3d20 6c65   self.n_dim = le
+00006bf0: 6e28 696d 6167 655f 7369 7a65 290a 2020  n(image_size).  
+00006c00: 2020 2020 2020 6966 2072 6573 697a 655f        if resize_
+00006c10: 696d 6167 653a 2073 656c 662e 7265 7368  image: self.resh
+00006c20: 6170 6520 3d20 5b28 312c 292c 2028 6469  ape = [(1,), (di
+00006c30: 6d31 2c20 6469 6d32 295d 0a0a 2020 2020  m1, dim2)]..    
+00006c40: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
+00006c50: 662c 2058 293a 0a20 2020 2020 2020 2058  f, X):.        X
+00006c60: 203d 2073 7570 6572 2829 2e5f 5f63 616c   = super().__cal
+00006c70: 6c5f 5f28 5829 0a20 2020 2020 2020 2064  l__(X).        d
+00006c80: 696d 312c 2064 696d 3220 3d20 7365 6c66  im1, dim2 = self
+00006c90: 2e64 696d 312c 2073 656c 662e 6469 6d32  .dim1, self.dim2
+00006ca0: 0a20 2020 2020 2020 2073 656c 6563 7431  .        select1
+00006cb0: 203d 2028 736c 6963 6528 4e6f 6e65 292c   = (slice(None),
+00006cc0: 2920 2a20 582e 6368 616e 6e65 6c5f 6469  ) * X.channel_di
+00006cd0: 6d20 2b20 2864 696d 312c 290a 2020 2020  m + (dim1,).    
+00006ce0: 2020 2020 7365 6c65 6374 3220 3d20 2873      select2 = (s
+00006cf0: 6c69 6365 284e 6f6e 6529 2c29 202a 2058  lice(None),) * X
+00006d00: 2e63 6861 6e6e 656c 5f64 696d 202b 2028  .channel_dim + (
+00006d10: 6469 6d32 2c29 0a20 2020 2020 2020 2069  dim2,).        i
+00006d20: 6620 7365 6c66 2e69 6d61 6765 5f73 697a  f self.image_siz
+00006d30: 6520 6973 204e 6f6e 653a 206d 6178 5f72  e is None: max_r
+00006d40: 616e 6765 203d 2058 5b73 656c 6563 7431  ange = X[select1
+00006d50: 5d2e 6d61 7828 290a 2020 2020 2020 2020  ].max().        
+00006d60: 656c 7365 3a20 6d61 785f 7261 6e67 6520  else: max_range 
+00006d70: 3d20 7365 6c66 2e69 6d61 6765 5f73 697a  = self.image_siz
+00006d80: 655b 6469 6d31 5d0a 2020 2020 2020 2020  e[dim1].        
+00006d90: 585b 7365 6c65 6374 325d 203d 2058 5b73  X[select2] = X[s
+00006da0: 656c 6563 7432 5d20 2b20 6d61 785f 7261  elect2] + max_ra
+00006db0: 6e67 6520 2d20 585b 7365 6c65 6374 315d  nge - X[select1]
+00006dc0: 0a20 2020 2020 2020 2058 5b73 656c 6563  .        X[selec
+00006dd0: 7431 5d20 3d20 585b 7365 6c65 6374 325d  t1] = X[select2]
+00006de0: 202b 2058 5b73 656c 6563 7431 5d20 2d20   + X[select1] - 
+00006df0: 6d61 785f 7261 6e67 650a 2020 2020 2020  max_range.      
+00006e00: 2020 585b 7365 6c65 6374 325d 203d 2058    X[select2] = X
+00006e10: 5b73 656c 6563 7432 5d20 2d20 585b 7365  [select2] - X[se
+00006e20: 6c65 6374 315d 0a20 2020 2020 2020 2072  lect1].        r
+00006e30: 6574 7572 6e20 580a 2020 2020 2020 2020  eturn X.        
+00006e40: 0a20 2020 2064 6566 2061 6666 696e 6528  .    def affine(
+00006e50: 7365 6c66 2c20 6e5f 6469 6d3d 4e6f 6e65  self, n_dim=None
+00006e60: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00006e70: 6c66 2e69 6d61 6765 5f73 697a 6520 6973  lf.image_size is
+00006e80: 204e 6f6e 653a 2072 6574 7572 6e0a 2020   None: return.  
+00006e90: 2020 2020 2020 6966 206e 5f64 696d 2069        if n_dim i
+00006ea0: 7320 4e6f 6e65 2061 6e64 2073 656c 662e  s None and self.
+00006eb0: 6e5f 6469 6d20 6973 204e 6f6e 653a 2072  n_dim is None: r
+00006ec0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+00006ed0: 206e 5f64 696d 2069 7320 4e6f 6e65 3a20   n_dim is None: 
+00006ee0: 6e5f 6469 6d20 3d20 7365 6c66 2e6e 5f64  n_dim = self.n_d
+00006ef0: 696d 0a20 2020 2020 2020 2061 766f 7563  im.        avouc
+00006f00: 6828 7365 6c66 2e6e 5f64 696d 2069 7320  h(self.n_dim is 
+00006f10: 4e6f 6e65 206f 7220 7365 6c66 2e6e 5f64  None or self.n_d
+00006f20: 696d 203d 3d20 6e5f 6469 6d29 0a20 2020  im == n_dim).   
+00006f30: 2020 2020 2064 696d 312c 2064 696d 3220       dim1, dim2 
+00006f40: 3d20 7365 6c66 2e64 696d 312c 2073 656c  = self.dim1, sel
+00006f50: 662e 6469 6d32 0a20 2020 2020 2020 2061  f.dim2.        a
+00006f60: 6666 203d 2062 742e 6579 6528 6e5f 6469  ff = bt.eye(n_di
+00006f70: 6d20 2b20 3129 0a20 2020 2020 2020 2061  m + 1).        a
+00006f80: 6666 5b64 696d 315d 5b64 696d 315d 203d  ff[dim1][dim1] =
+00006f90: 2030 2e0a 2020 2020 2020 2020 6166 665b   0..        aff[
+00006fa0: 6469 6d31 5d5b 6469 6d32 5d20 3d20 312e  dim1][dim2] = 1.
+00006fb0: 0a20 2020 2020 2020 2061 6666 5b64 696d  .        aff[dim
+00006fc0: 325d 5b64 696d 325d 203d 2030 2e0a 2020  2][dim2] = 0..  
+00006fd0: 2020 2020 2020 6166 665b 6469 6d32 5d5b        aff[dim2][
+00006fe0: 6469 6d31 5d20 3d20 2d31 2e0a 2020 2020  dim1] = -1..    
+00006ff0: 2020 2020 6166 665b 6469 6d32 5d5b 2d31      aff[dim2][-1
+00007000: 5d20 3d20 666c 6f61 7428 7365 6c66 2e69  ] = float(self.i
+00007010: 6d61 6765 5f73 697a 655b 6469 6d31 5d29  mage_size[dim1])
+00007020: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007030: 6166 662e 756e 7371 7565 657a 6528 5b5d  aff.unsqueeze([]
+00007040: 290a 2020 2020 0a20 2020 2064 6566 2069  ).    .    def i
+00007050: 6e76 2873 656c 6629 3a20 7265 7475 726e  nv(self): return
+00007060: 2052 6f74 6174 696f 6e39 3028 7365 6c66   Rotation90(self
+00007070: 2e64 696d 312c 2073 656c 662e 6469 6d32  .dim1, self.dim2
+00007080: 2c20 696d 6167 655f 7369 7a65 203d 2073  , image_size = s
+00007090: 656c 662e 696d 6167 655f 7369 7a65 2c20  elf.image_size, 
+000070a0: 7265 7369 7a65 5f69 6d61 6765 203d 2073  resize_image = s
+000070b0: 656c 662e 7265 7369 7a65 5f69 6d61 6765  elf.resize_image
+000070c0: 292e 6261 636b 7761 7264 5f28 7365 6c66  ).backward_(self
+000070d0: 2e62 6163 6b77 6172 6429 0a0a 636c 6173  .backward)..clas
+000070e0: 7320 526f 7461 7469 6f6e 3138 3028 5370  s Rotation180(Sp
+000070f0: 6174 6961 6c54 7261 6e73 666f 726d 6174  atialTransformat
+00007100: 696f 6e29 3a0a 2020 2020 6465 6620 5f5f  ion):.    def __
+00007110: 696e 6974 5f5f 2873 656c 662c 2064 696d  init__(self, dim
+00007120: 312c 2064 696d 322c 2069 6d61 6765 5f73  1, dim2, image_s
+00007130: 697a 653d 4e6f 6e65 293a 0a20 2020 2020  ize=None):.     
+00007140: 2020 2027 2727 0a20 2020 2020 2020 2054     '''.        T
+00007150: 7261 6e73 666f 726d 6174 696f 6e20 7468  ransformation th
+00007160: 6174 2072 6f74 6174 6573 2061 6e20 696d  at rotates an im
+00007170: 6167 6520 6279 2031 3830 2064 6567 7265  age by 180 degre
+00007180: 6573 2e0a 2020 2020 2020 2020 0a20 2020  es..        .   
+00007190: 2020 2020 2050 6172 616d 733a 0a20 2020       Params:.   
+000071a0: 2020 2020 2020 2020 2064 696d 312c 2064           dim1, d
+000071b0: 696d 3220 5b69 6e74 5d3a 2054 6865 2070  im2 [int]: The p
+000071c0: 6c61 6e65 2077 6520 726f 7461 7465 206f  lane we rotate o
+000071d0: 6e2e 2044 6972 6563 7469 6f6e 206f 6620  n. Direction of 
+000071e0: 7468 6520 726f 7461 7469 6f6e 2069 7320  the rotation is 
+000071f0: 6672 6f6d 2060 6469 6d31 6020 746f 2060  from `dim1` to `
+00007200: 6469 6d32 602e 0a20 2020 2020 2020 2020  dim2`..         
+00007210: 2020 2020 2020 2069 2e65 2e20 726f 7461         i.e. rota
+00007220: 7469 6f6e 2077 6974 6820 6469 6d31 2061  tion with dim1 a
+00007230: 7320 782d 6178 6973 2061 6e64 2064 696d  s x-axis and dim
+00007240: 3220 6173 2079 2d61 7869 733a 205b 6469  2 as y-axis: [di
+00007250: 6d31 2c20 6469 6d32 5d20 636f 6f72 6469  m1, dim2] coordi
+00007260: 6e61 7465 7320 2878 2c20 7929 2062 6563  nates (x, y) bec
+00007270: 6f6d 6573 2028 786d 6178 2d78 2c20 796d  omes (xmax-x, ym
+00007280: 6178 2d79 292e 0a20 2020 2020 2020 2020  ax-y)..         
+00007290: 2020 2069 6d61 6765 5f73 697a 6520 5b74     image_size [t
+000072a0: 7570 6c65 206f 7220 6274 2e54 656e 736f  uple or bt.Tenso
+000072b0: 725d 3a20 5468 6520 7369 7a65 206f 6620  r]: The size of 
+000072c0: 7468 6520 696d 6167 652c 206f 7220 7468  the image, or th
+000072d0: 6520 696d 6167 6520 6974 7365 6c66 2e20  e image itself. 
+000072e0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+000072f0: 2020 2020 2020 5768 656e 2069 7420 6973        When it is
+00007300: 2063 616c 6c65 643a 0a20 2020 2020 2020   called:.       
+00007310: 2020 2020 2058 205b 6274 2e54 656e 736f       X [bt.Tenso
+00007320: 725d 3a20 436f 6f72 6469 6e61 7465 7320  r]: Coordinates 
+00007330: 746f 2062 6520 7472 616e 7366 6f72 6d65  to be transforme
+00007340: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
+00007350: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
+00007360: 6368 3a6f 7074 696f 6e61 6c5d 2c20 7b6e  ch:optional], {n
+00007370: 5f64 696d 7d2c 206e 5f31 2c20 6e5f 322c  _dim}, n_1, n_2,
+00007380: 202e 2e2e 2c20 6e5f 7229 0a20 2020 2020   ..., n_r).     
+00007390: 2020 2020 2020 206f 7574 7075 7420 5b62         output [b
+000073a0: 742e 5465 6e73 6f72 5d3a 2054 6865 2074  t.Tensor]: The t
+000073b0: 7261 6e73 666f 726d 6564 2063 6f6f 7264  ransformed coord
+000073c0: 696e 6174 6573 2e0a 2020 2020 2020 2020  inates..        
+000073d0: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+000073e0: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
+000073f0: 7d2c 206e 5f31 2c20 6e5f 322c 202e 2e2e  }, n_1, n_2, ...
+00007400: 2c20 6e5f 7229 0a20 2020 2020 2020 2027  , n_r).        '
+00007410: 2727 0a20 2020 2020 2020 2073 7570 6572  ''.        super
+00007420: 2829 2e5f 5f69 6e69 745f 5f28 6469 6d31  ().__init__(dim1
+00007430: 3d64 696d 312c 2064 696d 323d 6469 6d32  =dim1, dim2=dim2
+00007440: 2c20 696d 6167 655f 7369 7a65 3d69 6d61  , image_size=ima
+00007450: 6765 5f73 697a 6529 0a0a 2020 2020 2020  ge_size)..      
+00007460: 2020 7365 6c66 2e64 696d 312c 2073 656c    self.dim1, sel
+00007470: 662e 6469 6d32 203d 2064 696d 312c 2064  f.dim2 = dim1, d
+00007480: 696d 320a 2020 2020 2020 2020 6966 2069  im2.        if i
+00007490: 7369 6e73 7461 6e63 6528 696d 6167 655f  sinstance(image_
+000074a0: 7369 7a65 2c20 6274 2e74 6f72 6368 2e54  size, bt.torch.T
+000074b0: 656e 736f 7229 3a20 696d 6167 655f 7369  ensor): image_si
+000074c0: 7a65 203d 2069 6d61 6765 5f73 697a 652e  ze = image_size.
+000074d0: 7368 6170 650a 2020 2020 2020 2020 7365  shape.        se
+000074e0: 6c66 2e69 6d61 6765 5f73 697a 6520 3d20  lf.image_size = 
+000074f0: 696d 6167 655f 7369 7a65 0a20 2020 2020  image_size.     
+00007500: 2020 2069 6620 696d 6167 655f 7369 7a65     if image_size
+00007510: 2069 7320 6e6f 7420 4e6f 6e65 3a20 7365   is not None: se
+00007520: 6c66 2e6e 5f64 696d 203d 206c 656e 2869  lf.n_dim = len(i
+00007530: 6d61 6765 5f73 697a 6529 0a0a 2020 2020  mage_size)..    
+00007540: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
+00007550: 662c 2058 293a 0a20 2020 2020 2020 2058  f, X):.        X
+00007560: 203d 2073 7570 6572 2829 2e5f 5f63 616c   = super().__cal
+00007570: 6c5f 5f28 5829 0a20 2020 2020 2020 2064  l__(X).        d
+00007580: 696d 312c 2064 696d 3220 3d20 7365 6c66  im1, dim2 = self
+00007590: 2e64 696d 312c 2073 656c 662e 6469 6d32  .dim1, self.dim2
+000075a0: 0a20 2020 2020 2020 2073 656c 6563 7431  .        select1
+000075b0: 203d 2028 736c 6963 6528 4e6f 6e65 292c   = (slice(None),
+000075c0: 2920 2a20 582e 6368 616e 6e65 6c5f 6469  ) * X.channel_di
+000075d0: 6d20 2b20 2864 696d 312c 290a 2020 2020  m + (dim1,).    
+000075e0: 2020 2020 7365 6c65 6374 3220 3d20 2873      select2 = (s
+000075f0: 6c69 6365 284e 6f6e 6529 2c29 202a 2058  lice(None),) * X
+00007600: 2e63 6861 6e6e 656c 5f64 696d 202b 2028  .channel_dim + (
+00007610: 6469 6d32 2c29 0a20 2020 2020 2020 2069  dim2,).        i
+00007620: 6620 7365 6c66 2e69 6d61 6765 5f73 697a  f self.image_siz
+00007630: 6520 6973 204e 6f6e 653a 206d 6178 5f72  e is None: max_r
+00007640: 616e 6765 312c 206d 6178 5f72 616e 6765  ange1, max_range
+00007650: 3220 3d20 585b 7365 6c65 6374 315d 2e6d  2 = X[select1].m
+00007660: 6178 2829 2c20 585b 7365 6c65 6374 325d  ax(), X[select2]
+00007670: 2e6d 6178 2829 0a20 2020 2020 2020 2065  .max().        e
+00007680: 6c73 653a 206d 6178 5f72 616e 6765 312c  lse: max_range1,
+00007690: 206d 6178 5f72 616e 6765 3220 3d20 7365   max_range2 = se
+000076a0: 6c66 2e69 6d61 6765 5f73 697a 655b 6469  lf.image_size[di
+000076b0: 6d31 5d2c 2073 656c 662e 696d 6167 655f  m1], self.image_
+000076c0: 7369 7a65 5b64 696d 325d 0a20 2020 2020  size[dim2].     
+000076d0: 2020 2058 5b73 656c 6563 7431 5d20 3d20     X[select1] = 
+000076e0: 6d61 785f 7261 6e67 6531 202d 2058 5b73  max_range1 - X[s
+000076f0: 656c 6563 7431 5d0a 2020 2020 2020 2020  elect1].        
+00007700: 585b 7365 6c65 6374 325d 203d 206d 6178  X[select2] = max
+00007710: 5f72 616e 6765 3220 2d20 585b 7365 6c65  _range2 - X[sele
+00007720: 6374 325d 0a20 2020 2020 2020 2072 6574  ct2].        ret
+00007730: 7572 6e20 580a 2020 2020 2020 2020 0a20  urn X.        . 
+00007740: 2020 2064 6566 2061 6666 696e 6528 7365     def affine(se
+00007750: 6c66 2c20 6e5f 6469 6d3d 4e6f 6e65 293a  lf, n_dim=None):
+00007760: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00007770: 2e69 6d61 6765 5f73 697a 6520 6973 204e  .image_size is N
+00007780: 6f6e 653a 2072 6574 7572 6e0a 2020 2020  one: return.    
+00007790: 2020 2020 6966 206e 5f64 696d 2069 7320      if n_dim is 
+000077a0: 4e6f 6e65 2061 6e64 2073 656c 662e 6e5f  None and self.n_
+000077b0: 6469 6d20 6973 204e 6f6e 653a 2072 6574  dim is None: ret
+000077c0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
+000077d0: 5f64 696d 2069 7320 4e6f 6e65 3a20 6e5f  _dim is None: n_
+000077e0: 6469 6d20 3d20 7365 6c66 2e6e 5f64 696d  dim = self.n_dim
+000077f0: 0a20 2020 2020 2020 2061 766f 7563 6828  .        avouch(
+00007800: 7365 6c66 2e6e 5f64 696d 2069 7320 4e6f  self.n_dim is No
+00007810: 6e65 206f 7220 7365 6c66 2e6e 5f64 696d  ne or self.n_dim
+00007820: 203d 3d20 6e5f 6469 6d29 0a20 2020 2020   == n_dim).     
+00007830: 2020 2064 696d 312c 2064 696d 3220 3d20     dim1, dim2 = 
+00007840: 7365 6c66 2e64 696d 312c 2073 656c 662e  self.dim1, self.
+00007850: 6469 6d32 0a20 2020 2020 2020 2061 6666  dim2.        aff
+00007860: 203d 2062 742e 6579 6528 6e5f 6469 6d20   = bt.eye(n_dim 
+00007870: 2b20 3129 0a20 2020 2020 2020 2061 6666  + 1).        aff
+00007880: 5b64 696d 315d 5b64 696d 315d 203d 202d  [dim1][dim1] = -
+00007890: 312e 0a20 2020 2020 2020 2061 6666 5b64  1..        aff[d
+000078a0: 696d 315d 5b2d 315d 203d 2066 6c6f 6174  im1][-1] = float
+000078b0: 2873 656c 662e 696d 6167 655f 7369 7a65  (self.image_size
+000078c0: 5b64 696d 315d 290a 2020 2020 2020 2020  [dim1]).        
+000078d0: 6166 665b 6469 6d32 5d5b 6469 6d32 5d20  aff[dim2][dim2] 
+000078e0: 3d20 2d31 2e0a 2020 2020 2020 2020 6166  = -1..        af
+000078f0: 665b 6469 6d32 5d5b 2d31 5d20 3d20 666c  f[dim2][-1] = fl
+00007900: 6f61 7428 7365 6c66 2e69 6d61 6765 5f73  oat(self.image_s
+00007910: 697a 655b 6469 6d32 5d29 0a20 2020 2020  ize[dim2]).     
+00007920: 2020 2072 6574 7572 6e20 6166 662e 756e     return aff.un
+00007930: 7371 7565 657a 6528 5b5d 290a 0a20 2020  squeeze([])..   
+00007940: 2064 6566 2069 6e76 2873 656c 6629 3a20   def inv(self): 
+00007950: 7265 7475 726e 2052 6f74 6174 696f 6e31  return Rotation1
+00007960: 3830 2873 656c 662e 6469 6d31 2c20 7365  80(self.dim1, se
+00007970: 6c66 2e64 696d 322c 2069 6d61 6765 5f73  lf.dim2, image_s
+00007980: 697a 6520 3d20 7365 6c66 2e69 6d61 6765  ize = self.image
+00007990: 5f73 697a 6529 2e62 6163 6b77 6172 645f  _size).backward_
+000079a0: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
+000079b0: 0a40 616c 6961 7328 2252 6566 6c65 6374  .@alias("Reflect
+000079c0: 2229 0a63 6c61 7373 2052 6566 6c65 6374  ").class Reflect
+000079d0: 696f 6e28 5370 6174 6961 6c54 7261 6e73  ion(SpatialTrans
+000079e0: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
+000079f0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00007a00: 662c 202a 6469 6d2c 2069 6d61 6765 5f73  f, *dim, image_s
+00007a10: 697a 653d 4e6f 6e65 293a 0a20 2020 2020  ize=None):.     
+00007a20: 2020 2027 2727 0a20 2020 2020 2020 2054     '''.        T
+00007a30: 7261 6e73 666f 726d 6174 696f 6e20 7468  ransformation th
+00007a40: 6174 2072 6566 6c65 6374 7320 616e 2069  at reflects an i
+00007a50: 6d61 6765 2061 6c6f 6e67 2064 696d 656e  mage along dimen
+00007a60: 7369 6f6e 2064 696d 2e0a 2020 2020 2020  sion dim..      
+00007a70: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
+00007a80: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+00007a90: 696d 205b 696e 745d 3a20 5468 6520 6469  im [int]: The di
+00007aa0: 6d65 6e73 696f 6e20 7765 2072 6566 6c65  mension we refle
+00007ab0: 6374 2074 6865 2069 6d61 6765 2061 6c6f  ct the image alo
+00007ac0: 6e67 2e20 0a20 2020 2020 2020 2020 2020  ng. .           
+00007ad0: 2020 2020 2069 2e65 2e20 7265 666c 6563       i.e. reflec
+00007ae0: 7469 6f6e 206f 6e20 6469 6d3a 205b 6469  tion on dim: [di
+00007af0: 6d5d 2063 6f6f 7264 696e 6174 6520 7820  m] coordinate x 
+00007b00: 6265 636f 6d65 7320 786d 6178 2d78 2e0a  becomes xmax-x..
+00007b10: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+00007b20: 655f 7369 7a65 205b 7475 706c 6520 6f72  e_size [tuple or
+00007b30: 2062 742e 5465 6e73 6f72 5d3a 2054 6865   bt.Tensor]: The
+00007b40: 2073 697a 6520 6f66 2074 6865 2069 6d61   size of the ima
+00007b50: 6765 2c20 6f72 2074 6865 2069 6d61 6765  ge, or the image
+00007b60: 2069 7473 656c 662e 200a 2020 2020 2020   itself. .      
+00007b70: 2020 2020 2020 0a20 2020 2020 2020 2057        .        W
+00007b80: 6865 6e20 6974 2069 7320 6361 6c6c 6564  hen it is called
+00007b90: 3a0a 2020 2020 2020 2020 2020 2020 5820  :.            X 
+00007ba0: 5b62 742e 5465 6e73 6f72 5d3a 2043 6f6f  [bt.Tensor]: Coo
+00007bb0: 7264 696e 6174 6573 2074 6f20 6265 2074  rdinates to be t
+00007bc0: 7261 6e73 666f 726d 6564 2e0a 2020 2020  ransformed..    
+00007bd0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00007be0: 3a20 285b 6e5f 6261 7463 683a 6f70 7469  : ([n_batch:opti
+00007bf0: 6f6e 616c 5d2c 207b 6e5f 6469 6d7d 2c20  onal], {n_dim}, 
+00007c00: 6e5f 312c 206e 5f32 2c20 2e2e 2e2c 206e  n_1, n_2, ..., n
+00007c10: 5f72 290a 2020 2020 2020 2020 2020 2020  _r).            
+00007c20: 6f75 7470 7574 205b 6274 2e54 656e 736f  output [bt.Tenso
+00007c30: 725d 3a20 5468 6520 7472 616e 7366 6f72  r]: The transfor
+00007c40: 6d65 6420 636f 6f72 6469 6e61 7465 732e  med coordinates.
+00007c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007c60: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+00007c70: 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f 312c  ], {n_dim}, n_1,
+00007c80: 206e 5f32 2c20 2e2e 2e2c 206e 5f72 290a   n_2, ..., n_r).
+00007c90: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00007ca0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00007cb0: 6974 5f5f 2864 696d 733d 6469 6d2c 2069  it__(dims=dim, i
+00007cc0: 6d61 6765 5f73 697a 653d 696d 6167 655f  mage_size=image_
+00007cd0: 7369 7a65 290a 0a20 2020 2020 2020 2069  size)..        i
+00007ce0: 6620 6c65 6e28 6469 6d29 203d 3d20 3120  f len(dim) == 1 
+00007cf0: 616e 6420 6973 696e 7374 616e 6365 2864  and isinstance(d
+00007d00: 696d 5b30 5d2c 2028 6c69 7374 2c20 7475  im[0], (list, tu
+00007d10: 706c 6529 293a 2064 696d 203d 2064 696d  ple)): dim = dim
+00007d20: 5b30 5d0a 2020 2020 2020 2020 7365 6c66  [0].        self
+00007d30: 2e64 696d 7320 3d20 6469 6d0a 2020 2020  .dims = dim.    
+00007d40: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00007d50: 6528 696d 6167 655f 7369 7a65 2c20 6274  e(image_size, bt
+00007d60: 2e74 6f72 6368 2e54 656e 736f 7229 3a20  .torch.Tensor): 
+00007d70: 696d 6167 655f 7369 7a65 203d 2069 6d61  image_size = ima
+00007d80: 6765 5f73 697a 652e 7368 6170 650a 2020  ge_size.shape.  
+00007d90: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
+00007da0: 5f73 697a 6520 3d20 696d 6167 655f 7369  _size = image_si
+00007db0: 7a65 0a20 2020 2020 2020 2069 6620 696d  ze.        if im
+00007dc0: 6167 655f 7369 7a65 2069 7320 6e6f 7420  age_size is not 
+00007dd0: 4e6f 6e65 3a20 7365 6c66 2e6e 5f64 696d  None: self.n_dim
+00007de0: 203d 206c 656e 2869 6d61 6765 5f73 697a   = len(image_siz
+00007df0: 6529 0a0a 2020 2020 6465 6620 5f5f 6361  e)..    def __ca
+00007e00: 6c6c 5f5f 2873 656c 662c 2058 293a 0a20  ll__(self, X):. 
+00007e10: 2020 2020 2020 2058 203d 2073 7570 6572         X = super
+00007e20: 2829 2e5f 5f63 616c 6c5f 5f28 5829 0a20  ().__call__(X). 
+00007e30: 2020 2020 2020 2064 696d 7320 3d20 7365         dims = se
+00007e40: 6c66 2e64 696d 730a 2020 2020 2020 2020  lf.dims.        
+00007e50: 666f 7220 6469 6d20 696e 2064 696d 733a  for dim in dims:
+00007e60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007e70: 6563 7420 3d20 2873 6c69 6365 284e 6f6e  ect = (slice(Non
+00007e80: 6529 2c29 202a 2058 2e63 6861 6e6e 656c  e),) * X.channel
+00007e90: 5f64 696d 202b 2028 6469 6d2c 290a 2020  _dim + (dim,).  
+00007ea0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00007eb0: 662e 696d 6167 655f 7369 7a65 2069 7320  f.image_size is 
+00007ec0: 4e6f 6e65 3a20 6d61 785f 7261 6e67 6520  None: max_range 
+00007ed0: 3d20 585b 7365 6c65 6374 5d2e 6d61 7828  = X[select].max(
+00007ee0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00007ef0: 7365 3a20 6d61 785f 7261 6e67 6520 3d20  se: max_range = 
+00007f00: 7365 6c66 2e69 6d61 6765 5f73 697a 655b  self.image_size[
+00007f10: 6469 6d5d 0a20 2020 2020 2020 2020 2020  dim].           
+00007f20: 2058 5b73 656c 6563 745d 203d 206d 6178   X[select] = max
+00007f30: 5f72 616e 6765 202d 2058 5b73 656c 6563  _range - X[selec
+00007f40: 745d 0a20 2020 2020 2020 2072 6574 7572  t].        retur
+00007f50: 6e20 580a 2020 2020 2020 2020 0a20 2020  n X.        .   
+00007f60: 2064 6566 2061 6666 696e 6528 7365 6c66   def affine(self
+00007f70: 2c20 6e5f 6469 6d3d 4e6f 6e65 293a 0a20  , n_dim=None):. 
+00007f80: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00007f90: 6d61 6765 5f73 697a 6520 6973 204e 6f6e  mage_size is Non
+00007fa0: 653a 2072 6574 7572 6e0a 2020 2020 2020  e: return.      
+00007fb0: 2020 6966 206e 5f64 696d 2069 7320 4e6f    if n_dim is No
+00007fc0: 6e65 2061 6e64 2073 656c 662e 6e5f 6469  ne and self.n_di
+00007fd0: 6d20 6973 204e 6f6e 653a 2072 6574 7572  m is None: retur
+00007fe0: 6e0a 2020 2020 2020 2020 6966 206e 5f64  n.        if n_d
+00007ff0: 696d 2069 7320 4e6f 6e65 3a20 6e5f 6469  im is None: n_di
+00008000: 6d20 3d20 7365 6c66 2e6e 5f64 696d 0a20  m = self.n_dim. 
+00008010: 2020 2020 2020 2061 766f 7563 6828 7365         avouch(se
+00008020: 6c66 2e6e 5f64 696d 2069 7320 4e6f 6e65  lf.n_dim is None
+00008030: 206f 7220 7365 6c66 2e6e 5f64 696d 203d   or self.n_dim =
+00008040: 3d20 6e5f 6469 6d29 0a20 2020 2020 2020  = n_dim).       
+00008050: 2061 6666 203d 2062 742e 6579 6528 6e5f   aff = bt.eye(n_
+00008060: 6469 6d20 2b20 3129 0a20 2020 2020 2020  dim + 1).       
+00008070: 2066 6f72 2064 696d 2069 6e20 7365 6c66   for dim in self
+00008080: 2e64 696d 733a 0a20 2020 2020 2020 2020  .dims:.         
+00008090: 2020 2061 6666 5b64 696d 5d5b 6469 6d5d     aff[dim][dim]
+000080a0: 203d 202d 312e 0a20 2020 2020 2020 2020   = -1..         
+000080b0: 2020 2061 6666 5b64 696d 5d5b 2d31 5d20     aff[dim][-1] 
+000080c0: 3d20 666c 6f61 7428 7365 6c66 2e69 6d61  = float(self.ima
+000080d0: 6765 5f73 697a 655b 6469 6d5d 290a 2020  ge_size[dim]).  
+000080e0: 2020 2020 2020 7265 7475 726e 2061 6666        return aff
+000080f0: 2e75 6e73 7175 6565 7a65 285b 5d29 0a0a  .unsqueeze([])..
+00008100: 2020 2020 6465 6620 696e 7628 7365 6c66      def inv(self
+00008110: 293a 2072 6574 7572 6e20 5265 666c 6563  ): return Reflec
+00008120: 7428 2a73 656c 662e 6469 6d73 2c20 696d  t(*self.dims, im
+00008130: 6167 655f 7369 7a65 203d 2073 656c 662e  age_size = self.
+00008140: 696d 6167 655f 7369 7a65 292e 6261 636b  image_size).back
+00008150: 7761 7264 5f28 7365 6c66 2e62 6163 6b77  ward_(self.backw
+00008160: 6172 6429 0a0a 4061 6c69 6173 2822 5065  ard)..@alias("Pe
+00008170: 726d 7574 6564 696d 2229 0a63 6c61 7373  rmutedim").class
+00008180: 2044 696d 5065 726d 7574 6174 696f 6e28   DimPermutation(
+00008190: 5370 6174 6961 6c54 7261 6e73 666f 726d  SpatialTransform
+000081a0: 6174 696f 6e29 3a0a 2020 2020 6465 6620  ation):.    def 
+000081b0: 5f5f 696e 6974 5f5f 2873 656c 662c 202a  __init__(self, *
+000081c0: 6469 6d73 2c20 7265 7369 7a65 5f69 6d61  dims, resize_ima
+000081d0: 6765 3d54 7275 6529 3a0a 2020 2020 2020  ge=True):.      
+000081e0: 2020 2727 270a 2020 2020 2020 2020 5065    '''.        Pe
+000081f0: 726d 7574 6520 7468 6520 6469 6d65 6e73  rmute the dimens
+00008200: 696f 6e73 2066 6f72 2061 6e20 696d 6167  ions for an imag
+00008210: 652c 2073 696d 696c 6172 2074 6f20 6e70  e, similar to np
+00008220: 2e74 7261 6e73 706f 7365 206f 7220 746f  .transpose or to
+00008230: 7263 682f 6261 746f 7263 682e 7065 726d  rch/batorch.perm
+00008240: 7574 652e 0a20 2020 2020 2020 200a 2020  ute..        .  
+00008250: 2020 2020 2020 5061 7261 6d73 3a0a 2020        Params:.  
+00008260: 2020 2020 2020 2020 2020 6469 6d73 205b            dims [
+00008270: 6c69 7374 206f 7220 7475 706c 6520 6f72  list or tuple or
+00008280: 2062 742e 5465 6e73 6f72 5d3a 2054 6865   bt.Tensor]: The
+00008290: 2064 696d 656e 7369 6f6e 2070 6572 6d75   dimension permu
+000082a0: 6174 696f 6e2e 200a 2020 2020 2020 2020  ation. .        
+000082b0: 2020 2020 2020 2020 7369 7a65 3a20 6c65          size: le
+000082c0: 6e67 7468 286e 5f64 696d 2920 6f72 2028  ngth(n_dim) or (
+000082d0: 5b6e 5f62 6174 6368 3a6f 7074 696f 6e61  [n_batch:optiona
+000082e0: 6c5d 2c20 7b6e 5f64 696d 7d29 2e0a 0a20  l], {n_dim})... 
+000082f0: 2020 2020 2020 2057 6865 6e20 6974 2069         When it i
+00008300: 7320 6361 6c6c 6564 3a0a 2020 2020 2020  s called:.      
+00008310: 2020 2020 2020 5820 5b62 742e 5465 6e73        X [bt.Tens
+00008320: 6f72 5d3a 2043 6f6f 7264 696e 6174 6573  or]: Coordinates
+00008330: 2074 6f20 6265 2074 7261 6e73 666f 726d   to be transform
+00008340: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00008350: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+00008360: 7463 683a 6f70 7469 6f6e 616c 5d2c 207b  tch:optional], {
+00008370: 6e5f 6469 6d7d 2c20 6e5f 312c 206e 5f32  n_dim}, n_1, n_2
+00008380: 2c20 2e2e 2e2c 206e 5f72 290a 2020 2020  , ..., n_r).    
+00008390: 2020 2020 2020 2020 6f75 7470 7574 205b          output [
+000083a0: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
+000083b0: 7472 616e 7366 6f72 6d65 6420 636f 6f72  transformed coor
+000083c0: 6469 6e61 7465 732e 0a20 2020 2020 2020  dinates..       
+000083d0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
+000083e0: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
+000083f0: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
+00008400: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
+00008410: 2727 270a 2020 2020 2020 2020 6966 206c  '''.        if l
+00008420: 656e 2864 696d 7329 203d 3d20 313a 2064  en(dims) == 1: d
+00008430: 696d 7320 3d20 6469 6d73 5b30 5d0a 2020  ims = dims[0].  
+00008440: 2020 2020 2020 6469 6d73 203d 2062 6174        dims = bat
+00008450: 6f72 6368 5f74 656e 736f 7228 6c69 7374  orch_tensor(list
+00008460: 2864 696d 7329 292e 7371 7565 657a 6528  (dims)).squeeze(
+00008470: 290a 2020 2020 2020 2020 6469 6d73 203d  ).        dims =
+00008480: 2064 696d 732e 6c6f 6e67 2829 0a20 2020   dims.long().   
+00008490: 2020 2020 2069 6620 6469 6d73 2e6e 5f64       if dims.n_d
+000084a0: 696d 203c 3d20 313a 2064 696d 7320 3d20  im <= 1: dims = 
+000084b0: 6469 6d73 2e75 6e73 7175 6565 7a65 285b  dims.unsqueeze([
+000084c0: 5d29 0a20 2020 2020 2020 2069 6620 6469  ]).        if di
+000084d0: 6d73 2e6e 5f64 696d 203d 3d20 323a 0a20  ms.n_dim == 2:. 
+000084e0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000084f0: 7420 6469 6d73 2e68 6173 5f62 6174 6368  t dims.has_batch
+00008500: 3a20 6469 6d73 2e62 6174 6368 5f64 696d  : dims.batch_dim
+00008510: 656e 7369 6f6e 203d 2030 0a20 2020 2020  ension = 0.     
+00008520: 2020 2020 2020 2069 6620 6e6f 7420 6469         if not di
+00008530: 6d73 2e68 6173 5f63 6861 6e6e 656c 3a20  ms.has_channel: 
+00008540: 6469 6d73 2e63 6861 6e6e 656c 5f64 696d  dims.channel_dim
+00008550: 656e 7369 6f6e 203d 2030 2069 6620 6469  ension = 0 if di
+00008560: 6d73 2e62 6174 6368 5f64 696d 656e 7369  ms.batch_dimensi
+00008570: 6f6e 203e 2030 2065 6c73 6520 310a 2020  on > 0 else 1.  
+00008580: 2020 2020 2020 6176 6f75 6368 2864 696d        avouch(dim
+00008590: 732e 6861 735f 6261 7463 6820 616e 6420  s.has_batch and 
+000085a0: 6469 6d73 2e68 6173 5f63 6861 6e6e 656c  dims.has_channel
+000085b0: 2c20 6622 506c 6561 7365 2075 7365 2062  , f"Please use b
+000085c0: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
+000085d0: 2073 697a 6520 5c0a 2020 2020 2020 2020   size \.        
+000085e0: 2020 2020 285b 6e5f 6261 7463 683a 6f70      ([n_batch:op
+000085f0: 7469 6f6e 616c 5d2c 207b 7b6e 5f64 696d  tional], {{n_dim
+00008600: 7d7d 2920 666f 7220 5472 616e 736c 6174  }}) for Translat
+00008610: 696f 6e20 7061 7261 6d65 7465 7273 2c20  ion parameters, 
+00008620: 696e 7374 6561 6420 6f66 207b 6469 6d73  instead of {dims
+00008630: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+00008640: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00008650: 6974 5f5f 2864 696d 732c 2072 6573 697a  it__(dims, resiz
+00008660: 655f 696d 6167 653d 7265 7369 7a65 5f69  e_image=resize_i
+00008670: 6d61 6765 290a 0a20 2020 2020 2020 2073  mage)..        s
+00008680: 656c 662e 6469 6d73 203d 2064 696d 730a  elf.dims = dims.
+00008690: 2020 2020 2020 2020 7365 6c66 2e6e 5f64          self.n_d
+000086a0: 696d 203d 2064 696d 732e 6e5f 6368 616e  im = dims.n_chan
+000086b0: 6e65 6c0a 2020 2020 2020 2020 7365 6c66  nel.        self
+000086c0: 2e72 6573 697a 655f 696d 6167 6520 3d20  .resize_image = 
+000086d0: 7265 7369 7a65 5f69 6d61 6765 0a20 2020  resize_image.   
+000086e0: 2020 2020 2069 6620 7265 7369 7a65 5f69       if resize_i
+000086f0: 6d61 6765 3a0a 2020 2020 2020 2020 2020  mage:.          
+00008700: 2020 6966 2064 696d 732e 6e5f 6261 7463    if dims.n_batc
+00008710: 6820 3e20 313a 0a20 2020 2020 2020 2020  h > 1:.         
+00008720: 2020 2020 2020 2064 696d 735f 6361 7020         dims_cap 
+00008730: 3d20 6469 6d73 2e73 616d 706c 6528 7261  = dims.sample(ra
+00008740: 6e64 6f6d 3d46 616c 7365 2c20 6469 6d3d  ndom=False, dim=
+00008750: 5b5d 290a 2020 2020 2020 2020 2020 2020  []).            
+00008760: 2020 2020 6176 6f75 6368 2862 742e 6e6f      avouch(bt.no
+00008770: 726d 2864 696d 7320 2d20 6469 6d73 5f63  rm(dims - dims_c
+00008780: 6170 292e 7375 6d28 2920 3c20 3165 2d34  ap).sum() < 1e-4
+00008790: 2c20 2243 616e 6e6f 7420 7265 7369 7a65  , "Cannot resize
+000087a0: 2069 6d61 6765 2077 6865 6e20 6469 6666   image when diff
+000087b0: 6572 656e 7420 7065 726d 7574 6174 696f  erent permutatio
+000087c0: 6e20 646f 6e65 2066 6f72 2064 6966 6665  n done for diffe
+000087d0: 7265 6e74 2062 6174 6368 206d 656d 6265  rent batch membe
+000087e0: 7273 2e20 2229 0a20 2020 2020 2020 2020  rs. ").         
+000087f0: 2020 2064 696d 7320 3d20 6469 6d73 2e70     dims = dims.p
+00008800: 6963 6b28 302c 205b 5d29 2e74 6f6c 6973  ick(0, []).tolis
+00008810: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00008820: 7669 7369 7465 6420 3d20 5b5d 0a20 2020  visited = [].   
+00008830: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00008840: 7368 6170 6520 3d20 5b28 312c 295d 0a20  shape = [(1,)]. 
+00008850: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+00008860: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
+00008870: 5f64 696d 293a 0a20 2020 2020 2020 2020  _dim):.         
+00008880: 2020 2020 2020 2069 6620 7020 696e 2076         if p in v
+00008890: 6973 6974 6564 3a20 636f 6e74 696e 7565  isited: continue
+000088a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000088b0: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088d0: 2076 6973 6974 6564 2e61 7070 656e 6428   visited.append(
+000088e0: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
+000088f0: 2020 2020 2020 2071 203d 2064 696d 735b         q = dims[
+00008900: 705d 0a20 2020 2020 2020 2020 2020 2020  p].             
+00008910: 2020 2020 2020 2069 6620 7120 696e 2076         if q in v
+00008920: 6973 6974 6564 3a20 6272 6561 6b0a 2020  isited: break.  
+00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008940: 2020 7365 6c66 2e72 6573 6861 7065 2e61    self.reshape.a
+00008950: 7070 656e 6428 2870 2c20 7129 290a 2020  ppend((p, q)).  
+00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008970: 2020 7020 3d20 710a 0a20 2020 2064 6566    p = q..    def
+00008980: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
+00008990: 5829 3a0a 2020 2020 2020 2020 5820 3d20  X):.        X = 
+000089a0: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
+000089b0: 2858 290a 2020 2020 2020 2020 7265 7475  (X).        retu
+000089c0: 726e 2058 2e67 6174 6865 7228 582e 6368  rn X.gather(X.ch
+000089d0: 616e 6e65 6c5f 6469 6d65 6e73 696f 6e2c  annel_dimension,
+000089e0: 2073 656c 662e 6469 6d73 2e65 7870 616e   self.dims.expan
+000089f0: 645f 746f 2858 2929 0a20 2020 2020 2020  d_to(X)).       
+00008a00: 200a 2020 2020 6465 6620 6166 6669 6e65   .    def affine
+00008a10: 2873 656c 662c 206e 5f64 696d 3d4e 6f6e  (self, n_dim=Non
+00008a20: 6529 3a0a 2020 2020 2020 2020 6176 6f75  e):.        avou
+00008a30: 6368 286e 5f64 696d 2069 7320 4e6f 6e65  ch(n_dim is None
+00008a40: 206f 7220 7365 6c66 2e6e 5f64 696d 203d   or self.n_dim =
+00008a50: 3d20 6e5f 6469 6d29 0a20 2020 2020 2020  = n_dim).       
+00008a60: 2069 6620 6e5f 6469 6d20 6973 204e 6f6e   if n_dim is Non
+00008a70: 653a 206e 5f64 696d 203d 2073 656c 662e  e: n_dim = self.
+00008a80: 6e5f 6469 6d0a 2020 2020 2020 2020 6e5f  n_dim.        n_
+00008a90: 6261 7463 6820 3d20 7365 6c66 2e6e 5f62  batch = self.n_b
+00008aa0: 6174 6368 0a20 2020 2020 2020 2069 6620  atch.        if 
+00008ab0: 6e5f 6261 7463 6820 6973 204e 6f6e 653a  n_batch is None:
+00008ac0: 206e 5f62 6174 6368 203d 2031 0a20 2020   n_batch = 1.   
+00008ad0: 2020 2020 2061 6666 203d 2062 742e 6469       aff = bt.di
+00008ae0: 6167 2862 742e 6f6e 655f 686f 7428 2d31  ag(bt.one_hot(-1
+00008af0: 2c20 6e5f 6469 6d20 2b20 3129 2e66 6c6f  , n_dim + 1).flo
+00008b00: 6174 2829 2e6d 756c 7469 706c 7928 6e5f  at().multiply(n_
+00008b10: 6261 7463 682c 205b 5d29 290a 2020 2020  batch, [])).    
+00008b20: 2020 2020 6220 3d20 6274 2e62 6174 6368      b = bt.batch
+00008b30: 5f74 656e 736f 7228 6274 2e61 7261 6e67  _tensor(bt.arang
+00008b40: 6528 6e5f 6261 7463 6829 292e 6578 7061  e(n_batch)).expa
+00008b50: 6e64 5f74 6f28 7365 6c66 2e64 696d 7329  nd_to(self.dims)
+00008b60: 0a20 2020 2020 2020 2069 203d 2062 742e  .        i = bt.
+00008b70: 6172 616e 6765 286e 5f64 696d 292e 6d75  arange(n_dim).mu
+00008b80: 6c74 6970 6c79 286e 5f62 6174 6368 2c20  ltiply(n_batch, 
+00008b90: 5b5d 290a 2020 2020 2020 2020 6166 665b  []).        aff[
+00008ba0: 622c 2069 2c20 7365 6c66 2e64 696d 735d  b, i, self.dims]
+00008bb0: 203d 2031 2e0a 2020 2020 2020 2020 7265   = 1..        re
+00008bc0: 7475 726e 2061 6666 0a0a 2020 2020 6465  turn aff..    de
+00008bd0: 6620 696e 7628 7365 6c66 293a 0a20 2020  f inv(self):.   
+00008be0: 2020 2020 206e 5f64 696d 203d 2073 656c       n_dim = sel
+00008bf0: 662e 6e5f 6469 6d0a 2020 2020 2020 2020  f.n_dim.        
+00008c00: 6e65 775f 7065 726d 7574 6520 3d20 2873  new_permute = (s
+00008c10: 656c 662e 6469 6d73 203d 3d20 6274 2e61  elf.dims == bt.a
+00008c20: 7261 6e67 6528 6e5f 6469 6d29 2e76 6965  range(n_dim).vie
+00008c30: 7728 5b31 5d2c 206e 5f64 696d 2c20 7b31  w([1], n_dim, {1
+00008c40: 7d29 292e 666c 6f61 7428 292e 6172 676d  })).float().argm
+00008c50: 6178 282d 3129 2e63 6861 6e6e 656c 5f64  ax(-1).channel_d
+00008c60: 696d 656e 7369 6f6e 5f28 2d31 290a 2020  imension_(-1).  
+00008c70: 2020 2020 2020 7265 7475 726e 2050 6572        return Per
+00008c80: 6d75 7465 6469 6d28 6e65 775f 7065 726d  mutedim(new_perm
+00008c90: 7574 652c 2072 6573 697a 655f 696d 6167  ute, resize_imag
+00008ca0: 6520 3d20 7365 6c66 2e72 6573 697a 655f  e = self.resize_
+00008cb0: 696d 6167 6529 2e62 6163 6b77 6172 645f  image).backward_
+00008cc0: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
+00008cd0: 0a40 616c 6961 7328 2252 6573 6361 6c65  .@alias("Rescale
+00008ce0: 2229 0a63 6c61 7373 2052 6573 6361 6c69  ").class Rescali
+00008cf0: 6e67 2853 7061 7469 616c 5472 616e 7366  ng(SpatialTransf
+00008d00: 6f72 6d61 7469 6f6e 293a 0a20 2020 2064  ormation):.    d
+00008d10: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00008d20: 2c20 2a73 6361 6c65 2c20 7265 7369 7a65  , *scale, resize
+00008d30: 5f69 6d61 6765 3d54 7275 6529 3a0a 2020  _image=True):.  
+00008d40: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00008d50: 2020 5363 616c 6520 616e 2069 6d61 6765    Scale an image
+00008d60: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00008d70: 2020 204e 6f74 653a 2054 6865 2073 6361     Note: The sca
+00008d80: 6c69 6e67 2069 7320 666f 7220 636f 6f72  ling is for coor
+00008d90: 6469 6e61 7465 732c 2068 656e 6365 2074  dinates, hence t
+00008da0: 6865 2069 6d61 6765 2077 6f75 6c64 2073  he image would s
+00008db0: 6872 696e 6b20 6966 2073 6361 6c65 203e  hrink if scale >
+00008dc0: 2031 2e20 0a20 2020 2020 2020 200a 2020   1. .        .  
+00008dd0: 2020 2020 2020 5061 7261 6d73 3a0a 2020        Params:.  
+00008de0: 2020 2020 2020 2020 2020 7363 616c 6520            scale 
+00008df0: 5b66 6c6f 6174 206f 7220 7475 706c 6520  [float or tuple 
+00008e00: 6f72 2062 742e 5465 6e73 6f72 5d3a 2054  or bt.Tensor]: T
+00008e10: 6865 2073 6361 6c69 6e67 2066 6f72 2061  he scaling for a
+00008e20: 6c6c 2064 696d 656e 7369 6f6e 7320 2866  ll dimensions (f
+00008e30: 6c6f 6174 2920 0a20 2020 2020 2020 2020  loat) .         
+00008e40: 2020 2020 2020 206f 7220 666f 7220 6561         or for ea
+00008e50: 6368 2064 696d 656e 7369 6f6e 2028 7475  ch dimension (tu
+00008e60: 706c 6529 2e20 3e31 206d 6561 6e73 2065  ple). >1 means e
+00008e70: 6e6c 6172 6769 6e67 2074 6865 2063 6f6f  nlarging the coo
+00008e80: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
+00008e90: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00008ea0: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
+00008eb0: 616c 5d2c 207b 6e5f 6469 6d7d 2920 666f  al], {n_dim}) fo
+00008ec0: 7220 6274 2e54 656e 736f 722e 0a20 2020  r bt.Tensor..   
+00008ed0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00008ee0: 2020 5768 656e 2069 7420 6973 2063 616c    When it is cal
+00008ef0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
+00008f00: 2058 205b 6274 2e54 656e 736f 725d 3a20   X [bt.Tensor]: 
+00008f10: 436f 6f72 6469 6e61 7465 7320 746f 2062  Coordinates to b
+00008f20: 6520 7472 616e 7366 6f72 6d65 642e 0a20  e transformed.. 
+00008f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008f40: 697a 653a 2028 5b6e 5f62 6174 6368 3a6f  ize: ([n_batch:o
+00008f50: 7074 696f 6e61 6c5d 2c20 7b6e 5f64 696d  ptional], {n_dim
+00008f60: 7d2c 206e 5f31 2c20 6e5f 322c 202e 2e2e  }, n_1, n_2, ...
+00008f70: 2c20 6e5f 7229 0a20 2020 2020 2020 2020  , n_r).         
+00008f80: 2020 206f 7574 7075 7420 5b62 742e 5465     output [bt.Te
+00008f90: 6e73 6f72 5d3a 2054 6865 2074 7261 6e73  nsor]: The trans
+00008fa0: 666f 726d 6564 2063 6f6f 7264 696e 6174  formed coordinat
+00008fb0: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+00008fc0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+00008fd0: 7463 685d 2c20 7b6e 5f64 696d 7d2c 206e  tch], {n_dim}, n
+00008fe0: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
+00008ff0: 7229 0a20 2020 2020 2020 2027 2727 0a20  r).        '''. 
+00009000: 2020 2020 2020 2069 6620 6c65 6e28 7363         if len(sc
+00009010: 616c 6529 203d 3d20 3120 616e 6420 6973  ale) == 1 and is
+00009020: 696e 7374 616e 6365 2873 6361 6c65 5b30  instance(scale[0
+00009030: 5d2c 2028 696e 742c 2066 6c6f 6174 2929  ], (int, float))
+00009040: 3a20 7363 616c 6520 3d20 7363 616c 655b  : scale = scale[
+00009050: 305d 202a 2062 742e 6f6e 6573 285b 315d  0] * bt.ones([1]
+00009060: 2c20 7b31 7d29 0a20 2020 2020 2020 2065  , {1}).        e
+00009070: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00009080: 2069 6620 6c65 6e28 7363 616c 6529 203d   if len(scale) =
+00009090: 3d20 313a 2073 6361 6c65 203d 2073 6361  = 1: scale = sca
+000090a0: 6c65 5b30 5d0a 2020 2020 2020 2020 2020  le[0].          
+000090b0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+000090c0: 6e63 6528 7363 616c 652c 2062 742e 5465  nce(scale, bt.Te
+000090d0: 6e73 6f72 293a 2073 6361 6c65 203d 2062  nsor): scale = b
+000090e0: 6174 6f72 6368 5f74 656e 736f 7228 6c69  atorch_tensor(li
+000090f0: 7374 2873 6361 6c65 2929 2e73 7175 6565  st(scale)).squee
+00009100: 7a65 2829 0a20 2020 2020 2020 2020 2020  ze().           
+00009110: 2069 6620 7363 616c 652e 6e5f 6469 6d20   if scale.n_dim 
+00009120: 3c3d 2031 3a20 7363 616c 6520 3d20 7363  <= 1: scale = sc
+00009130: 616c 652e 756e 7371 7565 657a 6528 5b5d  ale.unsqueeze([]
+00009140: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00009150: 2073 6361 6c65 2e6e 5f64 696d 203d 3d20   scale.n_dim == 
+00009160: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+00009170: 2020 2069 6620 6e6f 7420 7363 616c 652e     if not scale.
+00009180: 6861 735f 6261 7463 683a 2073 6361 6c65  has_batch: scale
+00009190: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+000091a0: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
+000091b0: 2020 2020 2069 6620 6e6f 7420 7363 616c       if not scal
+000091c0: 652e 6861 735f 6368 616e 6e65 6c3a 2073  e.has_channel: s
+000091d0: 6361 6c65 2e63 6861 6e6e 656c 5f64 696d  cale.channel_dim
+000091e0: 656e 7369 6f6e 203d 2030 2069 6620 7363  ension = 0 if sc
+000091f0: 616c 652e 6261 7463 685f 6469 6d65 6e73  ale.batch_dimens
+00009200: 696f 6e20 3e20 3020 656c 7365 2031 0a20  ion > 0 else 1. 
+00009210: 2020 2020 2020 2061 766f 7563 6828 7363         avouch(sc
+00009220: 616c 652e 6861 735f 6261 7463 6820 616e  ale.has_batch an
+00009230: 6420 7363 616c 652e 6861 735f 6368 616e  d scale.has_chan
+00009240: 6e65 6c2c 2066 2250 6c65 6173 6520 7573  nel, f"Please us
+00009250: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
+00009260: 206f 6620 7369 7a65 205c 0a20 2020 2020   of size \.     
+00009270: 2020 2020 2020 2028 5b6e 5f62 6174 6368         ([n_batch
+00009280: 3a6f 7074 696f 6e61 6c5d 2c20 7b7b 6e5f  :optional], {{n_
+00009290: 6469 6d7d 7d29 2066 6f72 2053 6361 6c69  dim}}) for Scali
+000092a0: 6e67 2070 6172 616d 6574 6572 732c 2069  ng parameters, i
+000092b0: 6e73 7465 6164 206f 6620 7b73 6361 6c65  nstead of {scale
+000092c0: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+000092d0: 2020 2020 6274 2e74 6f5f 6465 7669 6365      bt.to_device
+000092e0: 2873 6361 6c65 290a 2020 2020 2020 2020  (scale).        
+000092f0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00009300: 2873 6361 6c65 2c20 7265 7369 7a65 5f69  (scale, resize_i
+00009310: 6d61 6765 3d72 6573 697a 655f 696d 6167  mage=resize_imag
+00009320: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00009330: 2e73 6361 6c65 203d 2073 6361 6c65 0a20  .scale = scale. 
+00009340: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00009350: 6361 6c65 2e6e 5f63 6861 6e6e 656c 203e  cale.n_channel >
+00009360: 2031 3a20 7365 6c66 2e6e 5f64 696d 203d   1: self.n_dim =
+00009370: 2073 656c 662e 7363 616c 652e 6e5f 6368   self.scale.n_ch
+00009380: 616e 6e65 6c0a 2020 2020 2020 2020 6966  annel.        if
+00009390: 2072 6573 697a 655f 696d 6167 653a 0a20   resize_image:. 
+000093a0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+000093b0: 203d 2073 6361 6c65 2e73 7175 6565 7a65   = scale.squeeze
+000093c0: 285b 5d29 0a20 2020 2020 2020 2020 2020  ([]).           
+000093d0: 2061 766f 7563 6828 7363 616c 652e 6e64   avouch(scale.nd
+000093e0: 696d 203d 3d20 3129 0a20 2020 2020 2020  im == 1).       
+000093f0: 2020 2020 2073 656c 662e 7265 7368 6170       self.reshap
+00009400: 6520 3d20 5b74 7570 6c65 2828 312f 7363  e = [tuple((1/sc
+00009410: 616c 6529 2e74 6f6c 6973 7428 2929 5d0a  ale).tolist())].
+00009420: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+00009430: 697a 655f 696d 6167 6520 3d20 7265 7369  ize_image = resi
+00009440: 7a65 5f69 6d61 6765 0a20 2020 2020 2020  ze_image.       
+00009450: 2073 656c 662e 6261 7463 685f 7061 7261   self.batch_para
+00009460: 6d2e 6170 7065 6e64 2827 7363 616c 6527  m.append('scale'
+00009470: 290a 0a20 2020 2064 6566 205f 5f63 616c  )..    def __cal
+00009480: 6c5f 5f28 7365 6c66 2c20 5829 3a0a 2020  l__(self, X):.  
+00009490: 2020 2020 2020 5820 3d20 7375 7065 7228        X = super(
+000094a0: 292e 5f5f 6361 6c6c 5f5f 2858 290a 2020  ).__call__(X).  
+000094b0: 2020 2020 2020 7363 616c 6520 3d20 7365        scale = se
+000094c0: 6c66 2e73 6361 6c65 0a20 2020 2020 2020  lf.scale.       
+000094d0: 2072 6574 7572 6e20 5820 2a20 7363 616c   return X * scal
+000094e0: 650a 2020 2020 0a20 2020 2064 6566 2061  e.    .    def a
+000094f0: 6666 696e 6528 7365 6c66 2c20 6e5f 6469  ffine(self, n_di
+00009500: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00009510: 2069 6620 6e5f 6469 6d20 6973 204e 6f6e   if n_dim is Non
+00009520: 6520 616e 6420 7365 6c66 2e6e 5f64 696d  e and self.n_dim
+00009530: 2069 7320 4e6f 6e65 3a20 7265 7475 726e   is None: return
+00009540: 0a20 2020 2020 2020 2069 6620 6e5f 6469  .        if n_di
+00009550: 6d20 6973 204e 6f6e 653a 206e 5f64 696d  m is None: n_dim
+00009560: 203d 2073 656c 662e 6e5f 6469 6d0a 2020   = self.n_dim.  
+00009570: 2020 2020 2020 6176 6f75 6368 2873 656c        avouch(sel
+00009580: 662e 6e5f 6469 6d20 6973 204e 6f6e 6520  f.n_dim is None 
+00009590: 6f72 2073 656c 662e 6e5f 6469 6d20 3d3d  or self.n_dim ==
+000095a0: 206e 5f64 696d 290a 2020 2020 2020 2020   n_dim).        
+000095b0: 7363 616c 6520 3d20 7365 6c66 2e73 6361  scale = self.sca
+000095c0: 6c65 0a20 2020 2020 2020 2069 6620 6973  le.        if is
+000095d0: 696e 7374 616e 6365 2873 6361 6c65 2c20  instance(scale, 
+000095e0: 2869 6e74 2c20 666c 6f61 7429 293a 2072  (int, float)): r
+000095f0: 6574 7572 6e20 7363 616c 6520 2a20 6274  eturn scale * bt
+00009600: 2e65 7965 286e 5f64 696d 202b 2031 290a  .eye(n_dim + 1).
+00009610: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00009620: 742e 6469 6167 2862 742e 6361 7428 7363  t.diag(bt.cat(sc
+00009630: 616c 652c 2062 742e 6f6e 6573 285b 7363  ale, bt.ones([sc
+00009640: 616c 652e 6e5f 6261 7463 685d 2c20 3129  ale.n_batch], 1)
+00009650: 2c20 3129 290a 0a20 2020 2064 6566 2069  , 1))..    def i
+00009660: 6e76 2873 656c 6629 3a20 7265 7475 726e  nv(self): return
+00009670: 2052 6573 6361 6c65 2831 2f73 656c 662e   Rescale(1/self.
+00009680: 7363 616c 652c 2072 6573 697a 655f 696d  scale, resize_im
+00009690: 6167 6520 3d20 7365 6c66 2e72 6573 697a  age = self.resiz
+000096a0: 655f 696d 6167 6529 2e62 6163 6b77 6172  e_image).backwar
+000096b0: 645f 2873 656c 662e 6261 636b 7761 7264  d_(self.backward
+000096c0: 290a 0a40 616c 6961 7328 2254 7261 6e73  )..@alias("Trans
+000096d0: 6c61 7465 2229 0a63 6c61 7373 2054 7261  late").class Tra
+000096e0: 6e73 6c61 7469 6f6e 2853 7061 7469 616c  nslation(Spatial
+000096f0: 5472 616e 7366 6f72 6d61 7469 6f6e 293a  Transformation):
+00009700: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00009710: 5f28 7365 6c66 2c20 2a74 7261 6e73 6c61  _(self, *transla
+00009720: 7469 6f6e 293a 0a20 2020 2020 2020 2027  tion):.        '
+00009730: 2727 0a20 2020 2020 2020 2054 7261 6e73  ''.        Trans
+00009740: 6c61 7465 2061 6e20 696d 6167 652e 0a20  late an image.. 
+00009750: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00009760: 4e6f 7465 3a20 5468 6520 7472 616e 736c  Note: The transl
+00009770: 6174 696f 6e20 6973 2066 6f72 2063 6f6f  ation is for coo
+00009780: 7264 696e 6174 6573 2c20 6865 6e63 6520  rdinates, hence 
+00009790: 7468 6520 696d 6167 6520 776f 756c 6420  the image would 
+000097a0: 676f 2069 6e20 7468 6520 6f70 706f 7369  go in the opposi
+000097b0: 7465 2064 6972 6563 7469 6f6e 2e20 0a20  te direction. . 
+000097c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000097d0: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
+000097e0: 2020 2020 7472 616e 736c 6174 696f 6e20      translation 
+000097f0: 5b74 7570 6c65 206f 7220 6274 2e54 656e  [tuple or bt.Ten
+00009800: 736f 725d 3a20 5468 6520 7472 616e 736c  sor]: The transl
+00009810: 6174 696f 6e20 6f66 2074 6865 2063 6f6f  ation of the coo
+00009820: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
+00009830: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00009840: 6c65 6e67 7468 286e 5f64 696d 2920 6f72  length(n_dim) or
+00009850: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
+00009860: 6e61 6c5d 2c20 7b6e 5f64 696d 7d29 0a20  nal], {n_dim}). 
+00009870: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00009880: 2020 2020 5768 656e 2069 7420 6973 2063      When it is c
+00009890: 616c 6c65 643a 0a20 2020 2020 2020 2020  alled:.         
+000098a0: 2020 2058 205b 6274 2e54 656e 736f 725d     X [bt.Tensor]
+000098b0: 3a20 436f 6f72 6469 6e61 7465 7320 746f  : Coordinates to
+000098c0: 2062 6520 7472 616e 7366 6f72 6d65 642e   be transformed.
+000098d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000098e0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+000098f0: 3a6f 7074 696f 6e61 6c5d 2c20 7b6e 5f64  :optional], {n_d
+00009900: 696d 7d2c 206e 5f31 2c20 6e5f 322c 202e  im}, n_1, n_2, .
+00009910: 2e2e 2c20 6e5f 7229 0a20 2020 2020 2020  .., n_r).       
+00009920: 2020 2020 206f 7574 7075 7420 5b62 742e       output [bt.
+00009930: 5465 6e73 6f72 5d3a 2054 6865 2074 7261  Tensor]: The tra
+00009940: 6e73 666f 726d 6564 2063 6f6f 7264 696e  nsformed coordin
+00009950: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
+00009960: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
+00009970: 6261 7463 685d 2c20 7b6e 5f64 696d 7d2c  batch], {n_dim},
+00009980: 206e 5f31 2c20 6e5f 322c 202e 2e2e 2c20   n_1, n_2, ..., 
+00009990: 6e5f 7229 0a20 2020 2020 2020 2027 2727  n_r).        '''
+000099a0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+000099b0: 7472 616e 736c 6174 696f 6e29 203d 3d20  translation) == 
+000099c0: 313a 2074 7261 6e73 6c61 7469 6f6e 203d  1: translation =
+000099d0: 2074 7261 6e73 6c61 7469 6f6e 5b30 5d0a   translation[0].
+000099e0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000099f0: 7461 6e63 6528 7472 616e 736c 6174 696f  tance(translatio
+00009a00: 6e2c 2074 7570 6c65 293a 2074 7261 6e73  n, tuple): trans
+00009a10: 6c61 7469 6f6e 203d 206c 6973 7428 7472  lation = list(tr
+00009a20: 616e 736c 6174 696f 6e29 0a20 2020 2020  anslation).     
+00009a30: 2020 2074 7261 6e73 6c61 7469 6f6e 203d     translation =
+00009a40: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+00009a50: 7472 616e 736c 6174 696f 6e29 2e73 7175  translation).squ
+00009a60: 6565 7a65 2829 0a20 2020 2020 2020 2069  eeze().        i
+00009a70: 6620 7472 616e 736c 6174 696f 6e2e 6e5f  f translation.n_
+00009a80: 6469 6d20 3c3d 2031 3a20 7472 616e 736c  dim <= 1: transl
+00009a90: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
+00009aa0: 696f 6e2e 756e 7371 7565 657a 6528 5b5d  ion.unsqueeze([]
+00009ab0: 290a 2020 2020 2020 2020 6966 2074 7261  ).        if tra
+00009ac0: 6e73 6c61 7469 6f6e 2e6e 5f64 696d 203d  nslation.n_dim =
+00009ad0: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
+00009ae0: 2069 6620 6e6f 7420 7472 616e 736c 6174   if not translat
+00009af0: 696f 6e2e 6861 735f 6261 7463 683a 2074  ion.has_batch: t
+00009b00: 7261 6e73 6c61 7469 6f6e 2e62 6174 6368  ranslation.batch
+00009b10: 5f64 696d 656e 7369 6f6e 203d 2030 0a20  _dimension = 0. 
+00009b20: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00009b30: 7420 7472 616e 736c 6174 696f 6e2e 6861  t translation.ha
+00009b40: 735f 6368 616e 6e65 6c3a 2074 7261 6e73  s_channel: trans
+00009b50: 6c61 7469 6f6e 2e63 6861 6e6e 656c 5f64  lation.channel_d
+00009b60: 696d 656e 7369 6f6e 203d 2030 2069 6620  imension = 0 if 
+00009b70: 7472 616e 736c 6174 696f 6e2e 6261 7463  translation.batc
+00009b80: 685f 6469 6d65 6e73 696f 6e20 3e20 3020  h_dimension > 0 
+00009b90: 656c 7365 2031 0a20 2020 2020 2020 2061  else 1.        a
+00009ba0: 766f 7563 6828 7472 616e 736c 6174 696f  vouch(translatio
+00009bb0: 6e2e 6861 735f 6261 7463 6820 616e 6420  n.has_batch and 
+00009bc0: 7472 616e 736c 6174 696f 6e2e 6861 735f  translation.has_
+00009bd0: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
+00009be0: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
+00009bf0: 6e73 6f72 206f 6620 7369 7a65 205c 0a20  nsor of size \. 
+00009c00: 2020 2020 2020 2020 2020 2028 5b6e 5f62             ([n_b
+00009c10: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
+00009c20: 7b7b 6e5f 6469 6d7d 7d29 2066 6f72 2054  {{n_dim}}) for T
+00009c30: 7261 6e73 6c61 7469 6f6e 2070 6172 616d  ranslation param
+00009c40: 6574 6572 732c 2069 6e73 7465 6164 206f  eters, instead o
+00009c50: 6620 7b74 7261 6e73 6c61 7469 6f6e 2e73  f {translation.s
+00009c60: 6861 7065 7d2e 2022 290a 2020 2020 2020  hape}. ").      
+00009c70: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+00009c80: 5f5f 2874 7261 6e73 6c61 7469 6f6e 290a  __(translation).
+00009c90: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00009ca0: 616e 736c 6174 696f 6e20 3d20 7472 616e  anslation = tran
+00009cb0: 736c 6174 696f 6e0a 2020 2020 2020 2020  slation.        
+00009cc0: 7365 6c66 2e6e 5f64 696d 203d 2073 656c  self.n_dim = sel
+00009cd0: 662e 7472 616e 736c 6174 696f 6e2e 6e5f  f.translation.n_
+00009ce0: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
+00009cf0: 7365 6c66 2e62 6174 6368 5f70 6172 616d  self.batch_param
+00009d00: 2e61 7070 656e 6428 2774 7261 6e73 6c61  .append('transla
+00009d10: 7469 6f6e 2729 0a0a 2020 2020 6465 6620  tion')..    def 
+00009d20: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2058  __call__(self, X
+00009d30: 293a 0a20 2020 2020 2020 2058 203d 2073  ):.        X = s
+00009d40: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
+00009d50: 5829 0a20 2020 2020 2020 2072 6574 7572  X).        retur
+00009d60: 6e20 5820 2b20 7365 6c66 2e74 7261 6e73  n X + self.trans
+00009d70: 6c61 7469 6f6e 0a20 2020 200a 2020 2020  lation.    .    
+00009d80: 6465 6620 6166 6669 6e65 2873 656c 662c  def affine(self,
+00009d90: 206e 5f64 696d 3d4e 6f6e 6529 3a0a 2020   n_dim=None):.  
+00009da0: 2020 2020 2020 6176 6f75 6368 286e 5f64        avouch(n_d
+00009db0: 696d 2069 7320 4e6f 6e65 206f 7220 7365  im is None or se
+00009dc0: 6c66 2e6e 5f64 696d 203d 3d20 6e5f 6469  lf.n_dim == n_di
+00009dd0: 6d29 0a20 2020 2020 2020 2069 6620 6e5f  m).        if n_
+00009de0: 6469 6d20 6973 204e 6f6e 653a 206e 5f64  dim is None: n_d
+00009df0: 696d 203d 2073 656c 662e 6e5f 6469 6d0a  im = self.n_dim.
+00009e00: 2020 2020 2020 2020 6e5f 6261 7463 6820          n_batch 
+00009e10: 3d20 7365 6c66 2e74 7261 6e73 6c61 7469  = self.translati
+00009e20: 6f6e 2e6e 5f62 6174 6368 0a20 2020 2020  on.n_batch.     
+00009e30: 2020 2072 6574 7572 6e20 6274 2e63 6174     return bt.cat
+00009e40: 2862 742e 6361 7428 6274 2e65 7965 2873  (bt.cat(bt.eye(s
+00009e50: 656c 662e 6e5f 6469 6d29 2e6d 756c 7469  elf.n_dim).multi
+00009e60: 706c 7928 6e5f 6261 7463 682c 205b 5d29  ply(n_batch, [])
+00009e70: 2c20 7365 6c66 2e74 7261 6e73 6c61 7469  , self.translati
+00009e80: 6f6e 2e77 6974 685f 6368 616e 6e65 6c64  on.with_channeld
+00009e90: 696d 284e 6f6e 6529 2e75 6e73 7175 6565  im(None).unsquee
+00009ea0: 7a65 282d 3129 2c20 2d31 292c 2062 742e  ze(-1), -1), bt.
+00009eb0: 6f6e 655f 686f 7428 2d31 2c20 6e5f 6469  one_hot(-1, n_di
+00009ec0: 6d2b 3129 2e75 6e73 7175 6565 7a65 2830  m+1).unsqueeze(0
+00009ed0: 292e 6d75 6c74 6970 6c79 286e 5f62 6174  ).multiply(n_bat
+00009ee0: 6368 2c20 5b5d 292c 2031 290a 0a20 2020  ch, []), 1)..   
+00009ef0: 2064 6566 2069 6e76 2873 656c 6629 3a20   def inv(self): 
+00009f00: 7265 7475 726e 2054 7261 6e73 6c61 7465  return Translate
+00009f10: 282d 7365 6c66 2e74 7261 6e73 6c61 7469  (-self.translati
+00009f20: 6f6e 292e 6261 636b 7761 7264 5f28 7365  on).backward_(se
+00009f30: 6c66 2e62 6163 6b77 6172 6429 0a0a 4061  lf.backward)..@a
+00009f40: 6c69 6173 2822 5269 6722 290a 636c 6173  lias("Rig").clas
+00009f50: 7320 5269 6769 6428 5370 6174 6961 6c54  s Rigid(SpatialT
+00009f60: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
+00009f70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00009f80: 2873 656c 662c 2061 6e67 6c65 2c20 6178  (self, angle, ax
+00009f90: 6973 3d4e 6f6e 652c 2074 7261 6e73 6c61  is=None, transla
+00009fa0: 7469 6f6e 3d4e 6f6e 652c 2063 656e 7465  tion=None, cente
+00009fb0: 723d 4e6f 6e65 2c20 7472 616e 735f 7374  r=None, trans_st
+00009fc0: 7265 7463 683d 4e6f 6e65 2c20 7370 6163  retch=None, spac
+00009fd0: 696e 673d 3129 3a0a 2020 2020 2020 2020  ing=1):.        
+00009fe0: 2727 270a 2020 2020 2020 2020 5269 6769  '''.        Rigi
+00009ff0: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
+0000a000: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
+0000a010: 2070 6172 616d 6574 6572 732e 0a20 2020   parameters..   
+0000a020: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
+0000a030: 7261 6d73 2053 6574 2031 3a0a 2020 2020  rams Set 1:.    
+0000a040: 2020 2020 2020 2020 616e 676c 6520 5b62          angle [b
+0000a050: 742e 5465 6e73 6f72 206f 7220 6e70 2e6e  t.Tensor or np.n
+0000a060: 756d 7079 5d3a 2074 6865 205b 636c 6f63  umpy]: the [cloc
+0000a070: 6b77 6973 655d 2072 6f74 6174 696f 6e20  kwise] rotation 
+0000a080: 616e 676c 6573 2061 626f 7574 2074 6865  angles about the
+0000a090: 2061 7869 7365 7320 286f 7220 7a20 6469   axises (or z di
+0000a0a0: 7265 6374 696f 6e20 666f 7220 3244 292e  rection for 2D).
+0000a0b0: 2049 7420 6973 2063 6f75 6e74 6572 2d63   It is counter-c
+0000a0c0: 6c6f 636b 7769 7365 2066 6f72 2069 6d61  lockwise for ima
+0000a0d0: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
+0000a0e0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+0000a0f0: 7463 685d 2c29 0a20 2020 2020 2020 2020  tch],).         
+0000a100: 2020 2061 7869 7320 5b62 742e 5465 6e73     axis [bt.Tens
+0000a110: 6f72 206f 7220 6e70 2e6e 756d 7079 5d3a  or or np.numpy]:
+0000a120: 2074 6865 2072 6f74 6174 696f 6e20 6178   the rotation ax
+0000a130: 6973 6573 2c20 6e6f 726d 616c 697a 6564  ises, normalized
+0000a140: 2076 6563 746f 7273 2c20 4e6f 6e65 2066   vectors, None f
+0000a150: 6f72 2032 442e 200a 2020 2020 2020 2020  or 2D. .        
+0000a160: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+0000a170: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
+0000a180: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
+0000a190: 7261 6e73 6c61 7469 6f6e 205b 6274 2e54  ranslation [bt.T
+0000a1a0: 656e 736f 7220 6f72 206e 702e 6e75 6d70  ensor or np.nump
+0000a1b0: 795d 3a20 7468 6520 7472 616e 736c 6174  y]: the translat
+0000a1c0: 696f 6e73 2061 6674 6572 2074 6865 2072  ions after the r
+0000a1d0: 6f74 6174 696f 6e2c 207a 6572 6f73 2062  otation, zeros b
+0000a1e0: 7920 6465 6661 756c 742e 200a 2020 2020  y default. .    
+0000a1f0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+0000a200: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
+0000a210: 5f64 696d 7d29 0a20 2020 2020 2020 2020  _dim}).         
+0000a220: 2020 2063 656e 7465 7220 5b62 742e 5465     center [bt.Te
+0000a230: 6e73 6f72 206f 7220 6e70 2e6e 756d 7079  nsor or np.numpy
+0000a240: 5d3a 2074 6865 2063 656e 7465 7220 666f  ]: the center fo
+0000a250: 7220 7468 6520 726f 7461 7469 6f6e 732c  r the rotations,
+0000a260: 207a 6572 6f73 2062 7920 6465 6661 756c   zeros by defaul
+0000a270: 742e 200a 2020 2020 2020 2020 2020 2020  t. .            
+0000a280: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+0000a290: 7463 685d 2c20 7b6e 5f64 696d 7d29 0a20  tch], {n_dim}). 
+0000a2a0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+0000a2b0: 5f73 7472 6574 6368 205b 696e 745d 3a20  _stretch [int]: 
+0000a2c0: 6f6e 6c79 2075 7365 6420 666f 7220 6974  only used for it
+0000a2d0: 6572 6174 6976 6520 7061 7261 6d65 7465  erative paramete
+0000a2e0: 7220 7472 6169 6e69 6e67 2c20 3120 6279  r training, 1 by
+0000a2f0: 2064 6566 6175 6c74 2e20 3230 2073 6565   default. 20 see
+0000a300: 6d73 2074 6f20 6265 2061 2067 6f6f 6420  ms to be a good 
+0000a310: 6368 6f69 6365 2e20 0a20 2020 2020 2020  choice. .       
+0000a320: 2020 2020 2073 7061 6369 6e67 205b 7475       spacing [tu
+0000a330: 706c 655d 3a20 7468 6520 7370 6163 696e  ple]: the spacin
+0000a340: 6720 6f66 2074 6865 2074 7261 6e73 666f  g of the transfo
+0000a350: 726d 6564 200a 2020 2020 2020 2020 0a20  rmed .        . 
+0000a360: 2020 2020 2020 2050 6172 616d 7320 5365         Params Se
+0000a370: 7420 323a 0a20 2020 2020 2020 2020 2020  t 2:.           
+0000a380: 206d 6174 7269 7820 5b62 742e 5465 6e73   matrix [bt.Tens
+0000a390: 6f72 206f 7220 6e70 2e6e 756d 7079 5d3a  or or np.numpy]:
+0000a3a0: 2074 6865 2061 6666 696e 6520 6d61 7472   the affine matr
+0000a3b0: 6978 2c20 6974 2073 686f 756c 6420 6265  ix, it should be
+0000a3c0: 206f 7274 686f 676f 6e61 6c20 6f72 2077   orthogonal or w
+0000a3d0: 696c 6c20 6265 2070 726f 6a65 6374 6564  ill be projected
+0000a3e0: 2062 7920 5072 6f63 7275 7374 6573 2050   by Procrustes P
+0000a3f0: 726f 626c 656d 2e20 0a20 2020 2020 2020  roblem. .       
+0000a400: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
+0000a410: 5b6e 5f62 6174 6368 5d2c 206e 5f64 696d  [n_batch], n_dim
+0000a420: 202b 2031 2c20 6e5f 6469 6d20 2b20 3129   + 1, n_dim + 1)
+0000a430: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+0000a440: 6e73 5f73 7472 6574 6368 205b 696e 745d  ns_stretch [int]
+0000a450: 3a20 6f6e 6c79 2075 7365 6420 666f 7220  : only used for 
+0000a460: 6974 6572 6174 6976 6520 7061 7261 6d65  iterative parame
+0000a470: 7465 7220 7472 6169 6e69 6e67 2c20 3120  ter training, 1 
+0000a480: 6279 2064 6566 6175 6c74 2e20 3230 2073  by default. 20 s
+0000a490: 6565 6d73 2074 6f20 6265 2061 2067 6f6f  eems to be a goo
+0000a4a0: 6420 6368 6f69 6365 2e20 0a20 2020 2020  d choice. .     
+0000a4b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000a4c0: 5768 656e 2069 7420 6973 2063 616c 6c65  When it is calle
+0000a4d0: 643a 0a20 2020 2020 2020 2020 2020 2058  d:.            X
+0000a4e0: 205b 6274 2e54 656e 736f 725d 3a20 436f   [bt.Tensor]: Co
+0000a4f0: 6f72 6469 6e61 7465 7320 746f 2062 6520  ordinates to be 
+0000a500: 7472 616e 7366 6f72 6d65 642e 0a20 2020  transformed..   
+0000a510: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+0000a520: 653a 2028 5b6e 5f62 6174 6368 3a20 6f70  e: ([n_batch: op
+0000a530: 7469 6f6e 616c 5d2c 207b 6e5f 6469 6d7d  tional], {n_dim}
+0000a540: 2c20 6e5f 312c 206e 5f32 2c20 2e2e 2e2c  , n_1, n_2, ...,
+0000a550: 206e 5f72 290a 2020 2020 2020 2020 2020   n_r).          
+0000a560: 2020 6f75 7470 7574 205b 6274 2e54 656e    output [bt.Ten
+0000a570: 736f 725d 3a20 5468 6520 7472 616e 7366  sor]: The transf
+0000a580: 6f72 6d65 6420 636f 6f72 6469 6e61 7465  ormed coordinate
+0000a590: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+0000a5a0: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
+0000a5b0: 6368 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f  ch], {n_dim}, n_
+0000a5c0: 312c 206e 5f32 2c20 2e2e 2e2c 206e 5f72  1, n_2, ..., n_r
+0000a5d0: 290a 2020 2020 2020 2020 2727 270a 2020  ).        '''.  
+0000a5e0: 2020 2020 2020 616e 676c 6520 3d20 6261        angle = ba
+0000a5f0: 746f 7263 685f 7465 6e73 6f72 2861 6e67  torch_tensor(ang
+0000a600: 6c65 290a 2020 2020 2020 2020 6966 2061  le).        if a
+0000a610: 6e67 6c65 2e6e 5f64 696d 203c 3d20 3020  ngle.n_dim <= 0 
+0000a620: 616e 6420 6e6f 7420 616e 676c 652e 6861  and not angle.ha
+0000a630: 735f 6261 7463 683a 2061 6e67 6c65 203d  s_batch: angle =
+0000a640: 2061 6e67 6c65 2e75 6e73 7175 6565 7a65   angle.unsqueeze
+0000a650: 285b 5d29 0a20 2020 2020 2020 2069 6620  ([]).        if 
+0000a660: 616e 676c 652e 6e5f 6469 6d20 3d3d 2031  angle.n_dim == 1
+0000a670: 2061 6e64 206e 6f74 2061 6e67 6c65 2e68   and not angle.h
+0000a680: 6173 5f62 6174 6368 3a20 616e 676c 6520  as_batch: angle 
+0000a690: 3d20 616e 676c 652e 7769 7468 5f62 6174  = angle.with_bat
+0000a6a0: 6368 6469 6d28 3029 0a20 2020 2020 2020  chdim(0).       
+0000a6b0: 2069 6620 616e 676c 652e 6e5f 6469 6d20   if angle.n_dim 
+0000a6c0: 3d3d 2032 2061 6e64 206e 6f74 2061 6e67  == 2 and not ang
+0000a6d0: 6c65 2e68 6173 5f62 6174 6368 3a20 616e  le.has_batch: an
+0000a6e0: 676c 6520 3d20 616e 676c 652e 756e 7371  gle = angle.unsq
+0000a6f0: 7565 657a 6528 5b5d 290a 2020 2020 2020  ueeze([]).      
+0000a700: 2020 6966 2061 6e67 6c65 2e6e 5f64 696d    if angle.n_dim
+0000a710: 203d 3d20 3320 616e 6420 6e6f 7420 616e   == 3 and not an
+0000a720: 676c 652e 6861 735f 6261 7463 6820 616e  gle.has_batch an
+0000a730: 6420 616e 676c 652e 7368 6170 655b 315d  d angle.shape[1]
+0000a740: 203d 3d20 616e 676c 652e 7368 6170 655b   == angle.shape[
+0000a750: 325d 3a20 616e 676c 652e 6261 7463 685f  2]: angle.batch_
+0000a760: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
+0000a770: 2020 2020 2020 6176 6f75 6368 2861 6e67        avouch(ang
+0000a780: 6c65 2e68 6173 5f62 6174 6368 2c20 6622  le.has_batch, f"
+0000a790: 506c 6561 7365 2075 7365 2062 6174 6f72  Please use bator
+0000a7a0: 6368 2074 656e 736f 7220 6f66 2073 697a  ch tensor of siz
+0000a7b0: 6520 285b 6e5f 6261 7463 685d 2c29 2066  e ([n_batch],) f
+0000a7c0: 6f72 2052 6967 6964 2072 6f74 6174 696f  or Rigid rotatio
+0000a7d0: 6e20 616e 676c 6573 2c20 696e 7374 6561  n angles, instea
+0000a7e0: 6420 6f66 207b 616e 676c 652e 7368 6170  d of {angle.shap
+0000a7f0: 657d 2e20 2229 0a20 2020 2020 2020 206e  e}. ").        n
+0000a800: 5f62 6174 6368 203d 2061 6e67 6c65 2e6e  _batch = angle.n
+0000a810: 5f62 6174 6368 0a20 2020 2020 2020 206e  _batch.        n
+0000a820: 5f64 696d 203d 204e 6f6e 650a 2020 2020  _dim = None.    
+0000a830: 2020 2020 6966 2061 6e67 6c65 2e6e 5f64      if angle.n_d
+0000a840: 696d 203e 3d20 323a 0a20 2020 2020 2020  im >= 2:.       
+0000a850: 2020 2020 206d 6174 7269 7820 3d20 616e       matrix = an
+0000a860: 676c 650a 2020 2020 2020 2020 2020 2020  gle.            
+0000a870: 6e5f 6469 6d20 3d20 6d61 7472 6978 2e73  n_dim = matrix.s
+0000a880: 697a 6528 2d31 2920 2d20 310a 2020 2020  ize(-1) - 1.    
+0000a890: 2020 2020 2020 2020 6365 6e74 6572 203d          center =
+0000a8a0: 2062 742e 7a65 726f 7328 5b6e 5f62 6174   bt.zeros([n_bat
+0000a8b0: 6368 5d2c 207b 6e5f 6469 6d7d 290a 2020  ch], {n_dim}).  
+0000a8c0: 2020 2020 2020 2020 2020 7472 616e 736c            transl
+0000a8d0: 6174 696f 6e20 3d20 6d61 7472 6978 5b2e  ation = matrix[.
+0000a8e0: 2e2e 2c20 3a2d 312c 202d 315d 2e77 6974  .., :-1, -1].wit
+0000a8f0: 685f 6368 616e 6e65 6c64 696d 2831 290a  h_channeldim(1).
+0000a900: 2020 2020 2020 2020 2020 2020 4120 3d20              A = 
+0000a910: 6d61 7472 6978 5b2e 2e2e 2c20 3a2d 312c  matrix[..., :-1,
+0000a920: 203a 2d31 5d0a 2020 2020 2020 2020 2020   :-1].          
+0000a930: 2020 6176 6f75 6368 2862 742e 6e6f 726d    avouch(bt.norm
+0000a940: 2841 2e54 2040 2041 202d 2062 742e 6579  (A.T @ A - bt.ey
+0000a950: 6528 4129 292e 7375 6d28 2920 3c20 3165  e(A)).sum() < 1e
+0000a960: 2d34 2c20 2250 6c65 6173 6520 6d61 6b65  -4, "Please make
+0000a970: 2073 7572 6520 7468 6174 206d 6174 7269   sure that matri
+0000a980: 7820 696e 7075 7420 666f 7220 5269 6769  x input for Rigi
+0000a990: 6420 6973 206f 7274 686f 676f 6e61 6c2e  d is orthogonal.
+0000a9a0: 2055 7365 2041 6666 696e 6520 696e 7374   Use Affine inst
+0000a9b0: 6561 6420 6966 2069 7420 6973 206e 6f74  ead if it is not
+0000a9c0: 2e20 2229 0a20 2020 2020 2020 2020 2020  . ").           
+0000a9d0: 2023 2049 203d 2062 742e 6579 6528 4129   # I = bt.eye(A)
+0000a9e0: 0a20 2020 2020 2020 2020 2020 2023 205a  .            # Z
+0000a9f0: 5f6c 6566 7420 3d20 2841 202d 2049 295b  _left = (A - I)[
+0000aa00: 2e2e 2e2c 203a 2d31 5d20 2320 285b 6e5f  ..., :-1] # ([n_
+0000aa10: 6261 7463 685d 2c20 6e5f 6469 6d2c 206e  batch], n_dim, n
+0000aa20: 5f64 696d 2d31 290a 2020 2020 2020 2020  _dim-1).        
+0000aa30: 2020 2020 2320 5a5f 7269 6768 7420 3d20      # Z_right = 
+0000aa40: 2841 202d 2049 295b 2e2e 2e2c 202d 315d  (A - I)[..., -1]
+0000aa50: 2023 2028 5b6e 5f62 6174 6368 5d2c 206e   # ([n_batch], n
+0000aa60: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
+0000aa70: 2020 2320 5a54 5a20 3d20 5a5f 6c65 6674    # ZTZ = Z_left
+0000aa80: 2e54 2040 205a 5f6c 6566 740a 2020 2020  .T @ Z_left.    
+0000aa90: 2020 2020 2020 2020 2320 6966 206e 5f64          # if n_d
+0000aaa0: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
+0000aab0: 2020 2020 2023 2020 2020 2061 7869 7320       #     axis 
+0000aac0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000aad0: 2020 2023 2020 2020 2061 6e67 6c65 203d     #     angle =
+0000aae0: 2062 742e 7768 6572 6528 6274 2e61 6273   bt.where(bt.abs
+0000aaf0: 2862 742e 6465 7428 5a54 5a29 2920 3c20  (bt.det(ZTZ)) < 
+0000ab00: 3165 2d36 2c20 6274 2e7a 6572 6f73 285b  1e-6, bt.zeros([
+0000ab10: 6e5f 6261 7463 685d 292c 2062 742e 6163  n_batch]), bt.ac
+0000ab20: 6f73 2831 202d 205a 545a 202f 2032 292e  os(1 - ZTZ / 2).
+0000ab30: 7371 7565 657a 6528 2d31 2c20 2d31 2929  squeeze(-1, -1))
+0000ab40: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
+0000ab50: 6c69 6620 6e5f 6469 6d20 3d3d 2033 3a0a  lif n_dim == 3:.
+0000ab60: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0000ab70: 2020 696e 765a 545a 203d 2062 742e 696e    invZTZ = bt.in
+0000ab80: 7628 6274 2e77 6865 7265 2862 742e 6162  v(bt.where(bt.ab
+0000ab90: 7328 6274 2e64 6574 285a 545a 2929 2e75  s(bt.det(ZTZ)).u
+0000aba0: 6e73 7175 6565 7a65 282d 312c 202d 3129  nsqueeze(-1, -1)
+0000abb0: 203c 2031 652d 362c 2062 742e 6579 6528   < 1e-6, bt.eye(
+0000abc0: 5a54 5a29 2c20 5a54 5a29 290a 2020 2020  ZTZ), ZTZ)).    
+0000abd0: 2020 2020 2020 2020 2320 2020 2020 7665          #     ve
+0000abe0: 6374 6f72 203d 2062 742e 6361 7428 2d20  ctor = bt.cat(- 
+0000abf0: 696e 765a 545a 2040 205a 5f6c 6566 742e  invZTZ @ Z_left.
+0000ac00: 5420 4020 5a5f 7269 6768 742c 2062 742e  T @ Z_right, bt.
+0000ac10: 6f6e 6573 285b 6e5f 6261 7463 685d 2c20  ones([n_batch], 
+0000ac20: 3129 2c20 3129 2e77 6974 685f 6368 616e  1), 1).with_chan
+0000ac30: 6e65 6c64 696d 2831 290a 2020 2020 2020  neldim(1).      
+0000ac40: 2020 2020 2020 2320 2020 2020 616e 676c        #     angl
+0000ac50: 6520 3d20 6274 2e77 6865 7265 2862 742e  e = bt.where(bt.
+0000ac60: 6162 7328 6274 2e64 6574 285a 545a 2929  abs(bt.det(ZTZ))
+0000ac70: 203c 2031 652d 362c 2062 742e 7a65 726f   < 1e-6, bt.zero
+0000ac80: 7328 5b6e 5f62 6174 6368 5d29 2c20 7665  s([n_batch]), ve
+0000ac90: 6374 6f72 2e6e 6f72 6d28 2929 0a20 2020  ctor.norm()).   
+0000aca0: 2020 2020 2020 2020 2023 2020 2020 2061           #     a
+0000acb0: 7869 7320 3d20 6274 2e77 6865 7265 2828  xis = bt.where((
+0000acc0: 6274 2e61 6273 2862 742e 6465 7428 5a54  bt.abs(bt.det(ZT
+0000acd0: 5a29 2920 3c20 3165 2d36 292e 6d75 6c74  Z)) < 1e-6).mult
+0000ace0: 6970 6c79 286e 5f64 696d 2c20 7b7d 292c  iply(n_dim, {}),
+0000acf0: 2062 742e 6368 616e 6e65 6c5f 7465 6e73   bt.channel_tens
+0000ad00: 6f72 2862 742e 6f6e 655f 686f 7428 302c  or(bt.one_hot(0,
+0000ad10: 206e 5f64 696d 2929 2e6d 756c 7469 706c   n_dim)).multipl
+0000ad20: 7928 6e5f 6261 7463 682c 205b 5d29 2c20  y(n_batch, []), 
+0000ad30: 7665 6374 6f72 202f 2061 6e67 6c65 290a  vector / angle).
+0000ad40: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000ad50: 5f64 696d 203d 3d20 323a 2061 7869 7320  _dim == 2: axis 
+0000ad60: 3d20 4e6f 6e65 3b20 616e 676c 6520 3d20  = None; angle = 
+0000ad70: 6274 2e61 636f 7328 415b 2e2e 2e2c 2030  bt.acos(A[..., 0
+0000ad80: 2c20 305d 290a 2020 2020 2020 2020 2020  , 0]).          
+0000ad90: 2020 656c 6966 206e 5f64 696d 203d 3d20    elif n_dim == 
+0000ada0: 333a 0a20 2020 2020 2020 2020 2020 2020  3:.             
+0000adb0: 2020 2061 6e74 695f 7379 6d20 3d20 2841     anti_sym = (A
+0000adc0: 202d 2041 2e54 2920 2f20 320a 2020 2020   - A.T) / 2.    
+0000add0: 2020 2020 2020 2020 2020 2020 7379 6d20              sym 
+0000ade0: 3d20 2841 202b 2041 2e54 2920 2f20 3220  = (A + A.T) / 2 
+0000adf0: 2d20 6274 2e65 7965 2841 290a 2020 2020  - bt.eye(A).    
+0000ae00: 2020 2020 2020 2020 2020 2020 616e 676c              angl
+0000ae10: 6520 3d20 6274 2e61 636f 7328 2828 616e  e = bt.acos(((an
+0000ae20: 7469 5f73 796d 2040 2061 6e74 695f 7379  ti_sym @ anti_sy
+0000ae30: 6d29 202f 2073 796d 292e 6d65 616e 2829  m) / sym).mean()
+0000ae40: 202d 2031 290a 2020 2020 2020 2020 2020   - 1).          
+0000ae50: 2020 2020 2020 6178 6973 203d 2062 742e        axis = bt.
+0000ae60: 756e 6372 6f73 735f 6d61 7472 6978 2861  uncross_matrix(a
+0000ae70: 6e74 695f 7379 6d29 0a20 2020 2020 2020  nti_sym).       
+0000ae80: 2020 2020 2020 2020 2061 7869 7320 2f3d           axis /=
+0000ae90: 2062 742e 7369 6e28 616e 676c 6529 0a20   bt.sin(angle). 
+0000aea0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000aeb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aec0: 2072 6169 7365 2045 7272 6f72 2822 4e6f   raise Error("No
+0000aed0: 7449 6d70 6c65 6d65 6e74 6564 2229 2866  tImplemented")(f
+0000aee0: 2252 6967 6964 2074 7261 6e73 666f 726d  "Rigid transform
+0000aef0: 6174 696f 6e20 696e 206d 6963 6f6d 7075  ation in micompu
+0000af00: 7469 6e67 2064 6f65 7320 6e6f 7420 7375  ting does not su
+0000af10: 7070 6f72 7420 7b6e 5f64 696d 7d20 6469  pport {n_dim} di
+0000af20: 6d65 6e73 696f 6e61 6c20 7472 616e 7366  mensional transf
+0000af30: 6f72 6d73 2028 3220 2620 3344 206f 6e6c  orms (2 & 3D onl
+0000af40: 7929 2e20 2220 2b20 0a20 2020 2020 2020  y). " + .       
+0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af70: 2020 2020 2022 506c 6561 7365 2063 6f6e       "Please con
+0000af80: 7461 6374 2074 6865 2064 6576 656c 6f70  tact the develop
+0000af90: 6572 7320 6966 2074 6865 7265 2061 7265  ers if there are
+0000afa0: 2066 6561 7369 626c 6520 616c 676f 7269   feasible algori
+0000afb0: 7468 6d73 2028 4572 726f 7220 436f 6465  thms (Error Code
+0000afc0: 3a20 5433 3333 292e 2054 6861 6e6b 2079  : T333). Thank y
+0000afd0: 6f75 2e20 2229 0a0a 2020 2020 2020 2020  ou. ")..        
+0000afe0: 6966 2074 7261 6e73 6c61 7469 6f6e 2069  if translation i
+0000aff0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000b000: 2020 2020 2020 2020 7472 616e 736c 6174          translat
+0000b010: 696f 6e20 3d20 6261 746f 7263 685f 7465  ion = batorch_te
+0000b020: 6e73 6f72 2874 7261 6e73 6c61 7469 6f6e  nsor(translation
+0000b030: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000b040: 2074 7261 6e73 6c61 7469 6f6e 2e6e 5f64   translation.n_d
+0000b050: 696d 203c 3d20 3120 616e 6420 6e6f 7420  im <= 1 and not 
+0000b060: 7472 616e 736c 6174 696f 6e2e 6861 735f  translation.has_
+0000b070: 6261 7463 683a 2074 7261 6e73 6c61 7469  batch: translati
+0000b080: 6f6e 203d 2074 7261 6e73 6c61 7469 6f6e  on = translation
+0000b090: 2e75 6e73 7175 6565 7a65 285b 5d29 0a20  .unsqueeze([]). 
+0000b0a0: 2020 2020 2020 2020 2020 2069 6620 7472             if tr
+0000b0b0: 616e 736c 6174 696f 6e2e 6e5f 6469 6d20  anslation.n_dim 
+0000b0c0: 3d3d 2032 2061 6e64 206e 6f74 2074 7261  == 2 and not tra
+0000b0d0: 6e73 6c61 7469 6f6e 2e68 6173 5f62 6174  nslation.has_bat
+0000b0e0: 6368 3a20 7472 616e 736c 6174 696f 6e20  ch: translation 
+0000b0f0: 3d20 7472 616e 736c 6174 696f 6e2e 7769  = translation.wi
+0000b100: 7468 5f62 6174 6368 6469 6d28 2831 202d  th_batchdim((1 -
+0000b110: 2074 7261 6e73 6c61 7469 6f6e 2e63 6861   translation.cha
+0000b120: 6e6e 656c 5f64 696d 656e 7369 6f6e 2920  nnel_dimension) 
+0000b130: 6966 2074 7261 6e73 6c61 7469 6f6e 2e68  if translation.h
+0000b140: 6173 5f63 6861 6e6e 656c 2065 6c73 6520  as_channel else 
+0000b150: 3029 0a20 2020 2020 2020 2020 2020 2069  0).            i
+0000b160: 6620 7472 616e 736c 6174 696f 6e2e 6e5f  f translation.n_
+0000b170: 6469 6d20 3d3d 2032 2061 6e64 206e 6f74  dim == 2 and not
+0000b180: 2074 7261 6e73 6c61 7469 6f6e 2e68 6173   translation.has
+0000b190: 5f63 6861 6e6e 656c 3a20 7472 616e 736c  _channel: transl
+0000b1a0: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
+0000b1b0: 696f 6e2e 7769 7468 5f63 6861 6e6e 656c  ion.with_channel
+0000b1c0: 6469 6d28 3120 2d20 7472 616e 736c 6174  dim(1 - translat
+0000b1d0: 696f 6e2e 6261 7463 685f 6469 6d65 6e73  ion.batch_dimens
+0000b1e0: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+0000b1f0: 2061 766f 7563 6828 7472 616e 736c 6174   avouch(translat
+0000b200: 696f 6e2e 6861 735f 6261 7463 6820 616e  ion.has_batch an
+0000b210: 6420 7472 616e 736c 6174 696f 6e2e 6861  d translation.ha
+0000b220: 735f 6368 616e 6e65 6c2c 2066 2250 6c65  s_channel, f"Ple
+0000b230: 6173 6520 7573 6520 6261 746f 7263 6820  ase use batorch 
+0000b240: 7465 6e73 6f72 206f 6620 7369 7a65 2028  tensor of size (
+0000b250: 5b6e 5f62 6174 6368 5d2c 207b 7b6e 5f64  [n_batch], {{n_d
+0000b260: 696d 7d7d 2920 666f 7220 5269 6769 6420  im}}) for Rigid 
+0000b270: 7472 616e 736c 6174 696f 6e2c 2069 6e73  translation, ins
+0000b280: 7465 6164 206f 6620 7b74 7261 6e73 6c61  tead of {transla
+0000b290: 7469 6f6e 2e73 6861 7065 7d2e 2022 290a  tion.shape}. ").
+0000b2a0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000b2b0: 5f62 6174 6368 203d 3d20 3120 616e 6420  _batch == 1 and 
+0000b2c0: 7472 616e 736c 6174 696f 6e2e 6e5f 6261  translation.n_ba
+0000b2d0: 7463 6820 3e20 313a 206e 5f62 6174 6368  tch > 1: n_batch
+0000b2e0: 203d 2074 7261 6e73 6c61 7469 6f6e 2e6e   = translation.n
+0000b2f0: 5f62 6174 6368 0a20 2020 2020 2020 2020  _batch.         
+0000b300: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
+0000b310: 6f6e 653a 206e 5f64 696d 203d 2074 7261  one: n_dim = tra
+0000b320: 6e73 6c61 7469 6f6e 2e6e 5f63 6861 6e6e  nslation.n_chann
+0000b330: 656c 0a20 2020 2020 2020 2020 2020 2065  el.            e
+0000b340: 6c73 653a 2061 766f 7563 6828 6e5f 6469  lse: avouch(n_di
+0000b350: 6d20 3d3d 2074 7261 6e73 6c61 7469 6f6e  m == translation
+0000b360: 2e6e 5f63 6861 6e6e 656c 2c20 2253 7973  .n_channel, "Sys
+0000b370: 7465 6d61 7469 6320 6572 726f 722e 2050  tematic error. P
+0000b380: 6c65 6173 6520 636f 6e74 6163 7420 7468  lease contact th
+0000b390: 6520 6465 7665 6c6f 7065 7273 2066 6f72  e developers for
+0000b3a0: 2064 6574 6169 6c73 2028 4572 726f 7220   details (Error 
+0000b3b0: 436f 6465 3a20 5433 3332 292e 2022 290a  Code: T332). ").
+0000b3c0: 2020 2020 2020 2020 2020 2020 6e5f 6469              n_di
+0000b3d0: 6d20 3d20 7472 616e 736c 6174 696f 6e2e  m = translation.
+0000b3e0: 6e5f 6368 616e 6e65 6c0a 2020 2020 2020  n_channel.      
+0000b3f0: 2020 6966 2063 656e 7465 7220 6973 206e    if center is n
+0000b400: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000b410: 2020 2020 2063 656e 7465 7220 3d20 6261       center = ba
+0000b420: 746f 7263 685f 7465 6e73 6f72 2863 656e  torch_tensor(cen
+0000b430: 7465 7229 0a20 2020 2020 2020 2020 2020  ter).           
+0000b440: 2069 6620 6365 6e74 6572 2e6e 5f64 696d   if center.n_dim
+0000b450: 203c 3d20 3120 616e 6420 6e6f 7420 6365   <= 1 and not ce
+0000b460: 6e74 6572 2e68 6173 5f62 6174 6368 3a20  nter.has_batch: 
+0000b470: 6365 6e74 6572 203d 2063 656e 7465 722e  center = center.
+0000b480: 756e 7371 7565 657a 6528 5b5d 290a 2020  unsqueeze([]).  
+0000b490: 2020 2020 2020 2020 2020 6966 2063 656e            if cen
+0000b4a0: 7465 722e 6e5f 6469 6d20 3d3d 2032 2061  ter.n_dim == 2 a
+0000b4b0: 6e64 206e 6f74 2063 656e 7465 722e 6861  nd not center.ha
+0000b4c0: 735f 6261 7463 683a 2063 656e 7465 7220  s_batch: center 
+0000b4d0: 3d20 6365 6e74 6572 2e77 6974 685f 6261  = center.with_ba
+0000b4e0: 7463 6864 696d 2828 3120 2d20 6365 6e74  tchdim((1 - cent
+0000b4f0: 6572 2e63 6861 6e6e 656c 5f64 696d 656e  er.channel_dimen
+0000b500: 7369 6f6e 2920 6966 2063 656e 7465 722e  sion) if center.
+0000b510: 6861 735f 6368 616e 6e65 6c20 656c 7365  has_channel else
+0000b520: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
+0000b530: 6966 2063 656e 7465 722e 6e5f 6469 6d20  if center.n_dim 
+0000b540: 3d3d 2032 2061 6e64 206e 6f74 2063 656e  == 2 and not cen
+0000b550: 7465 722e 6861 735f 6368 616e 6e65 6c3a  ter.has_channel:
+0000b560: 2063 656e 7465 7220 3d20 6365 6e74 6572   center = center
+0000b570: 2e77 6974 685f 6368 616e 6e65 6c64 696d  .with_channeldim
+0000b580: 2831 202d 2063 656e 7465 722e 6261 7463  (1 - center.batc
+0000b590: 685f 6469 6d65 6e73 696f 6e29 0a20 2020  h_dimension).   
+0000b5a0: 2020 2020 2020 2020 2061 766f 7563 6828           avouch(
+0000b5b0: 6365 6e74 6572 2e68 6173 5f62 6174 6368  center.has_batch
+0000b5c0: 2061 6e64 2063 656e 7465 722e 6861 735f   and center.has_
+0000b5d0: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
+0000b5e0: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
+0000b5f0: 6e73 6f72 206f 6620 7369 7a65 2028 5b6e  nsor of size ([n
+0000b600: 5f62 6174 6368 5d2c 207b 7b6e 5f64 696d  _batch], {{n_dim
+0000b610: 7d7d 2920 666f 7220 5269 6769 6420 6365  }}) for Rigid ce
+0000b620: 6e74 6572 2c20 696e 7374 6561 6420 6f66  nter, instead of
+0000b630: 207b 6365 6e74 6572 2e73 6861 7065 7d2e   {center.shape}.
+0000b640: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
+0000b650: 6966 206e 5f62 6174 6368 203d 3d20 3120  if n_batch == 1 
+0000b660: 616e 6420 6365 6e74 6572 2e6e 5f62 6174  and center.n_bat
+0000b670: 6368 203e 2031 3a20 6e5f 6261 7463 6820  ch > 1: n_batch 
+0000b680: 3d20 6365 6e74 6572 2e6e 5f62 6174 6368  = center.n_batch
+0000b690: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b6a0: 6e5f 6469 6d20 6973 204e 6f6e 653a 206e  n_dim is None: n
+0000b6b0: 5f64 696d 203d 2063 656e 7465 722e 6e5f  _dim = center.n_
+0000b6c0: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
+0000b6d0: 2020 2020 656c 7365 3a20 6176 6f75 6368      else: avouch
+0000b6e0: 286e 5f64 696d 203d 3d20 6365 6e74 6572  (n_dim == center
+0000b6f0: 2e6e 5f63 6861 6e6e 656c 2c20 6622 4365  .n_channel, f"Ce
+0000b700: 6e74 6572 287b 6365 6e74 6572 2e6e 5f63  nter({center.n_c
+0000b710: 6861 6e6e 656c 7d44 2920 616e 6420 7472  hannel}D) and tr
+0000b720: 616e 736c 6174 696f 6e28 7b6e 5f64 696d  anslation({n_dim
+0000b730: 7d44 2920 696e 2074 7261 6e73 2e52 6967  }D) in trans.Rig
+0000b740: 6964 2073 686f 756c 6420 6861 7665 2074  id should have t
+0000b750: 6865 2073 616d 6520 6469 6d65 6e73 696f  he same dimensio
+0000b760: 6e2e 2022 290a 2020 2020 2020 2020 2020  n. ").          
+0000b770: 2020 6e5f 6469 6d20 3d20 6365 6e74 6572    n_dim = center
+0000b780: 2e6e 5f63 6861 6e6e 656c 0a20 2020 2020  .n_channel.     
+0000b790: 2020 2069 6620 6178 6973 2069 7320 6e6f     if axis is no
+0000b7a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000b7b0: 2020 2020 6178 6973 203d 2062 6174 6f72      axis = bator
+0000b7c0: 6368 5f74 656e 736f 7228 6178 6973 290a  ch_tensor(axis).
+0000b7d0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0000b7e0: 7869 732e 6e5f 6469 6d20 3c3d 2031 2061  xis.n_dim <= 1 a
+0000b7f0: 6e64 206e 6f74 2061 7869 732e 6861 735f  nd not axis.has_
+0000b800: 6261 7463 683a 2061 7869 7320 3d20 6178  batch: axis = ax
+0000b810: 6973 2e75 6e73 7175 6565 7a65 285b 5d29  is.unsqueeze([])
+0000b820: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b830: 6178 6973 2e6e 5f64 696d 203d 3d20 3220  axis.n_dim == 2 
+0000b840: 616e 6420 6e6f 7420 6178 6973 2e68 6173  and not axis.has
+0000b850: 5f62 6174 6368 3a20 6178 6973 203d 2061  _batch: axis = a
+0000b860: 7869 732e 7769 7468 5f62 6174 6368 6469  xis.with_batchdi
+0000b870: 6d28 2831 202d 2061 7869 732e 6368 616e  m((1 - axis.chan
+0000b880: 6e65 6c5f 6469 6d65 6e73 696f 6e29 2069  nel_dimension) i
+0000b890: 6620 6178 6973 2e68 6173 5f63 6861 6e6e  f axis.has_chann
+0000b8a0: 656c 2065 6c73 6520 3029 0a20 2020 2020  el else 0).     
+0000b8b0: 2020 2020 2020 2069 6620 6178 6973 2e6e         if axis.n
+0000b8c0: 5f64 696d 203d 3d20 3220 616e 6420 6e6f  _dim == 2 and no
+0000b8d0: 7420 6178 6973 2e68 6173 5f63 6861 6e6e  t axis.has_chann
+0000b8e0: 656c 3a20 6178 6973 203d 2061 7869 732e  el: axis = axis.
+0000b8f0: 7769 7468 5f63 6861 6e6e 656c 6469 6d28  with_channeldim(
+0000b900: 3120 2d20 6178 6973 2e62 6174 6368 5f64  1 - axis.batch_d
+0000b910: 696d 656e 7369 6f6e 290a 2020 2020 2020  imension).      
+0000b920: 2020 2020 2020 6176 6f75 6368 2861 7869        avouch(axi
+0000b930: 732e 6861 735f 6261 7463 6820 616e 6420  s.has_batch and 
+0000b940: 6178 6973 2e68 6173 5f63 6861 6e6e 656c  axis.has_channel
+0000b950: 2c20 6622 506c 6561 7365 2075 7365 2062  , f"Please use b
+0000b960: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
+0000b970: 2073 697a 6520 285b 6e5f 6261 7463 685d   size ([n_batch]
+0000b980: 2c20 7b7b 6e5f 6469 6d7d 7d29 2066 6f72  , {{n_dim}}) for
+0000b990: 2052 6967 6964 2061 7869 7365 732c 2069   Rigid axises, i
+0000b9a0: 6e73 7465 6164 206f 6620 7b61 7869 732e  nstead of {axis.
+0000b9b0: 7368 6170 657d 2e20 2229 0a20 2020 2020  shape}. ").     
+0000b9c0: 2020 2020 2020 2069 6620 2828 6178 6973         if ((axis
+0000b9d0: 2e6e 6f72 6d28 2920 2d20 3129 202a 2a20  .norm() - 1) ** 
+0000b9e0: 3229 2e73 756d 2829 2e73 756d 2829 203e  2).sum().sum() >
+0000b9f0: 3d20 3165 2d34 3a0a 2020 2020 2020 2020  = 1e-4:.        
+0000ba00: 2020 2020 2020 2020 7072 696e 7428 2277          print("w
+0000ba10: 6172 6e69 6e67 3a20 7061 7261 6d2e 2061  arning: param. a
+0000ba20: 7869 7365 7320 666f 7220 2752 6967 6964  xises for 'Rigid
+0000ba30: 2720 7472 616e 7366 6f72 6d61 7469 6f6e  ' transformation
+0000ba40: 2073 686f 756c 6420 6265 206e 6f72 6d2d   should be norm-
+0000ba50: 3120 7665 6374 6f72 732c 2061 7574 6f2d  1 vectors, auto-
+0000ba60: 6e6f 726d 616c 697a 6174 696f 6e20 776f  normalization wo
+0000ba70: 756c 6420 6265 2070 6572 666f 726d 6564  uld be performed
+0000ba80: 2e20 506c 6561 7365 2063 6f6e 7461 6374  . Please contact
+0000ba90: 2074 6865 2064 6576 656c 6f70 6572 7320   the developers 
+0000baa0: 6966 206e 6563 6573 7361 7279 2028 4572  if necessary (Er
+0000bab0: 726f 7220 436f 6465 3a20 5433 3331 292e  ror Code: T331).
+0000bac0: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
+0000bad0: 2020 2020 6178 6973 203d 2061 7869 7320      axis = axis 
+0000bae0: 2f20 6178 6973 2e6e 6f72 6d28 290a 2020  / axis.norm().  
+0000baf0: 2020 2020 2020 2020 2020 6966 206e 5f62            if n_b
+0000bb00: 6174 6368 203d 3d20 3120 616e 6420 6178  atch == 1 and ax
+0000bb10: 6973 2e6e 5f62 6174 6368 203e 2031 3a20  is.n_batch > 1: 
+0000bb20: 6e5f 6261 7463 6820 3d20 6178 6973 2e6e  n_batch = axis.n
+0000bb30: 5f62 6174 6368 0a20 2020 2020 2020 2020  _batch.         
+0000bb40: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
+0000bb50: 6f6e 653a 206e 5f64 696d 203d 2061 7869  one: n_dim = axi
+0000bb60: 732e 6e5f 6368 616e 6e65 6c0a 2020 2020  s.n_channel.    
+0000bb70: 2020 2020 2020 2020 656c 7365 3a20 6176          else: av
+0000bb80: 6f75 6368 286e 5f64 696d 203d 3d20 6178  ouch(n_dim == ax
+0000bb90: 6973 2e6e 5f63 6861 6e6e 656c 2c20 6622  is.n_channel, f"
+0000bba0: 5472 616e 736c 6174 696f 6e28 7b6e 5f64  Translation({n_d
+0000bbb0: 696d 7d44 2920 616e 6420 6178 6973 6573  im}D) and axises
+0000bbc0: 287b 6178 6973 2e6e 5f63 6861 6e6e 656c  ({axis.n_channel
+0000bbd0: 7d44 2929 2069 6e20 7472 616e 732e 5269  }D)) in trans.Ri
+0000bbe0: 6769 6420 7368 6f75 6c64 2068 6176 6520  gid should have 
+0000bbf0: 7468 6520 7361 6d65 2064 696d 656e 7369  the same dimensi
+0000bc00: 6f6e 2e20 2229 0a20 2020 2020 2020 2069  on. ").        i
+0000bc10: 6620 6e5f 6469 6d20 6973 204e 6f6e 653a  f n_dim is None:
+0000bc20: 206e 5f64 696d 203d 2032 2069 6620 6178   n_dim = 2 if ax
+0000bc30: 6973 2069 7320 4e6f 6e65 2065 6c73 6520  is is None else 
+0000bc40: 330a 2020 2020 2020 2020 6966 2074 7261  3.        if tra
+0000bc50: 6e73 6c61 7469 6f6e 2069 7320 4e6f 6e65  nslation is None
+0000bc60: 3a20 7472 616e 736c 6174 696f 6e20 3d20  : translation = 
+0000bc70: 6274 2e7a 6572 6f73 285b 6e5f 6261 7463  bt.zeros([n_batc
+0000bc80: 685d 2c20 7b6e 5f64 696d 7d29 0a20 2020  h], {n_dim}).   
+0000bc90: 2020 2020 2069 6620 6365 6e74 6572 2069       if center i
+0000bca0: 7320 4e6f 6e65 3a20 6365 6e74 6572 203d  s None: center =
+0000bcb0: 2062 742e 7a65 726f 7328 5b6e 5f62 6174   bt.zeros([n_bat
+0000bcc0: 6368 5d2c 207b 6e5f 6469 6d7d 290a 2020  ch], {n_dim}).  
+0000bcd0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+0000bce0: 204e 6f77 2077 6520 6372 6561 7465 2074   Now we create t
+0000bcf0: 6865 206d 6174 7269 780a 2020 2020 2020  he matrix.      
+0000bd00: 2020 616e 676c 6520 3d20 616e 676c 652e    angle = angle.
+0000bd10: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
+0000bd20: 6365 6e74 6572 203d 2063 656e 7465 722e  center = center.
+0000bd30: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
+0000bd40: 7472 616e 736c 6174 696f 6e20 3d20 7472  translation = tr
+0000bd50: 616e 736c 6174 696f 6e2e 666c 6f61 7428  anslation.float(
+0000bd60: 290a 2020 2020 2020 2020 6966 206e 5f64  ).        if n_d
+0000bd70: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
+0000bd80: 2020 2020 2041 203d 2062 742e 7374 6163       A = bt.stac
+0000bd90: 6b28 6274 2e63 6f73 2861 6e67 6c65 292c  k(bt.cos(angle),
+0000bda0: 2062 742e 7369 6e28 616e 676c 6529 2c20   bt.sin(angle), 
+0000bdb0: 2d62 742e 7369 6e28 616e 676c 6529 2c20  -bt.sin(angle), 
+0000bdc0: 6274 2e63 6f73 2861 6e67 6c65 292c 202d  bt.cos(angle), -
+0000bdd0: 3129 2e73 706c 6974 6469 6d28 2d31 2c20  1).splitdim(-1, 
+0000bde0: 322c 2032 290a 2020 2020 2020 2020 656c  2, 2).        el
+0000bdf0: 6966 206e 5f64 696d 203d 3d20 333a 0a20  if n_dim == 3:. 
+0000be00: 2020 2020 2020 2020 2020 2061 7869 7320             axis 
+0000be10: 3d20 6178 6973 2e66 6c6f 6174 2829 0a20  = axis.float(). 
+0000be20: 2020 2020 2020 2020 2020 2041 203d 2062             A = b
+0000be30: 742e 6579 6528 5b6e 5f62 6174 6368 5d2c  t.eye([n_batch],
+0000be40: 206e 5f64 696d 2920 2b20 2831 202d 2062   n_dim) + (1 - b
+0000be50: 742e 636f 7328 616e 676c 6529 2920 2a20  t.cos(angle)) * 
+0000be60: 6274 2e63 726f 7373 5f6d 6174 7269 7828  bt.cross_matrix(
+0000be70: 6178 6973 2920 4020 6274 2e63 726f 7373  axis) @ bt.cross
+0000be80: 5f6d 6174 7269 7828 6178 6973 2920 2b20  _matrix(axis) + 
+0000be90: 6274 2e73 696e 2861 6e67 6c65 2920 2a20  bt.sin(angle) * 
+0000bea0: 6274 2e63 726f 7373 5f6d 6174 7269 7828  bt.cross_matrix(
+0000beb0: 6178 6973 290a 2020 2020 2020 2020 656c  axis).        el
+0000bec0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000bed0: 7261 6973 6520 4572 726f 7228 224e 6f74  raise Error("Not
+0000bee0: 496d 706c 656d 656e 7465 6422 2928 6622  Implemented")(f"
+0000bef0: 5269 6769 6420 7472 616e 7366 6f72 6d61  Rigid transforma
+0000bf00: 7469 6f6e 2069 6e20 6d69 636f 6d70 7574  tion in micomput
+0000bf10: 696e 6720 646f 6573 206e 6f74 2073 7570  ing does not sup
+0000bf20: 706f 7274 207b 6e5f 6469 6d7d 2064 696d  port {n_dim} dim
+0000bf30: 656e 7369 6f6e 616c 2074 7261 6e73 666f  ensional transfo
+0000bf40: 726d 7320 2832 2026 2033 4420 6f6e 6c79  rms (2 & 3D only
+0000bf50: 292e 2022 202b 200a 2020 2020 2020 2020  ). " + .        
+0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf80: 2250 6c65 6173 6520 636f 6e74 6163 7420  "Please contact 
+0000bf90: 7468 6520 6465 7665 6c6f 7065 7273 2069  the developers i
+0000bfa0: 6620 7468 6572 6520 6172 6520 6665 6173  f there are feas
+0000bfb0: 6962 6c65 2061 6c67 6f72 6974 686d 7320  ible algorithms 
+0000bfc0: 2845 7272 6f72 2043 6f64 653a 2054 3333  (Error Code: T33
+0000bfd0: 3329 2e20 5468 616e 6b20 796f 752e 2022  3). Thank you. "
+0000bfe0: 290a 2020 2020 2020 2020 6d61 7472 6978  ).        matrix
+0000bff0: 203d 2062 742e 6361 7428 6274 2e63 6174   = bt.cat(bt.cat
+0000c000: 2841 2c20 2828 7472 616e 736c 6174 696f  (A, ((translatio
+0000c010: 6e20 2b20 6365 6e74 6572 292e 7769 7468  n + center).with
+0000c020: 5f63 6861 6e6e 656c 6469 6d28 4e6f 6e65  _channeldim(None
+0000c030: 2920 2d20 4120 4020 6365 6e74 6572 2e77  ) - A @ center.w
+0000c040: 6974 685f 6368 616e 6e65 6c64 696d 284e  ith_channeldim(N
+0000c050: 6f6e 6529 292e 756e 7371 7565 657a 6528  one)).unsqueeze(
+0000c060: 2d31 292c 202d 3129 2c20 0a20 2020 2020  -1), -1), .     
+0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c080: 2020 2062 742e 6361 7428 6274 2e7a 6572     bt.cat(bt.zer
+0000c090: 6f73 286e 5f64 696d 292c 2062 742e 6f6e  os(n_dim), bt.on
+0000c0a0: 6573 2831 2929 2e75 6e73 7175 6565 7a65  es(1)).unsqueeze
+0000c0b0: 285b 5d2c 2031 292c 2031 290a 2020 2020  ([], 1), 1).    
+0000c0c0: 2020 2020 6966 2074 7261 6e73 5f73 7472      if trans_str
+0000c0d0: 6574 6368 2069 7320 6e6f 7420 4e6f 6e65  etch is not None
+0000c0e0: 3a20 6d61 7472 6978 5b2e 2e2e 2c20 3a6e  : matrix[..., :n
+0000c0f0: 5f64 696d 2c20 2d31 5d20 2a3d 2074 7261  _dim, -1] *= tra
+0000c100: 6e73 5f73 7472 6574 6368 0a20 2020 2020  ns_stretch.     
+0000c110: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+0000c120: 616e 6365 2873 7061 6369 6e67 2c20 7475  ance(spacing, tu
+0000c130: 706c 6529 3a20 7370 6163 696e 6720 3d20  ple): spacing = 
+0000c140: 746f 5f74 7570 6c65 2873 7061 6369 6e67  to_tuple(spacing
+0000c150: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+0000c160: 2873 7061 6369 6e67 2920 3d3d 2031 3a20  (spacing) == 1: 
+0000c170: 7370 6163 696e 6720 3d20 7370 6163 696e  spacing = spacin
+0000c180: 6720 2a20 6e5f 6469 6d0a 2020 2020 2020  g * n_dim.      
+0000c190: 2020 4120 3d20 6274 2e64 6961 6728 6261    A = bt.diag(ba
+0000c1a0: 746f 7263 685f 7465 6e73 6f72 286c 6973  torch_tensor(lis
+0000c1b0: 7428 7370 6163 696e 6729 202b 205b 312e  t(spacing) + [1.
+0000c1c0: 5d29 292e 756e 7371 7565 657a 6528 5b5d  ])).unsqueeze([]
+0000c1d0: 292e 6173 7479 7065 286d 6174 7269 7829  ).astype(matrix)
+0000c1e0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0000c1f0: 2e5f 5f69 6e69 745f 5f28 616e 676c 652c  .__init__(angle,
+0000c200: 2061 7869 732c 2074 7261 6e73 6c61 7469   axis, translati
+0000c210: 6f6e 2c20 6365 6e74 6572 3d63 656e 7465  on, center=cente
+0000c220: 722c 2074 7261 6e73 5f73 7472 6574 6368  r, trans_stretch
+0000c230: 3d74 7261 6e73 5f73 7472 6574 6368 2c20  =trans_stretch, 
+0000c240: 7370 6163 696e 673d 7370 6163 696e 6729  spacing=spacing)
+0000c250: 0a0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
+0000c260: 5f64 696d 203d 206e 5f64 696d 0a20 2020  _dim = n_dim.   
+0000c270: 2020 2020 2073 656c 662e 7472 616e 735f       self.trans_
+0000c280: 7374 7265 7463 6820 3d20 7472 616e 735f  stretch = trans_
+0000c290: 7374 7265 7463 680a 2020 2020 2020 2020  stretch.        
+0000c2a0: 7365 6c66 2e73 7061 6369 6e67 203d 2073  self.spacing = s
+0000c2b0: 7061 6369 6e67 0a20 2020 2020 2020 2073  pacing.        s
+0000c2c0: 656c 662e 6d61 7472 6978 203d 2041 2e69  elf.matrix = A.i
+0000c2d0: 6e76 2829 2040 206d 6174 7269 7820 4020  nv() @ matrix @ 
+0000c2e0: 410a 2020 2020 2020 2020 7365 6c66 2e62  A.        self.b
+0000c2f0: 6174 6368 5f70 6172 616d 2e61 7070 656e  atch_param.appen
+0000c300: 6428 276d 6174 7269 7827 290a 0a20 2020  d('matrix')..   
+0000c310: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
+0000c320: 6c66 2c20 5829 3a0a 2020 2020 2020 2020  lf, X):.        
+0000c330: 5820 3d20 7375 7065 7228 292e 5f5f 6361  X = super().__ca
+0000c340: 6c6c 5f5f 2858 290a 2020 2020 2020 2020  ll__(X).        
+0000c350: 6d61 7472 6978 203d 2073 656c 662e 6d61  matrix = self.ma
+0000c360: 7472 6978 0a20 2020 2020 2020 206e 5f64  trix.        n_d
+0000c370: 696d 203d 2073 656c 662e 6e5f 6469 6d0a  im = self.n_dim.
+0000c380: 2020 2020 2020 2020 4120 3d20 6d61 7472          A = matr
+0000c390: 6978 5b3a 2c20 3a6e 5f64 696d 2c20 3a6e  ix[:, :n_dim, :n
+0000c3a0: 5f64 696d 5d0a 2020 2020 2020 2020 6220  _dim].        b 
+0000c3b0: 3d20 6d61 7472 6978 5b3a 2c20 3a6e 5f64  = matrix[:, :n_d
+0000c3c0: 696d 2c20 6e5f 6469 6d5d 0a20 2020 2020  im, n_dim].     
+0000c3d0: 2020 2073 6861 7065 203d 2058 2e73 6861     shape = X.sha
+0000c3e0: 7065 0a20 2020 2020 2020 2059 203d 2028  pe.        Y = (
+0000c3f0: 4120 4020 582e 666c 6174 7465 6e28 292e  A @ X.flatten().
+0000c400: 6368 616e 6e65 6c5f 6469 6d5f 284e 6f6e  channel_dim_(Non
+0000c410: 6529 202b 2062 2e75 6e73 7175 6565 7a65  e) + b.unsqueeze
+0000c420: 282d 3129 292e 7669 6577 2873 6861 7065  (-1)).view(shape
+0000c430: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000c440: 2059 0a20 2020 200a 2020 2020 6465 6620   Y.    .    def 
+0000c450: 6166 6669 6e65 2873 656c 662c 206e 5f64  affine(self, n_d
+0000c460: 696d 3d4e 6f6e 6529 3a0a 2020 2020 2020  im=None):.      
+0000c470: 2020 6176 6f75 6368 286e 5f64 696d 2069    avouch(n_dim i
+0000c480: 7320 4e6f 6e65 206f 7220 7365 6c66 2e6e  s None or self.n
+0000c490: 5f64 696d 203d 3d20 6e5f 6469 6d29 0a20  _dim == n_dim). 
+0000c4a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000c4b0: 6c66 2e6d 6174 7269 780a 0a20 2020 2064  lf.matrix..    d
+0000c4c0: 6566 2069 6e76 2873 656c 6629 3a0a 2020  ef inv(self):.  
+0000c4d0: 2020 2020 2020 4120 3d20 6274 2e64 6961        A = bt.dia
+0000c4e0: 6728 6261 746f 7263 685f 7465 6e73 6f72  g(batorch_tensor
+0000c4f0: 286c 6973 7428 7365 6c66 2e73 7061 6369  (list(self.spaci
+0000c500: 6e67 2920 2b20 5b31 2e5d 2929 2e75 6e73  ng) + [1.])).uns
+0000c510: 7175 6565 7a65 285b 5d29 2e61 7374 7970  queeze([]).astyp
+0000c520: 6528 7365 6c66 2e6d 6174 7269 7829 0a20  e(self.matrix). 
+0000c530: 2020 2020 2020 2072 6574 7572 6e20 5269         return Ri
+0000c540: 6769 6428 4120 4020 6274 2e69 6e76 2873  gid(A @ bt.inv(s
+0000c550: 656c 662e 6d61 7472 6978 2920 4020 412e  elf.matrix) @ A.
+0000c560: 696e 7628 292c 2074 7261 6e73 5f73 7472  inv(), trans_str
+0000c570: 6574 6368 203d 2031 2c20 7370 6163 696e  etch = 1, spacin
+0000c580: 673d 7365 6c66 2e73 7061 6369 6e67 292e  g=self.spacing).
+0000c590: 6261 636b 7761 7264 5f28 7365 6c66 2e62  backward_(self.b
+0000c5a0: 6163 6b77 6172 6429 0a0a 4061 6c69 6173  ackward)..@alias
+0000c5b0: 2822 4166 6622 290a 636c 6173 7320 4166  ("Aff").class Af
+0000c5c0: 6669 6e65 2853 7061 7469 616c 5472 616e  fine(SpatialTran
+0000c5d0: 7366 6f72 6d61 7469 6f6e 293a 0a20 2020  sformation):.   
+0000c5e0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0000c5f0: 6c66 2c20 6d61 7472 6978 2c20 7472 616e  lf, matrix, tran
+0000c600: 735f 7374 7265 7463 683d 4e6f 6e65 2c20  s_stretch=None, 
+0000c610: 7370 6163 696e 673d 3129 3a0a 2020 2020  spacing=1):.    
+0000c620: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+0000c630: 4166 6669 6e65 2074 7261 6e73 666f 726d  Affine transform
+0000c640: 6174 696f 6e20 7769 7468 2072 6573 7065  ation with respe
+0000c650: 6374 2074 6f20 7472 616e 7366 6f72 6d61  ct to transforma
+0000c660: 7469 6f6e 206d 6174 7269 782e 0a20 2020  tion matrix..   
+0000c670: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
+0000c680: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
+0000c690: 2020 6d61 7472 6978 205b 6274 2e54 656e    matrix [bt.Ten
+0000c6a0: 736f 7220 6f72 206e 702e 6e75 6d70 795d  sor or np.numpy]
+0000c6b0: 3a20 7468 6520 6166 6669 6e65 206d 6174  : the affine mat
+0000c6c0: 7269 782e 200a 2020 2020 2020 2020 2020  rix. .          
+0000c6d0: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
+0000c6e0: 6261 7463 685d 2c20 6e5f 6469 6d20 2b20  batch], n_dim + 
+0000c6f0: 312c 206e 5f64 696d 202b 2031 290a 2020  1, n_dim + 1).  
+0000c700: 2020 2020 2020 2020 2020 7472 616e 735f            trans_
+0000c710: 7374 7265 7463 6820 5b69 6e74 5d3a 206f  stretch [int]: o
+0000c720: 6e6c 7920 7573 6564 2066 6f72 2069 7465  nly used for ite
+0000c730: 7261 7469 7665 2070 6172 616d 6574 6572  rative parameter
+0000c740: 2074 7261 696e 696e 672c 2031 2062 7920   training, 1 by 
+0000c750: 6465 6661 756c 742e 2032 3020 7365 656d  default. 20 seem
+0000c760: 7320 746f 2062 6520 6120 676f 6f64 2063  s to be a good c
+0000c770: 686f 6963 652e 200a 2020 2020 2020 2020  hoice. .        
+0000c780: 2020 2020 0a20 2020 2020 2020 2057 6865      .        Whe
+0000c790: 6e20 6974 2069 7320 6361 6c6c 6564 3a0a  n it is called:.
+0000c7a0: 2020 2020 2020 2020 2020 2020 5820 5b62              X [b
+0000c7b0: 742e 5465 6e73 6f72 5d3a 2043 6f6f 7264  t.Tensor]: Coord
+0000c7c0: 696e 6174 6573 2074 6f20 6265 2074 7261  inates to be tra
+0000c7d0: 6e73 666f 726d 6564 2e0a 2020 2020 2020  nsformed..      
+0000c7e0: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+0000c7f0: 285b 6e5f 6261 7463 683a 206f 7074 696f  ([n_batch: optio
+0000c800: 6e61 6c5d 2c20 7b6e 5f64 696d 7d2c 206e  nal], {n_dim}, n
+0000c810: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
+0000c820: 7229 0a20 2020 2020 2020 2020 2020 206f  r).            o
+0000c830: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
+0000c840: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
+0000c850: 6564 2063 6f6f 7264 696e 6174 6573 2e0a  ed coordinates..
+0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c870: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
+0000c880: 2c20 7b6e 5f64 696d 7d2c 206e 5f31 2c20  , {n_dim}, n_1, 
+0000c890: 6e5f 322c 202e 2e2e 2c20 6e5f 7229 0a20  n_2, ..., n_r). 
+0000c8a0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0000c8b0: 2020 206d 6174 7269 7820 3d20 6261 746f     matrix = bato
+0000c8c0: 7263 685f 7465 6e73 6f72 286d 6174 7269  rch_tensor(matri
+0000c8d0: 7829 0a20 2020 2020 2020 206e 5f64 696d  x).        n_dim
+0000c8e0: 203d 206d 6174 7269 782e 7369 7a65 282d   = matrix.size(-
+0000c8f0: 3129 202d 2031 0a20 2020 2020 2020 2069  1) - 1.        i
+0000c900: 6620 6d61 7472 6978 2e6e 5f64 696d 203c  f matrix.n_dim <
+0000c910: 3d20 3220 616e 6420 6e6f 7420 6d61 7472  = 2 and not matr
+0000c920: 6978 2e68 6173 5f62 6174 6368 3a20 6d61  ix.has_batch: ma
+0000c930: 7472 6978 203d 206d 6174 7269 782e 756e  trix = matrix.un
+0000c940: 7371 7565 657a 6528 5b5d 290a 2020 2020  squeeze([]).    
+0000c950: 2020 2020 6966 206d 6174 7269 782e 6e5f      if matrix.n_
+0000c960: 6469 6d20 3d3d 2033 2061 6e64 206e 6f74  dim == 3 and not
+0000c970: 206d 6174 7269 782e 6861 735f 6261 7463   matrix.has_batc
+0000c980: 6820 616e 6420 6d61 7472 6978 2e73 6861  h and matrix.sha
+0000c990: 7065 5b31 5d20 3d3d 206d 6174 7269 782e  pe[1] == matrix.
+0000c9a0: 7368 6170 655b 325d 3a20 6d61 7472 6978  shape[2]: matrix
+0000c9b0: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+0000c9c0: 203d 2030 0a20 2020 2020 2020 2061 766f   = 0.        avo
+0000c9d0: 7563 6828 6d61 7472 6978 2e68 6173 5f62  uch(matrix.has_b
+0000c9e0: 6174 6368 2c20 6622 506c 6561 7365 2075  atch, f"Please u
+0000c9f0: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
+0000ca00: 7220 6f66 2073 697a 6520 285b 6e5f 6261  r of size ([n_ba
+0000ca10: 7463 685d 2c20 6e5f 6469 6d20 2b20 312c  tch], n_dim + 1,
+0000ca20: 206e 5f64 696d 202b 2031 2920 666f 7220   n_dim + 1) for 
+0000ca30: 4166 6669 6e65 2070 6172 616d 6574 6572  Affine parameter
+0000ca40: 732c 2069 6e73 7465 6164 206f 6620 7b6d  s, instead of {m
+0000ca50: 6174 7269 782e 7368 6170 657d 2e20 2229  atrix.shape}. ")
+0000ca60: 0a20 2020 2020 2020 2069 6620 7472 616e  .        if tran
+0000ca70: 735f 7374 7265 7463 6820 6973 206e 6f74  s_stretch is not
+0000ca80: 204e 6f6e 653a 206d 6174 7269 785b 2e2e   None: matrix[..
+0000ca90: 2e2c 203a 6e5f 6469 6d2c 202d 315d 202a  ., :n_dim, -1] *
+0000caa0: 3d20 7472 616e 735f 7374 7265 7463 680a  = trans_stretch.
+0000cab0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+0000cac0: 7369 6e73 7461 6e63 6528 7370 6163 696e  sinstance(spacin
+0000cad0: 672c 2074 7570 6c65 293a 2073 7061 6369  g, tuple): spaci
+0000cae0: 6e67 203d 2074 6f5f 7475 706c 6528 7370  ng = to_tuple(sp
+0000caf0: 6163 696e 6729 0a20 2020 2020 2020 2069  acing).        i
+0000cb00: 6620 6c65 6e28 7370 6163 696e 6729 203d  f len(spacing) =
+0000cb10: 3d20 313a 2073 7061 6369 6e67 203d 2073  = 1: spacing = s
+0000cb20: 7061 6369 6e67 202a 206e 5f64 696d 0a20  pacing * n_dim. 
+0000cb30: 2020 2020 2020 2041 203d 2062 742e 6469         A = bt.di
+0000cb40: 6167 2862 6174 6f72 6368 5f74 656e 736f  ag(batorch_tenso
+0000cb50: 7228 6c69 7374 2873 7061 6369 6e67 2920  r(list(spacing) 
+0000cb60: 2b20 5b31 2e5d 2929 2e75 6e73 7175 6565  + [1.])).unsquee
+0000cb70: 7a65 285b 5d29 2e61 7374 7970 6528 6d61  ze([]).astype(ma
+0000cb80: 7472 6978 290a 2020 2020 2020 2020 7375  trix).        su
+0000cb90: 7065 7228 292e 5f5f 696e 6974 5f5f 286d  per().__init__(m
+0000cba0: 6174 7269 782c 2074 7261 6e73 5f73 7472  atrix, trans_str
+0000cbb0: 6574 6368 3d74 7261 6e73 5f73 7472 6574  etch=trans_stret
+0000cbc0: 6368 2c20 7370 6163 696e 673d 7370 6163  ch, spacing=spac
+0000cbd0: 696e 6729 0a0a 2020 2020 2020 2020 7365  ing)..        se
+0000cbe0: 6c66 2e6e 5f64 696d 203d 206d 6174 7269  lf.n_dim = matri
+0000cbf0: 782e 7369 7a65 282d 3129 202d 2031 0a20  x.size(-1) - 1. 
+0000cc00: 2020 2020 2020 2073 656c 662e 7472 616e         self.tran
+0000cc10: 735f 7374 7265 7463 6820 3d20 7472 616e  s_stretch = tran
+0000cc20: 735f 7374 7265 7463 680a 2020 2020 2020  s_stretch.      
+0000cc30: 2020 7365 6c66 2e73 7061 6369 6e67 203d    self.spacing =
+0000cc40: 2073 7061 6369 6e67 0a20 2020 2020 2020   spacing.       
+0000cc50: 2073 656c 662e 6d61 7472 6978 203d 2041   self.matrix = A
+0000cc60: 2e69 6e76 2829 2040 206d 6174 7269 7820  .inv() @ matrix 
+0000cc70: 4020 410a 2020 2020 2020 2020 7365 6c66  @ A.        self
+0000cc80: 2e62 6174 6368 5f70 6172 616d 2e61 7070  .batch_param.app
+0000cc90: 656e 6428 276d 6174 7269 7827 290a 0a20  end('matrix').. 
+0000cca0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
+0000ccb0: 7365 6c66 2c20 5829 3a0a 2020 2020 2020  self, X):.      
+0000ccc0: 2020 5820 3d20 7375 7065 7228 292e 5f5f    X = super().__
+0000ccd0: 6361 6c6c 5f5f 2858 290a 2020 2020 2020  call__(X).      
+0000cce0: 2020 6d61 7472 6978 203d 2073 656c 662e    matrix = self.
+0000ccf0: 6d61 7472 6978 2e66 6c6f 6174 2829 0a20  matrix.float(). 
+0000cd00: 2020 2020 2020 206e 5f64 696d 203d 2073         n_dim = s
+0000cd10: 656c 662e 6e5f 6469 6d0a 2020 2020 2020  elf.n_dim.      
+0000cd20: 2020 4120 3d20 6d61 7472 6978 5b3a 2c20    A = matrix[:, 
+0000cd30: 3a6e 5f64 696d 2c20 3a6e 5f64 696d 5d0a  :n_dim, :n_dim].
+0000cd40: 2020 2020 2020 2020 6220 3d20 6d61 7472          b = matr
+0000cd50: 6978 5b3a 2c20 3a6e 5f64 696d 2c20 6e5f  ix[:, :n_dim, n_
+0000cd60: 6469 6d5d 0a20 2020 2020 2020 2073 6861  dim].        sha
+0000cd70: 7065 203d 2058 2e73 6861 7065 0a20 2020  pe = X.shape.   
+0000cd80: 2020 2020 2059 203d 2028 4120 4020 582e       Y = (A @ X.
+0000cd90: 666c 6174 7465 6e28 292e 6368 616e 6e65  flatten().channe
+0000cda0: 6c5f 6469 6d5f 284e 6f6e 6529 202b 2062  l_dim_(None) + b
+0000cdb0: 2e75 6e73 7175 6565 7a65 282d 3129 292e  .unsqueeze(-1)).
+0000cdc0: 7669 6577 2873 6861 7065 290a 2020 2020  view(shape).    
+0000cdd0: 2020 2020 7265 7475 726e 2059 0a20 2020      return Y.   
+0000cde0: 200a 2020 2020 6465 6620 6166 6669 6e65   .    def affine
+0000cdf0: 2873 656c 662c 206e 5f64 696d 3d4e 6f6e  (self, n_dim=Non
+0000ce00: 6529 3a0a 2020 2020 2020 2020 6176 6f75  e):.        avou
+0000ce10: 6368 286e 5f64 696d 2069 7320 4e6f 6e65  ch(n_dim is None
+0000ce20: 206f 7220 7365 6c66 2e6e 5f64 696d 203d   or self.n_dim =
+0000ce30: 3d20 6e5f 6469 6d29 0a20 2020 2020 2020  = n_dim).       
+0000ce40: 2072 6574 7572 6e20 7365 6c66 2e6d 6174   return self.mat
+0000ce50: 7269 780a 0a20 2020 2064 6566 2069 6e76  rix..    def inv
+0000ce60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ce70: 4120 3d20 6274 2e64 6961 6728 6261 746f  A = bt.diag(bato
+0000ce80: 7263 685f 7465 6e73 6f72 286c 6973 7428  rch_tensor(list(
+0000ce90: 7365 6c66 2e73 7061 6369 6e67 2920 2b20  self.spacing) + 
+0000cea0: 5b31 2e5d 2929 2e75 6e73 7175 6565 7a65  [1.])).unsqueeze
+0000ceb0: 285b 5d29 2e61 7374 7970 6528 7365 6c66  ([]).astype(self
+0000cec0: 2e6d 6174 7269 7829 0a20 2020 2020 2020  .matrix).       
+0000ced0: 2072 6574 7572 6e20 4166 6669 6e65 2841   return Affine(A
+0000cee0: 2040 2062 742e 696e 7628 7365 6c66 2e6d   @ bt.inv(self.m
+0000cef0: 6174 7269 7829 2040 2041 2e69 6e76 2829  atrix) @ A.inv()
+0000cf00: 2c20 7472 616e 735f 7374 7265 7463 6820  , trans_stretch 
+0000cf10: 3d20 312c 2073 7061 6369 6e67 3d73 656c  = 1, spacing=sel
+0000cf20: 662e 7370 6163 696e 6729 2e62 6163 6b77  f.spacing).backw
+0000cf30: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
+0000cf40: 7264 290a 0a40 616c 6961 7328 226c 6f67  rd)..@alias("log
+0000cf50: 4575 2229 0a63 6c61 7373 2050 6f6c 7941  Eu").class PolyA
+0000cf60: 6666 696e 6528 5370 6174 6961 6c54 7261  ffine(SpatialTra
+0000cf70: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
+0000cf80: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000cf90: 656c 662c 2064 6d61 7472 6963 6573 2c20  elf, dmatrices, 
+0000cfa0: 6d61 736b 732c 206f 7264 6572 3d32 2c20  masks, order=2, 
+0000cfb0: 6973 5f69 6e76 3d46 616c 7365 2c20 7472  is_inv=False, tr
+0000cfc0: 616e 735f 7374 7265 7463 683d 4e6f 6e65  ans_stretch=None
+0000cfd0: 293a 0a20 2020 2020 2020 2027 2727 0a20  ):.        '''. 
+0000cfe0: 2020 2020 2020 2050 6f6c 7920 6166 6669         Poly affi
+0000cff0: 6e65 2074 7261 6e73 666f 726d 6174 696f  ne transformatio
+0000d000: 6e20 7769 7468 2072 6573 7065 6374 2074  n with respect t
+0000d010: 6f20 7472 616e 7366 6f72 6d61 7469 6f6e  o transformation
+0000d020: 206d 6174 7269 6365 7320 5b31 5d2e 0a20   matrices [1].. 
+0000d030: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
+0000d040: 2064 6d61 7472 6963 6573 2066 6f72 2074   dmatrices for t
+0000d050: 6869 7320 7472 616e 666f 726d 6174 696f  his tranformatio
+0000d060: 6e20 4953 204e 4f54 2074 6865 2061 6374  n IS NOT the act
+0000d070: 7561 6c20 6166 6669 6e65 206d 6174 7269  ual affine matri
+0000d080: 6365 732c 2062 7574 2049 5320 6120 6469  ces, but IS a di
+0000d090: 6666 6572 656e 7469 6174 696f 6e20 696e  fferentiation in
+0000d0a0: 7374 6561 642e 0a20 2020 2020 2020 200a  stead..        .
+0000d0b0: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
+0000d0c0: 2020 2020 2020 2020 2020 2020 646d 6174              dmat
+0000d0d0: 7269 6365 7320 5b62 742e 5465 6e73 6f72  rices [bt.Tensor
+0000d0e0: 206f 7220 6e70 2e6e 756d 7079 5d3a 204f   or np.numpy]: O
+0000d0f0: 6e65 2061 6666 696e 6520 6d61 7472 6978  ne affine matrix
+0000d100: 2066 6f72 2065 6163 6820 7265 6769 6f6e   for each region
+0000d110: 2e20 0a20 2020 2020 2020 2020 2020 2020  . .             
+0000d120: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
+0000d130: 6368 5d2c 207b 6e5f 7265 6769 6f6e 7d2c  ch], {n_region},
+0000d140: 206e 5f64 696d 202b 2031 2c20 6e5f 6469   n_dim + 1, n_di
+0000d150: 6d20 2b20 3129 0a20 2020 2020 2020 2020  m + 1).         
+0000d160: 2020 206d 6173 6b73 205b 6274 2e54 656e     masks [bt.Ten
+0000d170: 736f 7220 6f72 206e 702e 6e75 6d70 795d  sor or np.numpy]
+0000d180: 3a20 4f6e 6520 302d 3120 6d61 736b 2066  : One 0-1 mask f
+0000d190: 6f72 2065 6163 6820 7265 6769 6f6e 2e20  or each region. 
+0000d1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d1b0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+0000d1c0: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
+0000d1d0: 4031 2c20 6e40 322c 202e 2e2e 2c20 6e40  @1, n@2, ..., n@
+0000d1e0: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
+0000d1f0: 2020 206f 7264 6572 205b 696e 745d 3a20     order [int]: 
+0000d200: 7468 6520 6f72 6465 7220 6f66 2069 6e74  the order of int
+0000d210: 6572 706f 6c61 7469 6f6e 2063 6f65 6666  erpolation coeff
+0000d220: 6963 6965 6e74 2e20 5468 6520 696e 666c  icient. The infl
+0000d230: 7565 6e63 6520 6f66 2061 6e20 6166 6669  uence of an affi
+0000d240: 6e65 2064 6563 6179 7320 6174 2061 2072  ne decays at a r
+0000d250: 6174 6520 6f66 2031 202f 2064 6973 7461  ate of 1 / dista
+0000d260: 6e63 655e 6f72 6465 722e 0a20 2020 2020  nce^order..     
+0000d270: 2020 2020 2020 2074 7261 6e73 5f73 7472         trans_str
+0000d280: 6574 6368 205b 696e 745d 3a20 6f6e 6c79  etch [int]: only
+0000d290: 2075 7365 6420 666f 7220 6974 6572 6174   used for iterat
+0000d2a0: 6976 6520 7061 7261 6d65 7465 7220 7472  ive parameter tr
+0000d2b0: 6169 6e69 6e67 2c20 3120 6279 2064 6566  aining, 1 by def
+0000d2c0: 6175 6c74 2e20 3230 2073 6565 6d73 2074  ault. 20 seems t
+0000d2d0: 6f20 6265 2061 2067 6f6f 6420 6368 6f69  o be a good choi
+0000d2e0: 6365 2e20 200a 2020 2020 2020 2020 2020  ce.  .          
+0000d2f0: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
+0000d300: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
+0000d310: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
+0000d320: 5465 6e73 6f72 5d3a 2043 6f6f 7264 696e  Tensor]: Coordin
+0000d330: 6174 6573 2074 6f20 6265 2074 7261 6e73  ates to be trans
+0000d340: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
+0000d350: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+0000d360: 6e5f 6261 7463 683a 206f 7074 696f 6e61  n_batch: optiona
+0000d370: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 4031  l], {n_dim}, n@1
+0000d380: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+0000d390: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+0000d3a0: 206f 7574 7075 7420 5b62 742e 5465 6e73   output [bt.Tens
+0000d3b0: 6f72 5d3a 2054 6865 2074 7261 6e73 666f  or]: The transfo
+0000d3c0: 726d 6564 2063 6f6f 7264 696e 6174 6573  rmed coordinates
+0000d3d0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d3e0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+0000d3f0: 685d 2c20 7b6e 5f64 696d 7d2c 206e 4031  h], {n_dim}, n@1
+0000d400: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+0000d410: 6469 6d29 0a0a 2020 2020 2020 2020 5b31  dim)..        [1
+0000d420: 5d20 4172 7369 676e 7920 5620 2c20 436f  ] Arsigny V , Co
+0000d430: 6d6d 6f77 6963 6b20 4f20 2c20 4179 6163  mmowick O , Ayac
+0000d440: 6865 204e 202c 2065 7420 616c 2e20 4120  he N , et al. A 
+0000d450: 4661 7374 2061 6e64 204c 6f67 2d45 7563  Fast and Log-Euc
+0000d460: 6c69 6465 616e 2050 6f6c 7961 6666 696e  lidean Polyaffin
+0000d470: 6520 4672 616d 6577 6f72 6b20 666f 7220  e Framework for 
+0000d480: 4c6f 6361 6c6c 7920 0a20 2020 2020 2020  Locally .       
+0000d490: 2020 2020 204c 696e 6561 7220 5265 6769       Linear Regi
+0000d4a0: 7374 7261 7469 6f6e 5b4a 5d2e 204a 6f75  stration[J]. Jou
+0000d4b0: 726e 616c 206f 6620 4d61 7468 656d 6174  rnal of Mathemat
+0000d4c0: 6963 616c 2049 6d61 6769 6e67 2026 2056  ical Imaging & V
+0000d4d0: 6973 696f 6e2c 2032 3030 392c 2033 3328  ision, 2009, 33(
+0000d4e0: 3229 3a32 3232 2d32 3338 2e0a 2020 2020  2):222-238..    
+0000d4f0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+0000d500: 696d 706f 7274 2053 696d 706c 6549 544b  import SimpleITK
+0000d510: 2061 7320 7369 746b 0a20 2020 2020 2020   as sitk.       
+0000d520: 2066 726f 6d20 2e66 756e 6373 2069 6d70   from .funcs imp
+0000d530: 6f72 7420 6469 6c61 7465 2c20 6469 7374  ort dilate, dist
+0000d540: 616e 6365 5f6d 6170 0a20 2020 2020 2020  ance_map.       
+0000d550: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000d560: 6365 2864 6d61 7472 6963 6573 2c20 6274  ce(dmatrices, bt
+0000d570: 2e54 656e 736f 7229 3a20 646d 6174 7269  .Tensor): dmatri
+0000d580: 6365 7320 3d20 6274 2e74 656e 736f 7228  ces = bt.tensor(
+0000d590: 646d 6174 7269 6365 7329 0a20 2020 2020  dmatrices).     
+0000d5a0: 2020 2069 6620 646d 6174 7269 6365 732e     if dmatrices.
+0000d5b0: 6e5f 6469 6d20 3c3d 2033 2061 6e64 206e  n_dim <= 3 and n
+0000d5c0: 6f74 2064 6d61 7472 6963 6573 2e68 6173  ot dmatrices.has
+0000d5d0: 5f62 6174 6368 3a20 646d 6174 7269 6365  _batch: dmatrice
+0000d5e0: 7320 3d20 646d 6174 7269 6365 732e 756e  s = dmatrices.un
+0000d5f0: 7371 7565 657a 6528 5b5d 290a 2020 2020  squeeze([]).    
+0000d600: 2020 2020 6966 2064 6d61 7472 6963 6573      if dmatrices
+0000d610: 2e6e 5f64 696d 203c 3d20 3320 616e 6420  .n_dim <= 3 and 
+0000d620: 6e6f 7420 646d 6174 7269 6365 732e 6861  not dmatrices.ha
+0000d630: 735f 6368 616e 6e65 6c3a 2064 6d61 7472  s_channel: dmatr
+0000d640: 6963 6573 203d 2064 6d61 7472 6963 6573  ices = dmatrices
+0000d650: 2e75 6e73 7175 6565 7a65 287b 7d29 0a20  .unsqueeze({}). 
+0000d660: 2020 2020 2020 2069 6620 646d 6174 7269         if dmatri
+0000d670: 6365 732e 6e5f 6469 6d20 3d3d 2034 2061  ces.n_dim == 4 a
+0000d680: 6e64 2064 6d61 7472 6963 6573 2e73 6861  nd dmatrices.sha
+0000d690: 7065 5b32 5d20 3d3d 2064 6d61 7472 6963  pe[2] == dmatric
+0000d6a0: 6573 2e73 6861 7065 5b33 5d3a 0a20 2020  es.shape[3]:.   
+0000d6b0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000d6c0: 646d 6174 7269 6365 732e 6861 735f 6261  dmatrices.has_ba
+0000d6d0: 7463 683a 2064 6d61 7472 6963 6573 2e62  tch: dmatrices.b
+0000d6e0: 6174 6368 5f64 696d 656e 7369 6f6e 203d  atch_dimension =
+0000d6f0: 2030 0a20 2020 2020 2020 2020 2020 2069   0.            i
+0000d700: 6620 6e6f 7420 646d 6174 7269 6365 732e  f not dmatrices.
+0000d710: 6861 735f 6368 616e 6e65 6c3a 2064 6d61  has_channel: dma
+0000d720: 7472 6963 6573 2e63 6861 6e6e 656c 5f64  trices.channel_d
+0000d730: 696d 656e 7369 6f6e 203d 2031 0a20 2020  imension = 1.   
+0000d740: 2020 2020 2061 766f 7563 6828 646d 6174       avouch(dmat
+0000d750: 7269 6365 732e 6861 735f 6261 7463 6820  rices.has_batch 
+0000d760: 616e 6420 646d 6174 7269 6365 732e 6861  and dmatrices.ha
+0000d770: 735f 6368 616e 6e65 6c2c 2022 506c 6561  s_channel, "Plea
+0000d780: 7365 2075 7365 2062 6174 6f72 6368 2074  se use batorch t
+0000d790: 656e 736f 7220 6f66 2073 697a 6520 285b  ensor of size ([
+0000d7a0: 6e5f 6261 7463 685d 2c20 7b6e 5f72 6567  n_batch], {n_reg
+0000d7b0: 696f 6e7d 2c22 202b 0a20 2020 2020 2020  ion}," +.       
+0000d7c0: 2020 2020 2020 2020 6622 6e5f 6469 6d20          f"n_dim 
+0000d7d0: 2b20 312c 206e 5f64 696d 202b 2031 2920  + 1, n_dim + 1) 
+0000d7e0: 666f 7220 506f 6c79 4166 6669 6e65 2070  for PolyAffine p
+0000d7f0: 6172 616d 6574 6572 732c 2069 6e73 7465  arameters, inste
+0000d800: 6164 206f 6620 7b64 6d61 7472 6963 6573  ad of {dmatrices
+0000d810: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+0000d820: 2020 2020 6966 2074 7261 6e73 5f73 7472      if trans_str
+0000d830: 6574 6368 2069 7320 6e6f 7420 4e6f 6e65  etch is not None
+0000d840: 3a20 646d 6174 7269 6365 735b 2e2e 2e2c  : dmatrices[...,
+0000d850: 203a 6e5f 6469 6d2c 202d 315d 202a 3d20   :n_dim, -1] *= 
+0000d860: 7472 616e 735f 7374 7265 7463 680a 2020  trans_stretch.  
+0000d870: 2020 2020 2020 6e5f 6469 6d20 3d20 646d        n_dim = dm
+0000d880: 6174 7269 6365 732e 7369 7a65 282d 3129  atrices.size(-1)
+0000d890: 202d 2031 0a20 2020 2020 2020 2069 6620   - 1.        if 
+0000d8a0: 6e6f 7420 6973 696e 7374 616e 6365 286d  not isinstance(m
+0000d8b0: 6173 6b73 2c20 6274 2e54 656e 736f 7229  asks, bt.Tensor)
+0000d8c0: 3a20 6d61 736b 7320 3d20 6274 2e74 656e  : masks = bt.ten
+0000d8d0: 736f 7228 6d61 736b 7329 0a20 2020 2020  sor(masks).     
+0000d8e0: 2020 2069 6620 6d61 736b 732e 6e5f 6469     if masks.n_di
+0000d8f0: 6d20 3c3d 206e 5f64 696d 202b 2031 2061  m <= n_dim + 1 a
+0000d900: 6e64 206e 6f74 206d 6173 6b73 2e68 6173  nd not masks.has
+0000d910: 5f62 6174 6368 3a20 6d61 736b 7320 3d20  _batch: masks = 
+0000d920: 6d61 736b 732e 756e 7371 7565 657a 6528  masks.unsqueeze(
+0000d930: 5b5d 290a 2020 2020 2020 2020 6966 206d  []).        if m
+0000d940: 6173 6b73 2e6e 5f64 696d 203c 3d20 6e5f  asks.n_dim <= n_
+0000d950: 6469 6d20 2b20 3120 616e 6420 6e6f 7420  dim + 1 and not 
+0000d960: 6d61 736b 732e 6861 735f 6368 616e 6e65  masks.has_channe
+0000d970: 6c3a 206d 6173 6b73 203d 206d 6173 6b73  l: masks = masks
+0000d980: 2e75 6e73 7175 6565 7a65 287b 7d29 0a20  .unsqueeze({}). 
+0000d990: 2020 2020 2020 2069 6620 6d61 736b 732e         if masks.
+0000d9a0: 6e5f 6469 6d20 3d3d 206e 5f64 696d 202b  n_dim == n_dim +
+0000d9b0: 2032 2061 6e64 206e 6f74 206d 6173 6b73   2 and not masks
+0000d9c0: 2e68 6173 5f62 6174 6368 3a20 6d61 736b  .has_batch: mask
+0000d9d0: 732e 6261 7463 685f 6469 6d65 6e73 696f  s.batch_dimensio
+0000d9e0: 6e20 3d20 300a 2020 2020 2020 2020 6966  n = 0.        if
+0000d9f0: 206d 6173 6b73 2e6e 5f64 696d 203d 3d20   masks.n_dim == 
+0000da00: 6e5f 6469 6d20 2b20 3220 616e 6420 6e6f  n_dim + 2 and no
+0000da10: 7420 6d61 736b 732e 6861 735f 6368 616e  t masks.has_chan
+0000da20: 6e65 6c3a 206d 6173 6b73 2e63 6861 6e6e  nel: masks.chann
+0000da30: 656c 5f64 696d 656e 7369 6f6e 203d 2031  el_dimension = 1
+0000da40: 0a20 2020 2020 2020 2061 766f 7563 6828  .        avouch(
+0000da50: 6d61 736b 732e 6861 735f 6261 7463 6820  masks.has_batch 
+0000da60: 616e 6420 6d61 736b 732e 6861 735f 6368  and masks.has_ch
+0000da70: 616e 6e65 6c2c 2022 506c 6561 7365 2075  annel, "Please u
+0000da80: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
+0000da90: 7220 6f66 2073 697a 6520 285b 6e5f 6261  r of size ([n_ba
+0000daa0: 7463 685d 2c20 7b6e 5f72 6567 696f 6e7d  tch], {n_region}
+0000dab0: 2c22 202b 0a20 2020 2020 2020 2020 2020  ," +.           
+0000dac0: 2020 2020 6622 6e40 312c 206e 4032 2c20      f"n@1, n@2, 
+0000dad0: 2e2e 2e2c 206e 406e 5f64 696d 2920 666f  ..., n@n_dim) fo
+0000dae0: 7220 506f 6c79 4166 6669 6e65 2070 6172  r PolyAffine par
+0000daf0: 616d 6574 6572 732c 2069 6e73 7465 6164  ameters, instead
+0000db00: 206f 6620 7b6d 6173 6b73 2e73 6861 7065   of {masks.shape
+0000db10: 7d2e 2022 290a 0a20 2020 2020 2020 2023  }. ")..        #
+0000db20: 2070 7265 7072 6f63 6573 7320 6d61 736b   preprocess mask
+0000db30: 7320 285b 6e5f 6261 7463 685d 2c20 7b6e  s ([n_batch], {n
+0000db40: 5f72 6567 696f 6e7d 2c20 6e40 312c 206e  _region}, n@1, n
+0000db50: 4032 2c20 2e2e 2e2c 206e 406e 5f64 696d  @2, ..., n@n_dim
+0000db60: 290a 2020 2020 2020 2020 6e5f 6261 7463  ).        n_batc
+0000db70: 6820 3d20 6d61 736b 732e 6e5f 6261 7463  h = masks.n_batc
+0000db80: 680a 2020 2020 2020 2020 6e5f 7265 6769  h.        n_regi
+0000db90: 6f6e 203d 206d 6173 6b73 2e6e 5f63 6861  on = masks.n_cha
+0000dba0: 6e6e 656c 0a20 2020 2020 2020 2064 6973  nnel.        dis
+0000dbb0: 203d 2064 6973 7461 6e63 655f 6d61 7028   = distance_map(
+0000dbc0: 6d61 736b 7329 0a20 2020 2020 2020 2064  masks).        d
+0000dbd0: 6973 203d 2028 6469 7320 2b20 3129 2e63  is = (dis + 1).c
+0000dbe0: 6c61 6d70 2830 290a 2020 2020 2020 2020  lamp(0).        
+0000dbf0: 2320 696d 706f 7274 206d 6963 6f6d 7075  # import micompu
+0000dc00: 7469 6e67 2e70 6c6f 7420 6173 2070 6c74  ting.plot as plt
+0000dc10: 0a20 2020 2020 2020 2023 2070 6c74 2e73  .        # plt.s
+0000dc20: 7562 706c 6f74 7328 3229 0a20 2020 2020  ubplots(2).     
+0000dc30: 2020 2023 2070 6c74 2e69 6d73 7368 6f77     # plt.imsshow
+0000dc40: 2864 6973 5b30 2c20 305d 2c20 6469 735b  (dis[0, 0], dis[
+0000dc50: 302c 2031 5d29 0a20 2020 2020 2020 2023  0, 1]).        #
+0000dc60: 2070 6c74 2e73 686f 7728 290a 2020 2020   plt.show().    
+0000dc70: 2020 2020 7765 6967 6874 7320 3d20 3120      weights = 1 
+0000dc80: 2f20 2864 6973 202a 2a20 6f72 6465 7220  / (dis ** order 
+0000dc90: 2b20 3165 2d35 290a 2020 2020 2020 2020  + 1e-5).        
+0000dca0: 7765 6967 6874 7320 3d20 7765 6967 6874  weights = weight
+0000dcb0: 7320 2f20 7765 6967 6874 732e 7375 6d28  s / weights.sum(
+0000dcc0: 7b7d 2920 2320 285b 6e5f 6261 7463 685d  {}) # ([n_batch]
+0000dcd0: 2c20 7b6e 5f72 6567 696f 6e7d 2c20 6e40  , {n_region}, n@
+0000dce0: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+0000dcf0: 5f64 696d 290a 2020 2020 2020 2020 0a20  _dim).        . 
+0000dd00: 2020 2020 2020 2023 2023 2064 6570 7265         # # depre
+0000dd10: 6361 7465 6420 7072 6570 726f 6365 7373  cated preprocess
+0000dd20: 206f 6620 6d61 736b 730a 2020 2020 2020   of masks.      
+0000dd30: 2020 2320 6d61 736b 7320 3d20 6d61 736b    # masks = mask
+0000dd40: 732e 6e75 6d70 7928 292e 6173 7479 7065  s.numpy().astype
+0000dd50: 286e 702e 696e 7429 0a20 2020 2020 2020  (np.int).       
+0000dd60: 2023 206e 5f62 6174 6368 2c20 6e5f 7265   # n_batch, n_re
+0000dd70: 6769 6f6e 2c20 2a5f 203d 206d 6173 6b73  gion, *_ = masks
+0000dd80: 2e73 6861 7065 0a20 2020 2020 2020 2023  .shape.        #
+0000dd90: 205f 6469 735f 6d61 7020 3d20 6274 2e7a   _dis_map = bt.z
+0000dda0: 6572 6f73 282a 6d61 736b 732e 7368 6170  eros(*masks.shap
+0000ddb0: 6529 0a20 2020 2020 2020 2023 2066 6f72  e).        # for
+0000ddc0: 2069 2069 6e20 7261 6e67 6528 6e5f 6261   i in range(n_ba
+0000ddd0: 7463 6829 3a0a 2020 2020 2020 2020 2320  tch):.        # 
+0000dde0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+0000ddf0: 6765 286e 5f72 6567 696f 6e29 3a0a 2020  ge(n_region):.  
+0000de00: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0000de10: 6d61 736b 5f69 6d61 6765 203d 2073 6974  mask_image = sit
+0000de20: 6b2e 4765 7449 6d61 6765 4672 6f6d 4172  k.GetImageFromAr
+0000de30: 7261 7928 6d61 736b 735b 692c 206a 5d2c  ray(masks[i, j],
+0000de40: 2069 7356 6563 746f 7220 3d20 4661 6c73   isVector = Fals
+0000de50: 6529 0a20 2020 2020 2020 2023 2020 2020  e).        #    
+0000de60: 2020 2020 2064 6973 5f6d 6170 203d 2073       dis_map = s
+0000de70: 6974 6b2e 4765 7441 7272 6179 5669 6577  itk.GetArrayView
+0000de80: 4672 6f6d 496d 6167 6528 7369 746b 2e53  FromImage(sitk.S
+0000de90: 6967 6e65 644d 6175 7265 7244 6973 7461  ignedMaurerDista
+0000dea0: 6e63 654d 6170 286d 6173 6b5f 696d 6167  nceMap(mask_imag
+0000deb0: 652c 2073 7175 6172 6564 4469 7374 616e  e, squaredDistan
+0000dec0: 6365 203d 2046 616c 7365 2c20 7573 6549  ce = False, useI
+0000ded0: 6d61 6765 5370 6163 696e 6720 3d20 4661  mageSpacing = Fa
+0000dee0: 6c73 6529 290a 2020 2020 2020 2020 2320  lse)).        # 
+0000def0: 2020 2020 2020 2020 6469 735f 6d61 7020          dis_map 
+0000df00: 3d20 6e70 2e61 7272 6179 2864 6973 5f6d  = np.array(dis_m
+0000df10: 6170 292e 6173 7479 7065 286e 702e 666c  ap).astype(np.fl
+0000df20: 6f61 7429 0a20 2020 2020 2020 2023 2020  oat).        #  
+0000df30: 2020 2020 2020 205f 6469 735f 6d61 705b         _dis_map[
+0000df40: 692c 206a 5d20 3d20 6274 2e74 656e 736f  i, j] = bt.tenso
+0000df50: 7228 6469 735f 6d61 7020 2a20 2864 6973  r(dis_map * (dis
+0000df60: 5f6d 6170 203e 2030 292e 6173 7479 7065  _map > 0).astype
+0000df70: 286e 702e 666c 6f61 7429 290a 2020 2020  (np.float)).    
+0000df80: 2020 2020 2320 6b20 3d20 320a 2020 2020      # k = 2.    
+0000df90: 2020 2020 2320 696e 7670 6f77 6b5f 6469      # invpowk_di
+0000dfa0: 735f 6d61 7020 3d20 3120 2f20 285f 6469  s_map = 1 / (_di
+0000dfb0: 735f 6d61 7020 2a2a 206b 202b 2031 652d  s_map ** k + 1e-
+0000dfc0: 3529 0a20 2020 2020 2020 2023 2073 756d  5).        # sum
+0000dfd0: 5f64 6973 5f6d 6170 203d 2069 6e76 706f  _dis_map = invpo
+0000dfe0: 776b 5f64 6973 5f6d 6170 2e73 756d 2831  wk_dis_map.sum(1
+0000dff0: 2c20 6b65 6570 6469 6d20 3d20 5472 7565  , keepdim = True
+0000e000: 290a 2020 2020 2020 2020 2320 7765 6967  ).        # weig
+0000e010: 6874 7320 3d20 696e 7670 6f77 6b5f 6469  hts = invpowk_di
+0000e020: 735f 6d61 7020 2f20 7375 6d5f 6469 735f  s_map / sum_dis_
+0000e030: 6d61 700a 2020 2020 2020 2020 2320 6672  map.        # fr
+0000e040: 6f6d 206d 6174 706c 6f74 6c69 6220 696d  om matplotlib im
+0000e050: 706f 7274 2070 7970 6c6f 7420 6173 2070  port pyplot as p
+0000e060: 6c74 0a20 2020 2020 2020 2023 2070 6c74  lt.        # plt
+0000e070: 2e73 7562 706c 6f74 2831 3231 293b 2070  .subplot(121); p
+0000e080: 6c74 2e69 6d73 686f 7728 7765 6967 6874  lt.imshow(weight
+0000e090: 735b 302c 2030 5d29 0a20 2020 2020 2020  s[0, 0]).       
+0000e0a0: 2023 2070 6c74 2e73 7562 706c 6f74 2831   # plt.subplot(1
+0000e0b0: 3232 293b 2070 6c74 2e69 6d73 686f 7728  22); plt.imshow(
+0000e0c0: 7765 6967 6874 735b 302c 2031 5d29 0a20  weights[0, 1]). 
+0000e0d0: 2020 2020 2020 2023 2070 6c74 2e73 686f         # plt.sho
+0000e0e0: 7728 290a 2020 2020 2020 2020 2320 6966  w().        # if
+0000e0f0: 2074 7261 6e73 5f73 7472 6574 6368 2069   trans_stretch i
+0000e100: 7320 6e6f 7420 4e6f 6e65 3a20 646d 6174  s not None: dmat
+0000e110: 7269 6365 7320 3d20 646d 6174 7269 6365  rices = dmatrice
+0000e120: 7320 2a20 6274 2e74 656e 736f 7228 5b31  s * bt.tensor([1
+0000e130: 2e5d 202a 206e 5f64 696d 202b 205b 7472  .] * n_dim + [tr
+0000e140: 616e 735f 7374 7265 7463 685d 292e 756e  ans_stretch]).un
+0000e150: 7371 7565 657a 6528 302c 2030 2c20 3029  squeeze(0, 0, 0)
+0000e160: 0a0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+0000e170: 292e 5f5f 696e 6974 5f5f 2864 6d61 7472  ).__init__(dmatr
+0000e180: 6963 6573 2c20 6d61 736b 733d 6d61 736b  ices, masks=mask
+0000e190: 732c 206f 7264 6572 3d6f 7264 6572 2c20  s, order=order, 
+0000e1a0: 6973 5f69 6e76 3d69 735f 696e 762c 2074  is_inv=is_inv, t
+0000e1b0: 7261 6e73 5f73 7472 6574 6368 3d74 7261  rans_stretch=tra
+0000e1c0: 6e73 5f73 7472 6574 6368 290a 2020 2020  ns_stretch).    
+0000e1d0: 2020 2020 7365 6c66 2e6e 5f62 6174 6368      self.n_batch
+0000e1e0: 203d 206e 5f62 6174 6368 0a20 2020 2020   = n_batch.     
+0000e1f0: 2020 2073 656c 662e 6e5f 6469 6d20 3d20     self.n_dim = 
+0000e200: 6e5f 6469 6d0a 2020 2020 2020 2020 7365  n_dim.        se
+0000e210: 6c66 2e6d 6173 6b73 203d 206d 6173 6b73  lf.masks = masks
+0000e220: 0a20 2020 2020 2020 2073 656c 662e 7765  .        self.we
+0000e230: 6967 6874 7320 3d20 7765 6967 6874 730a  ights = weights.
+0000e240: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+0000e250: 6e73 5f73 7472 6574 6368 203d 2074 7261  ns_stretch = tra
+0000e260: 6e73 5f73 7472 6574 6368 0a20 2020 2020  ns_stretch.     
+0000e270: 2020 2073 656c 662e 646d 6174 7269 6365     self.dmatrice
+0000e280: 7320 3d20 646d 6174 7269 6365 730a 2020  s = dmatrices.  
+0000e290: 2020 2020 2020 7365 6c66 2e69 735f 696e        self.is_in
+0000e2a0: 7620 3d20 6973 5f69 6e76 0a20 2020 2020  v = is_inv.     
+0000e2b0: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
+0000e2c0: 6f72 6465 720a 0a20 2020 2064 6566 205f  order..    def _
+0000e2d0: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
+0000e2e0: 3a0a 2020 2020 2020 2020 5820 3d20 7375  :.        X = su
+0000e2f0: 7065 7228 292e 5f5f 6361 6c6c 5f5f 2858  per().__call__(X
+0000e300: 290a 2020 2020 2020 2020 646d 6174 7269  ).        dmatri
+0000e310: 6365 7320 3d20 7365 6c66 2e64 6d61 7472  ces = self.dmatr
+0000e320: 6963 6573 2023 2028 5b6e 5f62 6174 6368  ices # ([n_batch
+0000e330: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
+0000e340: 5f64 696d 202b 2031 2c20 6e5f 6469 6d20  _dim + 1, n_dim 
+0000e350: 2b20 3129 0a20 2020 2020 2020 2077 6569  + 1).        wei
+0000e360: 6768 7473 203d 2073 656c 662e 7765 6967  ghts = self.weig
+0000e370: 6874 7320 2320 285b 6e5f 6261 7463 685d  hts # ([n_batch]
+0000e380: 2c20 7b6e 5f72 6567 696f 6e7d 2c20 6e40  , {n_region}, n@
+0000e390: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+0000e3a0: 5f64 696d 290a 2020 2020 2020 2020 6e5f  _dim).        n_
+0000e3b0: 6469 6d20 3d20 7365 6c66 2e6e 5f64 696d  dim = self.n_dim
+0000e3c0: 0a20 2020 2020 2020 206e 5f72 6567 696f  .        n_regio
+0000e3d0: 6e20 3d20 646d 6174 7269 6365 732e 6e5f  n = dmatrices.n_
+0000e3e0: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
+0000e3f0: 5873 203d 2058 2e6d 756c 7469 706c 7928  Xs = X.multiply(
+0000e400: 6e5f 7265 6769 6f6e 2c20 7b7d 2920 2320  n_region, {}) # 
+0000e410: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
+0000e420: 6567 696f 6e7d 2c20 6e5f 6469 6d2c 206e  egion}, n_dim, n
+0000e430: 4031 2c20 6e40 322c 202e 2e2e 2c20 6e40  @1, n@2, ..., n@
+0000e440: 6e5f 6469 6d29 0a20 2020 2020 2020 2041  n_dim).        A
+0000e450: 203d 2064 6d61 7472 6963 6573 5b2e 2e2e   = dmatrices[...
+0000e460: 2c20 3a6e 5f64 696d 2c20 3a6e 5f64 696d  , :n_dim, :n_dim
+0000e470: 5d0a 2020 2020 2020 2020 6220 3d20 646d  ].        b = dm
+0000e480: 6174 7269 6365 735b 2e2e 2e2c 203a 6e5f  atrices[..., :n_
+0000e490: 6469 6d2c 206e 5f64 696d 3a5d 0a20 2020  dim, n_dim:].   
+0000e4a0: 2020 2020 2059 203d 2028 4120 4020 5873       Y = (A @ Xs
+0000e4b0: 2e66 6c61 7474 656e 2833 2920 2b20 6229  .flatten(3) + b)
+0000e4c0: 2e76 6965 775f 6173 2858 7329 0a20 2020  .view_as(Xs).   
+0000e4d0: 2020 2020 2044 203d 2028 5920 2a20 7765       D = (Y * we
+0000e4e0: 6967 6874 732e 756e 7371 7565 657a 6528  ights.unsqueeze(
+0000e4f0: 2929 2e73 756d 287b 7d29 2e77 6974 685f  )).sum({}).with_
+0000e500: 6368 616e 6e65 6c64 696d 2831 2920 2d20  channeldim(1) - 
+0000e510: 580a 2020 2020 2020 2020 6966 2073 656c  X.        if sel
+0000e520: 662e 6973 5f69 6e76 3a20 4420 3d20 2d44  f.is_inv: D = -D
+0000e530: 0a20 2020 2020 2020 2074 7261 6e73 203d  .        trans =
+0000e540: 2044 656e 7365 4469 7370 6c61 6365 6d65   DenseDisplaceme
+0000e550: 6e74 4669 656c 6428 4429 0a20 2020 2020  ntField(D).     
+0000e560: 2020 2074 7261 6e73 3220 3d20 4465 6e73     trans2 = Dens
+0000e570: 6544 6973 706c 6163 656d 656e 7446 6965  eDisplacementFie
+0000e580: 6c64 2874 7261 6e73 2874 7261 6e73 2858  ld(trans(trans(X
+0000e590: 2929 202d 2058 290a 2020 2020 2020 2020  )) - X).        
+0000e5a0: 7472 616e 7334 203d 2044 656e 7365 4469  trans4 = DenseDi
+0000e5b0: 7370 6c61 6365 6d65 6e74 4669 656c 6428  splacementField(
+0000e5c0: 7472 616e 7332 2874 7261 6e73 3228 5829  trans2(trans2(X)
+0000e5d0: 2920 2d20 5829 0a20 2020 2020 2020 2074  ) - X).        t
+0000e5e0: 7261 6e73 3820 3d20 4465 6e73 6544 6973  rans8 = DenseDis
+0000e5f0: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
+0000e600: 7261 6e73 3428 7472 616e 7334 2858 2929  rans4(trans4(X))
+0000e610: 202d 2058 290a 2020 2020 2020 2020 7472   - X).        tr
+0000e620: 616e 7331 3620 3d20 4465 6e73 6544 6973  ans16 = DenseDis
+0000e630: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
+0000e640: 7261 6e73 3828 7472 616e 7338 2858 2929  rans8(trans8(X))
+0000e650: 202d 2058 290a 2020 2020 2020 2020 7472   - X).        tr
+0000e660: 616e 7333 3220 3d20 4465 6e73 6544 6973  ans32 = DenseDis
+0000e670: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
+0000e680: 7261 6e73 3136 2874 7261 6e73 3136 2858  rans16(trans16(X
+0000e690: 2929 202d 2058 290a 2020 2020 2020 2020  )) - X).        
+0000e6a0: 7472 616e 7336 3420 3d20 4465 6e73 6544  trans64 = DenseD
+0000e6b0: 6973 706c 6163 656d 656e 7446 6965 6c64  isplacementField
+0000e6c0: 2874 7261 6e73 3332 2874 7261 6e73 3332  (trans32(trans32
+0000e6d0: 2858 2929 202d 2058 290a 2020 2020 2020  (X)) - X).      
+0000e6e0: 2020 7265 7475 726e 2074 7261 6e73 3634    return trans64
+0000e6f0: 2858 290a 0a20 2020 2064 6566 2069 6e76  (X)..    def inv
+0000e700: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000e710: 7265 7475 726e 2050 6f6c 7941 6666 696e  return PolyAffin
+0000e720: 6528 7365 6c66 2e64 6d61 7472 6963 6573  e(self.dmatrices
+0000e730: 2c20 7365 6c66 2e6d 6173 6b73 2c20 6f72  , self.masks, or
+0000e740: 6465 723d 7365 6c66 2e6f 7264 6572 2c20  der=self.order, 
+0000e750: 6973 5f69 6e76 3d6e 6f74 2073 656c 662e  is_inv=not self.
+0000e760: 6973 5f69 6e76 2c20 7472 616e 735f 7374  is_inv, trans_st
+0000e770: 7265 7463 6820 3d20 3129 2e62 6163 6b77  retch = 1).backw
+0000e780: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
+0000e790: 7264 290a 2020 2020 2020 2020 2320 6e5f  rd).        # n_
+0000e7a0: 6261 7463 6820 3d20 7365 6c66 2e64 6d61  batch = self.dma
+0000e7b0: 7472 6963 6573 2e6e 5f62 6174 6368 0a20  trices.n_batch. 
+0000e7c0: 2020 2020 2020 2023 2061 6666 7320 3d20         # affs = 
+0000e7d0: 6274 2e69 6e76 2873 656c 662e 646d 6174  bt.inv(self.dmat
+0000e7e0: 7269 6365 7329 0a20 2020 2020 2020 2023  rices).        #
+0000e7f0: 206d 6173 6b73 203d 2069 6e74 6572 706f   masks = interpo
+0000e800: 6c61 7469 6f6e 2873 656c 662e 6d61 736b  lation(self.mask
+0000e810: 732e 6d65 7267 6564 696d 7328 5b5d 2c20  s.mergedims([], 
+0000e820: 7b7d 292c 2041 6666 696e 6528 6274 2e6d  {}), Affine(bt.m
+0000e830: 6174 706f 7728 6166 6673 2e6d 6572 6765  atpow(affs.merge
+0000e840: 6469 6d73 285b 5d2c 207b 7d29 2c20 3634  dims([], {}), 64
+0000e850: 2929 292e 7370 6c69 7464 696d 285b 5d2c  ))).splitdim([],
+0000e860: 205b 6e5f 6261 7463 685d 2c20 7b2d 317d   [n_batch], {-1}
+0000e870: 290a 2020 2020 2020 2020 2320 7265 7475  ).        # retu
+0000e880: 726e 2050 6f6c 7941 6666 696e 6528 6166  rn PolyAffine(af
+0000e890: 6673 2c20 6d61 736b 7320 3d20 6d61 736b  fs, masks = mask
+0000e8a0: 732c 2074 7261 6e73 5f73 7472 6574 6368  s, trans_stretch
+0000e8b0: 203d 2073 656c 662e 7472 616e 735f 7374   = self.trans_st
+0000e8c0: 7265 7463 6829 2e62 6163 6b77 6172 645f  retch).backward_
+0000e8d0: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
+0000e8e0: 0a40 616c 6961 7328 224c 4152 4d22 290a  .@alias("LARM").
+0000e8f0: 636c 6173 7320 4c6f 6361 6c6c 7941 6666  class LocallyAff
+0000e900: 696e 6528 5370 6174 6961 6c54 7261 6e73  ine(SpatialTrans
+0000e910: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
+0000e920: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000e930: 662c 206d 6174 7269 6365 732c 206d 6173  f, matrices, mas
+0000e940: 6b73 2c20 6f72 6465 723d 322c 2074 7261  ks, order=2, tra
+0000e950: 6e73 5f73 7472 6574 6368 3d4e 6f6e 652c  ns_stretch=None,
+0000e960: 2061 766f 6964 5f63 6f6e 666c 6963 743d   avoid_conflict=
+0000e970: 5472 7565 293a 0a20 2020 2020 2020 2027  True):.        '
+0000e980: 2727 0a20 2020 2020 2020 204c 6f63 616c  ''.        Local
+0000e990: 6c79 2061 6666 696e 6520 7472 616e 7366  ly affine transf
+0000e9a0: 6f72 6d61 7469 6f6e 2077 6974 6820 7265  ormation with re
+0000e9b0: 7370 6563 7420 746f 2074 7261 6e73 666f  spect to transfo
+0000e9c0: 726d 6174 696f 6e20 6d61 7472 6963 6573  rmation matrices
+0000e9d0: 205b 315d 2e0a 2020 2020 2020 2020 0a20   [1]..        . 
+0000e9e0: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
+0000e9f0: 2020 2020 2020 2020 2020 206d 6174 7269             matri
+0000ea00: 6365 7320 5b62 742e 5465 6e73 6f72 206f  ces [bt.Tensor o
+0000ea10: 7220 6e70 2e6e 756d 7079 5d3a 204f 6e65  r np.numpy]: One
+0000ea20: 2061 6666 696e 6520 6d61 7472 6978 2066   affine matrix f
+0000ea30: 6f72 2065 6163 6820 7265 6769 6f6e 2e20  or each region. 
+0000ea40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea50: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+0000ea60: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
+0000ea70: 5f64 696d 202b 2031 2c20 6e5f 6469 6d20  _dim + 1, n_dim 
+0000ea80: 2b20 3129 0a20 2020 2020 2020 2020 2020  + 1).           
+0000ea90: 206d 6173 6b73 205b 6274 2e54 656e 736f   masks [bt.Tenso
+0000eaa0: 7220 6f72 206e 702e 6e75 6d70 795d 3a20  r or np.numpy]: 
+0000eab0: 4f6e 6520 302d 3120 6d61 736b 2066 6f72  One 0-1 mask for
+0000eac0: 2065 6163 6820 7265 6769 6f6e 2e20 0a20   each region. . 
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eae0: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
+0000eaf0: 207b 6e5f 7265 6769 6f6e 7d2c 206e 4031   {n_region}, n@1
+0000eb00: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+0000eb10: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+0000eb20: 206f 7264 6572 205b 696e 745d 3a20 7468   order [int]: th
+0000eb30: 6520 6f72 6465 7220 6f66 2069 6e74 6572  e order of inter
+0000eb40: 706f 6c61 7469 6f6e 2063 6f65 6666 6963  polation coeffic
+0000eb50: 6965 6e74 2e20 5468 6520 696e 666c 7565  ient. The influe
+0000eb60: 6e63 6520 6f66 2061 6e20 6166 6669 6e65  nce of an affine
+0000eb70: 2064 6563 6179 7320 6174 2061 2072 6174   decays at a rat
+0000eb80: 6520 6f66 2031 202f 2064 6973 7461 6e63  e of 1 / distanc
+0000eb90: 655e 6f72 6465 722e 0a20 2020 2020 2020  e^order..       
+0000eba0: 2020 2020 2074 7261 6e73 5f73 7472 6574       trans_stret
+0000ebb0: 6368 205b 696e 745d 3a20 6f6e 6c79 2075  ch [int]: only u
+0000ebc0: 7365 6420 666f 7220 6974 6572 6174 6976  sed for iterativ
+0000ebd0: 6520 7061 7261 6d65 7465 7220 7472 6169  e parameter trai
+0000ebe0: 6e69 6e67 2c20 3120 6279 2064 6566 6175  ning, 1 by defau
+0000ebf0: 6c74 2e20 3230 2073 6565 6d73 2074 6f20  lt. 20 seems to 
+0000ec00: 6265 2061 2067 6f6f 6420 6368 6f69 6365  be a good choice
+0000ec10: 2e20 200a 2020 2020 2020 2020 2020 2020  .  .            
+0000ec20: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
+0000ec30: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
+0000ec40: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
+0000ec50: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
+0000ec60: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
+0000ec70: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
+0000ec80: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
+0000ec90: 6261 7463 683a 206f 7074 696f 6e61 6c5d  batch: optional]
+0000eca0: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
+0000ecb0: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+0000ecc0: 6d29 0a20 2020 2020 2020 2020 2020 206f  m).            o
+0000ecd0: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
+0000ece0: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
+0000ecf0: 6564 2063 6f6f 7264 696e 6174 6573 2e0a  ed coordinates..
+0000ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed10: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
+0000ed20: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
+0000ed30: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+0000ed40: 6d29 0a0a 2020 2020 2020 2020 5b31 5d20  m)..        [1] 
+0000ed50: 5a68 7561 6e67 2058 202c 2052 686f 6465  Zhuang X , Rhode
+0000ed60: 204b 202c 2041 7272 6964 6765 2053 202c   K , Arridge S ,
+0000ed70: 2065 7420 616c 2e20 416e 2041 746c 6173   et al. An Atlas
+0000ed80: 2d42 6173 6564 2053 6567 6d65 6e74 6174  -Based Segmentat
+0000ed90: 696f 6e20 5072 6f70 6167 6174 696f 6e20  ion Propagation 
+0000eda0: 4672 616d 6577 6f72 6b20 5573 696e 6720  Framework Using 
+0000edb0: 4c6f 6361 6c6c 7920 4166 6669 6e65 200a  Locally Affine .
+0000edc0: 2020 2020 2020 2020 2020 2020 5265 6769              Regi
+0000edd0: 7374 7261 7469 6f6e 202d 2041 7070 6c69  stration - Appli
+0000ede0: 6361 7469 6f6e 2074 6f20 4175 746f 6d61  cation to Automa
+0000edf0: 7469 6320 5768 6f6c 6520 4865 6172 7420  tic Whole Heart 
+0000ee00: 5365 676d 656e 7461 7469 6f6e 5b4a 5d2e  Segmentation[J].
+0000ee10: 2053 7072 696e 6765 722c 2042 6572 6c69   Springer, Berli
+0000ee20: 6e2c 2048 6569 6465 6c62 6572 672c 2032  n, Heidelberg, 2
+0000ee30: 3030 382e 0a20 2020 2020 2020 2027 2727  008..        '''
+0000ee40: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+0000ee50: 5369 6d70 6c65 4954 4b20 6173 2073 6974  SimpleITK as sit
+0000ee60: 6b0a 2020 2020 2020 2020 6672 6f6d 202e  k.        from .
+0000ee70: 6675 6e63 7320 696d 706f 7274 2064 696c  funcs import dil
+0000ee80: 6174 652c 2064 6973 7461 6e63 655f 6d61  ate, distance_ma
+0000ee90: 700a 2020 2020 2020 2020 6d61 7472 6963  p.        matric
+0000eea0: 6573 203d 2062 6174 6f72 6368 5f74 656e  es = batorch_ten
+0000eeb0: 736f 7228 6d61 7472 6963 6573 290a 2020  sor(matrices).  
+0000eec0: 2020 2020 2020 6966 206d 6174 7269 6365        if matrice
+0000eed0: 732e 6e5f 6469 6d20 3c3d 2033 2061 6e64  s.n_dim <= 3 and
+0000eee0: 206e 6f74 206d 6174 7269 6365 732e 6861   not matrices.ha
+0000eef0: 735f 6261 7463 683a 206d 6174 7269 6365  s_batch: matrice
+0000ef00: 7320 3d20 6d61 7472 6963 6573 2e75 6e73  s = matrices.uns
+0000ef10: 7175 6565 7a65 285b 5d29 0a20 2020 2020  queeze([]).     
+0000ef20: 2020 2069 6620 6d61 7472 6963 6573 2e6e     if matrices.n
+0000ef30: 5f64 696d 203c 3d20 3320 616e 6420 6e6f  _dim <= 3 and no
+0000ef40: 7420 6d61 7472 6963 6573 2e68 6173 5f63  t matrices.has_c
+0000ef50: 6861 6e6e 656c 3a20 6d61 7472 6963 6573  hannel: matrices
+0000ef60: 203d 206d 6174 7269 6365 732e 756e 7371   = matrices.unsq
+0000ef70: 7565 657a 6528 7b7d 290a 2020 2020 2020  ueeze({}).      
+0000ef80: 2020 6966 206d 6174 7269 6365 732e 6e5f    if matrices.n_
+0000ef90: 6469 6d20 3d3d 2034 2061 6e64 206d 6174  dim == 4 and mat
+0000efa0: 7269 6365 732e 7368 6170 655b 325d 203d  rices.shape[2] =
+0000efb0: 3d20 6d61 7472 6963 6573 2e73 6861 7065  = matrices.shape
+0000efc0: 5b33 5d3a 0a20 2020 2020 2020 2020 2020  [3]:.           
+0000efd0: 2069 6620 6e6f 7420 6d61 7472 6963 6573   if not matrices
+0000efe0: 2e68 6173 5f62 6174 6368 3a20 6d61 7472  .has_batch: matr
+0000eff0: 6963 6573 2e62 6174 6368 5f64 696d 656e  ices.batch_dimen
+0000f000: 7369 6f6e 203d 2030 0a20 2020 2020 2020  sion = 0.       
+0000f010: 2020 2020 2069 6620 6e6f 7420 6d61 7472       if not matr
+0000f020: 6963 6573 2e68 6173 5f63 6861 6e6e 656c  ices.has_channel
+0000f030: 3a20 6d61 7472 6963 6573 2e63 6861 6e6e  : matrices.chann
+0000f040: 656c 5f64 696d 656e 7369 6f6e 203d 2031  el_dimension = 1
+0000f050: 0a20 2020 2020 2020 2061 766f 7563 6828  .        avouch(
+0000f060: 6d61 7472 6963 6573 2e68 6173 5f62 6174  matrices.has_bat
+0000f070: 6368 2061 6e64 206d 6174 7269 6365 732e  ch and matrices.
+0000f080: 6861 735f 6368 616e 6e65 6c2c 2022 506c  has_channel, "Pl
+0000f090: 6561 7365 2075 7365 2062 6174 6f72 6368  ease use batorch
+0000f0a0: 2074 656e 736f 7220 6f66 2073 697a 6520   tensor of size 
+0000f0b0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
+0000f0c0: 6567 696f 6e7d 2c22 202b 0a20 2020 2020  egion}," +.     
+0000f0d0: 2020 2020 2020 2020 2020 6622 6e5f 6469            f"n_di
+0000f0e0: 6d20 2b20 312c 206e 5f64 696d 202b 2031  m + 1, n_dim + 1
+0000f0f0: 2920 666f 7220 4c6f 6361 6c6c 7941 6666  ) for LocallyAff
+0000f100: 696e 6520 7061 7261 6d65 7465 7273 2c20  ine parameters, 
+0000f110: 696e 7374 6561 6420 6f66 207b 6d61 7472  instead of {matr
+0000f120: 6963 6573 2e73 6861 7065 7d2e 2022 290a  ices.shape}. ").
+0000f130: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
+0000f140: 5f73 7472 6574 6368 2069 7320 6e6f 7420  _stretch is not 
+0000f150: 4e6f 6e65 3a20 6d61 7472 6963 6573 5b2e  None: matrices[.
+0000f160: 2e2e 2c20 3a6e 5f64 696d 2c20 2d31 5d20  .., :n_dim, -1] 
+0000f170: 2a3d 2074 7261 6e73 5f73 7472 6574 6368  *= trans_stretch
+0000f180: 0a20 2020 2020 2020 206e 5f64 696d 203d  .        n_dim =
+0000f190: 206d 6174 7269 6365 732e 7369 7a65 282d   matrices.size(-
+0000f1a0: 3129 202d 2031 0a20 2020 2020 2020 206d  1) - 1.        m
+0000f1b0: 6173 6b73 203d 2062 6174 6f72 6368 5f74  asks = batorch_t
+0000f1c0: 656e 736f 7228 6d61 736b 7329 0a20 2020  ensor(masks).   
+0000f1d0: 2020 2020 2069 6620 6d61 736b 732e 6e5f       if masks.n_
+0000f1e0: 6469 6d20 3c3d 206e 5f64 696d 202b 2031  dim <= n_dim + 1
+0000f1f0: 2061 6e64 206e 6f74 206d 6173 6b73 2e68   and not masks.h
+0000f200: 6173 5f62 6174 6368 3a20 6d61 736b 7320  as_batch: masks 
+0000f210: 3d20 6d61 736b 732e 756e 7371 7565 657a  = masks.unsqueez
+0000f220: 6528 5b5d 290a 2020 2020 2020 2020 6966  e([]).        if
+0000f230: 206d 6173 6b73 2e6e 5f64 696d 203c 3d20   masks.n_dim <= 
+0000f240: 6e5f 6469 6d20 2b20 3120 616e 6420 6e6f  n_dim + 1 and no
+0000f250: 7420 6d61 736b 732e 6861 735f 6368 616e  t masks.has_chan
+0000f260: 6e65 6c3a 206d 6173 6b73 203d 206d 6173  nel: masks = mas
+0000f270: 6b73 2e75 6e73 7175 6565 7a65 287b 7d29  ks.unsqueeze({})
+0000f280: 0a20 2020 2020 2020 2069 6620 6d61 736b  .        if mask
+0000f290: 732e 6e5f 6469 6d20 3d3d 206e 5f64 696d  s.n_dim == n_dim
+0000f2a0: 202b 2032 2061 6e64 206e 6f74 206d 6173   + 2 and not mas
+0000f2b0: 6b73 2e68 6173 5f62 6174 6368 3a20 6d61  ks.has_batch: ma
+0000f2c0: 736b 732e 6261 7463 685f 6469 6d65 6e73  sks.batch_dimens
+0000f2d0: 696f 6e20 3d20 300a 2020 2020 2020 2020  ion = 0.        
+0000f2e0: 6966 206d 6173 6b73 2e6e 5f64 696d 203d  if masks.n_dim =
+0000f2f0: 3d20 6e5f 6469 6d20 2b20 3220 616e 6420  = n_dim + 2 and 
+0000f300: 6e6f 7420 6d61 736b 732e 6861 735f 6368  not masks.has_ch
+0000f310: 616e 6e65 6c3a 206d 6173 6b73 2e63 6861  annel: masks.cha
+0000f320: 6e6e 656c 5f64 696d 656e 7369 6f6e 203d  nnel_dimension =
+0000f330: 2031 0a20 2020 2020 2020 2061 766f 7563   1.        avouc
+0000f340: 6828 6d61 736b 732e 6861 735f 6261 7463  h(masks.has_batc
+0000f350: 6820 616e 6420 6d61 736b 732e 6861 735f  h and masks.has_
+0000f360: 6368 616e 6e65 6c2c 2022 506c 6561 7365  channel, "Please
+0000f370: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+0000f380: 736f 7220 6f66 2073 697a 6520 285b 6e5f  sor of size ([n_
+0000f390: 6261 7463 685d 2c20 7b6e 5f72 6567 696f  batch], {n_regio
+0000f3a0: 6e7d 2c22 202b 200a 2020 2020 2020 2020  n}," + .        
+0000f3b0: 2020 2020 2020 2066 226e 4031 2c20 6e40         f"n@1, n@
+0000f3c0: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
+0000f3d0: 2066 6f72 204c 6f63 616c 6c79 4166 6669   for LocallyAffi
+0000f3e0: 6e65 2070 6172 616d 6574 6572 732c 2069  ne parameters, i
+0000f3f0: 6e73 7465 6164 206f 6620 7b6d 6173 6b73  nstead of {masks
+0000f400: 2e73 6861 7065 7d2e 2022 290a 0a20 2020  .shape}. ")..   
+0000f410: 2020 2020 2023 2070 7265 7072 6f63 6573       # preproces
+0000f420: 7320 6d61 736b 730a 2020 2020 2020 2020  s masks.        
+0000f430: 6e5f 6261 7463 6820 3d20 6d61 7472 6963  n_batch = matric
+0000f440: 6573 2e6e 5f62 6174 6368 0a20 2020 2020  es.n_batch.     
+0000f450: 2020 206e 5f72 6567 696f 6e20 3d20 6d61     n_region = ma
+0000f460: 7472 6963 6573 2e6e 5f63 6861 6e6e 656c  trices.n_channel
+0000f470: 0a20 2020 2020 2020 2069 6620 6176 6f69  .        if avoi
+0000f480: 645f 636f 6e66 6c69 6374 3a0a 2020 2020  d_conflict:.    
+0000f490: 2020 2020 2020 2020 4769 203d 2041 6666          Gi = Aff
+0000f4a0: 696e 6528 6d61 7472 6963 6573 2e6d 6572  ine(matrices.mer
+0000f4b0: 6765 6469 6d73 287b 7d2c 205b 5d29 290a  gedims({}, [])).
+0000f4c0: 2020 2020 2020 2020 2020 2020 4769 5669              GiVi
+0000f4d0: 203d 2069 6e74 6572 706f 6c61 7469 6f6e   = interpolation
+0000f4e0: 286d 6173 6b73 2e6d 6572 6765 6469 6d73  (masks.mergedims
+0000f4f0: 287b 7d2c 205b 5d29 2c20 4769 2e69 6e76  ({}, []), Gi.inv
+0000f500: 2829 2c20 6d65 7468 6f64 3d27 4e65 6172  (), method='Near
+0000f510: 6573 7427 292e 7370 6c69 7464 696d 285b  est').splitdim([
+0000f520: 5d2c 205b 6e5f 6261 7463 685d 2c20 6e5f  ], [n_batch], n_
+0000f530: 7265 6769 6f6e 2920 2320 285b 6e5f 6261  region) # ([n_ba
+0000f540: 7463 685d 2c20 6e5f 7265 6769 6f6e 2c20  tch], n_region, 
+0000f550: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
+0000f560: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+0000f570: 2020 2020 4769 5669 6a6f 696e 476b 566b      GiVijoinGkVk
+0000f580: 203d 2028 4769 5669 2e75 6e73 7175 6565   = (GiVi.unsquee
+0000f590: 7a65 2831 2920 2a20 4769 5669 2e75 6e73  ze(1) * GiVi.uns
+0000f5a0: 7175 6565 7a65 2832 2929 2e6d 6572 6765  queeze(2)).merge
+0000f5b0: 6469 6d73 2831 2c20 5b5d 292e 7769 7468  dims(1, []).with
+0000f5c0: 5f63 6861 6e6e 656c 6469 6d28 3129 2023  _channeldim(1) #
+0000f5d0: 2028 5b6e 5f62 6174 6368 2078 206e 5f72   ([n_batch x n_r
+0000f5e0: 6567 696f 6e5d 2c20 7b6e 5f72 6567 696f  egion], {n_regio
+0000f5f0: 6e7d 2c20 6e40 312c 206e 4032 2c20 2e2e  n}, n@1, n@2, ..
+0000f600: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
+0000f610: 2020 2020 2020 2020 5269 6b20 3d20 696e          Rik = in
+0000f620: 7465 7270 6f6c 6174 696f 6e28 4769 5669  terpolation(GiVi
+0000f630: 6a6f 696e 476b 566b 2c20 4769 2c20 6d65  joinGkVk, Gi, me
+0000f640: 7468 6f64 3d27 4e65 6172 6573 7427 292e  thod='Nearest').
+0000f650: 7370 6c69 7464 696d 285b 5d2c 205b 6e5f  splitdim([], [n_
+0000f660: 6261 7463 685d 2c20 6e5f 7265 6769 6f6e  batch], n_region
+0000f670: 2920 2320 285b 6e5f 6261 7463 685d 2c20  ) # ([n_batch], 
+0000f680: 6e5f 7265 6769 6f6e 2c20 7b6e 5f72 6567  n_region, {n_reg
+0000f690: 696f 6e7d 2c20 6e40 312c 206e 4032 2c20  ion}, n@1, n@2, 
+0000f6a0: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
+0000f6b0: 2020 2020 2020 2020 2020 5552 696b 203d            URik =
+0000f6c0: 2028 5269 6b2e 7375 6d28 7b7d 292e 7769   (Rik.sum({}).wi
+0000f6d0: 7468 5f63 6861 6e6e 656c 6469 6d28 3129  th_channeldim(1)
+0000f6e0: 202d 206d 6173 6b73 203e 2030 2e31 292e   - masks > 0.1).
+0000f6f0: 666c 6f61 7428 2920 2320 285b 6e5f 6261  float() # ([n_ba
+0000f700: 7463 685d 2c20 7b6e 5f72 6567 696f 6e7d  tch], {n_region}
+0000f710: 2c20 6e40 312c 206e 4032 2c20 2e2e 2e2c  , n@1, n@2, ...,
+0000f720: 206e 406e 5f64 696d 290a 2020 2020 2020   n@n_dim).      
+0000f730: 2020 2020 2020 5552 696b 5f70 6c75 7320        URik_plus 
+0000f740: 3d20 6469 6c61 7465 2855 5269 6b2e 6d65  = dilate(URik.me
+0000f750: 7267 6564 696d 7328 7b7d 2c20 5b5d 292c  rgedims({}, []),
+0000f760: 2031 292e 7370 6c69 7464 696d 285b 5d2c   1).splitdim([],
+0000f770: 205b 6e5f 6261 7463 685d 2c20 6e5f 7265   [n_batch], n_re
+0000f780: 6769 6f6e 2920 2320 285b 6e5f 6261 7463  gion) # ([n_batc
+0000f790: 685d 2c20 7b6e 5f72 6567 696f 6e7d 2c20  h], {n_region}, 
+0000f7a0: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
+0000f7b0: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+0000f7c0: 2020 2020 6d61 736b 7320 3d20 286d 6173      masks = (mas
+0000f7d0: 6b73 202d 2055 5269 6b5f 706c 7573 203e  ks - URik_plus >
+0000f7e0: 2030 2e31 292e 666c 6f61 7428 2920 2320   0.1).float() # 
+0000f7f0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
+0000f800: 6567 696f 6e7d 2c20 6e40 312c 206e 4032  egion}, n@1, n@2
+0000f810: 2c20 2e2e 2e2c 206e 406e 5f64 696d 290a  , ..., n@n_dim).
+0000f820: 0a20 2020 2020 2020 2077 6569 6768 7473  .        weights
+0000f830: 203d 2031 202f 2028 6469 7374 616e 6365   = 1 / (distance
+0000f840: 5f6d 6170 286d 6173 6b73 2920 2a2a 206f  _map(masks) ** o
+0000f850: 7264 6572 202b 2031 652d 3529 0a20 2020  rder + 1e-5).   
+0000f860: 2020 2020 2077 6569 6768 7473 203d 2077       weights = w
+0000f870: 6569 6768 7473 202f 2077 6569 6768 7473  eights / weights
+0000f880: 2e73 756d 287b 7d29 2023 2028 5b6e 5f62  .sum({}) # ([n_b
+0000f890: 6174 6368 5d2c 207b 6e5f 7265 6769 6f6e  atch], {n_region
+0000f8a0: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
+0000f8b0: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
+0000f8c0: 2020 2023 2069 6620 7472 616e 735f 7374     # if trans_st
+0000f8d0: 7265 7463 6820 6973 206e 6f74 204e 6f6e  retch is not Non
+0000f8e0: 653a 206d 6174 7269 6365 7320 3d20 6d61  e: matrices = ma
+0000f8f0: 7472 6963 6573 202a 2062 6174 6f72 6368  trices * batorch
+0000f900: 5f74 656e 736f 7228 5b31 2e5d 202a 206e  _tensor([1.] * n
+0000f910: 5f64 696d 202b 205b 7472 616e 735f 7374  _dim + [trans_st
+0000f920: 7265 7463 685d 292e 756e 7371 7565 657a  retch]).unsqueez
+0000f930: 6528 302c 2030 2c20 3029 0a0a 2020 2020  e(0, 0, 0)..    
+0000f940: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+0000f950: 6974 5f5f 286d 6174 7269 6365 732c 206d  it__(matrices, m
+0000f960: 6173 6b73 3d6d 6173 6b73 2c20 6f72 6465  asks=masks, orde
+0000f970: 723d 6f72 6465 722c 2074 7261 6e73 5f73  r=order, trans_s
+0000f980: 7472 6574 6368 3d74 7261 6e73 5f73 7472  tretch=trans_str
+0000f990: 6574 6368 290a 2020 2020 2020 2020 7365  etch).        se
+0000f9a0: 6c66 2e6e 5f62 6174 6368 203d 206e 5f62  lf.n_batch = n_b
+0000f9b0: 6174 6368 0a20 2020 2020 2020 2073 656c  atch.        sel
+0000f9c0: 662e 6e5f 6469 6d20 3d20 6e5f 6469 6d0a  f.n_dim = n_dim.
+0000f9d0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+0000f9e0: 6b73 203d 206d 6173 6b73 0a20 2020 2020  ks = masks.     
+0000f9f0: 2020 2073 656c 662e 7765 6967 6874 7320     self.weights 
+0000fa00: 3d20 7765 6967 6874 730a 2020 2020 2020  = weights.      
+0000fa10: 2020 7365 6c66 2e74 7261 6e73 5f73 7472    self.trans_str
+0000fa20: 6574 6368 203d 2074 7261 6e73 5f73 7472  etch = trans_str
+0000fa30: 6574 6368 0a20 2020 2020 2020 2073 656c  etch.        sel
+0000fa40: 662e 6d61 7472 6963 6573 203d 206d 6174  f.matrices = mat
+0000fa50: 7269 6365 730a 2020 2020 2020 2020 7365  rices.        se
+0000fa60: 6c66 2e62 6174 6368 5f70 6172 616d 2e65  lf.batch_param.e
+0000fa70: 7874 656e 6428 5b27 6d61 7472 6963 6573  xtend(['matrices
+0000fa80: 272c 2027 7765 6967 6874 7327 2c20 276d  ', 'weights', 'm
+0000fa90: 6173 6b73 275d 290a 0a20 2020 2064 6566  asks'])..    def
+0000faa0: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
+0000fab0: 5829 3a0a 2020 2020 2020 2020 5820 3d20  X):.        X = 
+0000fac0: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
+0000fad0: 2858 290a 2020 2020 2020 2020 6d61 7472  (X).        matr
+0000fae0: 6963 6573 203d 2073 656c 662e 6d61 7472  ices = self.matr
+0000faf0: 6963 6573 0a20 2020 2020 2020 206d 6173  ices.        mas
+0000fb00: 6b73 203d 2073 656c 662e 6d61 736b 7320  ks = self.masks 
+0000fb10: 2320 285b 6e5f 6261 7463 685d 2c20 7b6e  # ([n_batch], {n
+0000fb20: 5f72 6567 696f 6e7d 2c20 6e40 312c 206e  _region}, n@1, n
+0000fb30: 4032 2c20 2e2e 2e2c 206e 406e 5f64 696d  @2, ..., n@n_dim
+0000fb40: 290a 2020 2020 2020 2020 7765 6967 6874  ).        weight
+0000fb50: 7320 3d20 7365 6c66 2e77 6569 6768 7473  s = self.weights
+0000fb60: 2023 2028 5b6e 5f62 6174 6368 5d2c 207b   # ([n_batch], {
+0000fb70: 6e5f 7265 6769 6f6e 7d2c 206e 4031 2c20  n_region}, n@1, 
+0000fb80: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+0000fb90: 6d29 0a20 2020 2020 2020 206e 5f64 696d  m).        n_dim
+0000fba0: 203d 2073 656c 662e 6e5f 6469 6d0a 2020   = self.n_dim.  
+0000fbb0: 2020 2020 2020 6e5f 7265 6769 6f6e 203d        n_region =
+0000fbc0: 206d 6174 7269 6365 732e 6e5f 6368 616e   matrices.n_chan
+0000fbd0: 6e65 6c0a 2020 2020 2020 2020 5873 203d  nel.        Xs =
+0000fbe0: 2058 2e6d 756c 7469 706c 7928 6e5f 7265   X.multiply(n_re
+0000fbf0: 6769 6f6e 2c20 7b7d 2920 2320 285b 6e5f  gion, {}) # ([n_
+0000fc00: 6261 7463 685d 2c20 7b6e 5f72 6567 696f  batch], {n_regio
+0000fc10: 6e7d 2c20 6e5f 6469 6d2c 206e 4031 2c20  n}, n_dim, n@1, 
+0000fc20: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+0000fc30: 6d29 0a20 2020 2020 2020 2041 203d 206d  m).        A = m
+0000fc40: 6174 7269 6365 735b 2e2e 2e2c 203a 6e5f  atrices[..., :n_
+0000fc50: 6469 6d2c 203a 6e5f 6469 6d5d 0a20 2020  dim, :n_dim].   
+0000fc60: 2020 2020 2062 203d 206d 6174 7269 6365       b = matrice
+0000fc70: 735b 2e2e 2e2c 203a 6e5f 6469 6d2c 206e  s[..., :n_dim, n
+0000fc80: 5f64 696d 3a5d 0a20 2020 2020 2020 2059  _dim:].        Y
+0000fc90: 203d 2028 4120 4020 5873 2e66 6c61 7474   = (A @ Xs.flatt
+0000fca0: 656e 2833 2920 2b20 6229 2e76 6965 775f  en(3) + b).view_
+0000fcb0: 6173 2858 7329 0a20 2020 2020 2020 2072  as(Xs).        r
+0000fcc0: 6574 7572 6e20 2877 6569 6768 7473 2e75  eturn (weights.u
+0000fcd0: 6e73 7175 6565 7a65 2829 202a 2059 292e  nsqueeze() * Y).
+0000fce0: 7375 6d28 7b7d 292e 7769 7468 5f63 6861  sum({}).with_cha
+0000fcf0: 6e6e 656c 6469 6d28 3129 202a 2028 3120  nneldim(1) * (1 
+0000fd00: 2d20 6d61 736b 732e 7375 6d28 7b7d 292e  - masks.sum({}).
+0000fd10: 756e 7371 7565 657a 6528 7b7d 2929 202b  unsqueeze({})) +
+0000fd20: 2028 5920 2a20 6d61 736b 732e 756e 7371   (Y * masks.unsq
+0000fd30: 7565 657a 6528 2929 2e73 756d 287b 7d29  ueeze()).sum({})
+0000fd40: 2e77 6974 685f 6368 616e 6e65 6c64 696d  .with_channeldim
+0000fd50: 2831 290a 0a20 2020 2064 6566 2069 6e76  (1)..    def inv
+0000fd60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000fd70: 6e5f 6261 7463 6820 3d20 7365 6c66 2e6d  n_batch = self.m
+0000fd80: 6174 7269 6365 732e 6e5f 6261 7463 680a  atrices.n_batch.
+0000fd90: 2020 2020 2020 2020 6166 6673 203d 2062          affs = b
+0000fda0: 742e 696e 7628 7365 6c66 2e6d 6174 7269  t.inv(self.matri
+0000fdb0: 6365 7329 0a20 2020 2020 2020 206d 6173  ces).        mas
+0000fdc0: 6b73 203d 2069 6e74 6572 706f 6c61 7469  ks = interpolati
+0000fdd0: 6f6e 2873 656c 662e 6d61 736b 732e 6d65  on(self.masks.me
+0000fde0: 7267 6564 696d 7328 5b5d 2c20 7b7d 292c  rgedims([], {}),
+0000fdf0: 2041 6666 696e 6528 6166 6673 2e6d 6572   Affine(affs.mer
+0000fe00: 6765 6469 6d73 285b 5d2c 207b 7d29 2929  gedims([], {})))
+0000fe10: 2e73 706c 6974 6469 6d28 5b5d 2c20 5b6e  .splitdim([], [n
+0000fe20: 5f62 6174 6368 5d2c 207b 2d31 7d29 0a20  _batch], {-1}). 
+0000fe30: 2020 2020 2020 2072 6574 7572 6e20 506f         return Po
+0000fe40: 6c79 4166 6669 6e65 2861 6666 732c 206d  lyAffine(affs, m
+0000fe50: 6173 6b73 203d 206d 6173 6b73 2c20 7472  asks = masks, tr
+0000fe60: 616e 735f 7374 7265 7463 6820 3d20 3129  ans_stretch = 1)
+0000fe70: 2e62 6163 6b77 6172 645f 2873 656c 662e  .backward_(self.
+0000fe80: 6261 636b 7761 7264 290a 0a40 616c 6961  backward)..@alia
+0000fe90: 7328 2246 4644 2229 0a63 6c61 7373 2046  s("FFD").class F
+0000fea0: 7265 6546 6f72 6d44 6566 6f72 6d61 7469  reeFormDeformati
+0000feb0: 6f6e 2853 7061 7469 616c 5472 616e 7366  on(SpatialTransf
+0000fec0: 6f72 6d61 7469 6f6e 293a 0a0a 2020 2020  ormation):..    
+0000fed0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000fee0: 662c 206f 6666 7365 7473 2c20 7370 6163  f, offsets, spac
+0000fef0: 696e 673d 312c 206f 7269 6769 6e3d 3029  ing=1, origin=0)
+0000ff00: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+0000ff10: 2020 2020 2020 4672 6565 2046 6f72 6d20        Free Form 
+0000ff20: 4465 666f 726d 6174 696f 6e20 2846 4644  Deformation (FFD
+0000ff30: 2920 7472 616e 7366 6f72 6d61 7469 6f6e  ) transformation
+0000ff40: 205b 315d 2e0a 2020 2020 2020 2020 0a20   [1]..        . 
+0000ff50: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
+0000ff60: 2020 2020 2020 2020 2020 206f 6666 7365             offse
+0000ff70: 7473 205b 6274 2e54 656e 736f 725d 3a20  ts [bt.Tensor]: 
+0000ff80: 7468 6520 4646 4420 6f66 6673 6574 732e  the FFD offsets.
+0000ff90: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000ffa0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+0000ffb0: 685d 2c20 7b6e 5f64 696d 7d2c 206d 4031  h], {n_dim}, m@1
+0000ffc0: 2c20 6d40 322c 202e 2e2e 2c20 6d40 6e5f  , m@2, ..., m@n_
+0000ffd0: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+0000ffe0: 2020 2020 2066 6f72 206d 4031 2078 206d       for m@1 x m
+0000fff0: 4032 2078 202e 2e2e 2078 206d 406e 5f64  @2 x ... x m@n_d
+00010000: 696d 2067 7269 6420 6f66 20ce 9463 6f6e  im grid of ..con
+00010010: 7472 6f6c 2070 6f69 6e74 730a 2020 2020  trol points.    
+00010020: 2020 2020 2020 2020 7370 6163 696e 6720          spacing 
+00010030: 5b69 6e74 206f 7220 7475 706c 655d 3a20  [int or tuple]: 
+00010040: 4646 4420 7370 6163 696e 673b 2073 7061  FFD spacing; spa
+00010050: 6369 6e67 2062 6574 7765 656e 2046 4644  cing between FFD
+00010060: 2063 6f6e 7472 6f6c 2070 6f69 6e74 732e   control points.
+00010070: 200a 2020 2020 2020 2020 2020 2020 6f72   .            or
+00010080: 6967 696e 205b 696e 7420 6f72 2074 7570  igin [int or tup
+00010090: 6c65 5d3a 2046 4644 206f 7269 6769 6e3b  le]: FFD origin;
+000100a0: 2063 6f6f 7264 696e 6174 6520 666f 7220   coordinate for 
+000100b0: 7468 6520 2830 2c20 302c 2030 2920 636f  the (0, 0, 0) co
+000100c0: 6e74 726f 6c20 706f 696e 742e 200a 2020  ntrol point. .  
+000100d0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+000100e0: 2020 2057 6865 6e20 6974 2069 7320 6361     When it is ca
+000100f0: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
+00010100: 2020 5820 5b62 742e 5465 6e73 6f72 5d3a    X [bt.Tensor]:
+00010110: 2043 6f6f 7264 696e 6174 6573 2074 6f20   Coordinates to 
+00010120: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
+00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010140: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+00010150: 206f 7074 696f 6e61 6c5d 2c20 7b6e 5f64   optional], {n_d
+00010160: 696d 7d2c 206e 4031 2c20 6e40 322c 202e  im}, n@1, n@2, .
+00010170: 2e2e 2c20 6e40 6e5f 6469 6d29 0a20 2020  .., n@n_dim).   
+00010180: 2020 2020 2020 2020 206f 7574 7075 7420           output 
+00010190: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
+000101a0: 2074 7261 6e73 666f 726d 6564 2063 6f6f   transformed coo
+000101b0: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
+000101c0: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+000101d0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f64  ([n_batch], {n_d
+000101e0: 696d 7d2c 206e 4031 2c20 6e40 322c 202e  im}, n@1, n@2, .
+000101f0: 2e2e 2c20 6e40 6e5f 6469 6d29 0a20 2020  .., n@n_dim).   
+00010200: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00010210: 2020 2020 2020 5b31 5d20 5275 6563 6b65        [1] Ruecke
+00010220: 7274 2044 202c 2053 6f6e 6f64 6120 4c20  rt D , Sonoda L 
+00010230: 4920 2c20 4861 7965 7320 4320 2c20 6574  I , Hayes C , et
+00010240: 2061 6c2e 204e 6f6e 7269 6769 6420 7265   al. Nonrigid re
+00010250: 6769 7374 7261 7469 6f6e 2075 7369 6e67  gistration using
+00010260: 2066 7265 652d 666f 726d 2064 6566 6f72   free-form defor
+00010270: 6d61 7469 6f6e 733a 200a 2020 2020 2020  mations: .      
+00010280: 2020 2020 2020 6170 706c 6963 6174 696f        applicatio
+00010290: 6e20 746f 2062 7265 6173 7420 4d52 2069  n to breast MR i
+000102a0: 6d61 6765 735b 4a5d 2e20 4945 4545 2054  mages[J]. IEEE T
+000102b0: 7261 6e73 6163 7469 6f6e 7320 6f6e 204d  ransactions on M
+000102c0: 6564 6963 616c 2049 6d61 6769 6e67 2c20  edical Imaging, 
+000102d0: 3139 3939 2838 292e 0a20 2020 2020 2020  1999(8)..       
+000102e0: 2027 2727 0a20 2020 2020 2020 206f 6666   '''.        off
+000102f0: 7365 7473 203d 2062 6174 6f72 6368 5f74  sets = batorch_t
+00010300: 656e 736f 7228 6f66 6673 6574 7329 0a20  ensor(offsets). 
+00010310: 2020 2020 2020 2069 6620 6e6f 7420 6f66         if not of
+00010320: 6673 6574 732e 6861 735f 6368 616e 6e65  fsets.has_channe
+00010330: 6c3a 0a20 2020 2020 2020 2020 2020 2069  l:.            i
+00010340: 6620 6f66 6673 6574 732e 7369 7a65 2830  f offsets.size(0
+00010350: 2920 3d3d 206f 6666 7365 7473 2e6e 5f64  ) == offsets.n_d
+00010360: 696d 202d 2031 3a0a 2020 2020 2020 2020  im - 1:.        
+00010370: 2020 2020 2020 2020 6e5f 6469 6d20 3d20          n_dim = 
+00010380: 6f66 6673 6574 732e 7369 7a65 2830 290a  offsets.size(0).
+00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103a0: 6f66 6673 6574 732e 6368 616e 6e65 6c5f  offsets.channel_
+000103b0: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
+000103c0: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+000103d0: 6673 6574 7320 3d20 6f66 6673 6574 732e  fsets = offsets.
+000103e0: 756e 7371 7565 657a 6528 5b5d 290a 2020  unsqueeze([]).  
+000103f0: 2020 2020 2020 2020 2020 656c 6966 206f            elif o
+00010400: 6666 7365 7473 2e73 697a 6528 3129 203d  ffsets.size(1) =
+00010410: 3d20 6f66 6673 6574 732e 6e5f 6469 6d20  = offsets.n_dim 
+00010420: 2d20 323a 0a20 2020 2020 2020 2020 2020  - 2:.           
+00010430: 2020 2020 206e 5f64 696d 203d 206f 6666       n_dim = off
+00010440: 7365 7473 2e73 697a 6528 3129 0a20 2020  sets.size(1).   
+00010450: 2020 2020 2020 2020 2020 2020 206f 6666               off
+00010460: 7365 7473 2e63 6861 6e6e 656c 5f64 696d  sets.channel_dim
+00010470: 656e 7369 6f6e 203d 2031 0a20 2020 2020  ension = 1.     
+00010480: 2020 2020 2020 2065 6c73 653a 2072 6169         else: rai
+00010490: 7365 2054 7970 6545 7272 6f72 2866 2246  se TypeError(f"F
+000104a0: 4644 2070 6172 616d 6574 6572 7320 7769  FD parameters wi
+000104b0: 7468 2073 697a 6520 7b6f 6666 7365 7473  th size {offsets
+000104c0: 2e73 6861 7065 7d20 646f 6e6f 7420 6d61  .shape} donot ma
+000104d0: 7463 6820 285b 6e5f 6261 7463 685d 2c20  tch ([n_batch], 
+000104e0: 7b7b 6e5f 6469 6d7d 7d2c 206d 5f31 2c20  {{n_dim}}, m_1, 
+000104f0: 6d5f 322c 202e 2e2e 2c20 6d5f 7229 205b  m_2, ..., m_r) [
+00010500: 723d 6e5f 6469 6d5d 2e20 2229 0a20 2020  r=n_dim]. ").   
+00010510: 2020 2020 2069 6620 6e6f 7420 6f66 6673       if not offs
+00010520: 6574 732e 6861 735f 6261 7463 683a 0a20  ets.has_batch:. 
+00010530: 2020 2020 2020 2020 2020 206e 5f64 696d             n_dim
+00010540: 203d 206f 6666 7365 7473 2e6e 5f63 6861   = offsets.n_cha
+00010550: 6e6e 656c 0a20 2020 2020 2020 2020 2020  nnel.           
+00010560: 2069 6620 6f66 6673 6574 732e 6e5f 6469   if offsets.n_di
+00010570: 6d20 3c3d 206e 5f64 696d 202b 2031 3a20  m <= n_dim + 1: 
+00010580: 6f66 6673 6574 7320 3d20 6f66 6673 6574  offsets = offset
+00010590: 732e 756e 7371 7565 657a 6528 5b5d 290a  s.unsqueeze([]).
+000105a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000105b0: 3a20 6f66 6673 6574 732e 6261 7463 685f  : offsets.batch_
+000105c0: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
+000105d0: 2020 2020 2020 6176 6f75 6368 286f 6666        avouch(off
+000105e0: 7365 7473 2e68 6173 5f62 6174 6368 2061  sets.has_batch a
+000105f0: 6e64 206f 6666 7365 7473 2e68 6173 5f63  nd offsets.has_c
+00010600: 6861 6e6e 656c 2c20 6622 506c 6561 7365  hannel, f"Please
+00010610: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+00010620: 736f 7220 6f66 2073 697a 6520 5c0a 2020  sor of size \.  
+00010630: 2020 2020 2020 2020 2020 285b 6e5f 6261            ([n_ba
+00010640: 7463 685d 2c20 7b7b 6e5f 6469 6d7d 7d2c  tch], {{n_dim}},
+00010650: 206d 5f31 2c20 6d5f 322c 202e 2e2e 2c20   m_1, m_2, ..., 
+00010660: 6d5f 7229 205b 723d 6e5f 6469 6d5d 2066  m_r) [r=n_dim] f
+00010670: 6f72 2046 4644 2070 6172 616d 6574 6572  or FFD parameter
+00010680: 732c 2069 6e73 7465 6164 206f 6620 7b6f  s, instead of {o
+00010690: 6666 7365 7473 2e73 6861 7065 7d2e 2022  ffsets.shape}. "
+000106a0: 290a 2020 2020 2020 2020 6e5f 6469 6d20  ).        n_dim 
+000106b0: 3d20 6f66 6673 6574 732e 6e5f 6368 616e  = offsets.n_chan
+000106c0: 6e65 6c0a 2020 2020 2020 2020 7370 6163  nel.        spac
+000106d0: 696e 6720 3d20 746f 5f74 7570 6c65 2873  ing = to_tuple(s
+000106e0: 7061 6369 6e67 290a 2020 2020 2020 2020  pacing).        
+000106f0: 6f72 6967 696e 203d 2074 6f5f 7475 706c  origin = to_tupl
+00010700: 6528 6f72 6967 696e 290a 2020 2020 2020  e(origin).      
+00010710: 2020 6966 206c 656e 2873 7061 6369 6e67    if len(spacing
+00010720: 2920 3d3d 2031 3a20 7370 6163 696e 6720  ) == 1: spacing 
+00010730: 2a3d 206e 5f64 696d 0a20 2020 2020 2020  *= n_dim.       
+00010740: 2069 6620 6c65 6e28 6f72 6967 696e 2920   if len(origin) 
+00010750: 3d3d 2031 3a20 6f72 6967 696e 202a 3d20  == 1: origin *= 
+00010760: 6e5f 6469 6d0a 2020 2020 2020 2020 7375  n_dim.        su
+00010770: 7065 7228 292e 5f5f 696e 6974 5f5f 286f  per().__init__(o
+00010780: 6666 7365 7473 2c20 7370 6163 696e 673d  ffsets, spacing=
+00010790: 7370 6163 696e 672c 206f 7269 6769 6e3d  spacing, origin=
+000107a0: 6f72 6967 696e 290a 0a20 2020 2020 2020  origin)..       
+000107b0: 2073 656c 662e 6e5f 6469 6d20 3d20 6e5f   self.n_dim = n_
+000107c0: 6469 6d0a 2020 2020 2020 2020 7365 6c66  dim.        self
+000107d0: 2e6f 6666 7365 7473 203d 206f 6666 7365  .offsets = offse
+000107e0: 7473 0a20 2020 2020 2020 2073 656c 662e  ts.        self.
+000107f0: 7370 6163 696e 6720 3d20 7370 6163 696e  spacing = spacin
+00010800: 670a 2020 2020 2020 2020 7365 6c66 2e6f  g.        self.o
+00010810: 7269 6769 6e20 3d20 6f72 6967 696e 0a20  rigin = origin. 
+00010820: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
+00010830: 685f 7061 7261 6d2e 6170 7065 6e64 2827  h_param.append('
+00010840: 6f66 6673 6574 7327 290a 2020 2020 0a20  offsets').    . 
+00010850: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
+00010860: 7365 6c66 2c20 5829 3a0a 2020 2020 2020  self, X):.      
+00010870: 2020 5820 3d20 7375 7065 7228 292e 5f5f    X = super().__
+00010880: 6361 6c6c 5f5f 2858 290a 2020 2020 2020  call__(X).      
+00010890: 2020 7368 6170 6520 3d20 582e 7368 6170    shape = X.shap
+000108a0: 650a 2020 2020 2020 2020 6e5f 6469 6d20  e.        n_dim 
+000108b0: 3d20 7365 6c66 2e6e 5f64 696d 0a20 2020  = self.n_dim.   
+000108c0: 2020 2020 206f 6666 7365 7473 203d 2073       offsets = s
+000108d0: 656c 662e 6f66 6673 6574 732e 666c 6f61  elf.offsets.floa
+000108e0: 7428 290a 2020 2020 2020 2020 7370 6163  t().        spac
+000108f0: 696e 6720 3d20 7365 6c66 2e73 7061 6369  ing = self.spaci
+00010900: 6e67 0a20 2020 2020 2020 206e 5f62 6174  ng.        n_bat
+00010910: 6368 203d 206f 6666 7365 7473 2e6e 5f62  ch = offsets.n_b
+00010920: 6174 6368 0a20 2020 2020 2020 2023 2058  atch.        # X
+00010930: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
+00010940: 5f64 696d 7d2c 206e 5f64 6174 6120 3d20  _dim}, n_data = 
+00010950: 6e5f 3120 7820 6e5f 3220 7820 2e2e 2e20  n_1 x n_2 x ... 
+00010960: 7820 6e5f 7229 0a20 2020 2020 2020 2058  x n_r).        X
+00010970: 203d 2058 2e66 6c61 7474 656e 2829 0a20   = X.flatten(). 
+00010980: 2020 2020 2020 2058 202d 3d20 6274 2e63         X -= bt.c
+00010990: 6861 6e6e 656c 5f74 656e 736f 7228 7365  hannel_tensor(se
+000109a0: 6c66 2e6f 7269 6769 6e29 0a20 2020 2020  lf.origin).     
+000109b0: 2020 206e 5f64 6174 6120 3d20 582e 7369     n_data = X.si
+000109c0: 7a65 282d 3129 0a20 2020 2020 2020 2073  ze(-1).        s
+000109d0: 697a 6520 3d20 6274 2e63 6861 6e6e 656c  ize = bt.channel
+000109e0: 5f74 656e 736f 7228 6f66 6673 6574 732e  _tensor(offsets.
+000109f0: 7370 6163 6529 0a20 2020 2020 2020 2023  space).        #
+00010a00: 204e 6f72 6d61 6c69 7a65 2058 2069 6e20   Normalize X in 
+00010a10: 7468 6520 646f 6d61 696e 2028 6d5f 312c  the domain (m_1,
+00010a20: 206d 5f32 2c20 2e2e 2e2c 206d 5f7b 6e5f   m_2, ..., m_{n_
+00010a30: 6469 6d7d 292e 0a20 2020 2020 2020 2046  dim})..        F
+00010a40: 4644 5820 3d20 5820 2f20 6274 2e63 6861  FDX = X / bt.cha
+00010a50: 6e6e 656c 5f74 656e 736f 7228 7370 6163  nnel_tensor(spac
+00010a60: 696e 6729 2e66 6c6f 6174 2829 0a20 2020  ing).float().   
+00010a70: 2020 2020 2069 5820 3d20 6274 2e66 6c6f       iX = bt.flo
+00010a80: 6f72 2846 4644 5829 2e66 6c6f 6174 2829  or(FFDX).float()
+00010a90: 3b20 7558 203d 2046 4644 5820 2d20 6958  ; uX = FFDX - iX
+00010aa0: 0a20 2020 2020 2020 2023 2043 6f6d 7075  .        # Compu
+00010ab0: 7465 2074 6865 2077 6569 6768 7473 2e20  te the weights. 
+00010ac0: 573a 2028 342c 205b 6e5f 6261 7463 685d  W: (4, [n_batch]
+00010ad0: 2c20 7b6e 5f64 696d 7d2c 206e 5f64 6174  , {n_dim}, n_dat
+00010ae0: 6120 3d20 6e5f 3120 7820 6e5f 3220 7820  a = n_1 x n_2 x 
+00010af0: 2e2e 2e20 7820 6e5f 7229 0a20 2020 2020  ... x n_r).     
+00010b00: 2020 2069 203d 2062 742e 6172 616e 6765     i = bt.arange
+00010b10: 282d 312c 2033 292e 6578 7061 6e64 5f74  (-1, 3).expand_t
+00010b20: 6f28 342c 205b 6e5f 6261 7463 685d 2c20  o(4, [n_batch], 
+00010b30: 7b6e 5f64 696d 7d2c 206e 5f64 6174 612c  {n_dim}, n_data,
+00010b40: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+00010b50: 2057 203d 2042 7370 6c69 6e65 2869 2c20   W = Bspline(i, 
+00010b60: 7558 2e6d 756c 7469 706c 7928 342c 2030  uX.multiply(4, 0
+00010b70: 2929 0a20 2020 2020 2020 2022 436f 6d70  )).        "Comp
+00010b80: 7574 6520 4646 4420 5472 616e 7366 6f72  ute FFD Transfor
+00010b90: 6d61 7469 6f6e 220a 2020 2020 2020 2020  mation".        
+00010ba0: 6f75 7470 7574 203d 2062 742e 7a65 726f  output = bt.zero
+00010bb0: 735f 6c69 6b65 2858 290a 2020 2020 2020  s_like(X).      
+00010bc0: 2020 2320 4c6f 6f70 2069 6e20 7468 6520    # Loop in the 
+00010bd0: 7370 6163 6520 7b2d 312c 2030 2c20 312c  space {-1, 0, 1,
+00010be0: 2032 7d20 5e20 6e5f 6469 6d3b 2047 2069   2} ^ n_dim; G i
+00010bf0: 7320 696e 2028 302c 2031 2c20 322c 2033  s in (0, 1, 2, 3
+00010c00: 290a 2020 2020 2020 2020 666f 7220 4720  ).        for G 
+00010c10: 696e 2062 742e 696d 6167 655f 6772 6964  in bt.image_grid
+00010c20: 285b 345d 2a6e 5f64 696d 292e 666c 6174  ([4]*n_dim).flat
+00010c30: 7465 6e28 292e 7472 616e 7370 6f73 6528  ten().transpose(
+00010c40: 302c 2031 293a 0a20 2020 2020 2020 2020  0, 1):.         
+00010c50: 2020 2047 203d 2062 742e 6368 616e 6e65     G = bt.channe
+00010c60: 6c5f 7465 6e73 6f72 2847 290a 2020 2020  l_tensor(G).    
+00010c70: 2020 2020 2020 2020 2320 5765 6967 6874          # Weight
+00010c80: 7320 666f 7220 6561 6368 2070 6f69 6e74  s for each point
+00010c90: 3a20 5b70 726f 6475 6374 206f 6620 575b  : [product of W[
+00010ca0: 475b 445d 2c20 742c 2044 2c20 785d 2066  G[D], t, D, x] f
+00010cb0: 6f72 2044 2069 6e20 7261 6e67 6528 6e5f  or D in range(n_
+00010cc0: 6469 6d29 5d20 666f 7220 706f 696e 7420  dim)] for point 
+00010cd0: 7820 616e 6420 6261 7463 6820 742e 0a20  x and batch t.. 
+00010ce0: 2020 2020 2020 2020 2020 2023 2057 673a             # Wg:
+00010cf0: 2028 5b6e 5f62 6174 6368 5d2c 207b 317d   ([n_batch], {1}
+00010d00: 2c20 6e5f 6461 7461 203d 206e 5f31 2078  , n_data = n_1 x
+00010d10: 206e 5f32 2078 202e 2e2e 2078 206e 5f72   n_2 x ... x n_r
+00010d20: 290a 2020 2020 2020 2020 2020 2020 5767  ).            Wg
+00010d30: 203d 2057 2e67 6174 6865 7228 302c 2047   = W.gather(0, G
+00010d40: 2e65 7870 616e 645f 746f 2828 312c 2920  .expand_to((1,) 
+00010d50: 2b20 572e 7368 6170 655b 313a 5d29 292e  + W.shape[1:])).
+00010d60: 7371 7565 657a 6528 3029 2e70 726f 6428  squeeze(0).prod(
+00010d70: 7b7d 2c20 6b65 6570 6469 6d3d 5472 7565  {}, keepdim=True
+00010d80: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00010d90: 436f 6d70 7574 6520 7468 6520 696e 6469  Compute the indi
+00010da0: 6365 7320 6f66 2072 656c 6174 6564 2063  ces of related c
+00010db0: 6f6e 7472 6f6c 2070 6f69 6e74 732e 2049  ontrol points. I
+00010dc0: 6e64 3a20 285b 6e5f 6261 7463 685d 2c20  nd: ([n_batch], 
+00010dd0: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6120  {n_dim}, n_data 
+00010de0: 3d20 6e5f 3120 7820 6e5f 3220 7820 2e2e  = n_1 x n_2 x ..
+00010df0: 2e20 7820 6e5f 7229 0a20 2020 2020 2020  . x n_r).       
+00010e00: 2020 2020 2049 6e64 203d 2062 742e 636c       Ind = bt.cl
+00010e10: 616d 7028 6958 2e6c 6f6e 6728 2920 2b20  amp(iX.long() + 
+00010e20: 4720 2d20 312c 206d 696e 3d30 290a 2020  G - 1, min=0).  
+00010e30: 2020 2020 2020 2020 2020 496e 6420 3d20            Ind = 
+00010e40: 6274 2e6d 696e 2849 6e64 2c20 2873 697a  bt.min(Ind, (siz
+00010e50: 6520 2d20 3129 2e65 7870 616e 645f 746f  e - 1).expand_to
+00010e60: 2849 6e64 2929 0a20 2020 2020 2020 2020  (Ind)).         
+00010e70: 2020 2023 2043 6f6e 7665 7274 2074 6865     # Convert the
+00010e80: 2069 6e64 6963 6573 2074 6f20 3120 6469   indices to 1 di
+00010e90: 6d65 6e73 696f 6e61 6c2e 2044 6f74 3a20  mensional. Dot: 
+00010ea0: 285b 6e5f 6261 7463 685d 2c20 6e5f 6461  ([n_batch], n_da
+00010eb0: 7461 203d 206e 5f31 2078 206e 5f32 2078  ta = n_1 x n_2 x
+00010ec0: 202e 2e2e 2078 206e 5f72 290a 2020 2020   ... x n_r).    
+00010ed0: 2020 2020 2020 2020 446f 7420 3d20 496e          Dot = In
+00010ee0: 645b 3a2c 2030 5d0a 2020 2020 2020 2020  d[:, 0].        
+00010ef0: 2020 2020 666f 7220 7220 696e 2072 616e      for r in ran
+00010f00: 6765 2831 2c20 6e5f 6469 6d29 3a20 446f  ge(1, n_dim): Do
+00010f10: 7420 2a3d 2073 697a 655b 725d 3b20 446f  t *= size[r]; Do
+00010f20: 7420 2b3d 2049 6e64 5b3a 2c20 725d 0a20  t += Ind[:, r]. 
+00010f30: 2020 2020 2020 2020 2020 2023 204f 6274             # Obt
+00010f40: 6169 6e20 7468 6520 636f 6f72 6469 6e61  ain the coordina
+00010f50: 7465 7320 6f66 2074 6865 2063 6f6e 7472  tes of the contr
+00010f60: 6f6c 2070 6f69 6e74 732e 2043 506f 696e  ol points. CPoin
+00010f70: 7473 3a20 285b 6e5f 6261 7463 685d 2c20  ts: ([n_batch], 
+00010f80: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6120  {n_dim}, n_data 
+00010f90: 3d20 6e5f 3120 7820 6e5f 3220 7820 2e2e  = n_1 x n_2 x ..
+00010fa0: 2e20 7820 6e5f 7229 0a20 2020 2020 2020  . x n_r).       
+00010fb0: 2020 2020 2043 506f 696e 7473 203d 206f       CPoints = o
+00010fc0: 6666 7365 7473 2e66 6c61 7474 656e 2829  ffsets.flatten()
+00010fd0: 2e67 6174 6865 7228 2d31 2c20 446f 742e  .gather(-1, Dot.
+00010fe0: 6c6f 6e67 2829 2e65 7870 616e 645f 746f  long().expand_to
+00010ff0: 2849 6e64 2929 2e66 6c6f 6174 2829 0a20  (Ind)).float(). 
+00011000: 2020 2020 2020 2020 2020 2023 2041 6464             # Add
+00011010: 2074 6865 2077 6569 6768 7465 6420 636f   the weighted co
+00011020: 6e74 726f 6c20 636f 6f72 6469 6e61 7465  ntrol coordinate
+00011030: 7320 746f 2074 6865 206f 7574 7075 7420  s to the output 
+00011040: 636f 6f72 6469 6e61 7465 732e 0a20 2020  coordinates..   
+00011050: 2020 2020 2020 2020 206f 7574 7075 7420           output 
+00011060: 2b3d 2028 5767 202a 2043 506f 696e 7473  += (Wg * CPoints
+00011070: 292e 7669 6577 5f61 7328 5829 0a20 2020  ).view_as(X).   
+00011080: 2020 2020 2023 2044 656e 6f72 6d61 6c69       # Denormali
+00011090: 7a65 2074 6865 206f 7574 7075 7473 2e0a  ze the outputs..
+000110a0: 2020 2020 2020 2020 6f75 7470 7574 202b          output +
+000110b0: 3d20 580a 2020 2020 2020 2020 6f75 7470  = X.        outp
+000110c0: 7574 202b 3d20 6274 2e63 6861 6e6e 656c  ut += bt.channel
+000110d0: 5f74 656e 736f 7228 7365 6c66 2e6f 7269  _tensor(self.ori
+000110e0: 6769 6e29 0a20 2020 2020 2020 2072 6574  gin).        ret
+000110f0: 7572 6e20 6f75 7470 7574 2e76 6965 7728  urn output.view(
+00011100: 7368 6170 6529 0a0a 4061 6c69 6173 2822  shape)..@alias("
+00011110: 4444 4622 290a 636c 6173 7320 4465 6e73  DDF").class Dens
+00011120: 6544 6973 706c 6163 656d 656e 7446 6965  eDisplacementFie
+00011130: 6c64 2853 7061 7469 616c 5472 616e 7366  ld(SpatialTransf
+00011140: 6f72 6d61 7469 6f6e 293a 0a20 2020 2064  ormation):.    d
+00011150: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00011160: 2c20 6469 7370 6c61 6365 6d65 6e74 732c  , displacements,
+00011170: 2073 6861 7065 3d4e 6f6e 652c 2069 6e74   shape=None, int
+00011180: 6572 706f 6c61 7465 3d46 616c 7365 293a  erpolate=False):
+00011190: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000111a0: 2020 2020 2044 656e 7365 2044 6973 706c       Dense Displ
+000111b0: 6163 656d 656e 7420 4669 656c 6420 2844  acement Field (D
+000111c0: 4446 2920 7472 616e 7366 6f72 6d61 7469  DF) transformati
+000111d0: 6f6e 2e0a 2020 2020 2020 2020 0a20 2020  on..        .   
+000111e0: 2020 2020 2050 6172 616d 733a 0a20 2020       Params:.   
+000111f0: 2020 2020 2020 2020 2064 6973 706c 6163           displac
+00011200: 656d 656e 7473 205b 6274 2e54 656e 736f  ements [bt.Tenso
+00011210: 725d 3a20 7468 6520 6469 7370 6c61 6365  r]: the displace
+00011220: 6d65 6e74 206f 6620 6561 6368 2076 6f78  ment of each vox
+00011230: 656c 2e20 0a20 2020 2020 2020 2020 2020  el. .           
+00011240: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
+00011250: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
+00011260: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
+00011270: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+00011280: 2020 2020 7368 6170 6520 5b62 742e 5369      shape [bt.Si
+00011290: 7a65 206f 7220 7475 706c 655d 3a20 7468  ze or tuple]: th
+000112a0: 6520 7368 6170 6520 6f66 2064 6973 706c  e shape of displ
+000112b0: 6163 656d 656e 7420 286e 6565 6465 6420  acement (needed 
+000112c0: 6966 2069 6e70 7574 2064 6973 706c 6163  if input displac
+000112d0: 656d 656e 7420 6973 2061 2074 7261 6e73  ement is a trans
+000112e0: 666f 726d 6174 696f 6e29 2e20 0a20 2020  formation). .   
+000112f0: 2020 2020 2020 2020 2069 6e74 6572 706f           interpo
+00011300: 6c61 7465 205b 626f 6f6c 5d3a 2057 6865  late [bool]: Whe
+00011310: 7468 6572 2074 6f20 666f 7263 6520 696e  ther to force in
+00011320: 7465 7270 6f6c 6174 696f 6e20 696e 2061  terpolation in a
+00011330: 7070 6c79 2e20 0a20 2020 2020 2020 2020  pply. .         
+00011340: 2020 200a 2020 2020 2020 2020 5768 656e     .        When
+00011350: 2069 7420 6973 2063 616c 6c65 643a 0a20   it is called:. 
+00011360: 2020 2020 2020 2020 2020 2058 205b 6274             X [bt
+00011370: 2e54 656e 736f 725d 3a20 436f 6f72 6469  .Tensor]: Coordi
+00011380: 6e61 7465 7320 746f 2062 6520 7472 616e  nates to be tran
+00011390: 7366 6f72 6d65 642e 0a20 2020 2020 2020  sformed..       
+000113a0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
+000113b0: 5b6e 5f62 6174 6368 3a20 6f70 7469 6f6e  [n_batch: option
+000113c0: 616c 5d2c 207b 6e5f 6469 6d7d 2c20 6e40  al], {n_dim}, n@
+000113d0: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+000113e0: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
+000113f0: 2020 6f75 7470 7574 205b 6274 2e54 656e    output [bt.Ten
+00011400: 736f 725d 3a20 5468 6520 7472 616e 7366  sor]: The transf
+00011410: 6f72 6d65 6420 636f 6f72 6469 6e61 7465  ormed coordinate
+00011420: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+00011430: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
+00011440: 6368 5d2c 207b 6e5f 6469 6d7d 2c20 6e40  ch], {n_dim}, n@
+00011450: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+00011460: 5f64 696d 290a 2020 2020 2020 2020 2727  _dim).        ''
+00011470: 270a 2020 2020 2020 2020 6966 2069 7369  '.        if isi
+00011480: 6e73 7461 6e63 6528 6469 7370 6c61 6365  nstance(displace
+00011490: 6d65 6e74 732c 2053 7061 7469 616c 5472  ments, SpatialTr
+000114a0: 616e 7366 6f72 6d61 7469 6f6e 293a 2064  ansformation): d
+000114b0: 6973 706c 6163 656d 656e 7473 203d 2064  isplacements = d
+000114c0: 6973 706c 6163 656d 656e 7473 2e74 6f44  isplacements.toD
+000114d0: 4446 2873 6861 7065 290a 2020 2020 2020  DF(shape).      
+000114e0: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
+000114f0: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
+00011500: 2864 6973 706c 6163 656d 656e 7473 290a  (displacements).
+00011510: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
+00011520: 6973 706c 6163 656d 656e 7473 2e68 6173  isplacements.has
+00011530: 5f63 6861 6e6e 656c 3a0a 2020 2020 2020  _channel:.      
+00011540: 2020 2020 2020 6966 2064 6973 706c 6163        if displac
+00011550: 656d 656e 7473 2e73 697a 6528 3029 203d  ements.size(0) =
+00011560: 3d20 6469 7370 6c61 6365 6d65 6e74 732e  = displacements.
+00011570: 6e5f 6469 6d20 2d20 313a 0a20 2020 2020  n_dim - 1:.     
+00011580: 2020 2020 2020 2020 2020 206e 5f64 696d             n_dim
+00011590: 203d 2064 6973 706c 6163 656d 656e 7473   = displacements
+000115a0: 2e73 697a 6528 3029 0a20 2020 2020 2020  .size(0).       
+000115b0: 2020 2020 2020 2020 2064 6973 706c 6163           displac
+000115c0: 656d 656e 7473 2e63 6861 6e6e 656c 5f64  ements.channel_d
+000115d0: 696d 656e 7369 6f6e 203d 2030 0a20 2020  imension = 0.   
+000115e0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000115f0: 706c 6163 656d 656e 7473 203d 2064 6973  placements = dis
+00011600: 706c 6163 656d 656e 7473 2e75 6e73 7175  placements.unsqu
+00011610: 6565 7a65 285b 5d29 0a20 2020 2020 2020  eeze([]).       
+00011620: 2020 2020 2065 6c69 6620 6469 7370 6c61       elif displa
+00011630: 6365 6d65 6e74 732e 7369 7a65 2831 2920  cements.size(1) 
+00011640: 3d3d 2064 6973 706c 6163 656d 656e 7473  == displacements
+00011650: 2e6e 5f64 696d 202d 2032 3a0a 2020 2020  .n_dim - 2:.    
+00011660: 2020 2020 2020 2020 2020 2020 6e5f 6469              n_di
+00011670: 6d20 3d20 6469 7370 6c61 6365 6d65 6e74  m = displacement
+00011680: 732e 7369 7a65 2831 290a 2020 2020 2020  s.size(1).      
+00011690: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+000116a0: 6365 6d65 6e74 732e 6368 616e 6e65 6c5f  cements.channel_
+000116b0: 6469 6d65 6e73 696f 6e20 3d20 310a 2020  dimension = 1.  
+000116c0: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
+000116d0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+000116e0: 6622 4444 4620 7061 7261 6d65 7465 7273  f"DDF parameters
+000116f0: 2077 6974 6820 7369 7a65 207b 6469 7370   with size {disp
+00011700: 6c61 6365 6d65 6e74 732e 7368 6170 657d  lacements.shape}
+00011710: 2064 6f6e 6f74 206d 6174 6368 2028 5b6e   donot match ([n
+00011720: 5f62 6174 6368 5d2c 207b 7b6e 5f64 696d  _batch], {{n_dim
+00011730: 7d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  }}, n@1, n@2, ..
+00011740: 2e2c 206e 406e 5f64 696d 292e 2022 290a  ., n@n_dim). ").
+00011750: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
+00011760: 6973 706c 6163 656d 656e 7473 2e68 6173  isplacements.has
+00011770: 5f62 6174 6368 3a0a 2020 2020 2020 2020  _batch:.        
+00011780: 2020 2020 6e5f 6469 6d20 3d20 6469 7370      n_dim = disp
+00011790: 6c61 6365 6d65 6e74 732e 6e5f 6368 616e  lacements.n_chan
+000117a0: 6e65 6c0a 2020 2020 2020 2020 2020 2020  nel.            
+000117b0: 6966 2064 6973 706c 6163 656d 656e 7473  if displacements
+000117c0: 2e6e 5f64 696d 203c 3d20 6e5f 6469 6d20  .n_dim <= n_dim 
+000117d0: 2b20 313a 2064 6973 706c 6163 656d 656e  + 1: displacemen
+000117e0: 7473 203d 2064 6973 706c 6163 656d 656e  ts = displacemen
+000117f0: 7473 2e75 6e73 7175 6565 7a65 285b 5d29  ts.unsqueeze([])
+00011800: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00011810: 653a 2064 6973 706c 6163 656d 656e 7473  e: displacements
+00011820: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+00011830: 203d 2030 0a20 2020 2020 2020 2064 6973   = 0.        dis
+00011840: 706c 6163 656d 656e 7473 203d 2064 6973  placements = dis
+00011850: 706c 6163 656d 656e 7473 2e66 6c6f 6174  placements.float
+00011860: 2829 0a20 2020 2020 2020 2061 766f 7563  ().        avouc
+00011870: 6828 6469 7370 6c61 6365 6d65 6e74 732e  h(displacements.
+00011880: 6861 735f 6261 7463 6820 616e 6420 6469  has_batch and di
+00011890: 7370 6c61 6365 6d65 6e74 732e 6861 735f  splacements.has_
+000118a0: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
+000118b0: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
+000118c0: 6e73 6f72 206f 6620 7369 7a65 205c 0a20  nsor of size \. 
+000118d0: 2020 2020 2020 2020 2020 2028 5b6e 5f62             ([n_b
+000118e0: 6174 6368 5d2c 207b 7b6e 5f64 696d 7d7d  atch], {{n_dim}}
+000118f0: 2c20 6e40 312c 206e 4032 2c20 2e2e 2e2c  , n@1, n@2, ...,
+00011900: 206e 406e 5f64 696d 2920 666f 7220 4444   n@n_dim) for DD
+00011910: 4620 7061 7261 6d65 7465 7273 2c20 696e  F parameters, in
+00011920: 7374 6561 6420 6f66 207b 6469 7370 6c61  stead of {displa
+00011930: 6365 6d65 6e74 732e 7368 6170 657d 2e20  cements.shape}. 
+00011940: 2229 0a20 2020 2020 2020 2073 7570 6572  ").        super
+00011950: 2829 2e5f 5f69 6e69 745f 5f28 6469 7370  ().__init__(disp
+00011960: 6c61 6365 6d65 6e74 732c 2073 6861 7065  lacements, shape
+00011970: 3d73 6861 7065 2c20 696e 7465 7270 6f6c  =shape, interpol
+00011980: 6174 653d 696e 7465 7270 6f6c 6174 6529  ate=interpolate)
+00011990: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
+000119a0: 6469 6d20 3d20 6469 7370 6c61 6365 6d65  dim = displaceme
+000119b0: 6e74 732e 6e5f 6368 616e 6e65 6c0a 2020  nts.n_channel.  
+000119c0: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
+000119d0: 6163 656d 656e 7473 203d 2064 6973 706c  acements = displ
+000119e0: 6163 656d 656e 7473 0a20 2020 2020 2020  acements.       
+000119f0: 2073 656c 662e 696e 7465 7270 6f6c 6174   self.interpolat
+00011a00: 6520 3d20 696e 7465 7270 6f6c 6174 650a  e = interpolate.
+00011a10: 2020 2020 2020 2020 7365 6c66 2e62 6174          self.bat
+00011a20: 6368 5f70 6172 616d 2e61 7070 656e 6428  ch_param.append(
+00011a30: 2764 6973 706c 6163 656d 656e 7473 2729  'displacements')
+00011a40: 0a20 2020 200a 2020 2020 6465 6620 5f5f  .    .    def __
+00011a50: 6361 6c6c 5f5f 2873 656c 662c 2058 293a  call__(self, X):
+00011a60: 0a20 2020 2020 2020 2058 203d 2073 7570  .        X = sup
+00011a70: 6572 2829 2e5f 5f63 616c 6c5f 5f28 5829  er().__call__(X)
+00011a80: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
+00011a90: 656d 656e 7473 203d 2073 656c 662e 6469  ements = self.di
+00011aa0: 7370 6c61 6365 6d65 6e74 730a 2020 2020  splacements.    
+00011ab0: 2020 2020 6e5f 6469 6d20 3d20 7365 6c66      n_dim = self
+00011ac0: 2e6e 5f64 696d 0a20 2020 2020 2020 2069  .n_dim.        i
+00011ad0: 6620 582e 6e5f 7370 6163 6520 3d3d 2030  f X.n_space == 0
+00011ae0: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
+00011af0: 6528 2d31 290a 2020 2020 2020 2020 6966  e(-1).        if
+00011b00: 206e 6f74 2073 656c 662e 696e 7465 7270   not self.interp
+00011b10: 6f6c 6174 6520 616e 6420 582e 7370 6163  olate and X.spac
+00011b20: 6520 3d3d 2064 6973 706c 6163 656d 656e  e == displacemen
+00011b30: 7473 2e73 7061 6365 2061 6e64 2058 2e6e  ts.space and X.n
+00011b40: 5f63 6861 6e6e 656c 203d 3d20 6469 7370  _channel == disp
+00011b50: 6c61 6365 6d65 6e74 732e 6e5f 6368 616e  lacements.n_chan
+00011b60: 6e65 6c3a 2072 6574 7572 6e20 5820 2b20  nel: return X + 
+00011b70: 6469 7370 6c61 6365 6d65 6e74 730a 2020  displacements.  
+00011b80: 2020 2020 2020 656c 7365 3a20 7265 7475        else: retu
+00011b90: 726e 2058 202b 2069 6e74 6572 706f 6c61  rn X + interpola
+00011ba0: 7469 6f6e 2864 6973 706c 6163 656d 656e  tion(displacemen
+00011bb0: 7473 2c20 7461 7267 6574 5f73 7061 6365  ts, target_space
+00011bc0: 3d58 292e 6368 616e 6e65 6c5f 6469 6d65  =X).channel_dime
+00011bd0: 6e73 696f 6e5f 2831 290a 0a40 616c 6961  nsion_(1)..@alia
+00011be0: 7328 224d 4c50 2229 0a63 6c61 7373 204d  s("MLP").class M
+00011bf0: 756c 7469 4c61 7965 7250 6572 6365 7074  ultiLayerPercept
+00011c00: 696f 6e28 5370 6174 6961 6c54 7261 6e73  ion(SpatialTrans
+00011c10: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
+00011c20: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00011c30: 662c 2077 6569 6768 7473 2c20 6869 6464  f, weights, hidd
+00011c40: 656e 5f6c 6179 6572 733d 5b5d 2c20 6163  en_layers=[], ac
+00011c50: 7469 7665 5f66 756e 6374 696f 6e3d 4e6f  tive_function=No
+00011c60: 6e65 2c20 7472 616e 735f 7374 7265 7463  ne, trans_stretc
+00011c70: 683d 3129 3a0a 2020 2020 2020 2020 2727  h=1):.        ''
+00011c80: 270a 2020 2020 2020 2020 4120 7472 616e  '.        A tran
+00011c90: 7366 6f72 6d61 7469 6f6e 2064 6566 696e  sformation defin
+00011ca0: 6564 2062 7920 6120 4d4c 502e 200a 2020  ed by a MLP. .  
+00011cb0: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
+00011cc0: 6172 616d 733a 0a20 2020 2020 2020 2020  arams:.         
+00011cd0: 2020 2077 6569 6768 7473 205b 6274 2e54     weights [bt.T
+00011ce0: 656e 736f 725d 3a20 7468 6520 7765 6967  ensor]: the weig
+00011cf0: 6874 7320 666f 7220 7468 6520 7065 7263  hts for the perc
+00011d00: 6570 7469 6f6e 206e 6574 776f 726b 2e20  eption network. 
+00011d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d20: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+00011d30: 5d2c 206e 5f64 696d 202a 206e 5f68 6c5f  ], n_dim * n_hl_
+00011d40: 3120 2b20 6e5f 686c 5f31 202b 2073 756d  1 + n_hl_1 + sum
+00011d50: 2869 3d31 2e2e 6b2d 3129 7b6e 5f68 6c5f  (i=1..k-1){n_hl_
+00011d60: 6920 2a20 6e5f 686c 5f7b 692b 317d 202b  i * n_hl_{i+1} +
+00011d70: 206e 5f68 6c5f 7b69 2b31 7d7d 202b 206e   n_hl_{i+1}} + n
+00011d80: 5f68 6c5f 6b20 2a20 6e5f 6469 6d20 2b20  _hl_k * n_dim + 
+00011d90: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
+00011da0: 2020 2020 2020 2077 6865 7265 206b 2069         where k i
+00011db0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
+00011dc0: 6869 6464 656e 206c 6179 6572 7320 616e  hidden layers an
+00011dd0: 6420 6e5f 686c 5f69 2069 7320 7468 6520  d n_hl_i is the 
+00011de0: 6c65 6e67 7468 206f 6620 7468 6520 692d  length of the i-
+00011df0: 7468 2068 6964 6465 6e20 6c61 7965 722e  th hidden layer.
+00011e00: 200a 2020 2020 2020 2020 2020 2020 6869   .            hi
+00011e10: 6464 656e 5f6c 6179 6572 7320 5b6c 6973  dden_layers [lis
+00011e20: 7420 6f66 2069 6e74 5d3a 2074 6865 206c  t of int]: the l
+00011e30: 656e 6774 6873 2066 6f72 2074 6865 2068  engths for the h
+00011e40: 6964 6465 6e20 6c61 7965 7273 2c20 692e  idden layers, i.
+00011e50: 652e 205b 6e5f 686c 5f31 2c20 6e5f 686c  e. [n_hl_1, n_hl
+00011e60: 5f32 2c20 2e2e 2e2c 206e 5f68 6c5f 6b5d  _2, ..., n_hl_k]
+00011e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011e80: 2049 7420 6973 2062 7920 6465 6661 756c   It is by defaul
+00011e90: 7420 275b 5d27 2073 6f20 7468 6174 2074  t '[]' so that t
+00011ea0: 6865 2064 6566 6175 6c74 204d 4c50 2069  he default MLP i
+00011eb0: 7320 616e 2061 6666 696e 6520 7472 616e  s an affine tran
+00011ec0: 7366 6f72 6d61 7469 6f6e 2e20 0a20 2020  sformation. .   
+00011ed0: 2020 2020 2020 2020 2061 6374 6976 655f           active_
+00011ee0: 6675 6e63 7469 6f6e 205b 636c 6173 735d  function [class]
+00011ef0: 3a20 7468 6520 6163 7469 7665 5f66 756e  : the active_fun
+00011f00: 6374 696f 6e2e 200a 2020 2020 2020 2020  ction. .        
+00011f10: 2020 2020 7472 616e 735f 7374 7265 7463      trans_stretc
+00011f20: 6820 5b69 6e74 5d3a 2031 2062 7920 6465  h [int]: 1 by de
+00011f30: 6661 756c 742e 2032 3020 7365 656d 7320  fault. 20 seems 
+00011f40: 746f 2062 6520 6120 676f 6f64 2063 686f  to be a good cho
+00011f50: 6963 652e 200a 2020 2020 2020 2020 2020  ice. .          
+00011f60: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
+00011f70: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
+00011f80: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
+00011f90: 5465 6e73 6f72 5d3a 2043 6f6f 7264 696e  Tensor]: Coordin
+00011fa0: 6174 6573 2074 6f20 6265 2074 7261 6e73  ates to be trans
+00011fb0: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
+00011fc0: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+00011fd0: 6e5f 6261 7463 683a 206f 7074 696f 6e61  n_batch: optiona
+00011fe0: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 4031  l], {n_dim}, n@1
+00011ff0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+00012000: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+00012010: 206f 7574 7075 7420 5b62 742e 5465 6e73   output [bt.Tens
+00012020: 6f72 5d3a 2054 6865 2074 7261 6e73 666f  or]: The transfo
+00012030: 726d 6564 2063 6f6f 7264 696e 6174 6573  rmed coordinates
+00012040: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012050: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+00012060: 685d 2c20 7b6e 5f64 696d 7d2c 206e 4031  h], {n_dim}, n@1
+00012070: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+00012080: 6469 6d29 0a20 2020 2020 2020 2027 2727  dim).        '''
+00012090: 0a20 2020 2020 2020 2073 656c 662e 6869  .        self.hi
+000120a0: 6464 656e 5f6c 6179 6572 7320 3d20 6869  dden_layers = hi
+000120b0: 6464 656e 5f6c 6179 6572 730a 2020 2020  dden_layers.    
+000120c0: 2020 2020 6966 206e 6f74 2077 6569 6768      if not weigh
+000120d0: 7473 2e68 6173 5f62 6174 6368 3a0a 2020  ts.has_batch:.  
+000120e0: 2020 2020 2020 2020 2020 6966 2077 6569            if wei
+000120f0: 6768 7473 2e6e 5f64 696d 203d 3d20 323a  ghts.n_dim == 2:
+00012100: 2077 6569 6768 7473 2e62 6174 6368 5f64   weights.batch_d
+00012110: 696d 203d 2030 0a20 2020 2020 2020 2020  im = 0.         
+00012120: 2020 2065 6c73 653a 2077 6569 6768 7473     else: weights
+00012130: 203d 2077 6569 6768 7473 2e75 6e73 7175   = weights.unsqu
+00012140: 6565 7a65 285b 5d29 0a20 2020 2020 2020  eeze([]).       
+00012150: 2073 656c 662e 7765 6967 6874 7320 3d20   self.weights = 
+00012160: 7765 6967 6874 730a 2020 2020 2020 2020  weights.        
+00012170: 7365 6c66 2e74 7261 6e73 5f73 7472 6574  self.trans_stret
+00012180: 6368 203d 2074 7261 6e73 5f73 7472 6574  ch = trans_stret
+00012190: 6368 0a20 2020 2020 2020 2073 7570 6572  ch.        super
+000121a0: 2829 2e5f 5f69 6e69 745f 5f28 7765 6967  ().__init__(weig
+000121b0: 6874 732c 2068 6964 6465 6e5f 6c61 7965  hts, hidden_laye
+000121c0: 7273 203d 2068 6964 6465 6e5f 6c61 7965  rs = hidden_laye
+000121d0: 7273 2c20 7472 616e 735f 7374 7265 7463  rs, trans_stretc
+000121e0: 6820 3d20 7472 616e 735f 7374 7265 7463  h = trans_stretc
+000121f0: 6829 0a20 2020 2020 2020 2064 696d 5f63  h).        dim_c
+00012200: 6f6e 7374 203d 2077 6569 6768 7473 2e73  onst = weights.s
+00012210: 697a 6528 2d31 2920 2d20 7375 6d28 6869  ize(-1) - sum(hi
+00012220: 6464 656e 5f6c 6179 6572 7329 202d 2073  dden_layers) - s
+00012230: 756d 2878 202a 2079 2066 6f72 2078 2c20  um(x * y for x, 
+00012240: 7920 696e 207a 6970 2868 6964 6465 6e5f  y in zip(hidden_
+00012250: 6c61 7965 7273 5b3a 2d31 5d2c 2068 6964  layers[:-1], hid
+00012260: 6465 6e5f 6c61 7965 7273 5b31 3a5d 2929  den_layers[1:]))
+00012270: 0a20 2020 2020 2020 2064 696d 5f63 6f65  .        dim_coe
+00012280: 6666 203d 2068 6964 6465 6e5f 6c61 7965  ff = hidden_laye
+00012290: 7273 5b30 5d20 2b20 6869 6464 656e 5f6c  rs[0] + hidden_l
+000122a0: 6179 6572 735b 2d31 5d20 2b20 310a 2020  ayers[-1] + 1.  
+000122b0: 2020 2020 2020 6176 6f75 6368 2864 696d        avouch(dim
+000122c0: 5f63 6f6e 7374 2025 2064 696d 5f63 6f65  _const % dim_coe
+000122d0: 6666 203d 3d20 302c 2066 2257 726f 6e67  ff == 0, f"Wrong
+000122e0: 2077 6569 6768 7420 6c65 6e67 7468 2066   weight length f
+000122f0: 6f72 2068 6964 6465 6e20 6c61 7965 7273  or hidden layers
+00012300: 206f 6620 7369 7a65 7320 7b68 6964 6465   of sizes {hidde
+00012310: 6e5f 6c61 7965 7273 7d2c 207b 6469 6d5f  n_layers}, {dim_
+00012320: 636f 6566 667d 2078 206e 5f64 696d 202b  coeff} x n_dim +
+00012330: 207b 6469 6d5f 636f 6e73 747d 2065 7870   {dim_const} exp
+00012340: 6563 7465 642c 2062 7574 2067 6f74 207b  ected, but got {
+00012350: 7765 6967 6874 732e 7369 7a65 282d 3129  weights.size(-1)
+00012360: 7d2e 2229 0a20 2020 2020 2020 2073 656c  }.").        sel
+00012370: 662e 6e5f 6469 6d20 3d20 6469 6d5f 636f  f.n_dim = dim_co
+00012380: 6e73 7420 2f2f 2064 696d 5f63 6f65 6666  nst // dim_coeff
+00012390: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
+000123a0: 6261 7463 6820 3d20 7765 6967 6874 732e  batch = weights.
+000123b0: 6e5f 6261 7463 680a 2020 2020 2020 2020  n_batch.        
+000123c0: 7365 6c66 2e6c 6179 6572 7320 3d20 5b5d  self.layers = []
+000123d0: 0a20 2020 2020 2020 2070 203d 2030 0a20  .        p = 0. 
+000123e0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000123f0: 7261 6e67 6528 6c65 6e28 6869 6464 656e  range(len(hidden
+00012400: 5f6c 6179 6572 7329 202b 2031 293a 0a20  _layers) + 1):. 
+00012410: 2020 2020 2020 2020 2020 2069 6e5f 6665             in_fe
+00012420: 6174 7572 6573 203d 2073 656c 662e 6e5f  atures = self.n_
+00012430: 6469 6d20 6966 2069 203d 3d20 3020 656c  dim if i == 0 el
+00012440: 7365 2068 6964 6465 6e5f 6c61 7965 7273  se hidden_layers
+00012450: 5b69 202d 2031 5d0a 2020 2020 2020 2020  [i - 1].        
+00012460: 2020 2020 6f75 745f 6665 6174 7572 6573      out_features
+00012470: 203d 2073 656c 662e 6e5f 6469 6d20 6966   = self.n_dim if
+00012480: 2069 203d 3d20 6c65 6e28 6869 6464 656e   i == len(hidden
+00012490: 5f6c 6179 6572 7329 2065 6c73 6520 6869  _layers) else hi
+000124a0: 6464 656e 5f6c 6179 6572 735b 695d 0a20  dden_layers[i]. 
+000124b0: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+000124c0: 5f77 6569 6768 7473 203d 2077 6569 6768  _weights = weigh
+000124d0: 7473 5b2e 2e2e 2c20 703a 702b 6f75 745f  ts[..., p:p+out_
+000124e0: 6665 6174 7572 6573 2a69 6e5f 6665 6174  features*in_feat
+000124f0: 7572 6573 5d2e 7669 6577 285b 7365 6c66  ures].view([self
+00012500: 2e6e 5f62 6174 6368 5d2c 206f 7574 5f66  .n_batch], out_f
+00012510: 6561 7475 7265 732c 2069 6e5f 6665 6174  eatures, in_feat
 00012520: 7572 6573 290a 2020 2020 2020 2020 2020  ures).          
 00012530: 2020 7020 2b3d 206f 7574 5f66 6561 7475    p += out_featu
-00012540: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
-00012550: 7365 6c66 2e6c 6179 6572 732e 6170 7065  self.layers.appe
-00012560: 6e64 2828 6c61 7965 725f 7765 6967 6874  nd((layer_weight
-00012570: 732c 206c 6179 6572 5f62 6961 7329 290a  s, layer_bias)).
-00012580: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-00012590: 6976 655f 6675 6e63 7469 6f6e 203d 2061  ive_function = a
-000125a0: 6374 6976 655f 6675 6e63 7469 6f6e 0a20  ctive_function. 
-000125b0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-000125c0: 6374 6976 655f 6675 6e63 7469 6f6e 2069  ctive_function i
-000125d0: 7320 4e6f 6e65 3a20 7365 6c66 2e61 6374  s None: self.act
-000125e0: 6976 655f 6675 6e63 7469 6f6e 203d 2062  ive_function = b
-000125f0: 742e 6e6e 2e52 654c 550a 2020 2020 0a20  t.nn.ReLU.    . 
-00012600: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00012610: 2064 6566 206e 5f77 6569 6768 745f 6c65   def n_weight_le
-00012620: 6e67 7468 2873 656c 6629 3a0a 2020 2020  ngth(self):.    
-00012630: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00012640: 6e5f 6469 6d20 2a20 2873 656c 662e 6869  n_dim * (self.hi
-00012650: 6464 656e 5f6c 6179 6572 735b 305d 202b  dden_layers[0] +
-00012660: 2073 656c 662e 6869 6464 656e 5f6c 6179   self.hidden_lay
-00012670: 6572 735b 2d31 5d20 2b20 3129 202b 2073  ers[-1] + 1) + s
-00012680: 756d 2873 656c 662e 6869 6464 656e 5f6c  um(self.hidden_l
-00012690: 6179 6572 7329 202b 2073 756d 2878 202a  ayers) + sum(x *
-000126a0: 2079 2066 6f72 2078 2c20 7920 696e 207a   y for x, y in z
-000126b0: 6970 2873 656c 662e 6869 6464 656e 5f6c  ip(self.hidden_l
-000126c0: 6179 6572 735b 3a2d 315d 2c20 7365 6c66  ayers[:-1], self
-000126d0: 2e68 6964 6465 6e5f 6c61 7965 7273 5b31  .hidden_layers[1
-000126e0: 3a5d 2929 0a20 2020 200a 2020 2020 6465  :])).    .    de
-000126f0: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
-00012700: 2058 293a 0a20 2020 2020 2020 2058 203d   X):.        X =
-00012710: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
-00012720: 5f28 5829 0a20 2020 2020 2020 2069 6620  _(X).        if 
-00012730: 582e 6e5f 7370 6163 6520 3d3d 2030 3a20  X.n_space == 0: 
-00012740: 5820 3d20 582e 756e 7371 7565 657a 6528  X = X.unsqueeze(
-00012750: 2d31 290a 2020 2020 2020 2020 5920 3d20  -1).        Y = 
-00012760: 582e 666c 6174 7465 6e28 292e 6368 616e  X.flatten().chan
-00012770: 6e65 6c5f 6469 6d5f 284e 6f6e 6529 0a20  nel_dim_(None). 
-00012780: 2020 2020 2020 2066 6f72 2069 2c20 2877         for i, (w
-00012790: 6569 6768 7473 2c20 6269 6173 2920 696e  eights, bias) in
-000127a0: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
-000127b0: 6c61 7965 7273 293a 0a20 2020 2020 2020  layers):.       
-000127c0: 2020 2020 2059 203d 2077 6569 6768 7473       Y = weights
-000127d0: 2040 2059 0a20 2020 2020 2020 2020 2020   @ Y.           
-000127e0: 2069 6620 6920 3c20 6c65 6e28 7365 6c66   if i < len(self
-000127f0: 2e6c 6179 6572 7329 202d 2031 3a20 5920  .layers) - 1: Y 
-00012800: 3d20 7365 6c66 2e61 6374 6976 655f 6675  = self.active_fu
-00012810: 6e63 7469 6f6e 2829 2859 202b 2062 6961  nction()(Y + bia
-00012820: 732e 756e 7371 7565 657a 6528 2d31 2929  s.unsqueeze(-1))
-00012830: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00012840: 653a 2059 202b 3d20 7365 6c66 2e74 7261  e: Y += self.tra
-00012850: 6e73 5f73 7472 6574 6368 202a 2062 6961  ns_stretch * bia
-00012860: 732e 756e 7371 7565 657a 6528 2d31 290a  s.unsqueeze(-1).
-00012870: 2020 2020 2020 2020 7265 7475 726e 2058          return X
-00012880: 202b 2059 2e76 6965 775f 6173 2858 292e   + Y.view_as(X).
-00012890: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
-000128a0: 6e5f 2831 290a 0a40 616c 6961 7328 2272  n_(1)..@alias("r
-000128b0: 6573 616d 706c 6522 290a 6465 6620 696e  esample").def in
-000128c0: 7465 7270 6f6c 6174 696f 6e28 0a20 2020  terpolation(.   
-000128d0: 2020 2020 2069 6d61 6765 3a20 6274 2e54       image: bt.T
-000128e0: 656e 736f 722c 200a 2020 2020 2020 2020  ensor, .        
-000128f0: 7472 616e 733a 2043 616c 6c61 626c 6520  trans: Callable 
-00012900: 3d20 4e6f 6e65 2c20 0a20 2020 2020 2020  = None, .       
-00012910: 206d 6574 686f 643a 2073 7472 203d 2027   method: str = '
-00012920: 4c69 6e65 6172 272c 200a 2020 2020 2020  Linear', .      
-00012930: 2020 7461 7267 6574 5f73 7061 6365 3a20    target_space: 
-00012940: 7475 706c 6520 3d20 4e6f 6e65 2c0a 2020  tuple = None,.  
-00012950: 2020 2020 2020 6669 6c6c 3a20 2873 7472        fill: (str
-00012960: 2c20 696e 742c 2066 6c6f 6174 2920 3d20  , int, float) = 
-00012970: 302c 0a20 2020 2020 2020 2064 6572 6976  0,.        deriv
-00012980: 6174 6976 653a 2062 6f6f 6c20 3d20 4661  ative: bool = Fa
-00012990: 6c73 650a 2020 2020 293a 0a20 2020 2027  lse.    ):.    '
-000129a0: 2727 0a20 2020 2049 6e74 6572 706f 6c61  ''.    Interpola
-000129b0: 7465 2075 7369 6e67 2062 6163 6b77 6172  te using backwar
-000129c0: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
-000129d0: 2e0a 2020 2020 692e 652e 2043 6f6d 7075  ..    i.e. Compu
-000129e0: 7465 2074 6865 2069 6d61 6765 2049 2073  te the image I s
-000129f0: 2e74 2e20 7472 616e 7328 7829 203d 2079  .t. trans(x) = y
-00012a00: 2066 6f72 2078 2069 6e20 4920 616e 6420   for x in I and 
-00012a10: 7920 696e 2069 6e70 7574 2069 6d61 6765  y in input image
-00012a20: 2075 7369 6e67 2069 6e74 6572 706f 6c61   using interpola
-00012a30: 7469 6f6e 206d 6574 686f 643a 0a20 2020  tion method:.   
-00012a40: 2020 2020 206d 6574 686f 6420 3d20 4c69       method = Li
-00012a50: 6e65 6172 3a20 4269 6c69 6e65 6172 2069  near: Bilinear i
-00012a60: 6e74 6572 706f 6c61 7469 6f6e 0a20 2020  nterpolation.   
-00012a70: 2020 2020 206d 6574 686f 6420 3d20 4e65       method = Ne
-00012a80: 6172 6573 7420 5b4e 4f20 4752 4144 4945  arest [NO GRADIE
-00012a90: 4e54 2121 215d 3a20 4e65 6172 6573 7420  NT!!!]: Nearest 
-00012aa0: 696e 7465 7270 6f6c 6174 696f 6e0a 0a20  interpolation.. 
-00012ab0: 2020 2050 6172 616d 733a 0a20 2020 2020     Params:.     
-00012ac0: 2020 2069 6d61 6765 205b 6274 2e54 656e     image [bt.Ten
-00012ad0: 736f 725d 3a20 5468 6520 7461 7267 6574  sor]: The target
-00012ae0: 2069 6d61 6765 2e0a 2020 2020 2020 2020   image..        
-00012af0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00012b00: 7463 683a 6f70 7469 6f6e 616c 5d2c 207b  tch:optional], {
-00012b10: 6e5f 6368 616e 6e65 6c3a 6f70 7469 6f6e  n_channel:option
-00012b20: 616c 7d2c 206d 4031 2c20 6d40 322c 202e  al}, m@1, m@2, .
-00012b30: 2e2e 2c20 6d40 6e5f 6469 6d29 0a20 2020  .., m@n_dim).   
-00012b40: 2020 2020 2074 7261 6e73 205b 4675 6e63       trans [Func
-00012b50: 7469 6f6e 206f 7220 6d69 636f 6d70 7574  tion or micomput
-00012b60: 696e 672e 5370 6174 6961 6c54 7261 6e73  ing.SpatialTrans
-00012b70: 666f 726d 6174 696f 6e5d 3a20 5472 616e  formation]: Tran
-00012b80: 7366 6f72 6d61 7469 6f6e 2066 756e 6374  sformation funct
-00012b90: 696f 6e2c 206d 6170 7069 6e67 0a20 2020  ion, mapping.   
-00012ba0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-00012bb0: 5b6e 5f62 6174 6368 3a6f 7074 696f 6e61  [n_batch:optiona
-00012bc0: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 4031  l], {n_dim}, n@1
-00012bd0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-00012be0: 6469 6d29 2074 6f20 285b 6e5f 6261 7463  dim) to ([n_batc
-00012bf0: 685d 2c20 7b6e 5f64 696d 7d2c 206e 4031  h], {n_dim}, n@1
-00012c00: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-00012c10: 6469 6d29 0a20 2020 2020 2020 206d 6574  dim).        met
-00012c20: 686f 6420 5b73 7472 3a20 6c69 6e65 6172  hod [str: linear
-00012c30: 7c6e 6561 7265 7374 5d3a 2054 6865 2069  |nearest]: The i
-00012c40: 6e74 6572 706f 6c61 7469 6f6e 206d 6574  nterpolation met
-00012c50: 686f 642e 200a 2020 2020 2020 2020 7461  hod. .        ta
-00012c60: 7267 6574 5f73 7061 6365 205b 7475 706c  rget_space [tupl
-00012c70: 6520 6f72 2062 742e 5465 6e73 6f72 5d3a  e or bt.Tensor]:
-00012c80: 0a20 2020 2020 2020 2020 2020 2053 697a  .            Siz
-00012c90: 6520 2874 7570 6c65 2920 6f66 2061 2074  e (tuple) of a t
-00012ca0: 6172 6765 7420 524f 4920 6174 2074 6865  arget ROI at the
-00012cb0: 2063 656e 7465 7220 6f66 2069 6d61 6765   center of image
-00012cc0: 2e20 0a20 2020 2020 2020 2020 2020 204f  . .            O
-00012cd0: 5220 5472 616e 7366 6f72 6d65 6420 636f  R Transformed co
-00012ce0: 6f72 6469 6e61 7465 2073 7061 6365 2028  ordinate space (
-00012cf0: 6274 2e54 656e 736f 7229 206f 6620 7468  bt.Tensor) of th
-00012d00: 6520 6f75 7470 7574 2069 6d61 6765 2e20  e output image. 
-00012d10: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00012d20: 653a 206c 656e 6774 6828 6e5f 6469 6d29  e: length(n_dim)
-00012d30: 206f 7220 285b 6e5f 6261 7463 683a 6f70   or ([n_batch:op
-00012d40: 7469 6f6e 616c 5d2c 207b 6e5f 6469 6d3a  tional], {n_dim:
-00012d50: 6f70 7469 6f6e 616c 7d2c 2073 697a 6540  optional}, size@
-00012d60: 312c 2073 697a 6540 322c 202e 2e2e 2c20  1, size@2, ..., 
-00012d70: 7369 7a65 4072 290a 2020 2020 2020 2020  size@r).        
-00012d80: 6669 6c6c 205b 7374 723a 206e 6561 7265  fill [str: neare
-00012d90: 7374 7c62 6163 6b67 726f 756e 6420 6f72  st|background or
-00012da0: 2069 6e74 206f 7220 666c 6f61 7428 6e75   int or float(nu
-00012db0: 6d62 6572 295d 3a20 496e 6469 6361 7465  mber)]: Indicate
-00012dc0: 2074 6865 2077 6179 2074 6f20 6669 6c6c   the way to fill
-00012dd0: 2062 6163 6b67 726f 756e 6420 6f75 7473   background outs
-00012de0: 6964 6520 6053 7572 726f 756e 6469 6e67  ide `Surrounding
-00012df0: 602e 200a 2020 2020 2020 2020 6465 7269  `. .        deri
-00012e00: 7661 7469 7665 205b 626f 6f6c 5d3a 2057  vative [bool]: W
-00012e10: 6865 7468 6572 2074 6f20 7265 7475 726e  hether to return
-00012e20: 2074 6865 2067 7261 6469 656e 742e 204f   the gradient. O
-00012e30: 6e65 2063 616e 206f 6d69 7420 6974 2077  ne can omit it w
-00012e40: 6865 6e20 7573 696e 6720 746f 7263 682e  hen using torch.
-00012e50: 6175 746f 6772 6164 2e0a 0a20 2020 2020  autograd...     
-00012e60: 2020 206f 7574 7075 7420 5b62 742e 5465     output [bt.Te
-00012e70: 6e73 6f72 5d3a 2054 6865 2074 7261 6e73  nsor]: The trans
-00012e80: 666f 726d 6564 2069 6d61 6765 2e0a 2020  formed image..  
-00012e90: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00012ea0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f63  ([n_batch], {n_c
-00012eb0: 6861 6e6e 656c 3a6f 7074 696f 6e61 6c7d  hannel:optional}
-00012ec0: 2c20 6d40 312c 206d 4032 2c20 2e2e 2e2c  , m@1, m@2, ...,
-00012ed0: 206d 406e 5f64 696d 290a 2020 2020 2020   m@n_dim).      
-00012ee0: 2020 2020 2020 6f72 2077 6865 6e20 6074        or when `t
-00012ef0: 6172 6765 745f 7370 6163 6560 2069 7320  arget_space` is 
-00012f00: 6465 6669 6e65 6420 6279 2074 656e 736f  defined by tenso
-00012f10: 722e 200a 2020 2020 2020 2020 2020 2020  r. .            
-00012f20: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
-00012f30: 2c20 7369 7a65 4031 2c20 7369 7a65 4032  , size@1, size@2
-00012f40: 2c20 2e2e 2e2c 2073 697a 6540 6e5f 6469  , ..., size@n_di
-00012f50: 6d29 0a20 2020 2020 2020 2020 2020 206f  m).            o
-00012f60: 7220 7468 6520 6465 7269 7661 7469 7665  r the derivative
-00012f70: 2066 6f72 2074 6865 2069 6e74 6572 706f   for the interpo
-00012f80: 6c61 7469 6f6e 2e20 2869 6620 6064 6572  lation. (if `der
-00012f90: 6976 6174 6976 6520 3d20 5472 7565 6029  ivative = True`)
-00012fa0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00012fb0: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
-00012fc0: 6e5f 6469 6d7d 2c20 7369 7a65 4031 2c20  n_dim}, size@1, 
-00012fd0: 7369 7a65 4032 2c20 2e2e 2e2c 2073 697a  size@2, ..., siz
-00012fe0: 6540 6e5f 6469 6d29 0a0a 2020 2020 4578  e@n_dim)..    Ex
-00012ff0: 616d 706c 6573 3a0a 2020 2020 2d2d 2d2d  amples:.    ----
-00013000: 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e 2049  ------.    >>> I
-00013010: 6d61 6765 203d 2062 742e 7261 6e64 2833  mage = bt.rand(3
-00013020: 2c20 3130 302c 2031 3230 2c20 3830 290a  , 100, 120, 80).
-00013030: 2020 2020 3e3e 3e20 414d 203d 2062 742e      >>> AM = bt.
-00013040: 7261 6e64 2834 2c20 3429 0a20 2020 203e  rand(4, 4).    >
-00013050: 3e3e 2041 4d5b 332c 203a 5d20 3d20 6274  >> AM[3, :] = bt
-00013060: 2e6f 6e65 5f68 6f74 282d 312c 2034 290a  .one_hot(-1, 4).
-00013070: 2020 2020 3e3e 3e20 696e 7465 7270 6f6c      >>> interpol
-00013080: 6174 696f 6e28 496d 6167 652c 2041 6666  ation(Image, Aff
-00013090: 696e 6528 414d 292c 206d 6574 686f 643d  ine(AM), method=
-000130a0: 274c 696e 6561 7227 290a 2020 2020 2727  'Linear').    ''
-000130b0: 270a 2020 2020 6966 2074 7261 6e73 2069  '.    if trans i
-000130c0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206e  s not None and n
-000130d0: 6f74 2074 7261 6e73 2e62 6163 6b77 6172  ot trans.backwar
-000130e0: 643a 0a20 2020 2020 2020 2069 6620 6861  d:.        if ha
-000130f0: 7361 7474 7228 7472 616e 732c 2027 696e  sattr(trans, 'in
-00013100: 7627 293a 2074 7261 6e73 203d 2074 7261  v'): trans = tra
-00013110: 6e73 2e69 6e76 2829 2e66 616b 655f 696e  ns.inv().fake_in
-00013120: 7628 290a 2020 2020 2020 2020 656c 7365  v().        else
-00013130: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00013140: 696e 7428 2257 6172 6e69 6e67 3a20 466f  int("Warning: Fo
-00013150: 7277 6172 6420 7472 616e 7366 6f72 6d61  rward transforma
-00013160: 7469 6f6e 2066 6f75 6e64 2069 6e20 6d65  tion found in me
-00013170: 7468 6f64 2060 696e 7465 7270 6f6c 6174  thod `interpolat
-00013180: 696f 6e60 2e20 5573 696e 6720 6069 6e74  ion`. Using `int
-00013190: 6572 706f 6c61 7469 6f6e 5f66 6f72 7761  erpolation_forwa
-000131a0: 7264 6020 696e 7374 6561 642e 2022 290a  rd` instead. ").
-000131b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000131c0: 726e 2069 6e74 6572 706f 6c61 7469 6f6e  rn interpolation
-000131d0: 5f66 6f72 7761 7264 2869 6d61 6765 2c20  _forward(image, 
-000131e0: 7472 616e 732c 206d 6574 686f 6420 3d20  trans, method = 
-000131f0: 6d65 7468 6f64 2c20 7461 7267 6574 5f73  method, target_s
-00013200: 7061 6365 203d 2074 6172 6765 745f 7370  pace = target_sp
-00013210: 6163 652c 2066 696c 6c20 3d20 6669 6c6c  ace, fill = fill
-00013220: 290a 2020 2020 696d 6167 6520 3d20 6261  ).    image = ba
-00013230: 746f 7263 685f 7465 6e73 6f72 2869 6d61  torch_tensor(ima
-00013240: 6765 290a 2020 2020 7368 6170 655f 6f75  ge).    shape_ou
-00013250: 7420 3d20 696d 6167 652e 7368 6170 650a  t = image.shape.
-00013260: 2020 2020 6966 2074 7261 6e73 2069 7320      if trans is 
-00013270: 4e6f 6e65 206f 7220 7472 616e 732e 6e5f  None or trans.n_
-00013280: 6469 6d20 6973 204e 6f6e 653a 0a20 2020  dim is None:.   
-00013290: 2020 2020 2069 6620 6e6f 7420 696d 6167       if not imag
-000132a0: 652e 6861 735f 6261 7463 683a 2069 6d61  e.has_batch: ima
-000132b0: 6765 2e75 6e73 7175 6565 7a65 5f28 5b5d  ge.unsqueeze_([]
-000132c0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-000132d0: 2069 6d61 6765 2e68 6173 5f63 6861 6e6e   image.has_chann
-000132e0: 656c 3a20 696d 6167 652e 7374 616e 6461  el: image.standa
-000132f0: 7264 5f28 292e 756e 7371 7565 657a 655f  rd_().unsqueeze_
-00013300: 287b 317d 290a 2020 2020 2020 2020 6e5f  ({1}).        n_
-00013310: 6469 6d20 3d20 696d 6167 652e 6e5f 7370  dim = image.n_sp
-00013320: 6163 6520 2320 4765 7420 7468 6520 7370  ace # Get the sp
-00013330: 6174 6961 6c20 7261 6e6b 2e0a 2020 2020  atial rank..    
-00013340: 656c 7365 3a0a 2020 2020 2020 2020 6e5f  else:.        n_
-00013350: 6469 6d20 3d20 7472 616e 732e 6e5f 6469  dim = trans.n_di
-00013360: 6d0a 2020 2020 2020 2020 6966 2069 6d61  m.        if ima
-00013370: 6765 2e6e 5f64 696d 203d 3d20 6e5f 6469  ge.n_dim == n_di
-00013380: 6d3a 0a20 2020 2020 2020 2020 2020 2069  m:.            i
-00013390: 6620 696d 6167 652e 6861 735f 7370 6563  f image.has_spec
-000133a0: 6961 6c3a 0a20 2020 2020 2020 2020 2020  ial:.           
-000133b0: 2020 2020 2070 7269 6e74 2866 2257 6172       print(f"War
-000133c0: 6e69 6e67 3a20 2769 6e74 6572 706f 6c61  ning: 'interpola
-000133d0: 7469 6f6e 2720 7472 7969 6e67 2074 6f20  tion' trying to 
-000133e0: 7472 616e 7366 6f72 6d20 7b69 6d61 6765  transform {image
-000133f0: 2e6e 5f73 7061 6365 7d2b 7b69 6d61 6765  .n_space}+{image
-00013400: 2e6e 5f73 7065 6369 616c 7d44 2069 6d61  .n_special}D ima
-00013410: 6765 2028 7769 7468 2062 6174 6368 206f  ge (with batch o
-00013420: 7220 6368 616e 6e65 6c29 2062 7920 7b6e  r channel) by {n
-00013430: 5f64 696d 7d44 2074 7261 6e73 666f 726d  _dim}D transform
-00013440: 6174 696f 6e2c 2061 7574 6f2d 7265 6d6f  ation, auto-remo
-00013450: 7669 6e67 2073 7065 6369 616c 2064 696d  ving special dim
-00013460: 656e 7369 6f6e 732e 2229 0a20 2020 2020  ensions.").     
-00013470: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-00013480: 2e72 656d 6f76 655f 7370 6563 6961 6c5f  .remove_special_
-00013490: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-000134a0: 6d61 6765 2e75 6e73 7175 6565 7a65 5f28  mage.unsqueeze_(
-000134b0: 5b5d 292e 756e 7371 7565 657a 655f 287b  []).unsqueeze_({
-000134c0: 7d29 0a20 2020 2020 2020 2065 6c69 6620  }).        elif 
-000134d0: 696d 6167 652e 6e5f 6469 6d20 3d3d 206e  image.n_dim == n
-000134e0: 5f64 696d 202b 2031 3a0a 2020 2020 2020  _dim + 1:.      
-000134f0: 2020 2020 2020 6966 206e 6f74 2069 6d61        if not ima
-00013500: 6765 2e68 6173 5f62 6174 6368 3a0a 2020  ge.has_batch:.  
-00013510: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00013520: 2069 6d61 6765 2e68 6173 5f63 6861 6e6e   image.has_chann
-00013530: 656c 3a20 696d 6167 652e 756e 7371 7565  el: image.unsque
-00013540: 657a 655f 285b 5d29 0a20 2020 2020 2020  eze_([]).       
-00013550: 2020 2020 2020 2020 2065 6c73 653a 2069           else: i
-00013560: 6d61 6765 2e77 6974 685f 6261 7463 6864  mage.with_batchd
-00013570: 696d 2830 292e 756e 7371 7565 657a 655f  im(0).unsqueeze_
-00013580: 287b 317d 290a 2020 2020 2020 2020 2020  ({1}).          
-00013590: 2020 656c 6966 206e 6f74 2069 6d61 6765    elif not image
-000135a0: 2e68 6173 5f63 6861 6e6e 656c 3a20 696d  .has_channel: im
-000135b0: 6167 652e 756e 7371 7565 657a 655f 287b  age.unsqueeze_({
-000135c0: 7d29 0a20 2020 2020 2020 2020 2020 2065  }).            e
-000135d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000135e0: 2020 2020 2070 7269 6e74 2866 2257 6172       print(f"War
-000135f0: 6e69 6e67 3a20 2769 6e74 6572 706f 6c61  ning: 'interpola
-00013600: 7469 6f6e 2720 7472 7969 6e67 2074 6f20  tion' trying to 
-00013610: 7472 616e 7366 6f72 6d20 7b69 6d61 6765  transform {image
-00013620: 2e6e 5f73 7061 6365 7d2b 7b69 6d61 6765  .n_space}+{image
-00013630: 2e6e 5f73 7065 6369 616c 7d44 2069 6d61  .n_special}D ima
-00013640: 6765 2028 7769 7468 2062 6174 6368 206f  ge (with batch o
-00013650: 7220 6368 616e 6e65 6c29 2062 7920 7b6e  r channel) by {n
-00013660: 5f64 696d 7d44 2074 7261 6e73 666f 726d  _dim}D transform
-00013670: 6174 696f 6e2c 2061 7574 6f2d 7265 6d6f  ation, auto-remo
-00013680: 7669 6e67 2074 6865 2063 6861 6e6e 656c  ving the channel
-00013690: 2064 696d 656e 7369 6f6e 732e 2229 0a20   dimensions."). 
-000136a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000136b0: 6d61 6765 2e77 6974 685f 6368 616e 6e65  mage.with_channe
-000136c0: 6c64 696d 284e 6f6e 6529 2e75 6e73 7175  ldim(None).unsqu
-000136d0: 6565 7a65 5f28 7b7d 290a 2020 2020 2020  eeze_({}).      
-000136e0: 2020 656c 6966 2069 6d61 6765 2e6e 5f64    elif image.n_d
-000136f0: 696d 203d 3d20 6e5f 6469 6d20 2b20 323a  im == n_dim + 2:
-00013700: 0a20 2020 2020 2020 2020 2020 2023 205f  .            # _
-00013710: 6368 616e 6e61 6c2f 6261 7463 6820 6469  channal/batch di
-00013720: 6d65 6e73 696f 6e73 2075 7365 6420 6865  mensions used he
-00013730: 7265 2061 7320 7468 6579 2061 7265 206e  re as they are n
-00013740: 5f64 696d 2077 6865 6e20 6e6f 7420 6578  _dim when not ex
-00013750: 6973 7465 642e 200a 2020 2020 2020 2020  isted. .        
-00013760: 2020 2020 6966 2069 6d61 6765 2e6e 5f73      if image.n_s
-00013770: 7065 6369 616c 203d 3d20 313a 0a20 2020  pecial == 1:.   
-00013780: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00013790: 6e74 2866 2257 6172 6e69 6e67 3a20 2769  nt(f"Warning: 'i
-000137a0: 6e74 6572 706f 6c61 7469 6f6e 2720 7472  nterpolation' tr
-000137b0: 7969 6e67 2074 6f20 7472 616e 7366 6f72  ying to transfor
-000137c0: 6d20 7b69 6d61 6765 2e6e 5f73 7061 6365  m {image.n_space
-000137d0: 7d2b 3144 2069 6d61 6765 2028 7769 7468  }+1D image (with
-000137e0: 2062 6174 6368 206f 7220 6368 616e 6e65   batch or channe
-000137f0: 6c29 2062 7920 7b6e 5f64 696d 7d44 2074  l) by {n_dim}D t
-00013800: 7261 6e73 666f 726d 6174 696f 6e2c 2061  ransformation, a
-00013810: 7574 6f2d 696e 7365 7274 696e 6720 6e65  uto-inserting ne
-00013820: 7720 7370 6563 6961 6c20 6469 6d65 6e73  w special dimens
-00013830: 696f 6e2e 2229 0a20 2020 2020 2020 2020  ion.").         
-00013840: 2020 2069 6620 6e6f 7420 696d 6167 652e     if not image.
-00013850: 6861 735f 6261 7463 683a 2069 6d61 6765  has_batch: image
-00013860: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
-00013870: 203d 2030 2069 6620 696d 6167 652e 5f63   = 0 if image._c
-00013880: 6861 6e6e 656c 5f64 696d 656e 7369 6f6e  hannel_dimension
-00013890: 203e 2030 2065 6c73 6520 310a 2020 2020   > 0 else 1.    
-000138a0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-000138b0: 6d61 6765 2e68 6173 5f63 6861 6e6e 656c  mage.has_channel
-000138c0: 3a20 696d 6167 652e 6368 616e 6e65 6c5f  : image.channel_
-000138d0: 6469 6d65 6e73 696f 6e20 3d20 3020 6966  dimension = 0 if
-000138e0: 2069 6d61 6765 2e5f 6261 7463 685f 6469   image._batch_di
-000138f0: 6d65 6e73 696f 6e20 3e20 3020 656c 7365  mension > 0 else
-00013900: 2031 0a20 2020 2061 766f 7563 6828 696d   1.    avouch(im
-00013910: 6167 652e 6861 735f 6261 7463 6820 616e  age.has_batch an
-00013920: 6420 696d 6167 652e 6861 735f 6368 616e  d image.has_chan
-00013930: 6e65 6c2c 2022 506c 6561 7365 2075 7365  nel, "Please use
-00013940: 2062 6174 6f72 6368 2074 656e 736f 7220   batorch tensor 
-00013950: 6f66 2073 697a 6520 2220 2b0a 2020 2020  of size " +.    
-00013960: 2020 2020 2020 2020 2228 5b6e 5f62 6174          "([n_bat
-00013970: 6368 5d2c 207b 6e5f 6368 616e 6e65 6c2f  ch], {n_channel/
-00013980: 6e5f 6665 6174 7572 653a 6f70 7469 6f6e  n_feature:option
-00013990: 616c 7d2c 206d 5f31 2c20 6d5f 322c 202e  al}, m_1, m_2, .
-000139a0: 2e2e 2c20 6d5f 7229 205b 723d 6e5f 6469  .., m_r) [r=n_di
-000139b0: 6d5d 2066 6f72 2022 202b 200a 2020 2020  m] for " + .    
-000139c0: 2020 2020 2020 2020 6622 6461 7461 2074          f"data t
-000139d0: 6f20 6265 2073 7061 7469 616c 6c79 2069  o be spatially i
-000139e0: 6e74 6572 706f 6c61 7465 642c 2069 6e73  nterpolated, ins
-000139f0: 7465 6164 206f 6620 7b69 6d61 6765 2e73  tead of {image.s
-00013a00: 6861 7065 7d2e 2022 290a 2020 2020 6966  hape}. ").    if
-00013a10: 2074 7261 6e73 2069 7320 6e6f 7420 4e6f   trans is not No
-00013a20: 6e65 3a0a 2020 2020 2020 2020 6176 6f75  ne:.        avou
-00013a30: 6368 2869 6d61 6765 2e6e 5f62 6174 6368  ch(image.n_batch
-00013a40: 203d 3d20 3120 6f72 2074 7261 6e73 2e6e   == 1 or trans.n
-00013a50: 5f62 6174 6368 2069 6e20 284e 6f6e 652c  _batch in (None,
-00013a60: 2069 6d61 6765 2e6e 5f62 6174 6368 2c20   image.n_batch, 
-00013a70: 3129 2c20 2250 6c65 6173 6520 7573 6520  1), "Please use 
-00013a80: 7472 616e 7366 6f72 6d61 7469 6f6e 206f  transformation o
-00013a90: 6620 6120 2220 2b0a 2020 2020 2020 2020  f a " +.        
-00013aa0: 2020 2020 6622 7375 6974 6162 6c65 206e      f"suitable n
-00013ab0: 5f62 6174 6368 2074 6f20 7472 616e 7366  _batch to transf
-00013ac0: 6f72 6d20 696d 6167 6520 7769 7468 2062  orm image with b
-00013ad0: 6174 6368 7369 7a65 207b 696d 6167 652e  atchsize {image.
-00013ae0: 6e5f 6261 7463 687d 2c20 6375 7272 656e  n_batch}, curren
-00013af0: 746c 7920 7b74 7261 6e73 2e6e 5f62 6174  tly {trans.n_bat
-00013b00: 6368 7d2e 2229 0a0a 2020 2020 6e5f 6261  ch}.")..    n_ba
-00013b10: 7463 6820 3d20 696d 6167 652e 6e5f 6261  tch = image.n_ba
-00013b20: 7463 680a 2020 2020 6966 206e 5f62 6174  tch.    if n_bat
-00013b30: 6368 203d 3d20 3120 616e 6420 7472 616e  ch == 1 and tran
-00013b40: 7320 6973 206e 6f74 204e 6f6e 6520 616e  s is not None an
-00013b50: 6420 7472 616e 732e 6e5f 6261 7463 6820  d trans.n_batch 
-00013b60: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00013b70: 7472 616e 732e 6e5f 6261 7463 6820 3e20  trans.n_batch > 
-00013b80: 313a 206e 5f62 6174 6368 203d 2074 7261  1: n_batch = tra
-00013b90: 6e73 2e6e 5f62 6174 6368 0a20 2020 2069  ns.n_batch.    i
-00013ba0: 6620 6e5f 6261 7463 6820 3d3d 2031 2061  f n_batch == 1 a
-00013bb0: 6e64 2069 7369 6e73 7461 6e63 6528 7461  nd isinstance(ta
-00013bc0: 7267 6574 5f73 7061 6365 2c20 6274 2e54  rget_space, bt.T
-00013bd0: 656e 736f 7229 2061 6e64 2074 6172 6765  ensor) and targe
-00013be0: 745f 7370 6163 652e 6861 735f 6261 7463  t_space.has_batc
-00013bf0: 6820 616e 6420 7461 7267 6574 5f73 7061  h and target_spa
-00013c00: 6365 2e6e 5f62 6174 6368 203e 2031 3a20  ce.n_batch > 1: 
-00013c10: 6e5f 6261 7463 6820 3d20 7461 7267 6574  n_batch = target
-00013c20: 5f73 7061 6365 2e6e 5f62 6174 6368 0a20  _space.n_batch. 
-00013c30: 2020 2069 6620 696d 6167 652e 6e5f 6261     if image.n_ba
-00013c40: 7463 6820 3d3d 2031 3a20 696d 6167 6520  tch == 1: image 
-00013c50: 3d20 696d 6167 652e 7265 7065 6174 6564  = image.repeated
-00013c60: 286e 5f62 6174 6368 2c20 5b5d 290a 2020  (n_batch, []).  
-00013c70: 2020 6e5f 6665 6174 7572 6520 3d20 696d    n_feature = im
-00013c80: 6167 652e 6e5f 6368 616e 6e65 6c0a 2020  age.n_channel.  
-00013c90: 2020 7369 7a65 203d 2062 742e 6368 616e    size = bt.chan
-00013ca0: 6e65 6c5f 7465 6e73 6f72 2869 6d61 6765  nel_tensor(image
-00013cb0: 2e73 7061 6365 292e 696e 7428 290a 2020  .space).int().  
-00013cc0: 2020 6966 206e 5f62 6174 6368 203e 2031    if n_batch > 1
-00013cd0: 2061 6e64 206e 6f74 2073 6861 7065 5f6f   and not shape_o
-00013ce0: 7574 2e68 6173 5f62 6174 6368 3a20 7368  ut.has_batch: sh
-00013cf0: 6170 655f 6f75 7420 3d20 6274 2e53 697a  ape_out = bt.Siz
-00013d00: 6528 5b6e 5f62 6174 6368 5d29 202b 2073  e([n_batch]) + s
-00013d10: 6861 7065 5f6f 7574 0a20 2020 2069 6620  hape_out.    if 
-00013d20: 7461 7267 6574 5f73 7061 6365 2069 7320  target_space is 
-00013d30: 4e6f 6e65 3a0a 2020 2020 2020 2020 7363  None:.        sc
-00013d40: 616c 652c 202a 7061 6972 7320 3d20 7472  ale, *pairs = tr
-00013d50: 616e 732e 7265 7368 6170 650a 2020 2020  ans.reshape.    
-00013d60: 2020 2020 6966 206c 656e 2873 6361 6c65      if len(scale
-00013d70: 2920 3d3d 2031 3a20 7363 616c 6520 2a3d  ) == 1: scale *=
-00013d80: 206e 5f64 696d 0a20 2020 2020 2020 2074   n_dim.        t
-00013d90: 6172 6765 745f 7370 6163 6520 3d20 5b69  arget_space = [i
-00013da0: 6e74 2878 202a 2079 2920 666f 7220 782c  nt(x * y) for x,
-00013db0: 2079 2069 6e20 7a69 7028 696d 6167 652e   y in zip(image.
-00013dc0: 7370 6163 652c 2073 6361 6c65 295d 0a20  space, scale)]. 
-00013dd0: 2020 2020 2020 2066 6f72 2070 2c20 7120         for p, q 
-00013de0: 696e 2070 6169 7273 3a20 7461 7267 6574  in pairs: target
-00013df0: 5f73 7061 6365 5b70 5d2c 2074 6172 6765  _space[p], targe
-00013e00: 745f 7370 6163 655b 715d 203d 2074 6172  t_space[q] = tar
-00013e10: 6765 745f 7370 6163 655b 715d 2c20 7461  get_space[q], ta
-00013e20: 7267 6574 5f73 7061 6365 5b70 5d0a 2020  rget_space[p].  
-00013e30: 2020 2020 2020 7461 7267 6574 5f73 7061        target_spa
-00013e40: 6365 203d 2074 7570 6c65 2874 6172 6765  ce = tuple(targe
-00013e50: 745f 7370 6163 6529 0a20 2020 2020 2020  t_space).       
-00013e60: 2073 6861 7065 5f6f 7574 203d 2073 6861   shape_out = sha
-00013e70: 7065 5f6f 7574 2e72 6573 6574 5f73 7061  pe_out.reset_spa
-00013e80: 6365 2874 6172 6765 745f 7370 6163 6529  ce(target_space)
-00013e90: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
-00013ea0: 6365 2874 6172 6765 745f 7370 6163 652c  ce(target_space,
-00013eb0: 2074 7570 6c65 2920 616e 6420 6c65 6e28   tuple) and len(
-00013ec0: 7461 7267 6574 5f73 7061 6365 2920 3d3d  target_space) ==
-00013ed0: 206e 5f64 696d 3a20 7061 7373 0a20 2020   n_dim: pass.   
-00013ee0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00013ef0: 2874 6172 6765 745f 7370 6163 652c 2062  (target_space, b
-00013f00: 742e 746f 7263 682e 5465 6e73 6f72 293a  t.torch.Tensor):
-00013f10: 2070 6173 730a 2020 2020 656c 7365 3a20   pass.    else: 
-00013f20: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-00013f30: 6622 5772 6f6e 6720 7461 7267 6574 2073  f"Wrong target s
-00013f40: 7061 6365 2066 6f72 2069 6e74 6572 706f  pace for interpo
-00013f50: 6c61 7469 6f6e 3a20 7b74 6172 6765 745f  lation: {target_
-00013f60: 7370 6163 657d 2e20 2229 0a20 2020 2069  space}. ").    i
-00013f70: 6620 6973 696e 7374 616e 6365 2874 6172  f isinstance(tar
-00013f80: 6765 745f 7370 6163 652c 2074 7570 6c65  get_space, tuple
-00013f90: 293a 200a 2020 2020 2020 2020 2320 4372  ): .        # Cr
-00013fa0: 6561 7465 2061 2067 7269 6420 5820 7769  eate a grid X wi
-00013fb0: 7468 2073 697a 6520 287b 6e5f 6469 6d7d  th size ({n_dim}
-00013fc0: 2c20 7369 7a65 5f31 2c20 7369 7a65 5f32  , size_1, size_2
-00013fd0: 2c20 2e2e 2e2c 2073 697a 655f 7229 205b  , ..., size_r) [
-00013fe0: 723d 6e5f 6469 6d5d 2e0a 2020 2020 2020  r=n_dim]..      
-00013ff0: 2020 5820 3d20 6274 2e69 6d61 6765 5f67    X = bt.image_g
-00014000: 7269 6428 7461 7267 6574 5f73 7061 6365  rid(target_space
-00014010: 292e 666c 6f61 7428 2920 2320 2b20 6274  ).float() # + bt
-00014020: 2e63 6861 6e6e 656c 5f74 656e 736f 7228  .channel_tensor(
-00014030: 5b66 6c6f 6174 2861 2d62 292f 3220 666f  [float(a-b)/2 fo
-00014040: 7220 612c 2062 2069 6e20 7a69 7028 696d  r a, b in zip(im
-00014050: 6167 652e 7370 6163 652c 2074 6172 6765  age.space, targe
-00014060: 745f 7370 6163 6529 5d29 0a20 2020 2020  t_space)]).     
-00014070: 2020 2023 2043 6f6d 7075 7465 2074 6865     # Compute the
-00014080: 2074 7261 6e73 666f 726d 6564 2063 6f6f   transformed coo
-00014090: 7264 696e 6174 6573 2e20 593a 2028 5b6e  rdinates. Y: ([n
-000140a0: 5f62 6174 6368 5d2c 207b 6e5f 6469 6d7d  _batch], {n_dim}
-000140b0: 2c20 7369 7a65 5f31 2c20 7369 7a65 5f32  , size_1, size_2
-000140c0: 2c20 2e2e 2e2c 2073 697a 655f 7229 205b  , ..., size_r) [
-000140d0: 723d 6e5f 6469 6d5d 2e0a 2020 2020 2020  r=n_dim]..      
-000140e0: 2020 6966 2074 7261 6e73 2069 7320 4e6f    if trans is No
-000140f0: 6e65 3a20 7472 616e 7320 3d20 4964 656e  ne: trans = Iden
-00014100: 7469 7479 2829 0a20 2020 2020 2020 2059  tity().        Y
-00014110: 203d 2074 7261 6e73 2858 290a 2020 2020   = trans(X).    
-00014120: 2020 2020 6966 206e 6f74 2059 2e68 6173      if not Y.has
-00014130: 5f62 6174 6368 3a20 5920 3d20 592e 6d75  _batch: Y = Y.mu
-00014140: 6c74 6970 6c79 286e 5f62 6174 6368 2c20  ltiply(n_batch, 
-00014150: 5b5d 290a 2020 2020 2020 2020 6966 2059  []).        if Y
-00014160: 2e6e 5f62 6174 6368 203d 3d20 313a 2059  .n_batch == 1: Y
-00014170: 203d 2059 2e72 6570 6561 7465 6428 6e5f   = Y.repeated(n_
-00014180: 6261 7463 682c 205b 5d29 0a20 2020 2020  batch, []).     
-00014190: 2020 2059 203d 2059 2e61 6d70 6c69 6679     Y = Y.amplify
-000141a0: 286e 5f66 6561 7475 7265 2c20 5b5d 290a  (n_feature, []).
-000141b0: 2020 2020 2020 2020 7368 6170 655f 6f75          shape_ou
-000141c0: 7420 3d20 7368 6170 655f 6f75 742e 7265  t = shape_out.re
-000141d0: 7365 745f 7370 6163 6528 7461 7267 6574  set_space(target
-000141e0: 5f73 7061 6365 290a 2020 2020 656c 7365  _space).    else
-000141f0: 3a0a 2020 2020 2020 2020 7461 7267 6574  :.        target
-00014200: 5f73 7061 6365 203d 2062 6174 6f72 6368  _space = batorch
-00014210: 5f74 656e 736f 7228 7461 7267 6574 5f73  _tensor(target_s
-00014220: 7061 6365 290a 2020 2020 2020 2020 6966  pace).        if
-00014230: 206e 6f74 2074 6172 6765 745f 7370 6163   not target_spac
-00014240: 652e 6861 735f 6261 7463 683a 0a20 2020  e.has_batch:.   
-00014250: 2020 2020 2020 2020 2069 6620 7461 7267           if targ
-00014260: 6574 5f73 7061 6365 2e73 697a 6528 3029  et_space.size(0)
-00014270: 203d 3d20 6e5f 6261 7463 6820 616e 6420   == n_batch and 
-00014280: 6e5f 6261 7463 6820 213d 206e 5f64 696d  n_batch != n_dim
-00014290: 206f 7220 6c65 6e28 5b78 2066 6f72 2078   or len([x for x
-000142a0: 2069 6e20 7461 7267 6574 5f73 7061 6365   in target_space
-000142b0: 2e73 6861 7065 2069 6620 7820 3d3d 206e  .shape if x == n
-000142c0: 5f64 696d 5d29 203e 3d20 323a 0a20 2020  _dim]) >= 2:.   
-000142d0: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-000142e0: 6765 745f 7370 6163 652e 7769 7468 5f62  get_space.with_b
-000142f0: 6174 6368 6469 6d28 3029 0a20 2020 2020  atchdim(0).     
-00014300: 2020 2020 2020 2065 6c73 653a 2074 6172         else: tar
-00014310: 6765 745f 7370 6163 652e 756e 7371 7565  get_space.unsque
-00014320: 657a 655f 285b 5d29 0a20 2020 2020 2020  eze_([]).       
-00014330: 2069 6620 6e6f 7420 7461 7267 6574 5f73   if not target_s
-00014340: 7061 6365 2e68 6173 5f63 6861 6e6e 656c  pace.has_channel
-00014350: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00014360: 2074 6172 6765 745f 7370 6163 652e 6261   target_space.ba
-00014370: 7463 685f 6469 6d65 6e73 696f 6e20 213d  tch_dimension !=
-00014380: 2030 2061 6e64 2074 6172 6765 745f 7370   0 and target_sp
-00014390: 6163 652e 7369 7a65 2830 2920 3d3d 206e  ace.size(0) == n
-000143a0: 5f64 696d 3a20 7461 7267 6574 5f73 7061  _dim: target_spa
-000143b0: 6365 2e77 6974 685f 6368 616e 6e65 6c64  ce.with_channeld
-000143c0: 696d 2830 290a 2020 2020 2020 2020 2020  im(0).          
-000143d0: 2020 656c 6966 2074 6172 6765 745f 7370    elif target_sp
-000143e0: 6163 652e 6261 7463 685f 6469 6d65 6e73  ace.batch_dimens
-000143f0: 696f 6e20 213d 2031 2061 6e64 2074 6172  ion != 1 and tar
-00014400: 6765 745f 7370 6163 652e 7369 7a65 2831  get_space.size(1
-00014410: 2920 3d3d 206e 5f64 696d 3a20 7461 7267  ) == n_dim: targ
-00014420: 6574 5f73 7061 6365 2e77 6974 685f 6368  et_space.with_ch
-00014430: 616e 6e65 6c64 696d 2831 290a 2020 2020  anneldim(1).    
-00014440: 2020 2020 2020 2020 656c 6966 2074 6172          elif tar
-00014450: 6765 745f 7370 6163 652e 6261 7463 685f  get_space.batch_
-00014460: 6469 6d65 6e73 696f 6e20 213d 2074 6172  dimension != tar
-00014470: 6765 745f 7370 6163 652e 6e5f 6469 6d20  get_space.n_dim 
-00014480: 2d20 3120 616e 6420 7461 7267 6574 5f73  - 1 and target_s
-00014490: 7061 6365 2e73 697a 6528 2d31 2920 3d3d  pace.size(-1) ==
-000144a0: 206e 5f64 696d 3a20 7461 7267 6574 5f73   n_dim: target_s
-000144b0: 7061 6365 2e77 6974 685f 6368 616e 6e65  pace.with_channe
-000144c0: 6c64 696d 282d 3129 0a20 2020 2020 2020  ldim(-1).       
-000144d0: 2061 766f 7563 6828 7461 7267 6574 5f73   avouch(target_s
-000144e0: 7061 6365 2e68 6173 5f63 6861 6e6e 656c  pace.has_channel
-000144f0: 2061 6e64 2074 6172 6765 745f 7370 6163   and target_spac
-00014500: 652e 6e5f 6368 616e 6e65 6c20 3d3d 206e  e.n_channel == n
-00014510: 5f64 696d 2c20 2227 7461 7267 6574 5f73  _dim, "'target_s
-00014520: 7061 6365 2720 666f 7220 696e 7465 7270  pace' for interp
-00014530: 6f6c 6174 696f 6e20 7368 6f75 6c64 2068  olation should h
-00014540: 6176 6520 6120 6368 616e 6e65 6c20 6469  ave a channel di
-00014550: 6d65 6e73 696f 6e20 666f 7220 636f 6f72  mension for coor
-00014560: 6469 6e61 7465 732e 2022 290a 2020 2020  dinates. ").    
-00014570: 2020 2020 5920 3d20 7461 7267 6574 5f73      Y = target_s
-00014580: 7061 6365 2e72 6570 6561 7465 6428 6e5f  pace.repeated(n_
-00014590: 6261 7463 6820 2f2f 2074 6172 6765 745f  batch // target_
-000145a0: 7370 6163 652e 6e5f 6261 7463 682c 205b  space.n_batch, [
-000145b0: 5d29 2e61 6d70 6c69 6679 286e 5f66 6561  ]).amplify(n_fea
-000145c0: 7475 7265 2c20 5b5d 290a 2020 2020 2020  ture, []).      
-000145d0: 2020 7368 6170 655f 6f75 7420 3d20 7368    shape_out = sh
-000145e0: 6170 655f 6f75 742e 7265 7365 745f 7370  ape_out.reset_sp
-000145f0: 6163 6528 7461 7267 6574 5f73 7061 6365  ace(target_space
-00014600: 2e73 7061 6365 290a 2020 2020 2020 2020  .space).        
-00014610: 0a20 2020 2069 6d61 6765 203d 2069 6d61  .    image = ima
-00014620: 6765 2e6d 6572 6765 6469 6d73 287b 7d2c  ge.mergedims({},
-00014630: 205b 5d29 0a20 2020 206e 5f62 6174 6368   []).    n_batch
-00014640: 203d 2069 6d61 6765 2e6e 5f62 6174 6368   = image.n_batch
-00014650: 0a0a 2020 2020 6966 206d 6574 686f 642e  ..    if method.
-00014660: 6c6f 7765 7228 2920 3d3d 2027 6273 706c  lower() == 'bspl
-00014670: 696e 6527 3a0a 2020 2020 2020 2020 6966  ine':.        if
-00014680: 2064 6572 6976 6174 6976 653a 2072 6169   derivative: rai
-00014690: 7365 2054 7970 6545 7272 6f72 2822 4e6f  se TypeError("No
-000146a0: 2064 6572 6976 6174 6976 6573 2066 6f72   derivatives for
-000146b0: 2062 7370 6c69 6e65 2069 6e74 6572 706f   bspline interpo
-000146c0: 6c61 7469 6f6e 7320 6172 6520 6176 6169  lations are avai
-000146d0: 6c61 626c 6520 736f 2066 6172 2e20 506c  lable so far. Pl
-000146e0: 6561 7365 2077 7269 7465 2069 7420 6279  ease write it by
-000146f0: 2079 6f75 7273 656c 662e 2022 290a 2020   yourself. ").  
-00014700: 2020 2020 2020 2320 544f 444f 3a20 4646        # TODO: FF
-00014710: 440a 2020 2020 2020 2020 7261 6973 6520  D.        raise 
-00014720: 5479 7065 4572 726f 7228 2242 7370 6c69  TypeError("Bspli
-00014730: 6e65 2069 6e74 6572 706f 6c61 7469 6f6e  ne interpolation
-00014740: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
-00014750: 6520 736f 2066 6172 2e20 506c 6561 7365  e so far. Please
-00014760: 2077 7269 7465 2069 7420 6279 2079 6f75   write it by you
-00014770: 7273 656c 662e 2022 290a 0a20 2020 2069  rself. ")..    i
-00014780: 5920 3d20 6274 2e66 6c6f 6f72 2859 292e  Y = bt.floor(Y).
-00014790: 6c6f 6e67 2829 2023 2047 656e 6572 6174  long() # Generat
-000147a0: 6520 7468 6520 696e 7465 6765 7220 7061  e the integer pa
-000147b0: 7274 206f 6620 590a 2020 2020 6a59 203d  rt of Y.    jY =
-000147c0: 2069 5920 2b20 3120 2320 616e 6420 7468   iY + 1 # and th
-000147d0: 6520 696e 7465 6765 7220 7061 7274 2070  e integer part p
-000147e0: 6c75 7320 6f6e 652e 0a20 2020 2069 6620  lus one..    if 
-000147f0: 6d65 7468 6f64 2e6c 6f77 6572 2829 203d  method.lower() =
-00014800: 3d20 276c 696e 6561 7227 3a20 6659 203d  = 'linear': fY =
-00014810: 2059 202d 2069 592e 666c 6f61 7428 2920   Y - iY.float() 
-00014820: 2320 5468 6520 6465 6369 6d61 6c20 7061  # The decimal pa
-00014830: 7274 206f 6620 592e 0a20 2020 2065 6c69  rt of Y..    eli
-00014840: 6620 6d65 7468 6f64 2e6c 6f77 6572 2829  f method.lower()
-00014850: 203d 3d20 276e 6561 7265 7374 273a 2066   == 'nearest': f
-00014860: 5920 3d20 6274 2e66 6c6f 6f72 2859 202d  Y = bt.floor(Y -
-00014870: 2069 592e 666c 6f61 7428 2920 2b20 302e   iY.float() + 0.
-00014880: 3529 2023 2054 6865 2064 6563 696d 616c  5) # The decimal
-00014890: 2070 6172 7420 6f66 2059 2e0a 2020 2020   part of Y..    
-000148a0: 656c 7365 3a20 7261 6973 6520 5479 7065  else: raise Type
-000148b0: 4572 726f 7228 2255 6e72 6563 6f67 6e69  Error("Unrecogni
-000148c0: 7a65 6420 6172 6775 6d65 6e74 2027 6d65  zed argument 'me
-000148d0: 7468 6f64 272e 2022 290a 2020 2020 6259  thod'. ").    bY
-000148e0: 203d 2062 742e 7374 6163 6b28 2869 592c   = bt.stack((iY,
-000148f0: 206a 5929 2c20 3129 2e76 6965 7728 5b6e   jY), 1).view([n
-00014900: 5f62 6174 6368 5d2c 2032 2c20 7b6e 5f64  _batch], 2, {n_d
-00014910: 696d 7d2c 202d 3129 2023 2028 5b6e 5f62  im}, -1) # ([n_b
-00014920: 6174 6368 5d2c 2032 2c20 7b6e 5f64 696d  atch], 2, {n_dim
-00014930: 7d2c 206e 5f64 6174 6129 2e0a 2020 2020  }, n_data)..    
-00014940: 5720 3d20 6274 2e73 7461 636b 2828 3120  W = bt.stack((1 
-00014950: 2d20 6659 2c20 6659 292c 2031 292e 7669  - fY, fY), 1).vi
-00014960: 6577 285b 6e5f 6261 7463 685d 2c20 322c  ew([n_batch], 2,
-00014970: 207b 6e5f 6469 6d7d 2c20 2d31 2920 2320   {n_dim}, -1) # 
-00014980: 285b 6e5f 6261 7463 685d 2c20 322c 207b  ([n_batch], 2, {
-00014990: 6e5f 6469 6d7d 2c20 6e5f 6461 7461 292e  n_dim}, n_data).
-000149a0: 0a20 2020 206e 5f64 6174 6120 3d20 6259  .    n_data = bY
-000149b0: 2e73 697a 6528 2d31 290a 0a20 2020 2023  .size(-1)..    #
-000149c0: 2050 7265 7061 7265 2066 6f72 2074 6865   Prepare for the
-000149d0: 206f 7574 7075 7420 7370 6163 653a 206e   output space: n
-000149e0: 5f62 6174 6368 2c20 6d5f 312c 202e 2e2e  _batch, m_1, ...
-000149f0: 2c20 6d5f 730a 2020 2020 6966 2064 6572  , m_s.    if der
-00014a00: 6976 6174 6976 653a 206f 7574 7075 7420  ivative: output 
-00014a10: 3d20 6274 2e7a 6572 6f73 285b 6e5f 6261  = bt.zeros([n_ba
-00014a20: 7463 685d 2c20 7b6e 5f64 696d 7d2c 202a  tch], {n_dim}, *
-00014a30: 7368 6170 655f 6f75 742e 7370 6163 6529  shape_out.space)
-00014a40: 0a20 2020 2065 6c73 653a 206f 7574 7075  .    else: outpu
-00014a50: 7420 3d20 6274 2e7a 6572 6f73 2873 6861  t = bt.zeros(sha
-00014a60: 7065 5f6f 7574 290a 2020 2020 666f 7220  pe_out).    for 
-00014a70: 4720 696e 2062 742e 696d 6167 655f 6772  G in bt.image_gr
-00014a80: 6964 285b 325d 2a6e 5f64 696d 292e 666c  id([2]*n_dim).fl
-00014a90: 6174 7465 6e28 292e 7472 616e 7370 6f73  atten().transpos
-00014aa0: 6528 302c 2031 293a 0a20 2020 2020 2020  e(0, 1):.       
-00014ab0: 2023 2047 6574 2074 6865 2069 6e64 6963   # Get the indic
-00014ac0: 6573 2066 6f72 2074 6865 2074 6572 6d3a  es for the term:
-00014ad0: 2062 595b 3a2c 2047 5b44 5d2c 2044 2c20   bY[:, G[D], D, 
-00014ae0: 3a5d 2c20 7369 7a65 3d28 5b6e 5f62 6174  :], size=([n_bat
-00014af0: 6368 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f  ch], {n_dim}, n_
-00014b00: 6461 7461 290a 2020 2020 2020 2020 496e  data).        In
-00014b10: 6420 3d20 6259 2e67 6174 6865 7228 312c  d = bY.gather(1,
-00014b20: 2047 2e65 7870 616e 645f 746f 285b 6e5f   G.expand_to([n_
-00014b30: 6261 7463 685d 2c20 312c 207b 6e5f 6469  batch], 1, {n_di
-00014b40: 6d7d 2c20 6e5f 6461 7461 2929 2e73 7175  m}, n_data)).squ
-00014b50: 6565 7a65 2831 290a 2020 2020 2020 2020  eeze(1).        
-00014b60: 2320 436c 616d 7020 7468 6520 696e 6469  # Clamp the indi
-00014b70: 6365 7320 696e 2074 6865 2063 6f72 7265  ces in the corre
-00014b80: 6374 2072 616e 6765 2026 2043 6f6d 7075  ct range & Compu
-00014b90: 7465 2074 6865 2062 6f72 6465 7220 636f  te the border co
-00014ba0: 6e64 6974 696f 6e0a 2020 2020 2020 2020  ndition.        
-00014bb0: 636f 6e64 6974 696f 6e20 3d20 6274 2e73  condition = bt.s
-00014bc0: 756d 2828 496e 6420 3c20 3029 202b 2028  um((Ind < 0) + (
-00014bd0: 496e 6420 3e20 7369 7a65 202d 2031 292c  Ind > size - 1),
-00014be0: 2031 290a 2020 2020 2020 2020 496e 6420   1).        Ind 
-00014bf0: 3d20 6274 2e6d 696e 2862 742e 636c 616d  = bt.min(bt.clam
-00014c00: 7028 496e 642c 206d 696e 3d30 292c 2028  p(Ind, min=0), (
-00014c10: 7369 7a65 202d 2031 292e 6578 7061 6e64  size - 1).expand
-00014c20: 5f74 6f28 496e 6429 290a 2020 2020 2020  _to(Ind)).      
-00014c30: 2020 2320 436f 6e76 6572 7420 7468 6520    # Convert the 
-00014c40: 696e 6469 6365 7320 746f 2031 2064 696d  indices to 1 dim
-00014c50: 656e 7369 6f6e 616c 2e20 446f 743a 2028  ensional. Dot: (
-00014c60: 5b6e 5f62 6174 6368 5d2c 206e 5f64 6174  [n_batch], n_dat
-00014c70: 6129 0a20 2020 2020 2020 2044 6f74 203d  a).        Dot =
-00014c80: 2049 6e64 5b3a 2c20 305d 0a20 2020 2020   Ind[:, 0].     
-00014c90: 2020 2066 6f72 2072 2069 6e20 7261 6e67     for r in rang
-00014ca0: 6528 312c 206e 5f64 696d 293a 2044 6f74  e(1, n_dim): Dot
-00014cb0: 202a 3d20 7369 7a65 5b72 5d3b 2044 6f74   *= size[r]; Dot
-00014cc0: 202b 3d20 496e 645b 3a2c 2072 5d0a 2020   += Ind[:, r].  
-00014cd0: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
-00014ce0: 696d 6167 6520 7661 6c75 6573 2049 563a  image values IV:
-00014cf0: 2028 5b6e 5f62 6174 6368 5d2c 206e 5f64   ([n_batch], n_d
-00014d00: 6174 6129 0a20 2020 2020 2020 2049 5620  ata).        IV 
-00014d10: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
-00014d20: 6620 6973 696e 7374 616e 6365 2866 696c  f isinstance(fil
-00014d30: 6c2c 2073 7472 293a 0a20 2020 2020 2020  l, str):.       
-00014d40: 2020 2020 2069 6620 6669 6c6c 2e6c 6f77       if fill.low
-00014d50: 6572 2829 203d 3d20 276e 6561 7265 7374  er() == 'nearest
-00014d60: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00014d70: 2020 2049 5620 3d20 696d 6167 652e 666c     IV = image.fl
-00014d80: 6174 7465 6e28 292e 6761 7468 6572 2831  atten().gather(1
-00014d90: 2c20 446f 7429 0a20 2020 2020 2020 2020  , Dot).         
-00014da0: 2020 2065 6c69 6620 6669 6c6c 2e6c 6f77     elif fill.low
-00014db0: 6572 2829 203d 3d20 2762 6163 6b67 726f  er() == 'backgro
-00014dc0: 756e 6427 3a0a 2020 2020 2020 2020 2020  und':.          
-00014dd0: 2020 2020 2020 626b 5f76 616c 7565 203d        bk_value =
-00014de0: 2062 742e 7374 6163 6b28 5b69 6d61 6765   bt.stack([image
-00014df0: 5b28 736c 6963 6528 4e6f 6e65 292c 2920  [(slice(None),) 
-00014e00: 2b20 7475 706c 6528 6729 5d20 666f 7220  + tuple(g)] for 
-00014e10: 6720 696e 2028 6274 2e69 6d61 6765 5f67  g in (bt.image_g
-00014e20: 7269 6428 5b32 5d2a 6e5f 6469 6d29 202a  rid([2]*n_dim) *
-00014e30: 2062 742e 6368 616e 6e65 6c5f 7465 6e73   bt.channel_tens
-00014e40: 6f72 2873 697a 652d 3129 292e 666c 6174  or(size-1)).flat
-00014e50: 7465 6e28 292e 7472 616e 7370 6f73 6528  ten().transpose(
-00014e60: 302c 3129 5d2c 2031 292e 6d65 6469 616e  0,1)], 1).median
-00014e70: 2831 292e 7661 6c75 6573 0a20 2020 2020  (1).values.     
-00014e80: 2020 2020 2020 2020 2020 2062 6163 6b67             backg
-00014e90: 726f 756e 6420 3d20 626b 5f76 616c 7565  round = bk_value
-00014ea0: 202a 2062 742e 6f6e 6573 5f6c 696b 6528   * bt.ones_like(
-00014eb0: 446f 7429 0a20 2020 2020 2020 2020 2020  Dot).           
-00014ec0: 2065 6c69 6620 6669 6c6c 2e6c 6f77 6572   elif fill.lower
-00014ed0: 2829 203d 3d20 277a 6572 6f27 3a0a 2020  () == 'zero':.  
-00014ee0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00014ef0: 636b 6772 6f75 6e64 203d 2062 742e 7a65  ckground = bt.ze
-00014f00: 726f 735f 6c69 6b65 2844 6f74 290a 2020  ros_like(Dot).  
-00014f10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00014f20: 2020 2020 2020 2020 6261 636b 6772 6f75          backgrou
-00014f30: 6e64 203d 2066 696c 6c20 2a20 6274 2e6f  nd = fill * bt.o
-00014f40: 6e65 735f 6c69 6b65 2844 6f74 290a 2020  nes_like(Dot).  
-00014f50: 2020 2020 2020 6966 2049 5620 6973 204e        if IV is N
-00014f60: 6f6e 653a 2049 5620 3d20 6274 2e77 6865  one: IV = bt.whe
-00014f70: 7265 2863 6f6e 6469 7469 6f6e 203e 3d20  re(condition >= 
-00014f80: 312c 2062 6163 6b67 726f 756e 642e 666c  1, background.fl
-00014f90: 6f61 7428 292c 2069 6d61 6765 2e66 6c61  oat(), image.fla
-00014fa0: 7474 656e 2829 2e67 6174 6865 7228 312c  tten().gather(1,
-00014fb0: 2044 6f74 292e 666c 6f61 7428 2929 0a20   Dot).float()). 
-00014fc0: 2020 2020 2020 2023 2057 6569 6768 7473         # Weights
-00014fd0: 2066 6f72 2065 6163 6820 706f 696e 743a   for each point:
-00014fe0: 205b 7072 6f64 7563 7420 6f66 2057 5b3a   [product of W[:
-00014ff0: 2c20 475b 445d 2c20 442c 2078 5d20 666f  , G[D], D, x] fo
-00015000: 7220 4420 696e 2072 616e 6765 286e 5f64  r D in range(n_d
-00015010: 696d 295d 2066 6f72 2070 6f69 6e74 2078  im)] for point x
-00015020: 2e0a 2020 2020 2020 2020 2320 5767 3a20  ..        # Wg: 
-00015030: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f64  ([n_batch], {n_d
-00015040: 696d 7d2c 206e 5f64 6174 6129 0a20 2020  im}, n_data).   
-00015050: 2020 2020 2057 6720 3d20 572e 6761 7468       Wg = W.gath
-00015060: 6572 2831 2c20 472e 6578 7061 6e64 5f74  er(1, G.expand_t
-00015070: 6f28 5b6e 5f62 6174 6368 5d2c 2031 2c20  o([n_batch], 1, 
-00015080: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6129  {n_dim}, n_data)
-00015090: 292e 7371 7565 657a 6528 3129 0a20 2020  ).squeeze(1).   
-000150a0: 2020 2020 2069 6620 6e6f 7420 6465 7269       if not deri
-000150b0: 7661 7469 7665 3a0a 2020 2020 2020 2020  vative:.        
-000150c0: 2020 2020 6f75 7470 7574 202b 3d20 2857      output += (W
-000150d0: 672e 7072 6f64 2831 2920 2a20 4956 292e  g.prod(1) * IV).
-000150e0: 7669 6577 5f61 7328 6f75 7470 7574 290a  view_as(output).
-000150f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00015100: 2020 2020 2020 2020 2020 7465 6d70 5767            tempWg
-00015110: 4d61 7420 3d20 5767 2e6d 756c 7469 706c  Mat = Wg.multipl
-00015120: 7928 6e5f 6469 6d2c 2031 2920 2320 285b  y(n_dim, 1) # ([
-00015130: 6e5f 6261 7463 685d 2c20 6e5f 6469 6d2c  n_batch], n_dim,
-00015140: 207b 6e5f 6469 6d7d 2c20 6e5f 6461 7461   {n_dim}, n_data
-00015150: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
-00015160: 6d70 5767 4d61 745b 3a2c 2062 742e 6172  mpWgMat[:, bt.ar
-00015170: 616e 6765 286e 5f64 696d 292c 2062 742e  ange(n_dim), bt.
-00015180: 6172 616e 6765 286e 5f64 696d 295d 203d  arange(n_dim)] =
-00015190: 2031 0a20 2020 2020 2020 2020 2020 2064   1.            d
-000151a0: 5767 203d 2074 656d 7057 674d 6174 2e70  Wg = tempWgMat.p
-000151b0: 726f 6428 3129 202a 2028 4720 2a20 3220  rod(1) * (G * 2 
-000151c0: 2d20 3129 2e66 6c6f 6174 2829 0a20 2020  - 1).float().   
-000151d0: 2020 2020 2020 2020 206f 7574 7075 7420           output 
-000151e0: 2b3d 2028 6457 6720 2a20 4956 2e75 6e73  += (dWg * IV.uns
-000151f0: 7175 6565 7a65 2831 2929 2e76 6965 775f  queeze(1)).view_
-00015200: 6173 286f 7574 7075 7429 0a20 2020 2062  as(output).    b
-00015210: 742e 746f 7263 682e 6375 6461 2e65 6d70  t.torch.cuda.emp
-00015220: 7479 5f63 6163 6865 2829 0a20 2020 2065  ty_cache().    e
-00015230: 7073 203d 2031 652d 360a 2020 2020 6d20  ps = 1e-6.    m 
-00015240: 3d20 3020 6966 2069 6d61 6765 2e6d 696e  = 0 if image.min
-00015250: 2829 203e 202d 6570 7320 656c 7365 2069  () > -eps else i
-00015260: 6d61 6765 2e6d 696e 2829 2e69 7465 6d28  mage.min().item(
-00015270: 290a 2020 2020 4d20 3d20 3120 6966 2069  ).    M = 1 if i
-00015280: 6d61 6765 2e6d 6178 2829 203c 2031 202b  mage.max() < 1 +
-00015290: 2065 7073 2065 6c73 6520 696d 6167 652e   eps else image.
-000152a0: 6d61 7828 292e 6974 656d 2829 0a20 2020  max().item().   
-000152b0: 2072 6574 7572 6e20 6f75 7470 7574 2e63   return output.c
-000152c0: 6c61 6d70 286d 2c20 4d29 0a0a 4061 6c69  lamp(m, M)..@ali
-000152d0: 6173 2822 7265 7361 6d70 6c65 5f66 6f72  as("resample_for
-000152e0: 7761 7264 2229 0a64 6566 2069 6e74 6572  ward").def inter
-000152f0: 706f 6c61 7469 6f6e 5f66 6f72 7761 7264  polation_forward
-00015300: 280a 2020 2020 2020 2020 696d 6167 652c  (.        image,
-00015310: 200a 2020 2020 2020 2020 7472 616e 7320   .        trans 
-00015320: 3d20 4e6f 6e65 2c20 0a20 2020 2020 2020  = None, .       
-00015330: 206d 6574 686f 6420 3d20 274c 696e 6561   method = 'Linea
-00015340: 7227 2c20 0a20 2020 2020 2020 2074 6172  r', .        tar
-00015350: 6765 745f 7370 6163 6520 3d20 4e6f 6e65  get_space = None
-00015360: 2c0a 2020 2020 2020 2020 6669 6c6c 203d  ,.        fill =
-00015370: 2027 7a65 726f 272c 0a20 2020 2020 2020   'zero',.       
-00015380: 2064 6572 6976 6174 6976 6520 3d20 4661   derivative = Fa
-00015390: 6c73 650a 2020 2020 293a 0a20 2020 2027  lse.    ):.    '
-000153a0: 2727 0a20 2020 2049 6e74 6572 706f 6c61  ''.    Interpola
-000153b0: 7465 2075 7369 6e67 2066 6f72 7761 7264  te using forward
-000153c0: 2074 7261 6e73 666f 726d 6174 696f 6e2e   transformation.
-000153d0: 2049 7420 6973 206e 6f74 2079 6574 2069   It is not yet i
-000153e0: 6d70 6c65 6d65 6e74 6564 2e20 0a20 2020  mplemented. .   
-000153f0: 2069 2e65 2e20 436f 6d70 7574 6520 7468   i.e. Compute th
-00015400: 6520 696d 6167 6520 4920 732e 742e 2074  e image I s.t. t
-00015410: 7261 6e73 2878 2920 3d20 7920 666f 7220  rans(x) = y for 
-00015420: 7820 696e 2069 6e70 7574 2069 6d61 6765  x in input image
-00015430: 2061 6e64 2079 2069 6e20 7468 6520 6f75   and y in the ou
-00015440: 7470 7574 2049 2075 7369 6e67 2069 6e74  tput I using int
-00015450: 6572 706f 6c61 7469 6f6e 206d 6574 686f  erpolation metho
-00015460: 643a 0a20 2020 2020 2020 206d 6574 686f  d:.        metho
-00015470: 6420 3d20 4c69 6e65 6172 205b 4e4f 2047  d = Linear [NO G
-00015480: 5241 4449 454e 5421 2121 5d3a 2042 696c  RADIENT!!!]: Bil
-00015490: 696e 6561 7220 696e 7465 7270 6f6c 6174  inear interpolat
-000154a0: 696f 6e0a 2020 2020 2020 2020 6d65 7468  ion.        meth
-000154b0: 6f64 203d 204e 6561 7265 7374 205b 4e4f  od = Nearest [NO
-000154c0: 2047 5241 4449 454e 5421 2121 5d3a 204e   GRADIENT!!!]: N
-000154d0: 6561 7265 7374 2069 6e74 6572 706f 6c61  earest interpola
-000154e0: 7469 6f6e 0a0a 2020 2020 5061 7261 6d73  tion..    Params
-000154f0: 3a0a 2020 2020 2020 2020 696d 6167 6520  :.        image 
-00015500: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
-00015510: 2074 6172 6765 7420 696d 6167 652e 0a20   target image.. 
-00015520: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-00015530: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
-00015540: 6e61 6c5d 2c20 7b6e 5f63 6861 6e6e 656c  nal], {n_channel
-00015550: 3a6f 7074 696f 6e61 6c7d 2c20 6d40 312c  :optional}, m@1,
-00015560: 206d 4032 2c20 2e2e 2e2c 206d 406e 5f64   m@2, ..., m@n_d
-00015570: 696d 290a 2020 2020 2020 2020 7472 616e  im).        tran
-00015580: 7320 5b46 756e 6374 696f 6e20 6f72 206d  s [Function or m
-00015590: 6963 6f6d 7075 7469 6e67 2e53 7061 7469  icomputing.Spati
-000155a0: 616c 5472 616e 7366 6f72 6d61 7469 6f6e  alTransformation
-000155b0: 5d3a 2054 7261 6e73 666f 726d 6174 696f  ]: Transformatio
-000155c0: 6e20 6675 6e63 7469 6f6e 2c20 6d61 7070  n function, mapp
-000155d0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-000155e0: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
-000155f0: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
-00015600: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
-00015610: 2e2c 206e 406e 5f64 696d 2920 746f 2028  ., n@n_dim) to (
-00015620: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-00015630: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
-00015640: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
-00015650: 2020 2020 6d65 7468 6f64 205b 7374 723a      method [str:
-00015660: 206c 696e 6561 727c 6e65 6172 6573 745d   linear|nearest]
-00015670: 3a20 5468 6520 696e 7465 7270 6f6c 6174  : The interpolat
-00015680: 696f 6e20 6d65 7468 6f64 2e20 0a20 2020  ion method. .   
-00015690: 2020 2020 2074 6172 6765 745f 7370 6163       target_spac
-000156a0: 6520 5b74 7570 6c65 206f 7220 6274 2e54  e [tuple or bt.T
-000156b0: 656e 736f 725d 3a0a 2020 2020 2020 2020  ensor]:.        
-000156c0: 2020 2020 5369 7a65 2028 7475 706c 6529      Size (tuple)
-000156d0: 206f 6620 6120 7461 7267 6574 2052 4f49   of a target ROI
-000156e0: 2061 7420 7468 6520 6365 6e74 6572 206f   at the center o
-000156f0: 6620 696d 6167 652e 200a 2020 2020 2020  f image. .      
-00015700: 2020 2020 2020 4f52 2054 7261 6e73 666f        OR Transfo
-00015710: 726d 6564 2063 6f6f 7264 696e 6174 6520  rmed coordinate 
-00015720: 7370 6163 6520 2862 742e 5465 6e73 6f72  space (bt.Tensor
-00015730: 2920 6f66 2074 6865 206f 7574 7075 7420  ) of the output 
-00015740: 696d 6167 652e 200a 2020 2020 2020 2020  image. .        
-00015750: 2020 2020 7369 7a65 3a20 6c65 6e67 7468      size: length
-00015760: 286e 5f64 696d 2920 6f72 2028 5b6e 5f62  (n_dim) or ([n_b
-00015770: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
-00015780: 7b6e 5f64 696d 3a6f 7074 696f 6e61 6c7d  {n_dim:optional}
-00015790: 2c20 7369 7a65 4031 2c20 7369 7a65 4032  , size@1, size@2
-000157a0: 2c20 2e2e 2e2c 2073 697a 6540 6e5f 6469  , ..., size@n_di
-000157b0: 6d29 0a20 2020 2020 2020 2066 696c 6c20  m).        fill 
-000157c0: 5b73 7472 3a20 6e65 6172 6573 747c 6261  [str: nearest|ba
-000157d0: 636b 6772 6f75 6e64 206f 7220 696e 7420  ckground or int 
-000157e0: 6f72 2066 6c6f 6174 286e 756d 6265 7229  or float(number)
-000157f0: 5d3a 2049 6e64 6963 6174 6520 7468 6520  ]: Indicate the 
-00015800: 7761 7920 746f 2066 696c 6c20 6261 636b  way to fill back
-00015810: 6772 6f75 6e64 206f 7574 7369 6465 2060  ground outside `
-00015820: 5375 7272 6f75 6e64 696e 6760 2e20 0a20  Surrounding`. . 
-00015830: 2020 2020 2020 2064 6572 6976 6174 6976         derivativ
-00015840: 6520 5b62 6f6f 6c5d 3a20 5768 6574 6865  e [bool]: Whethe
-00015850: 7220 746f 2072 6574 7572 6e20 7468 6520  r to return the 
-00015860: 6772 6164 6965 6e74 2e20 4f6e 6520 6361  gradient. One ca
-00015870: 6e20 6f6d 6974 2069 7420 7768 656e 2075  n omit it when u
-00015880: 7369 6e67 2074 6f72 6368 2e61 7574 6f67  sing torch.autog
-00015890: 7261 642e 0a0a 2020 2020 2020 2020 6f75  rad...        ou
-000158a0: 7470 7574 205b 6274 2e54 656e 736f 725d  tput [bt.Tensor]
-000158b0: 3a20 5468 6520 7472 616e 7366 6f72 6d65  : The transforme
-000158c0: 6420 696d 6167 652e 0a20 2020 2020 2020  d image..       
-000158d0: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
-000158e0: 6174 6368 5d2c 207b 6e5f 6368 616e 6e65  atch], {n_channe
-000158f0: 6c3a 6f70 7469 6f6e 616c 7d2c 206d 4031  l:optional}, m@1
-00015900: 2c20 6d40 322c 202e 2e2e 2c20 6d40 6e5f  , m@2, ..., m@n_
-00015910: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-00015920: 206f 7220 7768 656e 2060 7461 7267 6574   or when `target
-00015930: 5f73 7061 6365 6020 6973 2064 6566 696e  _space` is defin
-00015940: 6564 2062 7920 7465 6e73 6f72 2e20 0a20  ed by tensor. . 
-00015950: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-00015960: 2028 5b6e 5f62 6174 6368 5d2c 2073 697a   ([n_batch], siz
-00015970: 6540 312c 2073 697a 6540 322c 202e 2e2e  e@1, size@2, ...
-00015980: 2c20 7369 7a65 406e 5f64 696d 290a 2020  , size@n_dim).  
-00015990: 2020 2020 2020 2020 2020 6f72 2074 6865            or the
-000159a0: 2064 6572 6976 6174 6976 6520 666f 7220   derivative for 
-000159b0: 7468 6520 696e 7465 7270 6f6c 6174 696f  the interpolatio
-000159c0: 6e2e 2028 6966 2060 6465 7269 7661 7469  n. (if `derivati
-000159d0: 7665 203d 2054 7275 6560 290a 2020 2020  ve = True`).    
-000159e0: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
-000159f0: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
-00015a00: 7d2c 2073 697a 6540 312c 2073 697a 6540  }, size@1, size@
-00015a10: 322c 202e 2e2e 2c20 7369 7a65 406e 5f64  2, ..., size@n_d
-00015a20: 696d 290a 0a20 2020 2045 7861 6d70 6c65  im)..    Example
-00015a30: 733a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  s:.    ---------
-00015a40: 2d0a 2020 2020 3e3e 3e20 496d 6167 6520  -.    >>> Image 
-00015a50: 3d20 6274 2e72 616e 6428 332c 2031 3030  = bt.rand(3, 100
-00015a60: 2c20 3132 302c 2038 3029 0a20 2020 203e  , 120, 80).    >
-00015a70: 3e3e 2041 4d20 3d20 6274 2e72 616e 6428  >> AM = bt.rand(
-00015a80: 342c 2034 290a 2020 2020 3e3e 3e20 414d  4, 4).    >>> AM
-00015a90: 5b33 2c20 3a5d 203d 2062 742e 6f6e 655f  [3, :] = bt.one_
-00015aa0: 686f 7428 2d31 2c20 3429 0a20 2020 203e  hot(-1, 4).    >
-00015ab0: 3e3e 2069 6e74 6572 706f 6c61 7469 6f6e  >> interpolation
-00015ac0: 2849 6d61 6765 2c20 4166 6669 6e65 2841  (Image, Affine(A
-00015ad0: 4d29 2c20 6d65 7468 6f64 3d27 4c69 6e65  M), method='Line
-00015ae0: 6172 2729 0a20 2020 2027 2727 0a20 2020  ar').    '''.   
-00015af0: 2069 6620 7472 616e 7320 6973 206e 6f74   if trans is not
-00015b00: 204e 6f6e 6520 616e 6420 7472 616e 732e   None and trans.
-00015b10: 6261 636b 7761 7264 3a0a 2020 2020 2020  backward:.      
-00015b20: 2020 6966 2068 6173 6174 7472 2874 7261    if hasattr(tra
-00015b30: 6e73 2c20 2769 6e76 2729 3a20 7472 616e  ns, 'inv'): tran
-00015b40: 7320 3d20 7472 616e 732e 696e 7628 292e  s = trans.inv().
-00015b50: 6661 6b65 5f69 6e76 2829 0a20 2020 2020  fake_inv().     
-00015b60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00015b70: 2020 2020 2070 7269 6e74 2822 5761 726e       print("Warn
-00015b80: 696e 673a 2042 6163 6b77 6172 6420 7472  ing: Backward tr
-00015b90: 616e 7366 6f72 6d61 7469 6f6e 2066 6f75  ansformation fou
-00015ba0: 6e64 2069 6e20 6d65 7468 6f64 2060 696e  nd in method `in
-00015bb0: 7465 7270 6f6c 6174 696f 6e5f 666f 7277  terpolation_forw
-00015bc0: 6172 6460 2e20 5573 696e 6720 6069 6e74  ard`. Using `int
-00015bd0: 6572 706f 6c61 7469 6f6e 6020 696e 7374  erpolation` inst
-00015be0: 6561 642e 2022 290a 2020 2020 2020 2020  ead. ").        
-00015bf0: 2020 2020 7265 7475 726e 2069 6e74 6572      return inter
-00015c00: 706f 6c61 7469 6f6e 2869 6d61 6765 2c20  polation(image, 
-00015c10: 7472 616e 732c 206d 6574 686f 6420 3d20  trans, method = 
-00015c20: 6d65 7468 6f64 2c20 7461 7267 6574 5f73  method, target_s
-00015c30: 7061 6365 203d 2074 6172 6765 745f 7370  pace = target_sp
-00015c40: 6163 652c 2066 696c 6c20 3d20 6669 6c6c  ace, fill = fill
-00015c50: 290a 2020 2020 7265 7475 726e 204e 6f74  ).    return Not
-00015c60: 496d 706c 656d 656e 7465 640a 0a23 2323  Implemented..###
-00015c70: 2323 2323 2323 2323 2320 496d 6167 6520  ######### Image 
-00015c80: 5472 616e 7366 6f72 6d61 7469 6f6e 7320  Transformations 
-00015c90: 2323 2323 2323 2323 2323 2323 0a0a 636c  ############..cl
-00015ca0: 6173 7320 496d 6167 6554 7261 6e73 666f  ass ImageTransfo
-00015cb0: 726d 6174 696f 6e28 5472 616e 7366 6f72  rmation(Transfor
-00015cc0: 6d61 7469 6f6e 293a 0a20 2020 2020 2020  mation):.       
-00015cd0: 200a 2020 2020 6465 6620 5f5f 6361 6c6c   .    def __call
-00015ce0: 5f5f 2873 656c 662c 2058 293a 0a20 2020  __(self, X):.   
-00015cf0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00015d00: 2058 205b 6274 2e54 656e 736f 725d 3a20   X [bt.Tensor]: 
-00015d10: 496d 6167 6520 746f 2062 6520 7472 616e  Image to be tran
-00015d20: 7366 6f72 6d65 642e 0a20 2020 2020 2020  sformed..       
-00015d30: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
-00015d40: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
-00015d50: 7b6e 5f63 6861 6e6e 656c 3a6f 7074 696f  {n_channel:optio
-00015d60: 6e61 6c7d 2c20 6e40 312c 206e 4032 2c20  nal}, n@1, n@2, 
-00015d70: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
-00015d80: 2020 2020 2020 6f75 7470 7574 205b 6274        output [bt
-00015d90: 2e54 656e 736f 725d 3a20 5468 6520 7472  .Tensor]: The tr
-00015da0: 616e 7366 6f72 6d65 6420 696d 6167 652e  ansformed image.
-00015db0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00015dc0: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
-00015dd0: 6e5f 6368 616e 6e65 6c7d 2c20 6e40 312c  n_channel}, n@1,
-00015de0: 206e 4032 2c20 2e2e 2e2c 206e 406e 5f64   n@2, ..., n@n_d
-00015df0: 696d 290a 2020 2020 2020 2020 2727 270a  im).        '''.
-00015e00: 2020 2020 2020 2020 5820 3d20 6261 746f          X = bato
-00015e10: 7263 685f 7465 6e73 6f72 2858 290a 2020  rch_tensor(X).  
-00015e20: 2020 2020 2020 6966 2073 656c 662e 6e5f        if self.n_
-00015e30: 6469 6d20 6973 204e 6f6e 653a 0a20 2020  dim is None:.   
-00015e40: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00015e50: 582e 6861 735f 6261 7463 683a 2058 203d  X.has_batch: X =
-00015e60: 2058 2e75 6e73 7175 6565 7a65 285b 5d29   X.unsqueeze([])
-00015e70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015e80: 6e6f 7420 582e 6861 735f 6368 616e 6e65  not X.has_channe
-00015e90: 6c3a 2058 203d 2058 2e73 7461 6e64 6172  l: X = X.standar
-00015ea0: 6428 292e 756e 7371 7565 657a 6528 7b31  d().unsqueeze({1
-00015eb0: 7d29 0a20 2020 2020 2020 2065 6c73 653a  }).        else:
-00015ec0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015ed0: 582e 6e5f 6469 6d20 3d3d 2073 656c 662e  X.n_dim == self.
-00015ee0: 6e5f 6469 6d3a 2058 203d 2058 2e72 656d  n_dim: X = X.rem
-00015ef0: 6f76 655f 7370 6563 6961 6c5f 2829 2e75  ove_special_().u
-00015f00: 6e73 7175 6565 7a65 285b 5d29 2e75 6e73  nsqueeze([]).uns
-00015f10: 7175 6565 7a65 287b 317d 290a 2020 2020  queeze({1}).    
-00015f20: 2020 2020 2020 2020 656c 6966 2058 2e6e          elif X.n
-00015f30: 5f64 696d 203d 3d20 7365 6c66 2e6e 5f64  _dim == self.n_d
-00015f40: 696d 202b 2031 3a0a 2020 2020 2020 2020  im + 1:.        
-00015f50: 2020 2020 2020 2020 6966 2058 2e68 6173          if X.has
-00015f60: 5f62 6174 6368 3a20 582e 6368 616e 6e65  _batch: X.channe
-00015f70: 6c5f 6469 6d65 6e73 696f 6e20 3d20 4e6f  l_dimension = No
-00015f80: 6e65 3b20 5820 3d20 582e 756e 7371 7565  ne; X = X.unsque
-00015f90: 657a 6528 7b30 2069 6620 582e 6261 7463  eze({0 if X.batc
-00015fa0: 685f 6469 6d65 6e73 696f 6e20 3e20 3020  h_dimension > 0 
-00015fb0: 656c 7365 2031 7d29 0a20 2020 2020 2020  else 1}).       
-00015fc0: 2020 2020 2020 2020 2065 6c69 6620 582e           elif X.
-00015fd0: 6861 735f 6368 616e 6e65 6c3a 2058 203d  has_channel: X =
-00015fe0: 2058 2e75 6e73 7175 6565 7a65 285b 5d29   X.unsqueeze([])
-00015ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016000: 2065 6c73 653a 2058 203d 2058 2e62 6174   else: X = X.bat
-00016010: 6368 5f64 696d 656e 7369 6f6e 5f28 3029  ch_dimension_(0)
-00016020: 2e75 6e73 7175 6565 7a65 287b 317d 290a  .unsqueeze({1}).
-00016030: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00016040: 2058 2e6e 5f64 696d 203d 3d20 7365 6c66   X.n_dim == self
-00016050: 2e6e 5f64 696d 202b 2032 3a0a 2020 2020  .n_dim + 2:.    
-00016060: 2020 2020 2020 2020 2020 2020 2320 5f63              # _c
-00016070: 6861 6e6e 616c 2f62 6174 6368 2064 696d  hannal/batch dim
-00016080: 656e 7369 6f6e 7320 7573 6564 2068 6572  ensions used her
-00016090: 6520 6173 2074 6865 7920 6172 6520 6e5f  e as they are n_
-000160a0: 6469 6d20 7768 656e 206e 6f74 2065 7869  dim when not exi
-000160b0: 7374 6564 2e20 0a20 2020 2020 2020 2020  sted. .         
-000160c0: 2020 2020 2020 2069 6620 6e6f 7420 582e         if not X.
-000160d0: 6861 735f 6261 7463 683a 2058 2e62 6174  has_batch: X.bat
-000160e0: 6368 5f64 696d 656e 7369 6f6e 203d 2030  ch_dimension = 0
-000160f0: 2069 6620 582e 5f63 6861 6e6e 656c 5f64   if X._channel_d
-00016100: 696d 656e 7369 6f6e 203e 2030 2065 6c73  imension > 0 els
-00016110: 6520 310a 2020 2020 2020 2020 2020 2020  e 1.            
-00016120: 2020 2020 6966 206e 6f74 2058 2e68 6173      if not X.has
-00016130: 5f63 6861 6e6e 656c 3a20 582e 6368 616e  _channel: X.chan
-00016140: 6e65 6c5f 6469 6d65 6e73 696f 6e20 3d20  nel_dimension = 
-00016150: 3020 6966 2058 2e5f 6261 7463 685f 6469  0 if X._batch_di
-00016160: 6d65 6e73 696f 6e20 3e20 3020 656c 7365  mension > 0 else
-00016170: 2031 0a20 2020 2020 2020 2061 766f 7563   1.        avouc
-00016180: 6828 582e 6861 735f 6261 7463 6820 616e  h(X.has_batch an
-00016190: 6420 582e 6861 735f 6368 616e 6e65 6c2c  d X.has_channel,
-000161a0: 2066 2250 6c65 6173 6520 7573 6520 6261   f"Please use ba
-000161b0: 746f 7263 6820 7465 6e73 6f72 206f 6620  torch tensor of 
-000161c0: 7369 7a65 205c 0a20 2020 2020 2020 2020  size \.         
-000161d0: 2020 2028 5b6e 5f62 6174 6368 5d2c 207b     ([n_batch], {
-000161e0: 7b6e 5f63 6861 6e6e 656c 2f6e 5f66 6561  {n_channel/n_fea
-000161f0: 7475 7265 3a6f 7074 696f 6e61 6c7d 7d2c  ture:optional}},
-00016200: 206d 5f31 2c20 6d5f 322c 202e 2e2e 2c20   m_1, m_2, ..., 
-00016210: 6d5f 7229 205b 723d 6e5f 6469 6d5d 2066  m_r) [r=n_dim] f
-00016220: 6f72 205c 0a20 2020 2020 2020 2020 2020  or \.           
-00016230: 2020 2020 207b 7365 6c66 2e5f 5f63 6c61       {self.__cla
-00016240: 7373 5f5f 2e5f 5f6e 616d 655f 5f2e 7370  ss__.__name__.sp
-00016250: 6c69 7428 272e 2729 5b2d 315d 7d20 5472  lit('.')[-1]} Tr
-00016260: 616e 7366 6f72 6d61 7469 6f6e 2c20 696e  ansformation, in
-00016270: 7374 6561 6420 6f66 207b 582e 7368 6170  stead of {X.shap
-00016280: 657d 2e20 2229 0a20 2020 2020 2020 2072  e}. ").        r
-00016290: 6574 7572 6e20 582e 636c 6f6e 6528 290a  eturn X.clone().
-000162a0: 0a63 6c61 7373 204e 6f72 6d61 6c69 7a65  .class Normalize
-000162b0: 2849 6d61 6765 5472 616e 7366 6f72 6d61  (ImageTransforma
-000162c0: 7469 6f6e 293a 0a20 2020 2064 6566 205f  tion):.    def _
-000162d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a5f  _init__(self, *_
-000162e0: 7261 6e67 6529 3a0a 2020 2020 2020 2020  range):.        
-000162f0: 2727 270a 2020 2020 2020 2020 4e6f 726d  '''.        Norm
-00016300: 616c 697a 6520 7468 6520 696e 7465 6e73  alize the intens
-00016310: 6974 7920 6f66 2061 6e20 696d 6167 652e  ity of an image.
-00016320: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00016330: 2020 5061 7261 6d73 3a0a 2020 2020 2020    Params:.      
-00016340: 2020 2020 2020 5f72 616e 6765 203d 2028        _range = (
-00016350: 6c6f 772c 2068 6967 6829 205b 696e 7420  low, high) [int 
-00016360: 6f72 2066 6c6f 6174 206f 7220 6274 2e54  or float or bt.T
-00016370: 656e 736f 725d 3a20 5468 6520 6c6f 7765  ensor]: The lowe
-00016380: 7374 2028 616e 6420 6869 6768 6573 7429  st (and highest)
-00016390: 2069 6e74 656e 7369 7479 2e20 0a20 2020   intensity. .   
-000163a0: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-000163b0: 653a 206c 656e 6774 6828 3229 206f 7220  e: length(2) or 
-000163c0: 285b 6e5f 6261 7463 685d 2c20 7b32 7d29  ([n_batch], {2})
-000163d0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-000163e0: 2020 2020 2020 5768 656e 2069 7420 6973        When it is
-000163f0: 2063 616c 6c65 643a 0a20 2020 2020 2020   called:.       
-00016400: 2020 2020 2058 205b 6274 2e54 656e 736f       X [bt.Tenso
-00016410: 725d 3a20 496d 6167 6520 746f 2062 6520  r]: Image to be 
-00016420: 7472 616e 7366 6f72 6d65 642e 0a20 2020  transformed..   
-00016430: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-00016440: 653a 2028 5b6e 5f62 6174 6368 3a6f 7074  e: ([n_batch:opt
-00016450: 696f 6e61 6c5d 2c20 7b6e 5f63 6861 6e6e  ional], {n_chann
-00016460: 656c 3a6f 7074 696f 6e61 6c7d 2c20 6e40  el:optional}, n@
-00016470: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-00016480: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
-00016490: 2020 6f75 7470 7574 205b 6274 2e54 656e    output [bt.Ten
-000164a0: 736f 725d 3a20 5468 6520 7472 616e 7366  sor]: The transf
-000164b0: 6f72 6d65 6420 696d 6167 652e 0a20 2020  ormed image..   
-000164c0: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-000164d0: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
-000164e0: 6e5f 6368 616e 6e65 6c7d 2c20 6e40 312c  n_channel}, n@1,
-000164f0: 206e 4032 2c20 2e2e 2e2c 206e 406e 5f64   n@2, ..., n@n_d
-00016500: 696d 290a 2020 2020 2020 2020 2727 270a  im).        '''.
-00016510: 2020 2020 2020 2020 6966 206c 656e 285f          if len(_
-00016520: 7261 6e67 6529 203d 3d20 303a 205f 7261  range) == 0: _ra
-00016530: 6e67 6520 3d20 4e6f 6e65 0a20 2020 2020  nge = None.     
-00016540: 2020 2065 6c69 6620 6c65 6e28 5f72 616e     elif len(_ran
-00016550: 6765 2920 3d3d 2031 2061 6e64 2069 7369  ge) == 1 and isi
-00016560: 6e73 7461 6e63 6528 5f72 616e 6765 5b30  nstance(_range[0
-00016570: 5d2c 2028 6c69 7374 2c20 7475 706c 6529  ], (list, tuple)
-00016580: 293a 205f 7261 6e67 6520 3d20 6261 746f  ): _range = bato
-00016590: 7263 685f 7465 6e73 6f72 286c 6973 7428  rch_tensor(list(
-000165a0: 5f72 616e 6765 5b30 5d29 290a 2020 2020  _range[0])).    
-000165b0: 2020 2020 656c 6966 206c 656e 285f 7261      elif len(_ra
-000165c0: 6e67 6529 203d 3d20 3120 616e 6420 6973  nge) == 1 and is
-000165d0: 696e 7374 616e 6365 285f 7261 6e67 655b  instance(_range[
-000165e0: 305d 2c20 6274 2e54 656e 736f 7229 3a20  0], bt.Tensor): 
-000165f0: 5f72 616e 6765 203d 205f 7261 6e67 655b  _range = _range[
-00016600: 305d 0a20 2020 2020 2020 2065 6c69 6620  0].        elif 
-00016610: 6c65 6e28 5f72 616e 6765 2920 3d3d 2031  len(_range) == 1
-00016620: 3a20 5f72 616e 6765 203d 2062 742e 6368  : _range = bt.ch
-00016630: 616e 6e65 6c5f 7465 6e73 6f72 2828 302c  annel_tensor((0,
-00016640: 205f 7261 6e67 6529 290a 2020 2020 2020   _range)).      
-00016650: 2020 656c 6966 206c 656e 285f 7261 6e67    elif len(_rang
-00016660: 6529 203d 3d20 323a 205f 7261 6e67 6520  e) == 2: _range 
-00016670: 3d20 6274 2e63 6861 6e6e 656c 5f74 656e  = bt.channel_ten
-00016680: 736f 7228 5f72 616e 6765 290a 2020 2020  sor(_range).    
-00016690: 2020 2020 656c 7365 3a20 7261 6973 6520      else: raise 
-000166a0: 5479 7065 4572 726f 7228 6622 496e 7661  TypeError(f"Inva
-000166b0: 6c69 6420 7261 6e67 6520 666f 7220 4e6f  lid range for No
-000166c0: 726d 616c 697a 653a 207b 5f72 616e 6765  rmalize: {_range
-000166d0: 7d2e 2022 290a 2020 2020 2020 2020 6966  }. ").        if
-000166e0: 205f 7261 6e67 6520 6973 204e 6f6e 653a   _range is None:
-000166f0: 2070 6173 730a 2020 2020 2020 2020 656c   pass.        el
-00016700: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016710: 6966 205f 7261 6e67 652e 6e5f 6469 6d20  if _range.n_dim 
-00016720: 3c20 323a 205f 7261 6e67 6520 3d20 5f72  < 2: _range = _r
-00016730: 616e 6765 2e75 6e73 7175 6565 7a65 285b  ange.unsqueeze([
-00016740: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
-00016750: 6620 6e6f 7420 5f72 616e 6765 2e68 6173  f not _range.has
-00016760: 5f62 6174 6368 3a20 5f72 616e 6765 2e62  _batch: _range.b
-00016770: 6174 6368 5f64 696d 656e 7369 6f6e 203d  atch_dimension =
-00016780: 2030 0a20 2020 2020 2020 2020 2020 2069   0.            i
-00016790: 6620 6e6f 7420 5f72 616e 6765 2e68 6173  f not _range.has
-000167a0: 5f63 6861 6e6e 656c 3a20 5f72 616e 6765  _channel: _range
-000167b0: 2e63 6861 6e6e 656c 5f64 696d 656e 7369  .channel_dimensi
-000167c0: 6f6e 203d 2031 0a20 2020 2020 2020 2020  on = 1.         
-000167d0: 2020 2061 766f 7563 6828 5f72 616e 6765     avouch(_range
-000167e0: 2e68 6173 5f62 6174 6368 2061 6e64 205f  .has_batch and _
-000167f0: 7261 6e67 652e 6861 735f 6368 616e 6e65  range.has_channe
-00016800: 6c2c 2066 2250 6c65 6173 6520 7573 6520  l, f"Please use 
-00016810: 6261 746f 7263 6820 7465 6e73 6f72 206f  batorch tensor o
-00016820: 6620 7369 7a65 205c 0a20 2020 2020 2020  f size \.       
-00016830: 2020 2020 2020 2020 2028 5b6e 5f62 6174           ([n_bat
-00016840: 6368 3a6f 7074 696f 6e61 6c5d 2c20 7b7b  ch:optional], {{
-00016850: 327d 7d29 2066 6f72 204e 6f72 6d61 6c69  2}}) for Normali
-00016860: 7a69 6e67 2070 6172 616d 6574 6572 732c  zing parameters,
-00016870: 2069 6e73 7465 6164 206f 6620 7b5f 7261   instead of {_ra
-00016880: 6e67 652e 7368 6170 657d 2e20 2229 0a20  nge.shape}. "). 
-00016890: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-000168a0: 5f69 6e69 745f 5f28 5f72 616e 6765 290a  _init__(_range).
-000168b0: 2020 2020 2020 2020 7365 6c66 2e72 616e          self.ran
-000168c0: 6765 203d 205f 7261 6e67 650a 2020 2020  ge = _range.    
-000168d0: 2020 2020 7365 6c66 2e5f 7261 6e67 6520      self._range 
-000168e0: 3d20 4e6f 6e65 0a0a 2020 2020 6465 6620  = None..    def 
-000168f0: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2058  __call__(self, X
-00016900: 293a 0a20 2020 2020 2020 2058 203d 2073  ):.        X = s
-00016910: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
-00016920: 5829 0a20 2020 2020 2020 205f 7261 6e67  X).        _rang
-00016930: 6520 3d20 7365 6c66 2e72 616e 6765 0a20  e = self.range. 
-00016940: 2020 2020 2020 2069 6620 5f72 616e 6765         if _range
-00016950: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00016960: 2020 2020 2020 5f72 616e 6765 203d 2062        _range = b
-00016970: 742e 7175 616e 7469 6c65 2858 2e66 6c61  t.quantile(X.fla
-00016980: 7474 656e 2829 2e66 6c6f 6174 2829 2c20  tten().float(), 
-00016990: 6261 746f 7263 685f 7465 6e73 6f72 285b  batorch_tensor([
-000169a0: 302e 3032 352c 2030 2e39 3735 5d29 2c20  0.025, 0.975]), 
-000169b0: 6178 6973 3d2d 3129 2e6d 6f76 6564 696d  axis=-1).movedim
-000169c0: 2830 2c20 2d31 292e 7370 6563 6961 6c5f  (0, -1).special_
-000169d0: 6672 6f6d 5f28 5829 0a20 2020 2020 2020  from_(X).       
-000169e0: 2020 2020 2073 656c 662e 5f72 616e 6765       self._range
-000169f0: 203d 205f 7261 6e67 650a 2020 2020 2020   = _range.      
-00016a00: 2020 7265 7475 726e 2028 2858 202d 205f    return ((X - _
-00016a10: 7261 6e67 655b 2e2e 2e2c 2030 5d29 202f  range[..., 0]) /
-00016a20: 2028 5f72 616e 6765 5b2e 2e2e 2c20 315d   (_range[..., 1]
-00016a30: 202d 205f 7261 6e67 655b 2e2e 2e2c 2030   - _range[..., 0
-00016a40: 5d29 292e 636c 616d 7028 302e 2c20 312e  ])).clamp(0., 1.
-00016a50: 290a 2020 2020 0a20 2020 2064 6566 2069  ).    .    def i
-00016a60: 6e76 2873 656c 6629 3a0a 2020 2020 2020  nv(self):.      
-00016a70: 2020 6966 2073 656c 662e 7261 6e67 6520    if self.range 
-00016a80: 6973 206e 6f74 204e 6f6e 653a 205f 7261  is not None: _ra
-00016a90: 6e67 6520 3d20 7365 6c66 2e72 616e 6765  nge = self.range
-00016aa0: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
-00016ab0: 6c66 2e5f 7261 6e67 6520 6973 206e 6f74  lf._range is not
-00016ac0: 204e 6f6e 653a 205f 7261 6e67 6520 3d20   None: _range = 
-00016ad0: 7365 6c66 2e5f 7261 6e67 650a 2020 2020  self._range.    
-00016ae0: 2020 2020 656c 7365 3a20 7265 7475 726e      else: return
-00016af0: 204e 6f72 6d61 6c69 7a65 284e 6f6e 6529   Normalize(None)
-00016b00: 0a20 2020 2020 2020 2064 656e 203d 205f  .        den = _
-00016b10: 7261 6e67 655b 2e2e 2e2c 2031 5d20 2d20  range[..., 1] - 
-00016b20: 5f72 616e 6765 5b2e 2e2e 2c20 305d 0a20  _range[..., 0]. 
-00016b30: 2020 2020 2020 205f 7261 6e67 6520 3d20         _range = 
-00016b40: 6274 2e73 7461 636b 282d 5f72 616e 6765  bt.stack(-_range
-00016b50: 5b2e 2e2e 2c20 305d 2c20 312d 5f72 616e  [..., 0], 1-_ran
-00016b60: 6765 5b2e 2e2e 2c20 305d 2c20 2d31 2920  ge[..., 0], -1) 
-00016b70: 2f20 6465 6e0a 2020 2020 2020 2020 7265  / den.        re
-00016b80: 7475 726e 204e 6f72 6d61 6c69 7a65 285f  turn Normalize(_
-00016b90: 7261 6e67 6529 0a0a 2323 2323 2323 2323  range)..########
-00016ba0: 2323 2323 2320 5375 7070 6f72 7469 6e67  ##### Supporting
-00016bb0: 2046 756e 6374 696f 6e73 2023 2323 2323   Functions #####
-00016bc0: 2323 2323 2323 230a 0a64 6566 2042 7370  #######..def Bsp
-00016bd0: 6c69 6e65 2869 2c20 5529 3a0a 2020 2020  line(i, U):.    
-00016be0: 2222 220a 2020 2020 4375 6269 6320 422d  """.    Cubic B-
-00016bf0: 7370 6c69 6e65 2066 756e 6374 696f 6e2e  spline function.
-00016c00: 200a 2020 2020 4e6f 7465 3a20 4173 206c   .    Note: As l
-00016c10: 6f6e 6720 6173 2069 2061 6e64 2055 2068  ong as i and U h
-00016c20: 6176 6520 7468 6520 7361 6d65 2073 697a  ave the same siz
-00016c30: 652c 2061 6e79 2073 6861 7065 206f 6620  e, any shape of 
-00016c40: 7465 6e73 6f72 7320 776f 756c 6420 646f  tensors would do
-00016c50: 2e0a 2020 2020 0a20 2020 2050 6172 616d  ..    .    Param
-00016c60: 733a 0a20 2020 2020 2020 2069 205b 6274  s:.        i [bt
-00016c70: 2e54 656e 736f 725d 3a20 7468 6520 696e  .Tensor]: the in
-00016c80: 6465 7820 6f66 2073 6567 6d65 6e74 2066  dex of segment f
-00016c90: 756e 6374 696f 6e20 6f66 2042 2d73 706c  unction of B-spl
-00016ca0: 696e 652e 0a20 2020 2020 2020 2020 2020  ine..           
-00016cb0: 2054 6865 2076 616c 7565 206f 6620 6561   The value of ea
-00016cc0: 6368 2065 6c65 6d65 6e74 2063 616e 2062  ch element can b
-00016cd0: 6520 6368 6f73 656e 2069 6e20 282d 312c  e chosen in (-1,
-00016ce0: 2030 2c20 312c 2032 292e 200a 2020 2020   0, 1, 2). .    
-00016cf0: 2020 2020 5520 5b62 742e 5465 6e73 6f72      U [bt.Tensor
-00016d00: 5d3a 2074 6865 2064 6563 696d 616c 2061  ]: the decimal a
-00016d10: 7267 756d 656e 7420 6f66 2042 2d73 706c  rgument of B-spl
-00016d20: 696e 6520 6675 6e63 7469 6f6e 2e20 4974  ine function. It
-00016d30: 2073 686f 756c 6420 6265 2077 6974 6869   should be withi
-00016d40: 6e20 7261 6e67 6520 5b30 2c20 3129 2e0a  n range [0, 1)..
-00016d50: 2020 2020 2222 220a 2020 2020 6920 3d20      """.    i = 
-00016d60: 6261 746f 7263 685f 7465 6e73 6f72 2869  batorch_tensor(i
-00016d70: 293b 2055 203d 2062 6174 6f72 6368 5f74  ); U = batorch_t
-00016d80: 656e 736f 7228 5529 0a20 2020 2072 6574  ensor(U).    ret
-00016d90: 7572 6e20 280a 2020 2020 2020 2020 6274  urn (.        bt
-00016da0: 2e77 6865 7265 2869 203d 3d20 2d31 2c20  .where(i == -1, 
-00016db0: 2831 202d 2055 2920 2a2a 2033 202f 2036  (1 - U) ** 3 / 6
-00016dc0: 2c0a 2020 2020 2020 2020 6274 2e77 6865  ,.        bt.whe
-00016dd0: 7265 2869 203d 3d20 302c 2055 202a 2a20  re(i == 0, U ** 
-00016de0: 3320 2f20 3220 2d20 5520 2a20 5520 2b20  3 / 2 - U * U + 
-00016df0: 3220 2f20 332c 0a20 2020 2020 2020 2062  2 / 3,.        b
-00016e00: 742e 7768 6572 6528 6920 3d3d 2031 2c20  t.where(i == 1, 
-00016e10: 282d 2033 202a 2055 202a 2a20 3320 2b20  (- 3 * U ** 3 + 
-00016e20: 3320 2a20 5520 2a20 5520 2b20 3320 2a20  3 * U * U + 3 * 
-00016e30: 5520 2b20 3129 202f 2036 2c0a 2020 2020  U + 1) / 6,.    
-00016e40: 2020 2020 6274 2e77 6865 7265 2869 203d      bt.where(i =
-00016e50: 3d20 322c 2055 202a 2a20 3320 2f20 362c  = 2, U ** 3 / 6,
-00016e60: 0a20 2020 2020 2020 2062 742e 7a65 726f  .        bt.zero
-00016e70: 735f 6c69 6b65 2855 2929 2929 290a 2020  s_like(U))))).  
-00016e80: 2020 290a 0a64 6566 2064 4273 706c 696e    )..def dBsplin
-00016e90: 6528 692c 2055 293a 0a20 2020 2022 2222  e(i, U):.    """
-00016ea0: 0a20 2020 2054 6865 2064 6572 6976 6174  .    The derivat
-00016eb0: 6976 6520 6f66 2042 2d73 706c 696e 6520  ive of B-spline 
-00016ec0: 6675 6e63 7469 6f6e 2c20 7769 7468 2072  function, with r
-00016ed0: 6573 7065 6374 2074 6f20 552e 200a 2020  espect to U. .  
-00016ee0: 2020 4e6f 7465 3a20 4173 206c 6f6e 6720    Note: As long 
-00016ef0: 6173 2069 2061 6e64 2055 2068 6176 6520  as i and U have 
-00016f00: 7468 6520 7361 6d65 2073 697a 652c 2061  the same size, a
-00016f10: 6e79 2073 6861 7065 206f 6620 7465 6e73  ny shape of tens
-00016f20: 6f72 7320 776f 756c 6420 646f 2e0a 2020  ors would do..  
-00016f30: 2020 0a20 2020 2050 6172 616d 733a 0a20    .    Params:. 
-00016f40: 2020 2020 2020 2069 205b 6274 2e54 656e         i [bt.Ten
-00016f50: 736f 725d 3a20 7468 6520 696e 6465 7820  sor]: the index 
-00016f60: 6f66 2073 6567 6d65 6e74 2066 756e 6374  of segment funct
-00016f70: 696f 6e20 6f66 2042 2d73 706c 696e 652e  ion of B-spline.
-00016f80: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00016f90: 2076 616c 7565 206f 6620 6561 6368 2065   value of each e
-00016fa0: 6c65 6d65 6e74 2063 616e 2062 6520 6368  lement can be ch
-00016fb0: 6f73 656e 2069 6e20 282d 312c 2030 2c20  osen in (-1, 0, 
-00016fc0: 312c 2032 292e 200a 2020 2020 2020 2020  1, 2). .        
-00016fd0: 5520 5b62 742e 5465 6e73 6f72 5d3a 2074  U [bt.Tensor]: t
-00016fe0: 6865 2064 6563 696d 616c 2061 7267 756d  he decimal argum
-00016ff0: 656e 7420 6f66 2042 2d73 706c 696e 6520  ent of B-spline 
-00017000: 6675 6e63 7469 6f6e 2e20 4974 2073 686f  function. It sho
-00017010: 756c 6420 6265 2077 6974 6869 6e20 7261  uld be within ra
-00017020: 6e67 6520 5b30 2c20 3129 2e0a 2020 2020  nge [0, 1)..    
-00017030: 2222 220a 2020 2020 6920 3d20 6261 746f  """.    i = bato
-00017040: 7263 685f 7465 6e73 6f72 2869 293b 2055  rch_tensor(i); U
-00017050: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
-00017060: 7228 5529 0a20 2020 2072 6574 7572 6e20  r(U).    return 
-00017070: 280a 2020 2020 2020 2020 6274 2e77 6865  (.        bt.whe
-00017080: 7265 2869 203d 3d20 2d31 2c20 2d20 3320  re(i == -1, - 3 
-00017090: 2a20 2831 202d 2055 2920 2a2a 2032 202f  * (1 - U) ** 2 /
-000170a0: 2036 2c0a 2020 2020 2020 2020 6274 2e77   6,.        bt.w
-000170b0: 6865 7265 2869 203d 3d20 302c 2033 202a  here(i == 0, 3 *
-000170c0: 2055 202a 2a20 3220 2f20 3220 2d20 3220   U ** 2 / 2 - 2 
-000170d0: 2a20 552c 0a20 2020 2020 2020 2062 742e  * U,.        bt.
-000170e0: 7768 6572 6528 6920 3d3d 2031 2c20 282d  where(i == 1, (-
-000170f0: 2033 202a 2055 202a 2a20 3220 2b20 3220   3 * U ** 2 + 2 
-00017100: 2a20 5520 2b20 3129 202f 2032 2c0a 2020  * U + 1) / 2,.  
-00017110: 2020 2020 2020 6274 2e77 6865 7265 2869        bt.where(i
-00017120: 203d 3d20 322c 2033 202a 2055 202a 2a20   == 2, 3 * U ** 
-00017130: 3220 2f20 362c 0a20 2020 2020 2020 2062  2 / 6,.        b
-00017140: 742e 7a65 726f 735f 6c69 6b65 2855 2929  t.zeros_like(U))
-00017150: 2929 290a 2020 2020 290a 0a64 6566 2066  ))).    )..def f
-00017160: 4273 706c 696e 6528 632c 2078 293a 0a20  Bspline(c, x):. 
-00017170: 2020 2063 203d 2062 6174 6f72 6368 5f74     c = batorch_t
-00017180: 656e 736f 7228 6329 3b20 7820 3d20 6261  ensor(c); x = ba
-00017190: 746f 7263 685f 7465 6e73 6f72 2878 290a  torch_tensor(x).
-000171a0: 2020 2020 6420 3d20 7820 2d20 630a 2020      d = x - c.  
-000171b0: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
-000171c0: 2020 2062 742e 7768 6572 6528 282d 3220     bt.where((-2 
-000171d0: 3c3d 2064 2920 2a20 2864 203c 202d 3129  <= d) * (d < -1)
-000171e0: 2c20 6420 2a2a 2033 202b 2036 202a 2064  , d ** 3 + 6 * d
-000171f0: 202a 2a20 3220 2b20 3132 202a 2064 202b   ** 2 + 12 * d +
-00017200: 2038 2c0a 2020 2020 2020 2020 6274 2e77   8,.        bt.w
-00017210: 6865 7265 2828 2d31 203c 3d20 6429 202a  here((-1 <= d) *
-00017220: 2028 6420 3c20 3029 2c20 2d20 3320 2a20   (d < 0), - 3 * 
-00017230: 6420 2a2a 2033 202d 2036 202a 2064 202a  d ** 3 - 6 * d *
-00017240: 2a20 3220 2b20 342c 0a20 2020 2020 2020  * 2 + 4,.       
-00017250: 2062 742e 7768 6572 6528 2830 203c 3d20   bt.where((0 <= 
-00017260: 6429 202a 2028 6420 3c20 3129 2c20 3320  d) * (d < 1), 3 
-00017270: 2a20 6420 2a2a 2033 202d 2036 202a 2064  * d ** 3 - 6 * d
-00017280: 202a 2a20 3220 2b20 342c 0a20 2020 2020   ** 2 + 4,.     
-00017290: 2020 2062 742e 7768 6572 6528 2831 203c     bt.where((1 <
-000172a0: 3d20 6429 202a 2028 6420 3c20 3229 2c20  = d) * (d < 2), 
-000172b0: 2d20 6420 2a2a 2033 202b 2036 202a 2064  - d ** 3 + 6 * d
-000172c0: 202a 2a20 3220 2d20 3132 202a 2064 202b   ** 2 - 12 * d +
-000172d0: 2038 2c0a 2020 2020 2020 2020 6274 2e7a   8,.        bt.z
-000172e0: 6572 6f73 5f6c 696b 6528 6429 2929 2929  eros_like(d)))))
-000172f0: 202f 2036 0a20 2020 2029 0a0a 6465 6620   / 6.    )..def 
-00017300: 4166 6669 6e65 3244 324d 6174 7269 7828  Affine2D2Matrix(
-00017310: 7061 7261 6d73 293a 0a20 2020 2022 2222  params):.    """
-00017320: 0a20 2020 2074 312c 2074 322c 20ce b82c  .    t1, t2, ..,
-00017330: 2073 312c 2073 322c 20cf 8131 2c20 cf81   s1, s2, ..1, ..
-00017340: 3220 696e 2073 697a 653a 2028 5b6e 5f62  2 in size: ([n_b
-00017350: 6174 6368 5d2c 207b 377d 290a 2020 2020  atch], {7}).    
-00017360: 7431 2c20 7432 2c20 6331 2c20 6332 2c20  t1, t2, c1, c2, 
-00017370: ceb8 2c20 7331 2c20 7332 2c20 cf81 312c  .., s1, s2, ..1,
-00017380: 20cf 8132 2069 6e20 7369 7a65 3a20 285b   ..2 in size: ([
-00017390: 6e5f 6261 7463 685d 2c20 7b39 7d29 0a20  n_batch], {9}). 
-000173a0: 2020 206f 7574 7075 7420 696e 2073 697a     output in siz
-000173b0: 653a 2028 5b6e 5f62 6174 6368 5d2c 2033  e: ([n_batch], 3
-000173c0: 2c20 3329 0a20 2020 2022 2222 0a20 2020  , 3).    """.   
-000173d0: 2070 6172 616d 7320 3d20 6261 746f 7263   params = batorc
-000173e0: 685f 7465 6e73 6f72 2870 6172 616d 7329  h_tensor(params)
-000173f0: 0a20 2020 2069 6620 7061 7261 6d73 2e6e  .    if params.n
-00017400: 5f64 696d 203c 3d20 3120 616e 6420 6e6f  _dim <= 1 and no
-00017410: 7420 7061 7261 6d73 2e68 6173 5f62 6174  t params.has_bat
-00017420: 6368 3a20 7061 7261 6d73 203d 2070 6172  ch: params = par
-00017430: 616d 732e 756e 7371 7565 657a 6528 5b5d  ams.unsqueeze([]
-00017440: 290a 2020 2020 6966 2070 6172 616d 732e  ).    if params.
-00017450: 6e5f 6469 6d20 3c3d 2031 2061 6e64 206e  n_dim <= 1 and n
-00017460: 6f74 2070 6172 616d 732e 6861 735f 6368  ot params.has_ch
-00017470: 616e 6e65 6c3a 2070 6172 616d 7320 3d20  annel: params = 
-00017480: 7061 7261 6d73 2e75 6e73 7175 6565 7a65  params.unsqueeze
-00017490: 287b 317d 290a 2020 2020 6966 2070 6172  ({1}).    if par
-000174a0: 616d 732e 6e5f 6469 6d20 3d3d 2032 2061  ams.n_dim == 2 a
-000174b0: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
-000174c0: 735f 6261 7463 683a 2070 6172 616d 732e  s_batch: params.
-000174d0: 6261 7463 685f 6469 6d65 6e73 696f 6e20  batch_dimension 
-000174e0: 3d20 300a 2020 2020 6966 2070 6172 616d  = 0.    if param
-000174f0: 732e 6e5f 6469 6d20 3d3d 2032 2061 6e64  s.n_dim == 2 and
-00017500: 206e 6f74 2070 6172 616d 732e 6861 735f   not params.has_
-00017510: 6368 616e 6e65 6c3a 2070 6172 616d 732e  channel: params.
-00017520: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
-00017530: 6e20 3d20 310a 2020 2020 6176 6f75 6368  n = 1.    avouch
-00017540: 2870 6172 616d 732e 6861 735f 6261 7463  (params.has_batc
-00017550: 682c 2066 2250 6c65 6173 6520 7573 6520  h, f"Please use 
-00017560: 6261 746f 7263 6820 7465 6e73 6f72 206f  batorch tensor o
-00017570: 6620 7369 7a65 2028 5b6e 5f62 6174 6368  f size ([n_batch
-00017580: 5d2c 207b 3720 6f72 2039 7d29 205c 0a20  ], {7 or 9}) \. 
-00017590: 2020 2020 2020 2066 6f72 2041 6666 696e         for Affin
-000175a0: 6520 7061 7261 6d65 7465 7273 2c20 696e  e parameters, in
-000175b0: 7374 6561 6420 6f66 207b 7061 7261 6d73  stead of {params
-000175c0: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-000175d0: 6e5f 6261 7463 6820 3d20 7061 7261 6d73  n_batch = params
-000175e0: 2e6e 5f62 6174 6368 0a20 2020 2069 6620  .n_batch.    if 
-000175f0: 7061 7261 6d73 2e73 697a 6528 3129 203d  params.size(1) =
-00017600: 3d20 373a 0a20 2020 2020 2020 2074 312c  = 7:.        t1,
-00017610: 2074 322c 20ce b82c 2073 312c 2073 322c   t2, .., s1, s2,
-00017620: 20cf 8131 2c20 cf81 3220 3d20 7061 7261   ..1, ..2 = para
-00017630: 6d73 2e73 706c 6974 2829 0a20 2020 2020  ms.split().     
-00017640: 2020 2063 3120 3d20 6274 2e7a 6572 6f73     c1 = bt.zeros
-00017650: 285b 6e5f 6261 7463 685d 2c20 3129 3b20  ([n_batch], 1); 
-00017660: 6332 203d 2062 742e 7a65 726f 7328 5b6e  c2 = bt.zeros([n
-00017670: 5f62 6174 6368 5d2c 2031 290a 2020 2020  _batch], 1).    
-00017680: 6966 2070 6172 616d 732e 7369 7a65 2831  if params.size(1
-00017690: 2920 3d3d 2039 3a0a 2020 2020 2020 2020  ) == 9:.        
-000176a0: 7431 2c20 7432 2c20 6331 2c20 6332 2c20  t1, t2, c1, c2, 
-000176b0: ceb8 2c20 7331 2c20 7332 2c20 cf81 312c  .., s1, s2, ..1,
-000176c0: 20cf 8132 203d 2070 6172 616d 732e 7370   ..2 = params.sp
-000176d0: 6c69 7428 290a 2020 2020 6120 3d20 28cf  lit().    a = (.
-000176e0: 8131 202a 20cf 8132 202b 2031 2920 2a20  .1 * ..2 + 1) * 
-000176f0: 7331 202a 2062 742e 636f 7328 ceb8 2920  s1 * bt.cos(..) 
-00017700: 2b20 cf81 3120 2a20 7332 202a 2062 742e  + ..1 * s2 * bt.
-00017710: 7369 6e28 ceb8 290a 2020 2020 6220 3d20  sin(..).    b = 
-00017720: 2d20 28cf 8131 202a 20cf 8132 202b 2031  - (..1 * ..2 + 1
-00017730: 2920 2a20 7331 202a 2062 742e 7369 6e28  ) * s1 * bt.sin(
-00017740: ceb8 2920 2b20 cf81 3120 2a20 7332 202a  ..) + ..1 * s2 *
-00017750: 2062 742e 636f 7328 ceb8 290a 2020 2020   bt.cos(..).    
-00017760: 6320 3d20 cf81 3220 2a20 7331 202a 2062  c = ..2 * s1 * b
-00017770: 742e 636f 7328 ceb8 2920 2b20 7332 202a  t.cos(..) + s2 *
-00017780: 2062 742e 7369 6e28 ceb8 290a 2020 2020   bt.sin(..).    
-00017790: 6420 3d20 2d20 cf81 3220 2a20 7331 202a  d = - ..2 * s1 *
-000177a0: 2062 742e 7369 6e28 ceb8 2920 2b20 7332   bt.sin(..) + s2
-000177b0: 202a 2062 742e 636f 7328 ceb8 290a 2020   * bt.cos(..).  
-000177c0: 2020 7265 7475 726e 2062 742e 6361 7428    return bt.cat(
-000177d0: 0a20 2020 2020 2020 2062 742e 6361 7428  .        bt.cat(
-000177e0: 2861 2c20 622c 2074 3120 2d20 6120 2a20  (a, b, t1 - a * 
-000177f0: 6331 202d 2062 202a 2063 3220 2b20 6331  c1 - b * c2 + c1
-00017800: 2c20 632c 2064 2c20 7432 202d 2063 202a  , c, d, t2 - c *
-00017810: 2063 3120 2d20 6420 2a20 6332 202b 2063   c1 - d * c2 + c
-00017820: 3229 2c20 7b7d 292e 7669 6577 285b 6e5f  2), {}).view([n_
-00017830: 6261 7463 685d 2c20 322c 2033 292c 200a  batch], 2, 3), .
-00017840: 2020 2020 2020 2020 6274 2e6f 6e65 5f68          bt.one_h
-00017850: 6f74 282d 312c 2033 292e 6d75 6c74 6970  ot(-1, 3).multip
-00017860: 6c79 286e 5f62 6174 6368 2c20 5b5d 292e  ly(n_batch, []).
-00017870: 7669 6577 285b 6e5f 6261 7463 685d 2c20  view([n_batch], 
-00017880: 312c 2033 292c 2031 0a20 2020 2029 0a0a  1, 3), 1.    )..
-00017890: 6465 6620 5175 6174 6572 6e73 324d 6174  def Quaterns2Mat
-000178a0: 7269 7828 7061 7261 6d73 293a 0a20 2020  rix(params):.   
-000178b0: 2022 2222 0a20 2020 2020 2020 2051 7561   """.        Qua
-000178c0: 7465 726e 3a20 7162 2c20 7163 2c20 7164  tern: qb, qc, qd
-000178d0: 2c20 7078 2c20 7079 2c20 707a 2069 6e20  , px, py, pz in 
-000178e0: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
-000178f0: 2c20 7b36 7d29 0a20 2020 2020 2020 204d  , {6}).        M
-00017900: 6174 7269 783a 2028 5b6e 5f62 6174 6368  atrix: ([n_batch
-00017910: 5d2c 2034 2c20 3429 0a20 2020 2022 2222  ], 4, 4).    """
-00017920: 0a20 2020 2070 6172 616d 7320 3d20 6261  .    params = ba
-00017930: 746f 7263 685f 7465 6e73 6f72 2870 6172  torch_tensor(par
-00017940: 616d 7329 0a20 2020 2069 6620 7061 7261  ams).    if para
-00017950: 6d73 2e6e 5f64 696d 203c 3d20 3120 616e  ms.n_dim <= 1 an
-00017960: 6420 6e6f 7420 7061 7261 6d73 2e68 6173  d not params.has
-00017970: 5f62 6174 6368 3a20 7061 7261 6d73 203d  _batch: params =
-00017980: 2070 6172 616d 732e 756e 7371 7565 657a   params.unsqueez
-00017990: 6528 5b5d 290a 2020 2020 6966 2070 6172  e([]).    if par
-000179a0: 616d 732e 6e5f 6469 6d20 3c3d 2031 2061  ams.n_dim <= 1 a
-000179b0: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
-000179c0: 735f 6368 616e 6e65 6c3a 2070 6172 616d  s_channel: param
-000179d0: 7320 3d20 7061 7261 6d73 2e75 6e73 7175  s = params.unsqu
-000179e0: 6565 7a65 287b 317d 290a 2020 2020 6966  eeze({1}).    if
-000179f0: 2070 6172 616d 732e 6e5f 6469 6d20 3d3d   params.n_dim ==
-00017a00: 2032 2061 6e64 206e 6f74 2070 6172 616d   2 and not param
-00017a10: 732e 6861 735f 6261 7463 683a 2070 6172  s.has_batch: par
-00017a20: 616d 732e 6261 7463 685f 6469 6d65 6e73  ams.batch_dimens
-00017a30: 696f 6e20 3d20 300a 2020 2020 6966 2070  ion = 0.    if p
-00017a40: 6172 616d 732e 6e5f 6469 6d20 3d3d 2032  arams.n_dim == 2
-00017a50: 2061 6e64 206e 6f74 2070 6172 616d 732e   and not params.
-00017a60: 6861 735f 6368 616e 6e65 6c3a 2070 6172  has_channel: par
-00017a70: 616d 732e 6368 616e 6e65 6c5f 6469 6d65  ams.channel_dime
-00017a80: 6e73 696f 6e20 3d20 310a 2020 2020 6176  nsion = 1.    av
-00017a90: 6f75 6368 2870 6172 616d 732e 6e5f 6469  ouch(params.n_di
-00017aa0: 6d20 3d3d 2032 2061 6e64 2070 6172 616d  m == 2 and param
-00017ab0: 732e 6861 735f 6261 7463 6820 616e 6420  s.has_batch and 
-00017ac0: 7061 7261 6d73 2e68 6173 5f63 6861 6e6e  params.has_chann
-00017ad0: 656c 2c20 0a20 2020 2020 2020 2020 2020  el, .           
-00017ae0: 6622 506c 6561 7365 2075 7365 2062 6174  f"Please use bat
-00017af0: 6f72 6368 2074 656e 736f 7220 6f66 2073  orch tensor of s
-00017b00: 697a 6520 285b 6e5f 6261 7463 685d 2c20  ize ([n_batch], 
-00017b10: 7b7b 367d 7d29 2066 6f72 2041 6666 696e  {{6}}) for Affin
-00017b20: 6520 7061 7261 6d65 7465 7273 2c20 696e  e parameters, in
-00017b30: 7374 6561 6420 6f66 207b 7061 7261 6d73  stead of {params
-00017b40: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-00017b50: 6e5f 6261 7463 6820 3d20 7061 7261 6d73  n_batch = params
-00017b60: 2e6e 5f62 6174 6368 0a20 2020 2062 2c20  .n_batch.    b, 
-00017b70: 632c 2064 2c20 782c 2079 2c20 7a20 3d20  c, d, x, y, z = 
-00017b80: 7061 7261 6d73 2e73 706c 6974 2829 0a20  params.split(). 
-00017b90: 2020 2061 203d 2062 742e 7371 7274 2828     a = bt.sqrt((
-00017ba0: 312d 622a 622d 632a 632d 642a 6429 2e63  1-b*b-c*c-d*d).c
-00017bb0: 6c61 6d70 2830 2929 0a20 2020 2052 3131  lamp(0)).    R11
-00017bc0: 203d 2061 2a61 2b62 2a62 2d63 2a63 2d64   = a*a+b*b-c*c-d
-00017bd0: 2a64 0a20 2020 2052 3132 203d 2032 2a62  *d.    R12 = 2*b
-00017be0: 2a63 2d32 2a61 2a64 0a20 2020 2052 3133  *c-2*a*d.    R13
-00017bf0: 203d 2032 2a62 2a64 2b32 2a61 2a63 0a20   = 2*b*d+2*a*c. 
-00017c00: 2020 2052 3231 203d 2032 2a62 2a63 2b32     R21 = 2*b*c+2
-00017c10: 2a61 2a64 0a20 2020 2052 3232 203d 2061  *a*d.    R22 = a
-00017c20: 2a61 2b63 2a63 2d62 2a62 2d64 2a64 0a20  *a+c*c-b*b-d*d. 
-00017c30: 2020 2052 3233 203d 2032 2a63 2a64 2d32     R23 = 2*c*d-2
-00017c40: 2a61 2a62 0a20 2020 2052 3331 203d 2032  *a*b.    R31 = 2
-00017c50: 2a62 2a64 2d32 2a61 2a63 0a20 2020 2052  *b*d-2*a*c.    R
-00017c60: 3332 203d 2032 2a63 2a64 2b32 2a61 2a62  32 = 2*c*d+2*a*b
-00017c70: 0a20 2020 2052 3333 203d 2061 2a61 2b64  .    R33 = a*a+d
-00017c80: 2a64 2d63 2a63 2d62 2a62 0a20 2020 2072  *d-c*c-b*b.    r
-00017c90: 6574 7572 6e20 6274 2e63 6174 280a 2020  eturn bt.cat(.  
-00017ca0: 2020 2020 2020 6274 2e63 6174 2828 5231        bt.cat((R1
-00017cb0: 312c 2052 3132 2c20 5231 332c 2078 2c20  1, R12, R13, x, 
-00017cc0: 5232 312c 2052 3232 2c20 5232 332c 2079  R21, R22, R23, y
-00017cd0: 2c20 5233 312c 2052 3332 2c20 5233 332c  , R31, R32, R33,
-00017ce0: 207a 292c 2031 292e 7669 6577 285b 6e5f   z), 1).view([n_
-00017cf0: 6261 7463 685d 2c20 332c 2034 292c 0a20  batch], 3, 4),. 
-00017d00: 2020 2020 2020 2062 742e 6f6e 655f 686f         bt.one_ho
-00017d10: 7428 2d31 2c20 3429 2e6d 756c 7469 706c  t(-1, 4).multipl
-00017d20: 7928 6e5f 6261 7463 682c 205b 5d29 2e76  y(n_batch, []).v
-00017d30: 6965 7728 5b6e 5f62 6174 6368 5d2c 2031  iew([n_batch], 1
-00017d40: 2c20 3429 2c20 310a 2020 2020 290a 0a64  , 4), 1.    )..d
-00017d50: 6566 204d 6174 7269 7832 5175 6174 6572  ef Matrix2Quater
-00017d60: 6e73 2870 6172 616d 7329 3a0a 2020 2020  ns(params):.    
-00017d70: 2222 220a 2020 2020 2020 2020 4d61 7472  """.        Matr
-00017d80: 6978 3a20 285b 6e5f 6261 7463 685d 2c20  ix: ([n_batch], 
-00017d90: 342c 2034 290a 2020 2020 2020 2020 5175  4, 4).        Qu
-00017da0: 6174 6572 6e3a 2071 622c 2071 632c 2071  atern: qb, qc, q
-00017db0: 642c 2070 782c 2070 792c 2070 7a20 696e  d, px, py, pz in
-00017dc0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-00017dd0: 5d2c 207b 367d 290a 2020 2020 2222 220a  ], {6}).    """.
-00017de0: 2020 2020 7061 7261 6d73 203d 2062 6174      params = bat
-00017df0: 6f72 6368 5f74 656e 736f 7228 7061 7261  orch_tensor(para
-00017e00: 6d73 290a 2020 2020 6966 2070 6172 616d  ms).    if param
-00017e10: 732e 6e5f 6469 6d20 3c3d 2032 2061 6e64  s.n_dim <= 2 and
-00017e20: 206e 6f74 2070 6172 616d 732e 6861 735f   not params.has_
-00017e30: 6261 7463 683a 2070 6172 616d 7320 3d20  batch: params = 
-00017e40: 7061 7261 6d73 2e75 6e73 7175 6565 7a65  params.unsqueeze
-00017e50: 285b 5d29 0a20 2020 2069 6620 7061 7261  ([]).    if para
-00017e60: 6d73 2e6e 5f64 696d 203d 3d20 3320 616e  ms.n_dim == 3 an
-00017e70: 6420 6e6f 7420 7061 7261 6d73 2e68 6173  d not params.has
-00017e80: 5f62 6174 6368 3a20 7061 7261 6d73 2e62  _batch: params.b
-00017e90: 6174 6368 5f64 696d 656e 7369 6f6e 203d  atch_dimension =
-00017ea0: 2030 0a20 2020 2069 6620 7061 7261 6d73   0.    if params
-00017eb0: 2e6e 5f64 696d 203d 3d20 3320 616e 6420  .n_dim == 3 and 
-00017ec0: 7061 7261 6d73 2e68 6173 5f63 6861 6e6e  params.has_chann
-00017ed0: 656c 3a20 7061 7261 6d73 2e63 6861 6e6e  el: params.chann
-00017ee0: 656c 5f64 696d 656e 7369 6f6e 203d 204e  el_dimension = N
-00017ef0: 6f6e 650a 2020 2020 6176 6f75 6368 2870  one.    avouch(p
-00017f00: 6172 616d 732e 6e5f 6469 6d20 3d3d 2033  arams.n_dim == 3
-00017f10: 2061 6e64 2070 6172 616d 732e 6861 735f   and params.has_
-00017f20: 6261 7463 6820 616e 6420 6e6f 7420 7061  batch and not pa
-00017f30: 7261 6d73 2e68 6173 5f63 6861 6e6e 656c  rams.has_channel
-00017f40: 2c20 0a20 2020 2020 2020 2020 2020 6622  , .           f"
-00017f50: 506c 6561 7365 2075 7365 2062 6174 6f72  Please use bator
-00017f60: 6368 2074 656e 736f 7220 6f66 2073 697a  ch tensor of siz
-00017f70: 6520 285b 6e5f 6261 7463 685d 2c20 342c  e ([n_batch], 4,
-00017f80: 2034 2920 666f 7220 4166 6669 6e65 206d   4) for Affine m
-00017f90: 6174 7269 782c 2069 6e73 7465 6164 206f  atrix, instead o
-00017fa0: 6620 7b70 6172 616d 732e 7368 6170 657d  f {params.shape}
-00017fb0: 2e20 2229 0a20 2020 206e 5f62 6174 6368  . ").    n_batch
-00017fc0: 203d 2070 6172 616d 732e 6e5f 6261 7463   = params.n_batc
-00017fd0: 680a 2020 2020 782c 2079 2c20 7a20 3d20  h.    x, y, z = 
-00017fe0: 7061 7261 6d73 5b2e 2e2e 2c20 3a33 2c20  params[..., :3, 
-00017ff0: 2d31 5d2e 6368 616e 6e65 6c5f 6469 6d5f  -1].channel_dim_
-00018000: 2831 292e 7370 6c69 7428 312c 2031 290a  (1).split(1, 1).
-00018010: 2020 2020 6132 203d 2028 6274 2e64 6961      a2 = (bt.dia
-00018020: 6728 7061 7261 6d73 292e 7375 6d28 292e  g(params).sum().
-00018030: 756e 7371 7565 657a 6528 7b7d 2920 2b20  unsqueeze({}) + 
-00018040: 3129 202f 2034 0a20 2020 2061 203d 2062  1) / 4.    a = b
-00018050: 742e 7371 7274 2861 3229 0a20 2020 2062  t.sqrt(a2).    b
-00018060: 3220 3d20 6132 202d 2028 7061 7261 6d73  2 = a2 - (params
-00018070: 5b2e 2e2e 2c20 312c 2031 5d20 2b20 7061  [..., 1, 1] + pa
-00018080: 7261 6d73 5b2e 2e2e 2c20 322c 2032 5d29  rams[..., 2, 2])
-00018090: 202f 2032 0a20 2020 2063 3220 3d20 6132   / 2.    c2 = a2
-000180a0: 202d 2028 7061 7261 6d73 5b2e 2e2e 2c20   - (params[..., 
-000180b0: 322c 2032 5d20 2b20 7061 7261 6d73 5b2e  2, 2] + params[.
-000180c0: 2e2e 2c20 302c 2030 5d29 202f 2032 0a20  .., 0, 0]) / 2. 
-000180d0: 2020 2064 3220 3d20 6132 202d 2028 7061     d2 = a2 - (pa
-000180e0: 7261 6d73 5b2e 2e2e 2c20 302c 2030 5d20  rams[..., 0, 0] 
-000180f0: 2b20 7061 7261 6d73 5b2e 2e2e 2c20 312c  + params[..., 1,
-00018100: 2031 5d29 202f 2032 0a20 2020 2044 203d   1]) / 2.    D =
-00018110: 2070 6172 616d 7320 2d20 7061 7261 6d73   params - params
-00018120: 2e54 0a20 2020 2062 203d 2062 742e 7369  .T.    b = bt.si
-00018130: 676e 2844 5b2e 2e2e 2c20 322c 2031 5d29  gn(D[..., 2, 1])
-00018140: 202a 2062 742e 7371 7274 2862 3229 0a20   * bt.sqrt(b2). 
-00018150: 2020 2063 203d 202d 2062 742e 7369 676e     c = - bt.sign
-00018160: 2844 5b2e 2e2e 2c20 322c 2030 5d29 202a  (D[..., 2, 0]) *
-00018170: 2062 742e 7371 7274 2863 3229 0a20 2020   bt.sqrt(c2).   
-00018180: 2064 203d 2062 742e 7369 676e 2844 5b2e   d = bt.sign(D[.
-00018190: 2e2e 2c20 312c 2030 5d29 202a 2062 742e  .., 1, 0]) * bt.
-000181a0: 7371 7274 2864 3229 0a20 2020 2072 6574  sqrt(d2).    ret
-000181b0: 7572 6e20 6274 2e63 6174 2862 2c20 632c  urn bt.cat(b, c,
-000181c0: 2064 2c20 782c 2079 2c20 7a2c 207b 7d29   d, x, y, z, {})
-000181d0: 0a                                       .
+00012540: 7265 7320 2a20 696e 5f66 6561 7475 7265  res * in_feature
+00012550: 730a 2020 2020 2020 2020 2020 2020 6c61  s.            la
+00012560: 7965 725f 6269 6173 203d 2077 6569 6768  yer_bias = weigh
+00012570: 7473 5b2e 2e2e 2c20 703a 702b 6f75 745f  ts[..., p:p+out_
+00012580: 6665 6174 7572 6573 5d2e 7669 6577 285b  features].view([
+00012590: 7365 6c66 2e6e 5f62 6174 6368 5d2c 206f  self.n_batch], o
+000125a0: 7574 5f66 6561 7475 7265 7329 0a20 2020  ut_features).   
+000125b0: 2020 2020 2020 2020 2070 202b 3d20 6f75           p += ou
+000125c0: 745f 6665 6174 7572 6573 0a20 2020 2020  t_features.     
+000125d0: 2020 2020 2020 2073 656c 662e 6c61 7965         self.laye
+000125e0: 7273 2e61 7070 656e 6428 286c 6179 6572  rs.append((layer
+000125f0: 5f77 6569 6768 7473 2c20 6c61 7965 725f  _weights, layer_
+00012600: 6269 6173 2929 0a20 2020 2020 2020 2073  bias)).        s
+00012610: 656c 662e 6163 7469 7665 5f66 756e 6374  elf.active_funct
+00012620: 696f 6e20 3d20 6163 7469 7665 5f66 756e  ion = active_fun
+00012630: 6374 696f 6e0a 2020 2020 2020 2020 6966  ction.        if
+00012640: 2073 656c 662e 6163 7469 7665 5f66 756e   self.active_fun
+00012650: 6374 696f 6e20 6973 204e 6f6e 653a 2073  ction is None: s
+00012660: 656c 662e 6163 7469 7665 5f66 756e 6374  elf.active_funct
+00012670: 696f 6e20 3d20 6274 2e6e 6e2e 5265 4c55  ion = bt.nn.ReLU
+00012680: 0a20 2020 200a 2020 2020 4070 726f 7065  .    .    @prope
+00012690: 7274 790a 2020 2020 6465 6620 6e5f 7765  rty.    def n_we
+000126a0: 6967 6874 5f6c 656e 6774 6828 7365 6c66  ight_length(self
+000126b0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000126c0: 6e20 7365 6c66 2e6e 5f64 696d 202a 2028  n self.n_dim * (
+000126d0: 7365 6c66 2e68 6964 6465 6e5f 6c61 7965  self.hidden_laye
+000126e0: 7273 5b30 5d20 2b20 7365 6c66 2e68 6964  rs[0] + self.hid
+000126f0: 6465 6e5f 6c61 7965 7273 5b2d 315d 202b  den_layers[-1] +
+00012700: 2031 2920 2b20 7375 6d28 7365 6c66 2e68   1) + sum(self.h
+00012710: 6964 6465 6e5f 6c61 7965 7273 2920 2b20  idden_layers) + 
+00012720: 7375 6d28 7820 2a20 7920 666f 7220 782c  sum(x * y for x,
+00012730: 2079 2069 6e20 7a69 7028 7365 6c66 2e68   y in zip(self.h
+00012740: 6964 6465 6e5f 6c61 7965 7273 5b3a 2d31  idden_layers[:-1
+00012750: 5d2c 2073 656c 662e 6869 6464 656e 5f6c  ], self.hidden_l
+00012760: 6179 6572 735b 313a 5d29 290a 2020 2020  ayers[1:])).    
+00012770: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
+00012780: 5f28 7365 6c66 2c20 5829 3a0a 2020 2020  _(self, X):.    
+00012790: 2020 2020 5820 3d20 7375 7065 7228 292e      X = super().
+000127a0: 5f5f 6361 6c6c 5f5f 2858 290a 2020 2020  __call__(X).    
+000127b0: 2020 2020 6966 2058 2e6e 5f73 7061 6365      if X.n_space
+000127c0: 203d 3d20 303a 2058 203d 2058 2e75 6e73   == 0: X = X.uns
+000127d0: 7175 6565 7a65 282d 3129 0a20 2020 2020  queeze(-1).     
+000127e0: 2020 2059 203d 2058 2e66 6c61 7474 656e     Y = X.flatten
+000127f0: 2829 2e63 6861 6e6e 656c 5f64 696d 5f28  ().channel_dim_(
+00012800: 4e6f 6e65 290a 2020 2020 2020 2020 666f  None).        fo
+00012810: 7220 692c 2028 7765 6967 6874 732c 2062  r i, (weights, b
+00012820: 6961 7329 2069 6e20 656e 756d 6572 6174  ias) in enumerat
+00012830: 6528 7365 6c66 2e6c 6179 6572 7329 3a0a  e(self.layers):.
+00012840: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
+00012850: 7765 6967 6874 7320 4020 590a 2020 2020  weights @ Y.    
+00012860: 2020 2020 2020 2020 6966 2069 203c 206c          if i < l
+00012870: 656e 2873 656c 662e 6c61 7965 7273 2920  en(self.layers) 
+00012880: 2d20 313a 2059 203d 2073 656c 662e 6163  - 1: Y = self.ac
+00012890: 7469 7665 5f66 756e 6374 696f 6e28 2928  tive_function()(
+000128a0: 5920 2b20 6269 6173 2e75 6e73 7175 6565  Y + bias.unsquee
+000128b0: 7a65 282d 3129 290a 2020 2020 2020 2020  ze(-1)).        
+000128c0: 2020 2020 656c 7365 3a20 5920 2b3d 2073      else: Y += s
+000128d0: 656c 662e 7472 616e 735f 7374 7265 7463  elf.trans_stretc
+000128e0: 6820 2a20 6269 6173 2e75 6e73 7175 6565  h * bias.unsquee
+000128f0: 7a65 282d 3129 0a20 2020 2020 2020 2072  ze(-1).        r
+00012900: 6574 7572 6e20 5820 2b20 592e 7669 6577  eturn X + Y.view
+00012910: 5f61 7328 5829 2e63 6861 6e6e 656c 5f64  _as(X).channel_d
+00012920: 696d 656e 7369 6f6e 5f28 3129 0a0a 4061  imension_(1)..@a
+00012930: 6c69 6173 2822 7265 7361 6d70 6c65 2229  lias("resample")
+00012940: 0a64 6566 2069 6e74 6572 706f 6c61 7469  .def interpolati
+00012950: 6f6e 280a 2020 2020 2020 2020 696d 6167  on(.        imag
+00012960: 653a 2062 742e 5465 6e73 6f72 2c20 0a20  e: bt.Tensor, . 
+00012970: 2020 2020 2020 2074 7261 6e73 3a20 4361         trans: Ca
+00012980: 6c6c 6162 6c65 203d 204e 6f6e 652c 200a  llable = None, .
+00012990: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+000129a0: 7374 7220 3d20 274c 696e 6561 7227 2c20  str = 'Linear', 
+000129b0: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
+000129c0: 7370 6163 653a 2074 7570 6c65 203d 204e  space: tuple = N
+000129d0: 6f6e 652c 0a20 2020 2020 2020 2066 696c  one,.        fil
+000129e0: 6c3a 2028 7374 722c 2069 6e74 2c20 666c  l: (str, int, fl
+000129f0: 6f61 7429 203d 2030 2c0a 2020 2020 2020  oat) = 0,.      
+00012a00: 2020 6465 7269 7661 7469 7665 3a20 626f    derivative: bo
+00012a10: 6f6c 203d 2046 616c 7365 0a20 2020 2029  ol = False.    )
+00012a20: 3a0a 2020 2020 2727 270a 2020 2020 496e  :.    '''.    In
+00012a30: 7465 7270 6f6c 6174 6520 7573 696e 6720  terpolate using 
+00012a40: 6261 636b 7761 7264 2074 7261 6e73 666f  backward transfo
+00012a50: 726d 6174 696f 6e2e 0a20 2020 2069 2e65  rmation..    i.e
+00012a60: 2e20 436f 6d70 7574 6520 7468 6520 696d  . Compute the im
+00012a70: 6167 6520 4920 732e 742e 2074 7261 6e73  age I s.t. trans
+00012a80: 2878 2920 3d20 7920 666f 7220 7820 696e  (x) = y for x in
+00012a90: 2049 2061 6e64 2079 2069 6e20 696e 7075   I and y in inpu
+00012aa0: 7420 696d 6167 6520 7573 696e 6720 696e  t image using in
+00012ab0: 7465 7270 6f6c 6174 696f 6e20 6d65 7468  terpolation meth
+00012ac0: 6f64 3a0a 2020 2020 2020 2020 6d65 7468  od:.        meth
+00012ad0: 6f64 203d 204c 696e 6561 723a 2042 696c  od = Linear: Bil
+00012ae0: 696e 6561 7220 696e 7465 7270 6f6c 6174  inear interpolat
+00012af0: 696f 6e0a 2020 2020 2020 2020 6d65 7468  ion.        meth
+00012b00: 6f64 203d 204e 6561 7265 7374 205b 4e4f  od = Nearest [NO
+00012b10: 2047 5241 4449 454e 5421 2121 5d3a 204e   GRADIENT!!!]: N
+00012b20: 6561 7265 7374 2069 6e74 6572 706f 6c61  earest interpola
+00012b30: 7469 6f6e 0a0a 2020 2020 5061 7261 6d73  tion..    Params
+00012b40: 3a0a 2020 2020 2020 2020 696d 6167 6520  :.        image 
+00012b50: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
+00012b60: 2074 6172 6765 7420 696d 6167 652e 0a20   target image.. 
+00012b70: 2020 2020 2020 2020 2020 2073 697a 653a             size:
+00012b80: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
+00012b90: 6e61 6c5d 2c20 7b6e 5f63 6861 6e6e 656c  nal], {n_channel
+00012ba0: 3a6f 7074 696f 6e61 6c7d 2c20 6d40 312c  :optional}, m@1,
+00012bb0: 206d 4032 2c20 2e2e 2e2c 206d 406e 5f64   m@2, ..., m@n_d
+00012bc0: 696d 290a 2020 2020 2020 2020 7472 616e  im).        tran
+00012bd0: 7320 5b46 756e 6374 696f 6e20 6f72 206d  s [Function or m
+00012be0: 6963 6f6d 7075 7469 6e67 2e53 7061 7469  icomputing.Spati
+00012bf0: 616c 5472 616e 7366 6f72 6d61 7469 6f6e  alTransformation
+00012c00: 5d3a 2054 7261 6e73 666f 726d 6174 696f  ]: Transformatio
+00012c10: 6e20 6675 6e63 7469 6f6e 2c20 6d61 7070  n function, mapp
+00012c20: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00012c30: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+00012c40: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
+00012c50: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
+00012c60: 2e2c 206e 406e 5f64 696d 2920 746f 2028  ., n@n_dim) to (
+00012c70: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
+00012c80: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
+00012c90: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
+00012ca0: 2020 2020 6d65 7468 6f64 205b 7374 723a      method [str:
+00012cb0: 206c 696e 6561 727c 6e65 6172 6573 745d   linear|nearest]
+00012cc0: 3a20 5468 6520 696e 7465 7270 6f6c 6174  : The interpolat
+00012cd0: 696f 6e20 6d65 7468 6f64 2e20 0a20 2020  ion method. .   
+00012ce0: 2020 2020 2074 6172 6765 745f 7370 6163       target_spac
+00012cf0: 6520 5b74 7570 6c65 206f 7220 6274 2e54  e [tuple or bt.T
+00012d00: 656e 736f 725d 3a0a 2020 2020 2020 2020  ensor]:.        
+00012d10: 2020 2020 5369 7a65 2028 7475 706c 6529      Size (tuple)
+00012d20: 206f 6620 6120 7461 7267 6574 2052 4f49   of a target ROI
+00012d30: 2061 7420 7468 6520 6365 6e74 6572 206f   at the center o
+00012d40: 6620 696d 6167 652e 200a 2020 2020 2020  f image. .      
+00012d50: 2020 2020 2020 4f52 2054 7261 6e73 666f        OR Transfo
+00012d60: 726d 6564 2063 6f6f 7264 696e 6174 6520  rmed coordinate 
+00012d70: 7370 6163 6520 2862 742e 5465 6e73 6f72  space (bt.Tensor
+00012d80: 2920 6f66 2074 6865 206f 7574 7075 7420  ) of the output 
+00012d90: 696d 6167 652e 200a 2020 2020 2020 2020  image. .        
+00012da0: 2020 2020 7369 7a65 3a20 6c65 6e67 7468      size: length
+00012db0: 286e 5f64 696d 2920 6f72 2028 5b6e 5f62  (n_dim) or ([n_b
+00012dc0: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
+00012dd0: 7b6e 5f64 696d 3a6f 7074 696f 6e61 6c7d  {n_dim:optional}
+00012de0: 2c20 7369 7a65 4031 2c20 7369 7a65 4032  , size@1, size@2
+00012df0: 2c20 2e2e 2e2c 2073 697a 6540 7229 0a20  , ..., size@r). 
+00012e00: 2020 2020 2020 2066 696c 6c20 5b73 7472         fill [str
+00012e10: 3a20 6e65 6172 6573 747c 6261 636b 6772  : nearest|backgr
+00012e20: 6f75 6e64 206f 7220 696e 7420 6f72 2066  ound or int or f
+00012e30: 6c6f 6174 286e 756d 6265 7229 5d3a 2049  loat(number)]: I
+00012e40: 6e64 6963 6174 6520 7468 6520 7761 7920  ndicate the way 
+00012e50: 746f 2066 696c 6c20 6261 636b 6772 6f75  to fill backgrou
+00012e60: 6e64 206f 7574 7369 6465 2060 5375 7272  nd outside `Surr
+00012e70: 6f75 6e64 696e 6760 2e20 0a20 2020 2020  ounding`. .     
+00012e80: 2020 2064 6572 6976 6174 6976 6520 5b62     derivative [b
+00012e90: 6f6f 6c5d 3a20 5768 6574 6865 7220 746f  ool]: Whether to
+00012ea0: 2072 6574 7572 6e20 7468 6520 6772 6164   return the grad
+00012eb0: 6965 6e74 2e20 4f6e 6520 6361 6e20 6f6d  ient. One can om
+00012ec0: 6974 2069 7420 7768 656e 2075 7369 6e67  it it when using
+00012ed0: 2074 6f72 6368 2e61 7574 6f67 7261 642e   torch.autograd.
+00012ee0: 0a0a 2020 2020 2020 2020 6f75 7470 7574  ..        output
+00012ef0: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
+00012f00: 6520 7472 616e 7366 6f72 6d65 6420 696d  e transformed im
+00012f10: 6167 652e 0a20 2020 2020 2020 2020 2020  age..           
+00012f20: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+00012f30: 5d2c 207b 6e5f 6368 616e 6e65 6c3a 6f70  ], {n_channel:op
+00012f40: 7469 6f6e 616c 7d2c 206d 4031 2c20 6d40  tional}, m@1, m@
+00012f50: 322c 202e 2e2e 2c20 6d40 6e5f 6469 6d29  2, ..., m@n_dim)
+00012f60: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
+00012f70: 7768 656e 2060 7461 7267 6574 5f73 7061  when `target_spa
+00012f80: 6365 6020 6973 2064 6566 696e 6564 2062  ce` is defined b
+00012f90: 7920 7465 6e73 6f72 2e20 0a20 2020 2020  y tensor. .     
+00012fa0: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
+00012fb0: 5f62 6174 6368 5d2c 2073 697a 6540 312c  _batch], size@1,
+00012fc0: 2073 697a 6540 322c 202e 2e2e 2c20 7369   size@2, ..., si
+00012fd0: 7a65 406e 5f64 696d 290a 2020 2020 2020  ze@n_dim).      
+00012fe0: 2020 2020 2020 6f72 2074 6865 2064 6572        or the der
+00012ff0: 6976 6174 6976 6520 666f 7220 7468 6520  ivative for the 
+00013000: 696e 7465 7270 6f6c 6174 696f 6e2e 2028  interpolation. (
+00013010: 6966 2060 6465 7269 7661 7469 7665 203d  if `derivative =
+00013020: 2054 7275 6560 290a 2020 2020 2020 2020   True`).        
+00013030: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+00013040: 7463 685d 2c20 7b6e 5f64 696d 7d2c 2073  tch], {n_dim}, s
+00013050: 697a 6540 312c 2073 697a 6540 322c 202e  ize@1, size@2, .
+00013060: 2e2e 2c20 7369 7a65 406e 5f64 696d 290a  .., size@n_dim).
+00013070: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
+00013080: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00013090: 2020 3e3e 3e20 496d 6167 6520 3d20 6274    >>> Image = bt
+000130a0: 2e72 616e 6428 332c 2031 3030 2c20 3132  .rand(3, 100, 12
+000130b0: 302c 2038 3029 0a20 2020 203e 3e3e 2041  0, 80).    >>> A
+000130c0: 4d20 3d20 6274 2e72 616e 6428 342c 2034  M = bt.rand(4, 4
+000130d0: 290a 2020 2020 3e3e 3e20 414d 5b33 2c20  ).    >>> AM[3, 
+000130e0: 3a5d 203d 2062 742e 6f6e 655f 686f 7428  :] = bt.one_hot(
+000130f0: 2d31 2c20 3429 0a20 2020 203e 3e3e 2069  -1, 4).    >>> i
+00013100: 6e74 6572 706f 6c61 7469 6f6e 2849 6d61  nterpolation(Ima
+00013110: 6765 2c20 4166 6669 6e65 2841 4d29 2c20  ge, Affine(AM), 
+00013120: 6d65 7468 6f64 3d27 4c69 6e65 6172 2729  method='Linear')
+00013130: 0a20 2020 2027 2727 0a20 2020 2069 6620  .    '''.    if 
+00013140: 7472 616e 7320 6973 206e 6f74 204e 6f6e  trans is not Non
+00013150: 6520 616e 6420 6e6f 7420 7472 616e 732e  e and not trans.
+00013160: 6261 636b 7761 7264 3a0a 2020 2020 2020  backward:.      
+00013170: 2020 6966 2068 6173 6174 7472 2874 7261    if hasattr(tra
+00013180: 6e73 2c20 2769 6e76 2729 3a20 7472 616e  ns, 'inv'): tran
+00013190: 7320 3d20 7472 616e 732e 696e 7628 292e  s = trans.inv().
+000131a0: 6661 6b65 5f69 6e76 2829 0a20 2020 2020  fake_inv().     
+000131b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000131c0: 2020 2020 2070 7269 6e74 2822 5761 726e       print("Warn
+000131d0: 696e 673a 2046 6f72 7761 7264 2074 7261  ing: Forward tra
+000131e0: 6e73 666f 726d 6174 696f 6e20 666f 756e  nsformation foun
+000131f0: 6420 696e 206d 6574 686f 6420 6069 6e74  d in method `int
+00013200: 6572 706f 6c61 7469 6f6e 602e 2055 7369  erpolation`. Usi
+00013210: 6e67 2060 696e 7465 7270 6f6c 6174 696f  ng `interpolatio
+00013220: 6e5f 666f 7277 6172 6460 2069 6e73 7465  n_forward` inste
+00013230: 6164 2e20 2229 0a20 2020 2020 2020 2020  ad. ").         
+00013240: 2020 2072 6574 7572 6e20 696e 7465 7270     return interp
+00013250: 6f6c 6174 696f 6e5f 666f 7277 6172 6428  olation_forward(
+00013260: 696d 6167 652c 2074 7261 6e73 2c20 6d65  image, trans, me
+00013270: 7468 6f64 203d 206d 6574 686f 642c 2074  thod = method, t
+00013280: 6172 6765 745f 7370 6163 6520 3d20 7461  arget_space = ta
+00013290: 7267 6574 5f73 7061 6365 2c20 6669 6c6c  rget_space, fill
+000132a0: 203d 2066 696c 6c29 0a20 2020 2069 6d61   = fill).    ima
+000132b0: 6765 203d 2062 6174 6f72 6368 5f74 656e  ge = batorch_ten
+000132c0: 736f 7228 696d 6167 6529 0a20 2020 2073  sor(image).    s
+000132d0: 6861 7065 5f6f 7574 203d 2069 6d61 6765  hape_out = image
+000132e0: 2e73 6861 7065 0a20 2020 2069 6620 7472  .shape.    if tr
+000132f0: 616e 7320 6973 204e 6f6e 6520 6f72 2074  ans is None or t
+00013300: 7261 6e73 2e6e 5f64 696d 2069 7320 4e6f  rans.n_dim is No
+00013310: 6e65 3a0a 2020 2020 2020 2020 6966 206e  ne:.        if n
+00013320: 6f74 2069 6d61 6765 2e68 6173 5f62 6174  ot image.has_bat
+00013330: 6368 3a20 696d 6167 652e 756e 7371 7565  ch: image.unsque
+00013340: 657a 655f 285b 5d29 0a20 2020 2020 2020  eze_([]).       
+00013350: 2069 6620 6e6f 7420 696d 6167 652e 6861   if not image.ha
+00013360: 735f 6368 616e 6e65 6c3a 2069 6d61 6765  s_channel: image
+00013370: 2e73 7461 6e64 6172 645f 2829 2e75 6e73  .standard_().uns
+00013380: 7175 6565 7a65 5f28 7b31 7d29 0a20 2020  queeze_({1}).   
+00013390: 2020 2020 206e 5f64 696d 203d 2069 6d61       n_dim = ima
+000133a0: 6765 2e6e 5f73 7061 6365 2023 2047 6574  ge.n_space # Get
+000133b0: 2074 6865 2073 7061 7469 616c 2072 616e   the spatial ran
+000133c0: 6b2e 0a20 2020 2065 6c73 653a 0a20 2020  k..    else:.   
+000133d0: 2020 2020 206e 5f64 696d 203d 2074 7261       n_dim = tra
+000133e0: 6e73 2e6e 5f64 696d 0a20 2020 2020 2020  ns.n_dim.       
+000133f0: 2069 6620 696d 6167 652e 6e5f 6469 6d20   if image.n_dim 
+00013400: 3d3d 206e 5f64 696d 3a0a 2020 2020 2020  == n_dim:.      
+00013410: 2020 2020 2020 6966 2069 6d61 6765 2e68        if image.h
+00013420: 6173 5f73 7065 6369 616c 3a0a 2020 2020  as_special:.    
+00013430: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00013440: 7428 6622 5761 726e 696e 673a 2027 696e  t(f"Warning: 'in
+00013450: 7465 7270 6f6c 6174 696f 6e27 2074 7279  terpolation' try
+00013460: 696e 6720 746f 2074 7261 6e73 666f 726d  ing to transform
+00013470: 207b 696d 6167 652e 6e5f 7370 6163 657d   {image.n_space}
+00013480: 2b7b 696d 6167 652e 6e5f 7370 6563 6961  +{image.n_specia
+00013490: 6c7d 4420 696d 6167 6520 2877 6974 6820  l}D image (with 
+000134a0: 6261 7463 6820 6f72 2063 6861 6e6e 656c  batch or channel
+000134b0: 2920 6279 207b 6e5f 6469 6d7d 4420 7472  ) by {n_dim}D tr
+000134c0: 616e 7366 6f72 6d61 7469 6f6e 2c20 6175  ansformation, au
+000134d0: 746f 2d72 656d 6f76 696e 6720 7370 6563  to-removing spec
+000134e0: 6961 6c20 6469 6d65 6e73 696f 6e73 2e22  ial dimensions."
+000134f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013500: 2020 696d 6167 652e 7265 6d6f 7665 5f73    image.remove_s
+00013510: 7065 6369 616c 5f28 290a 2020 2020 2020  pecial_().      
+00013520: 2020 2020 2020 696d 6167 652e 756e 7371        image.unsq
+00013530: 7565 657a 655f 285b 5d29 2e75 6e73 7175  ueeze_([]).unsqu
+00013540: 6565 7a65 5f28 7b7d 290a 2020 2020 2020  eeze_({}).      
+00013550: 2020 656c 6966 2069 6d61 6765 2e6e 5f64    elif image.n_d
+00013560: 696d 203d 3d20 6e5f 6469 6d20 2b20 313a  im == n_dim + 1:
+00013570: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013580: 6e6f 7420 696d 6167 652e 6861 735f 6261  not image.has_ba
+00013590: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
+000135a0: 2020 2020 2069 6620 696d 6167 652e 6861       if image.ha
+000135b0: 735f 6368 616e 6e65 6c3a 2069 6d61 6765  s_channel: image
+000135c0: 2e75 6e73 7175 6565 7a65 5f28 5b5d 290a  .unsqueeze_([]).
+000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135e0: 656c 7365 3a20 696d 6167 652e 7769 7468  else: image.with
+000135f0: 5f62 6174 6368 6469 6d28 3029 2e75 6e73  _batchdim(0).uns
+00013600: 7175 6565 7a65 5f28 7b31 7d29 0a20 2020  queeze_({1}).   
+00013610: 2020 2020 2020 2020 2065 6c69 6620 6e6f           elif no
+00013620: 7420 696d 6167 652e 6861 735f 6368 616e  t image.has_chan
+00013630: 6e65 6c3a 2069 6d61 6765 2e75 6e73 7175  nel: image.unsqu
+00013640: 6565 7a65 5f28 7b7d 290a 2020 2020 2020  eeze_({}).      
+00013650: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00013660: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00013670: 7428 6622 5761 726e 696e 673a 2027 696e  t(f"Warning: 'in
+00013680: 7465 7270 6f6c 6174 696f 6e27 2074 7279  terpolation' try
+00013690: 696e 6720 746f 2074 7261 6e73 666f 726d  ing to transform
+000136a0: 207b 696d 6167 652e 6e5f 7370 6163 657d   {image.n_space}
+000136b0: 2b7b 696d 6167 652e 6e5f 7370 6563 6961  +{image.n_specia
+000136c0: 6c7d 4420 696d 6167 6520 2877 6974 6820  l}D image (with 
+000136d0: 6261 7463 6820 6f72 2063 6861 6e6e 656c  batch or channel
+000136e0: 2920 6279 207b 6e5f 6469 6d7d 4420 7472  ) by {n_dim}D tr
+000136f0: 616e 7366 6f72 6d61 7469 6f6e 2c20 6175  ansformation, au
+00013700: 746f 2d72 656d 6f76 696e 6720 7468 6520  to-removing the 
+00013710: 6368 616e 6e65 6c20 6469 6d65 6e73 696f  channel dimensio
+00013720: 6e73 2e22 290a 2020 2020 2020 2020 2020  ns.").          
+00013730: 2020 2020 2020 696d 6167 652e 7769 7468        image.with
+00013740: 5f63 6861 6e6e 656c 6469 6d28 4e6f 6e65  _channeldim(None
+00013750: 292e 756e 7371 7565 657a 655f 287b 7d29  ).unsqueeze_({})
+00013760: 0a20 2020 2020 2020 2065 6c69 6620 696d  .        elif im
+00013770: 6167 652e 6e5f 6469 6d20 3d3d 206e 5f64  age.n_dim == n_d
+00013780: 696d 202b 2032 3a0a 2020 2020 2020 2020  im + 2:.        
+00013790: 2020 2020 2320 5f63 6861 6e6e 616c 2f62      # _channal/b
+000137a0: 6174 6368 2064 696d 656e 7369 6f6e 7320  atch dimensions 
+000137b0: 7573 6564 2068 6572 6520 6173 2074 6865  used here as the
+000137c0: 7920 6172 6520 6e5f 6469 6d20 7768 656e  y are n_dim when
+000137d0: 206e 6f74 2065 7869 7374 6564 2e20 0a20   not existed. . 
+000137e0: 2020 2020 2020 2020 2020 2069 6620 696d             if im
+000137f0: 6167 652e 6e5f 7370 6563 6961 6c20 3d3d  age.n_special ==
+00013800: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00013810: 2020 2020 7072 696e 7428 6622 5761 726e      print(f"Warn
+00013820: 696e 673a 2027 696e 7465 7270 6f6c 6174  ing: 'interpolat
+00013830: 696f 6e27 2074 7279 696e 6720 746f 2074  ion' trying to t
+00013840: 7261 6e73 666f 726d 207b 696d 6167 652e  ransform {image.
+00013850: 6e5f 7370 6163 657d 2b31 4420 696d 6167  n_space}+1D imag
+00013860: 6520 2877 6974 6820 6261 7463 6820 6f72  e (with batch or
+00013870: 2063 6861 6e6e 656c 2920 6279 207b 6e5f   channel) by {n_
+00013880: 6469 6d7d 4420 7472 616e 7366 6f72 6d61  dim}D transforma
+00013890: 7469 6f6e 2c20 6175 746f 2d69 6e73 6572  tion, auto-inser
+000138a0: 7469 6e67 206e 6577 2073 7065 6369 616c  ting new special
+000138b0: 2064 696d 656e 7369 6f6e 2e22 290a 2020   dimension.").  
+000138c0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000138d0: 2069 6d61 6765 2e68 6173 5f62 6174 6368   image.has_batch
+000138e0: 3a20 696d 6167 652e 6261 7463 685f 6469  : image.batch_di
+000138f0: 6d65 6e73 696f 6e20 3d20 3020 6966 2069  mension = 0 if i
+00013900: 6d61 6765 2e5f 6368 616e 6e65 6c5f 6469  mage._channel_di
+00013910: 6d65 6e73 696f 6e20 3e20 3020 656c 7365  mension > 0 else
+00013920: 2031 0a20 2020 2020 2020 2020 2020 2069   1.            i
+00013930: 6620 6e6f 7420 696d 6167 652e 6861 735f  f not image.has_
+00013940: 6368 616e 6e65 6c3a 2069 6d61 6765 2e63  channel: image.c
+00013950: 6861 6e6e 656c 5f64 696d 656e 7369 6f6e  hannel_dimension
+00013960: 203d 2030 2069 6620 696d 6167 652e 5f62   = 0 if image._b
+00013970: 6174 6368 5f64 696d 656e 7369 6f6e 203e  atch_dimension >
+00013980: 2030 2065 6c73 6520 310a 2020 2020 6176   0 else 1.    av
+00013990: 6f75 6368 2869 6d61 6765 2e68 6173 5f62  ouch(image.has_b
+000139a0: 6174 6368 2061 6e64 2069 6d61 6765 2e68  atch and image.h
+000139b0: 6173 5f63 6861 6e6e 656c 2c20 2250 6c65  as_channel, "Ple
+000139c0: 6173 6520 7573 6520 6261 746f 7263 6820  ase use batorch 
+000139d0: 7465 6e73 6f72 206f 6620 7369 7a65 2022  tensor of size "
+000139e0: 202b 0a20 2020 2020 2020 2020 2020 2022   +.            "
+000139f0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f63  ([n_batch], {n_c
+00013a00: 6861 6e6e 656c 2f6e 5f66 6561 7475 7265  hannel/n_feature
+00013a10: 3a6f 7074 696f 6e61 6c7d 2c20 6d5f 312c  :optional}, m_1,
+00013a20: 206d 5f32 2c20 2e2e 2e2c 206d 5f72 2920   m_2, ..., m_r) 
+00013a30: 5b72 3d6e 5f64 696d 5d20 666f 7220 2220  [r=n_dim] for " 
+00013a40: 2b20 0a20 2020 2020 2020 2020 2020 2066  + .            f
+00013a50: 2264 6174 6120 746f 2062 6520 7370 6174  "data to be spat
+00013a60: 6961 6c6c 7920 696e 7465 7270 6f6c 6174  ially interpolat
+00013a70: 6564 2c20 696e 7374 6561 6420 6f66 207b  ed, instead of {
+00013a80: 696d 6167 652e 7368 6170 657d 2e20 2229  image.shape}. ")
+00013a90: 0a20 2020 2069 6620 7472 616e 7320 6973  .    if trans is
+00013aa0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00013ab0: 2020 2061 766f 7563 6828 696d 6167 652e     avouch(image.
+00013ac0: 6e5f 6261 7463 6820 3d3d 2031 206f 7220  n_batch == 1 or 
+00013ad0: 7472 616e 732e 6e5f 6261 7463 6820 696e  trans.n_batch in
+00013ae0: 2028 4e6f 6e65 2c20 696d 6167 652e 6e5f   (None, image.n_
+00013af0: 6261 7463 682c 2031 292c 2022 506c 6561  batch, 1), "Plea
+00013b00: 7365 2075 7365 2074 7261 6e73 666f 726d  se use transform
+00013b10: 6174 696f 6e20 6f66 2061 2022 202b 0a20  ation of a " +. 
+00013b20: 2020 2020 2020 2020 2020 2066 2273 7569             f"sui
+00013b30: 7461 626c 6520 6e5f 6261 7463 6820 746f  table n_batch to
+00013b40: 2074 7261 6e73 666f 726d 2069 6d61 6765   transform image
+00013b50: 2077 6974 6820 6261 7463 6873 697a 6520   with batchsize 
+00013b60: 7b69 6d61 6765 2e6e 5f62 6174 6368 7d2c  {image.n_batch},
+00013b70: 2063 7572 7265 6e74 6c79 207b 7472 616e   currently {tran
+00013b80: 732e 6e5f 6261 7463 687d 2e22 290a 0a20  s.n_batch}.").. 
+00013b90: 2020 206e 5f62 6174 6368 203d 2069 6d61     n_batch = ima
+00013ba0: 6765 2e6e 5f62 6174 6368 0a20 2020 2069  ge.n_batch.    i
+00013bb0: 6620 6e5f 6261 7463 6820 3d3d 2031 2061  f n_batch == 1 a
+00013bc0: 6e64 2074 7261 6e73 2069 7320 6e6f 7420  nd trans is not 
+00013bd0: 4e6f 6e65 2061 6e64 2074 7261 6e73 2e6e  None and trans.n
+00013be0: 5f62 6174 6368 2069 7320 6e6f 7420 4e6f  _batch is not No
+00013bf0: 6e65 2061 6e64 2074 7261 6e73 2e6e 5f62  ne and trans.n_b
+00013c00: 6174 6368 203e 2031 3a20 6e5f 6261 7463  atch > 1: n_batc
+00013c10: 6820 3d20 7472 616e 732e 6e5f 6261 7463  h = trans.n_batc
+00013c20: 680a 2020 2020 6966 206e 5f62 6174 6368  h.    if n_batch
+00013c30: 203d 3d20 3120 616e 6420 6973 696e 7374   == 1 and isinst
+00013c40: 616e 6365 2874 6172 6765 745f 7370 6163  ance(target_spac
+00013c50: 652c 2062 742e 5465 6e73 6f72 2920 616e  e, bt.Tensor) an
+00013c60: 6420 7461 7267 6574 5f73 7061 6365 2e68  d target_space.h
+00013c70: 6173 5f62 6174 6368 2061 6e64 2074 6172  as_batch and tar
+00013c80: 6765 745f 7370 6163 652e 6e5f 6261 7463  get_space.n_batc
+00013c90: 6820 3e20 313a 206e 5f62 6174 6368 203d  h > 1: n_batch =
+00013ca0: 2074 6172 6765 745f 7370 6163 652e 6e5f   target_space.n_
+00013cb0: 6261 7463 680a 2020 2020 6966 2069 6d61  batch.    if ima
+00013cc0: 6765 2e6e 5f62 6174 6368 203d 3d20 313a  ge.n_batch == 1:
+00013cd0: 2069 6d61 6765 203d 2069 6d61 6765 2e72   image = image.r
+00013ce0: 6570 6561 7465 6428 6e5f 6261 7463 682c  epeated(n_batch,
+00013cf0: 205b 5d29 0a20 2020 206e 5f66 6561 7475   []).    n_featu
+00013d00: 7265 203d 2069 6d61 6765 2e6e 5f63 6861  re = image.n_cha
+00013d10: 6e6e 656c 0a20 2020 2073 697a 6520 3d20  nnel.    size = 
+00013d20: 6274 2e63 6861 6e6e 656c 5f74 656e 736f  bt.channel_tenso
+00013d30: 7228 696d 6167 652e 7370 6163 6529 2e69  r(image.space).i
+00013d40: 6e74 2829 0a20 2020 2069 6620 6e5f 6261  nt().    if n_ba
+00013d50: 7463 6820 3e20 3120 616e 6420 6e6f 7420  tch > 1 and not 
+00013d60: 7368 6170 655f 6f75 742e 6861 735f 6261  shape_out.has_ba
+00013d70: 7463 683a 2073 6861 7065 5f6f 7574 203d  tch: shape_out =
+00013d80: 2062 742e 5369 7a65 285b 6e5f 6261 7463   bt.Size([n_batc
+00013d90: 685d 2920 2b20 7368 6170 655f 6f75 740a  h]) + shape_out.
+00013da0: 2020 2020 6966 2074 6172 6765 745f 7370      if target_sp
+00013db0: 6163 6520 6973 204e 6f6e 653a 0a20 2020  ace is None:.   
+00013dc0: 2020 2020 2073 6361 6c65 2c20 2a70 6169       scale, *pai
+00013dd0: 7273 203d 2074 7261 6e73 2e72 6573 6861  rs = trans.resha
+00013de0: 7065 0a20 2020 2020 2020 2069 6620 6c65  pe.        if le
+00013df0: 6e28 7363 616c 6529 203d 3d20 313a 2073  n(scale) == 1: s
+00013e00: 6361 6c65 202a 3d20 6e5f 6469 6d0a 2020  cale *= n_dim.  
+00013e10: 2020 2020 2020 7461 7267 6574 5f73 7061        target_spa
+00013e20: 6365 203d 205b 696e 7428 7820 2a20 7929  ce = [int(x * y)
+00013e30: 2066 6f72 2078 2c20 7920 696e 207a 6970   for x, y in zip
+00013e40: 2869 6d61 6765 2e73 7061 6365 2c20 7363  (image.space, sc
+00013e50: 616c 6529 5d0a 2020 2020 2020 2020 666f  ale)].        fo
+00013e60: 7220 702c 2071 2069 6e20 7061 6972 733a  r p, q in pairs:
+00013e70: 2074 6172 6765 745f 7370 6163 655b 705d   target_space[p]
+00013e80: 2c20 7461 7267 6574 5f73 7061 6365 5b71  , target_space[q
+00013e90: 5d20 3d20 7461 7267 6574 5f73 7061 6365  ] = target_space
+00013ea0: 5b71 5d2c 2074 6172 6765 745f 7370 6163  [q], target_spac
+00013eb0: 655b 705d 0a20 2020 2020 2020 2074 6172  e[p].        tar
+00013ec0: 6765 745f 7370 6163 6520 3d20 7475 706c  get_space = tupl
+00013ed0: 6528 7461 7267 6574 5f73 7061 6365 290a  e(target_space).
+00013ee0: 2020 2020 2020 2020 7368 6170 655f 6f75          shape_ou
+00013ef0: 7420 3d20 7368 6170 655f 6f75 742e 7265  t = shape_out.re
+00013f00: 7365 745f 7370 6163 6528 7461 7267 6574  set_space(target
+00013f10: 5f73 7061 6365 290a 2020 2020 6966 2069  _space).    if i
+00013f20: 7369 6e73 7461 6e63 6528 7461 7267 6574  sinstance(target
+00013f30: 5f73 7061 6365 2c20 7475 706c 6529 2061  _space, tuple) a
+00013f40: 6e64 206c 656e 2874 6172 6765 745f 7370  nd len(target_sp
+00013f50: 6163 6529 203d 3d20 6e5f 6469 6d3a 2070  ace) == n_dim: p
+00013f60: 6173 730a 2020 2020 656c 6966 2069 7369  ass.    elif isi
+00013f70: 6e73 7461 6e63 6528 7461 7267 6574 5f73  nstance(target_s
+00013f80: 7061 6365 2c20 6274 2e74 6f72 6368 2e54  pace, bt.torch.T
+00013f90: 656e 736f 7229 3a20 7061 7373 0a20 2020  ensor): pass.   
+00013fa0: 2065 6c73 653a 2072 6169 7365 2054 7970   else: raise Typ
+00013fb0: 6545 7272 6f72 2866 2257 726f 6e67 2074  eError(f"Wrong t
+00013fc0: 6172 6765 7420 7370 6163 6520 666f 7220  arget space for 
+00013fd0: 696e 7465 7270 6f6c 6174 696f 6e3a 207b  interpolation: {
+00013fe0: 7461 7267 6574 5f73 7061 6365 7d2e 2022  target_space}. "
+00013ff0: 290a 2020 2020 6966 2069 7369 6e73 7461  ).    if isinsta
+00014000: 6e63 6528 7461 7267 6574 5f73 7061 6365  nce(target_space
+00014010: 2c20 7475 706c 6529 3a20 0a20 2020 2020  , tuple): .     
+00014020: 2020 2023 2043 7265 6174 6520 6120 6772     # Create a gr
+00014030: 6964 2058 2077 6974 6820 7369 7a65 2028  id X with size (
+00014040: 7b6e 5f64 696d 7d2c 2073 697a 655f 312c  {n_dim}, size_1,
+00014050: 2073 697a 655f 322c 202e 2e2e 2c20 7369   size_2, ..., si
+00014060: 7a65 5f72 2920 5b72 3d6e 5f64 696d 5d2e  ze_r) [r=n_dim].
+00014070: 0a20 2020 2020 2020 2058 203d 2062 742e  .        X = bt.
+00014080: 696d 6167 655f 6772 6964 2874 6172 6765  image_grid(targe
+00014090: 745f 7370 6163 6529 2e66 6c6f 6174 2829  t_space).float()
+000140a0: 2023 202b 2062 742e 6368 616e 6e65 6c5f   # + bt.channel_
+000140b0: 7465 6e73 6f72 285b 666c 6f61 7428 612d  tensor([float(a-
+000140c0: 6229 2f32 2066 6f72 2061 2c20 6220 696e  b)/2 for a, b in
+000140d0: 207a 6970 2869 6d61 6765 2e73 7061 6365   zip(image.space
+000140e0: 2c20 7461 7267 6574 5f73 7061 6365 295d  , target_space)]
+000140f0: 290a 2020 2020 2020 2020 2320 436f 6d70  ).        # Comp
+00014100: 7574 6520 7468 6520 7472 616e 7366 6f72  ute the transfor
+00014110: 6d65 6420 636f 6f72 6469 6e61 7465 732e  med coordinates.
+00014120: 2059 3a20 285b 6e5f 6261 7463 685d 2c20   Y: ([n_batch], 
+00014130: 7b6e 5f64 696d 7d2c 2073 697a 655f 312c  {n_dim}, size_1,
+00014140: 2073 697a 655f 322c 202e 2e2e 2c20 7369   size_2, ..., si
+00014150: 7a65 5f72 2920 5b72 3d6e 5f64 696d 5d2e  ze_r) [r=n_dim].
+00014160: 0a20 2020 2020 2020 2069 6620 7472 616e  .        if tran
+00014170: 7320 6973 204e 6f6e 653a 2074 7261 6e73  s is None: trans
+00014180: 203d 2049 6465 6e74 6974 7928 290a 2020   = Identity().  
+00014190: 2020 2020 2020 5920 3d20 7472 616e 7328        Y = trans(
+000141a0: 5829 0a20 2020 2020 2020 2069 6620 6e6f  X).        if no
+000141b0: 7420 592e 6861 735f 6261 7463 683a 2059  t Y.has_batch: Y
+000141c0: 203d 2059 2e6d 756c 7469 706c 7928 6e5f   = Y.multiply(n_
+000141d0: 6261 7463 682c 205b 5d29 0a20 2020 2020  batch, []).     
+000141e0: 2020 2069 6620 592e 6e5f 6261 7463 6820     if Y.n_batch 
+000141f0: 3d3d 2031 3a20 5920 3d20 592e 7265 7065  == 1: Y = Y.repe
+00014200: 6174 6564 286e 5f62 6174 6368 2c20 5b5d  ated(n_batch, []
+00014210: 290a 2020 2020 2020 2020 5920 3d20 592e  ).        Y = Y.
+00014220: 616d 706c 6966 7928 6e5f 6665 6174 7572  amplify(n_featur
+00014230: 652c 205b 5d29 0a20 2020 2020 2020 2073  e, []).        s
+00014240: 6861 7065 5f6f 7574 203d 2073 6861 7065  hape_out = shape
+00014250: 5f6f 7574 2e72 6573 6574 5f73 7061 6365  _out.reset_space
+00014260: 2874 6172 6765 745f 7370 6163 6529 0a20  (target_space). 
+00014270: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00014280: 2074 6172 6765 745f 7370 6163 6520 3d20   target_space = 
+00014290: 6261 746f 7263 685f 7465 6e73 6f72 2874  batorch_tensor(t
+000142a0: 6172 6765 745f 7370 6163 6529 0a20 2020  arget_space).   
+000142b0: 2020 2020 2069 6620 6e6f 7420 7461 7267       if not targ
+000142c0: 6574 5f73 7061 6365 2e68 6173 5f62 6174  et_space.has_bat
+000142d0: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+000142e0: 6966 2074 6172 6765 745f 7370 6163 652e  if target_space.
+000142f0: 7369 7a65 2830 2920 3d3d 206e 5f62 6174  size(0) == n_bat
+00014300: 6368 2061 6e64 206e 5f62 6174 6368 2021  ch and n_batch !
+00014310: 3d20 6e5f 6469 6d20 6f72 206c 656e 285b  = n_dim or len([
+00014320: 7820 666f 7220 7820 696e 2074 6172 6765  x for x in targe
+00014330: 745f 7370 6163 652e 7368 6170 6520 6966  t_space.shape if
+00014340: 2078 203d 3d20 6e5f 6469 6d5d 2920 3e3d   x == n_dim]) >=
+00014350: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+00014360: 2020 2020 7461 7267 6574 5f73 7061 6365      target_space
+00014370: 2e77 6974 685f 6261 7463 6864 696d 2830  .with_batchdim(0
+00014380: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00014390: 7365 3a20 7461 7267 6574 5f73 7061 6365  se: target_space
+000143a0: 2e75 6e73 7175 6565 7a65 5f28 5b5d 290a  .unsqueeze_([]).
+000143b0: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
+000143c0: 6172 6765 745f 7370 6163 652e 6861 735f  arget_space.has_
+000143d0: 6368 616e 6e65 6c3a 0a20 2020 2020 2020  channel:.       
+000143e0: 2020 2020 2069 6620 7461 7267 6574 5f73       if target_s
+000143f0: 7061 6365 2e62 6174 6368 5f64 696d 656e  pace.batch_dimen
+00014400: 7369 6f6e 2021 3d20 3020 616e 6420 7461  sion != 0 and ta
+00014410: 7267 6574 5f73 7061 6365 2e73 697a 6528  rget_space.size(
+00014420: 3029 203d 3d20 6e5f 6469 6d3a 2074 6172  0) == n_dim: tar
+00014430: 6765 745f 7370 6163 652e 7769 7468 5f63  get_space.with_c
+00014440: 6861 6e6e 656c 6469 6d28 3029 0a20 2020  hanneldim(0).   
+00014450: 2020 2020 2020 2020 2065 6c69 6620 7461           elif ta
+00014460: 7267 6574 5f73 7061 6365 2e62 6174 6368  rget_space.batch
+00014470: 5f64 696d 656e 7369 6f6e 2021 3d20 3120  _dimension != 1 
+00014480: 616e 6420 7461 7267 6574 5f73 7061 6365  and target_space
+00014490: 2e73 697a 6528 3129 203d 3d20 6e5f 6469  .size(1) == n_di
+000144a0: 6d3a 2074 6172 6765 745f 7370 6163 652e  m: target_space.
+000144b0: 7769 7468 5f63 6861 6e6e 656c 6469 6d28  with_channeldim(
+000144c0: 3129 0a20 2020 2020 2020 2020 2020 2065  1).            e
+000144d0: 6c69 6620 7461 7267 6574 5f73 7061 6365  lif target_space
+000144e0: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+000144f0: 2021 3d20 7461 7267 6574 5f73 7061 6365   != target_space
+00014500: 2e6e 5f64 696d 202d 2031 2061 6e64 2074  .n_dim - 1 and t
+00014510: 6172 6765 745f 7370 6163 652e 7369 7a65  arget_space.size
+00014520: 282d 3129 203d 3d20 6e5f 6469 6d3a 2074  (-1) == n_dim: t
+00014530: 6172 6765 745f 7370 6163 652e 7769 7468  arget_space.with
+00014540: 5f63 6861 6e6e 656c 6469 6d28 2d31 290a  _channeldim(-1).
+00014550: 2020 2020 2020 2020 6176 6f75 6368 2874          avouch(t
+00014560: 6172 6765 745f 7370 6163 652e 6861 735f  arget_space.has_
+00014570: 6368 616e 6e65 6c20 616e 6420 7461 7267  channel and targ
+00014580: 6574 5f73 7061 6365 2e6e 5f63 6861 6e6e  et_space.n_chann
+00014590: 656c 203d 3d20 6e5f 6469 6d2c 2022 2774  el == n_dim, "'t
+000145a0: 6172 6765 745f 7370 6163 6527 2066 6f72  arget_space' for
+000145b0: 2069 6e74 6572 706f 6c61 7469 6f6e 2073   interpolation s
+000145c0: 686f 756c 6420 6861 7665 2061 2063 6861  hould have a cha
+000145d0: 6e6e 656c 2064 696d 656e 7369 6f6e 2066  nnel dimension f
+000145e0: 6f72 2063 6f6f 7264 696e 6174 6573 2e20  or coordinates. 
+000145f0: 2229 0a20 2020 2020 2020 2059 203d 2074  ").        Y = t
+00014600: 6172 6765 745f 7370 6163 652e 7265 7065  arget_space.repe
+00014610: 6174 6564 286e 5f62 6174 6368 202f 2f20  ated(n_batch // 
+00014620: 7461 7267 6574 5f73 7061 6365 2e6e 5f62  target_space.n_b
+00014630: 6174 6368 2c20 5b5d 292e 616d 706c 6966  atch, []).amplif
+00014640: 7928 6e5f 6665 6174 7572 652c 205b 5d29  y(n_feature, [])
+00014650: 0a20 2020 2020 2020 2073 6861 7065 5f6f  .        shape_o
+00014660: 7574 203d 2073 6861 7065 5f6f 7574 2e72  ut = shape_out.r
+00014670: 6573 6574 5f73 7061 6365 2874 6172 6765  eset_space(targe
+00014680: 745f 7370 6163 652e 7370 6163 6529 0a20  t_space.space). 
+00014690: 2020 2020 2020 200a 2020 2020 696d 6167         .    imag
+000146a0: 6520 3d20 696d 6167 652e 6d65 7267 6564  e = image.merged
+000146b0: 696d 7328 7b7d 2c20 5b5d 290a 2020 2020  ims({}, []).    
+000146c0: 6e5f 6261 7463 6820 3d20 696d 6167 652e  n_batch = image.
+000146d0: 6e5f 6261 7463 680a 0a20 2020 2069 6620  n_batch..    if 
+000146e0: 6d65 7468 6f64 2e6c 6f77 6572 2829 203d  method.lower() =
+000146f0: 3d20 2762 7370 6c69 6e65 273a 0a20 2020  = 'bspline':.   
+00014700: 2020 2020 2069 6620 6465 7269 7661 7469       if derivati
+00014710: 7665 3a20 7261 6973 6520 5479 7065 4572  ve: raise TypeEr
+00014720: 726f 7228 224e 6f20 6465 7269 7661 7469  ror("No derivati
+00014730: 7665 7320 666f 7220 6273 706c 696e 6520  ves for bspline 
+00014740: 696e 7465 7270 6f6c 6174 696f 6e73 2061  interpolations a
+00014750: 7265 2061 7661 696c 6162 6c65 2073 6f20  re available so 
+00014760: 6661 722e 2050 6c65 6173 6520 7772 6974  far. Please writ
+00014770: 6520 6974 2062 7920 796f 7572 7365 6c66  e it by yourself
+00014780: 2e20 2229 0a20 2020 2020 2020 2023 2054  . ").        # T
+00014790: 4f44 4f3a 2046 4644 0a20 2020 2020 2020  ODO: FFD.       
+000147a0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+000147b0: 2822 4273 706c 696e 6520 696e 7465 7270  ("Bspline interp
+000147c0: 6f6c 6174 696f 6e20 6973 206e 6f74 2061  olation is not a
+000147d0: 7661 696c 6162 6c65 2073 6f20 6661 722e  vailable so far.
+000147e0: 2050 6c65 6173 6520 7772 6974 6520 6974   Please write it
+000147f0: 2062 7920 796f 7572 7365 6c66 2e20 2229   by yourself. ")
+00014800: 0a0a 2020 2020 6959 203d 2062 742e 666c  ..    iY = bt.fl
+00014810: 6f6f 7228 5929 2e6c 6f6e 6728 2920 2320  oor(Y).long() # 
+00014820: 4765 6e65 7261 7465 2074 6865 2069 6e74  Generate the int
+00014830: 6567 6572 2070 6172 7420 6f66 2059 0a20  eger part of Y. 
+00014840: 2020 206a 5920 3d20 6959 202b 2031 2023     jY = iY + 1 #
+00014850: 2061 6e64 2074 6865 2069 6e74 6567 6572   and the integer
+00014860: 2070 6172 7420 706c 7573 206f 6e65 2e0a   part plus one..
+00014870: 2020 2020 6966 206d 6574 686f 642e 6c6f      if method.lo
+00014880: 7765 7228 2920 3d3d 2027 6c69 6e65 6172  wer() == 'linear
+00014890: 273a 2066 5920 3d20 5920 2d20 6959 2e66  ': fY = Y - iY.f
+000148a0: 6c6f 6174 2829 2023 2054 6865 2064 6563  loat() # The dec
+000148b0: 696d 616c 2070 6172 7420 6f66 2059 2e0a  imal part of Y..
+000148c0: 2020 2020 656c 6966 206d 6574 686f 642e      elif method.
+000148d0: 6c6f 7765 7228 2920 3d3d 2027 6e65 6172  lower() == 'near
+000148e0: 6573 7427 3a20 6659 203d 2062 742e 666c  est': fY = bt.fl
+000148f0: 6f6f 7228 5920 2d20 6959 2e66 6c6f 6174  oor(Y - iY.float
+00014900: 2829 202b 2030 2e35 2920 2320 5468 6520  () + 0.5) # The 
+00014910: 6465 6369 6d61 6c20 7061 7274 206f 6620  decimal part of 
+00014920: 592e 0a20 2020 2065 6c73 653a 2072 6169  Y..    else: rai
+00014930: 7365 2054 7970 6545 7272 6f72 2822 556e  se TypeError("Un
+00014940: 7265 636f 676e 697a 6564 2061 7267 756d  recognized argum
+00014950: 656e 7420 276d 6574 686f 6427 2e20 2229  ent 'method'. ")
+00014960: 0a20 2020 2062 5920 3d20 6274 2e73 7461  .    bY = bt.sta
+00014970: 636b 2828 6959 2c20 6a59 292c 2031 292e  ck((iY, jY), 1).
+00014980: 7669 6577 285b 6e5f 6261 7463 685d 2c20  view([n_batch], 
+00014990: 322c 207b 6e5f 6469 6d7d 2c20 2d31 2920  2, {n_dim}, -1) 
+000149a0: 2320 285b 6e5f 6261 7463 685d 2c20 322c  # ([n_batch], 2,
+000149b0: 207b 6e5f 6469 6d7d 2c20 6e5f 6461 7461   {n_dim}, n_data
+000149c0: 292e 0a20 2020 2057 203d 2062 742e 7374  )..    W = bt.st
+000149d0: 6163 6b28 2831 202d 2066 592c 2066 5929  ack((1 - fY, fY)
+000149e0: 2c20 3129 2e76 6965 7728 5b6e 5f62 6174  , 1).view([n_bat
+000149f0: 6368 5d2c 2032 2c20 7b6e 5f64 696d 7d2c  ch], 2, {n_dim},
+00014a00: 202d 3129 2023 2028 5b6e 5f62 6174 6368   -1) # ([n_batch
+00014a10: 5d2c 2032 2c20 7b6e 5f64 696d 7d2c 206e  ], 2, {n_dim}, n
+00014a20: 5f64 6174 6129 2e0a 2020 2020 6e5f 6461  _data)..    n_da
+00014a30: 7461 203d 2062 592e 7369 7a65 282d 3129  ta = bY.size(-1)
+00014a40: 0a0a 2020 2020 2320 5072 6570 6172 6520  ..    # Prepare 
+00014a50: 666f 7220 7468 6520 6f75 7470 7574 2073  for the output s
+00014a60: 7061 6365 3a20 6e5f 6261 7463 682c 206d  pace: n_batch, m
+00014a70: 5f31 2c20 2e2e 2e2c 206d 5f73 0a20 2020  _1, ..., m_s.   
+00014a80: 2069 6620 6465 7269 7661 7469 7665 3a20   if derivative: 
+00014a90: 6f75 7470 7574 203d 2062 742e 7a65 726f  output = bt.zero
+00014aa0: 7328 5b6e 5f62 6174 6368 5d2c 207b 6e5f  s([n_batch], {n_
+00014ab0: 6469 6d7d 2c20 2a73 6861 7065 5f6f 7574  dim}, *shape_out
+00014ac0: 2e73 7061 6365 290a 2020 2020 656c 7365  .space).    else
+00014ad0: 3a20 6f75 7470 7574 203d 2062 742e 7a65  : output = bt.ze
+00014ae0: 726f 7328 7368 6170 655f 6f75 7429 0a20  ros(shape_out). 
+00014af0: 2020 2066 6f72 2047 2069 6e20 6274 2e69     for G in bt.i
+00014b00: 6d61 6765 5f67 7269 6428 5b32 5d2a 6e5f  mage_grid([2]*n_
+00014b10: 6469 6d29 2e66 6c61 7474 656e 2829 2e74  dim).flatten().t
+00014b20: 7261 6e73 706f 7365 2830 2c20 3129 3a0a  ranspose(0, 1):.
+00014b30: 2020 2020 2020 2020 2320 4765 7420 7468          # Get th
+00014b40: 6520 696e 6469 6365 7320 666f 7220 7468  e indices for th
+00014b50: 6520 7465 726d 3a20 6259 5b3a 2c20 475b  e term: bY[:, G[
+00014b60: 445d 2c20 442c 203a 5d2c 2073 697a 653d  D], D, :], size=
+00014b70: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f64  ([n_batch], {n_d
+00014b80: 696d 7d2c 206e 5f64 6174 6129 0a20 2020  im}, n_data).   
+00014b90: 2020 2020 2049 6e64 203d 2062 592e 6761       Ind = bY.ga
+00014ba0: 7468 6572 2831 2c20 472e 6578 7061 6e64  ther(1, G.expand
+00014bb0: 5f74 6f28 5b6e 5f62 6174 6368 5d2c 2031  _to([n_batch], 1
+00014bc0: 2c20 7b6e 5f64 696d 7d2c 206e 5f64 6174  , {n_dim}, n_dat
+00014bd0: 6129 292e 7371 7565 657a 6528 3129 0a20  a)).squeeze(1). 
+00014be0: 2020 2020 2020 2023 2043 6c61 6d70 2074         # Clamp t
+00014bf0: 6865 2069 6e64 6963 6573 2069 6e20 7468  he indices in th
+00014c00: 6520 636f 7272 6563 7420 7261 6e67 6520  e correct range 
+00014c10: 2620 436f 6d70 7574 6520 7468 6520 626f  & Compute the bo
+00014c20: 7264 6572 2063 6f6e 6469 7469 6f6e 0a20  rder condition. 
+00014c30: 2020 2020 2020 2063 6f6e 6469 7469 6f6e         condition
+00014c40: 203d 2062 742e 7375 6d28 2849 6e64 203c   = bt.sum((Ind <
+00014c50: 2030 2920 2b20 2849 6e64 203e 2073 697a   0) + (Ind > siz
+00014c60: 6520 2d20 3129 2c20 3129 0a20 2020 2020  e - 1), 1).     
+00014c70: 2020 2049 6e64 203d 2062 742e 6d69 6e28     Ind = bt.min(
+00014c80: 6274 2e63 6c61 6d70 2849 6e64 2c20 6d69  bt.clamp(Ind, mi
+00014c90: 6e3d 3029 2c20 2873 697a 6520 2d20 3129  n=0), (size - 1)
+00014ca0: 2e65 7870 616e 645f 746f 2849 6e64 2929  .expand_to(Ind))
+00014cb0: 0a20 2020 2020 2020 2023 2043 6f6e 7665  .        # Conve
+00014cc0: 7274 2074 6865 2069 6e64 6963 6573 2074  rt the indices t
+00014cd0: 6f20 3120 6469 6d65 6e73 696f 6e61 6c2e  o 1 dimensional.
+00014ce0: 2044 6f74 3a20 285b 6e5f 6261 7463 685d   Dot: ([n_batch]
+00014cf0: 2c20 6e5f 6461 7461 290a 2020 2020 2020  , n_data).      
+00014d00: 2020 446f 7420 3d20 496e 645b 3a2c 2030    Dot = Ind[:, 0
+00014d10: 5d0a 2020 2020 2020 2020 666f 7220 7220  ].        for r 
+00014d20: 696e 2072 616e 6765 2831 2c20 6e5f 6469  in range(1, n_di
+00014d30: 6d29 3a20 446f 7420 2a3d 2073 697a 655b  m): Dot *= size[
+00014d40: 725d 3b20 446f 7420 2b3d 2049 6e64 5b3a  r]; Dot += Ind[:
+00014d50: 2c20 725d 0a20 2020 2020 2020 2023 2047  , r].        # G
+00014d60: 6574 2074 6865 2069 6d61 6765 2076 616c  et the image val
+00014d70: 7565 7320 4956 3a20 285b 6e5f 6261 7463  ues IV: ([n_batc
+00014d80: 685d 2c20 6e5f 6461 7461 290a 2020 2020  h], n_data).    
+00014d90: 2020 2020 4956 203d 204e 6f6e 650a 2020      IV = None.  
+00014da0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00014db0: 6e63 6528 6669 6c6c 2c20 7374 7229 3a0a  nce(fill, str):.
+00014dc0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00014dd0: 696c 6c2e 6c6f 7765 7228 2920 3d3d 2027  ill.lower() == '
+00014de0: 6e65 6172 6573 7427 3a0a 2020 2020 2020  nearest':.      
+00014df0: 2020 2020 2020 2020 2020 4956 203d 2069            IV = i
+00014e00: 6d61 6765 2e66 6c61 7474 656e 2829 2e67  mage.flatten().g
+00014e10: 6174 6865 7228 312c 2044 6f74 290a 2020  ather(1, Dot).  
+00014e20: 2020 2020 2020 2020 2020 656c 6966 2066            elif f
+00014e30: 696c 6c2e 6c6f 7765 7228 2920 3d3d 2027  ill.lower() == '
+00014e40: 6261 636b 6772 6f75 6e64 273a 0a20 2020  background':.   
+00014e50: 2020 2020 2020 2020 2020 2020 2062 6b5f               bk_
+00014e60: 7661 6c75 6520 3d20 6274 2e73 7461 636b  value = bt.stack
+00014e70: 285b 696d 6167 655b 2873 6c69 6365 284e  ([image[(slice(N
+00014e80: 6f6e 6529 2c29 202b 2074 7570 6c65 2867  one),) + tuple(g
+00014e90: 295d 2066 6f72 2067 2069 6e20 2862 742e  )] for g in (bt.
+00014ea0: 696d 6167 655f 6772 6964 285b 325d 2a6e  image_grid([2]*n
+00014eb0: 5f64 696d 2920 2a20 6274 2e63 6861 6e6e  _dim) * bt.chann
+00014ec0: 656c 5f74 656e 736f 7228 7369 7a65 2d31  el_tensor(size-1
+00014ed0: 2929 2e66 6c61 7474 656e 2829 2e74 7261  )).flatten().tra
+00014ee0: 6e73 706f 7365 2830 2c31 295d 2c20 3129  nspose(0,1)], 1)
+00014ef0: 2e6d 6564 6961 6e28 3129 2e76 616c 7565  .median(1).value
+00014f00: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00014f10: 2020 6261 636b 6772 6f75 6e64 203d 2062    background = b
+00014f20: 6b5f 7661 6c75 6520 2a20 6274 2e6f 6e65  k_value * bt.one
+00014f30: 735f 6c69 6b65 2844 6f74 290a 2020 2020  s_like(Dot).    
+00014f40: 2020 2020 2020 2020 656c 6966 2066 696c          elif fil
+00014f50: 6c2e 6c6f 7765 7228 2920 3d3d 2027 7a65  l.lower() == 'ze
+00014f60: 726f 273a 0a20 2020 2020 2020 2020 2020  ro':.           
+00014f70: 2020 2020 2062 6163 6b67 726f 756e 6420       background 
+00014f80: 3d20 6274 2e7a 6572 6f73 5f6c 696b 6528  = bt.zeros_like(
+00014f90: 446f 7429 0a20 2020 2020 2020 2065 6c73  Dot).        els
+00014fa0: 653a 0a20 2020 2020 2020 2020 2020 2062  e:.            b
+00014fb0: 6163 6b67 726f 756e 6420 3d20 6669 6c6c  ackground = fill
+00014fc0: 202a 2062 742e 6f6e 6573 5f6c 696b 6528   * bt.ones_like(
+00014fd0: 446f 7429 0a20 2020 2020 2020 2069 6620  Dot).        if 
+00014fe0: 4956 2069 7320 4e6f 6e65 3a20 4956 203d  IV is None: IV =
+00014ff0: 2062 742e 7768 6572 6528 636f 6e64 6974   bt.where(condit
+00015000: 696f 6e20 3e3d 2031 2c20 6261 636b 6772  ion >= 1, backgr
+00015010: 6f75 6e64 2e66 6c6f 6174 2829 2c20 696d  ound.float(), im
+00015020: 6167 652e 666c 6174 7465 6e28 292e 6761  age.flatten().ga
+00015030: 7468 6572 2831 2c20 446f 7429 2e66 6c6f  ther(1, Dot).flo
+00015040: 6174 2829 290a 2020 2020 2020 2020 2320  at()).        # 
+00015050: 5765 6967 6874 7320 666f 7220 6561 6368  Weights for each
+00015060: 2070 6f69 6e74 3a20 5b70 726f 6475 6374   point: [product
+00015070: 206f 6620 575b 3a2c 2047 5b44 5d2c 2044   of W[:, G[D], D
+00015080: 2c20 785d 2066 6f72 2044 2069 6e20 7261  , x] for D in ra
+00015090: 6e67 6528 6e5f 6469 6d29 5d20 666f 7220  nge(n_dim)] for 
+000150a0: 706f 696e 7420 782e 0a20 2020 2020 2020  point x..       
+000150b0: 2023 2057 673a 2028 5b6e 5f62 6174 6368   # Wg: ([n_batch
+000150c0: 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f 6461  ], {n_dim}, n_da
+000150d0: 7461 290a 2020 2020 2020 2020 5767 203d  ta).        Wg =
+000150e0: 2057 2e67 6174 6865 7228 312c 2047 2e65   W.gather(1, G.e
+000150f0: 7870 616e 645f 746f 285b 6e5f 6261 7463  xpand_to([n_batc
+00015100: 685d 2c20 312c 207b 6e5f 6469 6d7d 2c20  h], 1, {n_dim}, 
+00015110: 6e5f 6461 7461 2929 2e73 7175 6565 7a65  n_data)).squeeze
+00015120: 2831 290a 2020 2020 2020 2020 6966 206e  (1).        if n
+00015130: 6f74 2064 6572 6976 6174 6976 653a 0a20  ot derivative:. 
+00015140: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00015150: 7420 2b3d 2028 5767 2e70 726f 6428 3129  t += (Wg.prod(1)
+00015160: 202a 2049 5629 2e76 6965 775f 6173 286f   * IV).view_as(o
+00015170: 7574 7075 7429 0a20 2020 2020 2020 2065  utput).        e
+00015180: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00015190: 2074 656d 7057 674d 6174 203d 2057 672e   tempWgMat = Wg.
+000151a0: 6d75 6c74 6970 6c79 286e 5f64 696d 2c20  multiply(n_dim, 
+000151b0: 3129 2023 2028 5b6e 5f62 6174 6368 5d2c  1) # ([n_batch],
+000151c0: 206e 5f64 696d 2c20 7b6e 5f64 696d 7d2c   n_dim, {n_dim},
+000151d0: 206e 5f64 6174 6129 0a20 2020 2020 2020   n_data).       
+000151e0: 2020 2020 2074 656d 7057 674d 6174 5b3a       tempWgMat[:
+000151f0: 2c20 6274 2e61 7261 6e67 6528 6e5f 6469  , bt.arange(n_di
+00015200: 6d29 2c20 6274 2e61 7261 6e67 6528 6e5f  m), bt.arange(n_
+00015210: 6469 6d29 5d20 3d20 310a 2020 2020 2020  dim)] = 1.      
+00015220: 2020 2020 2020 6457 6720 3d20 7465 6d70        dWg = temp
+00015230: 5767 4d61 742e 7072 6f64 2831 2920 2a20  WgMat.prod(1) * 
+00015240: 2847 202a 2032 202d 2031 292e 666c 6f61  (G * 2 - 1).floa
+00015250: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00015260: 6f75 7470 7574 202b 3d20 2864 5767 202a  output += (dWg *
+00015270: 2049 562e 756e 7371 7565 657a 6528 3129   IV.unsqueeze(1)
+00015280: 292e 7669 6577 5f61 7328 6f75 7470 7574  ).view_as(output
+00015290: 290a 2020 2020 6274 2e74 6f72 6368 2e63  ).    bt.torch.c
+000152a0: 7564 612e 656d 7074 795f 6361 6368 6528  uda.empty_cache(
+000152b0: 290a 2020 2020 6570 7320 3d20 3165 2d36  ).    eps = 1e-6
+000152c0: 0a20 2020 206d 203d 2030 2069 6620 696d  .    m = 0 if im
+000152d0: 6167 652e 6d69 6e28 2920 3e20 2d65 7073  age.min() > -eps
+000152e0: 2065 6c73 6520 696d 6167 652e 6d69 6e28   else image.min(
+000152f0: 292e 6974 656d 2829 0a20 2020 204d 203d  ).item().    M =
+00015300: 2031 2069 6620 696d 6167 652e 6d61 7828   1 if image.max(
+00015310: 2920 3c20 3120 2b20 6570 7320 656c 7365  ) < 1 + eps else
+00015320: 2069 6d61 6765 2e6d 6178 2829 2e69 7465   image.max().ite
+00015330: 6d28 290a 2020 2020 7265 7475 726e 206f  m().    return o
+00015340: 7574 7075 742e 636c 616d 7028 6d2c 204d  utput.clamp(m, M
+00015350: 290a 0a40 616c 6961 7328 2272 6573 616d  )..@alias("resam
+00015360: 706c 655f 666f 7277 6172 6422 290a 6465  ple_forward").de
+00015370: 6620 696e 7465 7270 6f6c 6174 696f 6e5f  f interpolation_
+00015380: 666f 7277 6172 6428 0a20 2020 2020 2020  forward(.       
+00015390: 2069 6d61 6765 2c20 0a20 2020 2020 2020   image, .       
+000153a0: 2074 7261 6e73 203d 204e 6f6e 652c 200a   trans = None, .
+000153b0: 2020 2020 2020 2020 6d65 7468 6f64 203d          method =
+000153c0: 2027 4c69 6e65 6172 272c 200a 2020 2020   'Linear', .    
+000153d0: 2020 2020 7461 7267 6574 5f73 7061 6365      target_space
+000153e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000153f0: 2066 696c 6c20 3d20 277a 6572 6f27 2c0a   fill = 'zero',.
+00015400: 2020 2020 2020 2020 6465 7269 7661 7469          derivati
+00015410: 7665 203d 2046 616c 7365 0a20 2020 2029  ve = False.    )
+00015420: 3a0a 2020 2020 2727 270a 2020 2020 496e  :.    '''.    In
+00015430: 7465 7270 6f6c 6174 6520 7573 696e 6720  terpolate using 
+00015440: 666f 7277 6172 6420 7472 616e 7366 6f72  forward transfor
+00015450: 6d61 7469 6f6e 2e20 4974 2069 7320 6e6f  mation. It is no
+00015460: 7420 7965 7420 696d 706c 656d 656e 7465  t yet implemente
+00015470: 642e 200a 2020 2020 692e 652e 2043 6f6d  d. .    i.e. Com
+00015480: 7075 7465 2074 6865 2069 6d61 6765 2049  pute the image I
+00015490: 2073 2e74 2e20 7472 616e 7328 7829 203d   s.t. trans(x) =
+000154a0: 2079 2066 6f72 2078 2069 6e20 696e 7075   y for x in inpu
+000154b0: 7420 696d 6167 6520 616e 6420 7920 696e  t image and y in
+000154c0: 2074 6865 206f 7574 7075 7420 4920 7573   the output I us
+000154d0: 696e 6720 696e 7465 7270 6f6c 6174 696f  ing interpolatio
+000154e0: 6e20 6d65 7468 6f64 3a0a 2020 2020 2020  n method:.      
+000154f0: 2020 6d65 7468 6f64 203d 204c 696e 6561    method = Linea
+00015500: 7220 5b4e 4f20 4752 4144 4945 4e54 2121  r [NO GRADIENT!!
+00015510: 215d 3a20 4269 6c69 6e65 6172 2069 6e74  !]: Bilinear int
+00015520: 6572 706f 6c61 7469 6f6e 0a20 2020 2020  erpolation.     
+00015530: 2020 206d 6574 686f 6420 3d20 4e65 6172     method = Near
+00015540: 6573 7420 5b4e 4f20 4752 4144 4945 4e54  est [NO GRADIENT
+00015550: 2121 215d 3a20 4e65 6172 6573 7420 696e  !!!]: Nearest in
+00015560: 7465 7270 6f6c 6174 696f 6e0a 0a20 2020  terpolation..   
+00015570: 2050 6172 616d 733a 0a20 2020 2020 2020   Params:.       
+00015580: 2069 6d61 6765 205b 6274 2e54 656e 736f   image [bt.Tenso
+00015590: 725d 3a20 5468 6520 7461 7267 6574 2069  r]: The target i
+000155a0: 6d61 6765 2e0a 2020 2020 2020 2020 2020  mage..          
+000155b0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+000155c0: 683a 6f70 7469 6f6e 616c 5d2c 207b 6e5f  h:optional], {n_
+000155d0: 6368 616e 6e65 6c3a 6f70 7469 6f6e 616c  channel:optional
+000155e0: 7d2c 206d 4031 2c20 6d40 322c 202e 2e2e  }, m@1, m@2, ...
+000155f0: 2c20 6d40 6e5f 6469 6d29 0a20 2020 2020  , m@n_dim).     
+00015600: 2020 2074 7261 6e73 205b 4675 6e63 7469     trans [Functi
+00015610: 6f6e 206f 7220 6d69 636f 6d70 7574 696e  on or micomputin
+00015620: 672e 5370 6174 6961 6c54 7261 6e73 666f  g.SpatialTransfo
+00015630: 726d 6174 696f 6e5d 3a20 5472 616e 7366  rmation]: Transf
+00015640: 6f72 6d61 7469 6f6e 2066 756e 6374 696f  ormation functio
+00015650: 6e2c 206d 6170 7069 6e67 0a20 2020 2020  n, mapping.     
+00015660: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
+00015670: 5f62 6174 6368 3a6f 7074 696f 6e61 6c5d  _batch:optional]
+00015680: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
+00015690: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+000156a0: 6d29 2074 6f20 285b 6e5f 6261 7463 685d  m) to ([n_batch]
+000156b0: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
+000156c0: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+000156d0: 6d29 0a20 2020 2020 2020 206d 6574 686f  m).        metho
+000156e0: 6420 5b73 7472 3a20 6c69 6e65 6172 7c6e  d [str: linear|n
+000156f0: 6561 7265 7374 5d3a 2054 6865 2069 6e74  earest]: The int
+00015700: 6572 706f 6c61 7469 6f6e 206d 6574 686f  erpolation metho
+00015710: 642e 200a 2020 2020 2020 2020 7461 7267  d. .        targ
+00015720: 6574 5f73 7061 6365 205b 7475 706c 6520  et_space [tuple 
+00015730: 6f72 2062 742e 5465 6e73 6f72 5d3a 0a20  or bt.Tensor]:. 
+00015740: 2020 2020 2020 2020 2020 2053 697a 6520             Size 
+00015750: 2874 7570 6c65 2920 6f66 2061 2074 6172  (tuple) of a tar
+00015760: 6765 7420 524f 4920 6174 2074 6865 2063  get ROI at the c
+00015770: 656e 7465 7220 6f66 2069 6d61 6765 2e20  enter of image. 
+00015780: 0a20 2020 2020 2020 2020 2020 204f 5220  .            OR 
+00015790: 5472 616e 7366 6f72 6d65 6420 636f 6f72  Transformed coor
+000157a0: 6469 6e61 7465 2073 7061 6365 2028 6274  dinate space (bt
+000157b0: 2e54 656e 736f 7229 206f 6620 7468 6520  .Tensor) of the 
+000157c0: 6f75 7470 7574 2069 6d61 6765 2e20 0a20  output image. . 
+000157d0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
+000157e0: 206c 656e 6774 6828 6e5f 6469 6d29 206f   length(n_dim) o
+000157f0: 7220 285b 6e5f 6261 7463 683a 6f70 7469  r ([n_batch:opti
+00015800: 6f6e 616c 5d2c 207b 6e5f 6469 6d3a 6f70  onal], {n_dim:op
+00015810: 7469 6f6e 616c 7d2c 2073 697a 6540 312c  tional}, size@1,
+00015820: 2073 697a 6540 322c 202e 2e2e 2c20 7369   size@2, ..., si
+00015830: 7a65 406e 5f64 696d 290a 2020 2020 2020  ze@n_dim).      
+00015840: 2020 6669 6c6c 205b 7374 723a 206e 6561    fill [str: nea
+00015850: 7265 7374 7c62 6163 6b67 726f 756e 6420  rest|background 
+00015860: 6f72 2069 6e74 206f 7220 666c 6f61 7428  or int or float(
+00015870: 6e75 6d62 6572 295d 3a20 496e 6469 6361  number)]: Indica
+00015880: 7465 2074 6865 2077 6179 2074 6f20 6669  te the way to fi
+00015890: 6c6c 2062 6163 6b67 726f 756e 6420 6f75  ll background ou
+000158a0: 7473 6964 6520 6053 7572 726f 756e 6469  tside `Surroundi
+000158b0: 6e67 602e 200a 2020 2020 2020 2020 6465  ng`. .        de
+000158c0: 7269 7661 7469 7665 205b 626f 6f6c 5d3a  rivative [bool]:
+000158d0: 2057 6865 7468 6572 2074 6f20 7265 7475   Whether to retu
+000158e0: 726e 2074 6865 2067 7261 6469 656e 742e  rn the gradient.
+000158f0: 204f 6e65 2063 616e 206f 6d69 7420 6974   One can omit it
+00015900: 2077 6865 6e20 7573 696e 6720 746f 7263   when using torc
+00015910: 682e 6175 746f 6772 6164 2e0a 0a20 2020  h.autograd...   
+00015920: 2020 2020 206f 7574 7075 7420 5b62 742e       output [bt.
+00015930: 5465 6e73 6f72 5d3a 2054 6865 2074 7261  Tensor]: The tra
+00015940: 6e73 666f 726d 6564 2069 6d61 6765 2e0a  nsformed image..
+00015950: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00015960: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
+00015970: 5f63 6861 6e6e 656c 3a6f 7074 696f 6e61  _channel:optiona
+00015980: 6c7d 2c20 6d40 312c 206d 4032 2c20 2e2e  l}, m@1, m@2, ..
+00015990: 2e2c 206d 406e 5f64 696d 290a 2020 2020  ., m@n_dim).    
+000159a0: 2020 2020 2020 2020 6f72 2077 6865 6e20          or when 
+000159b0: 6074 6172 6765 745f 7370 6163 6560 2069  `target_space` i
+000159c0: 7320 6465 6669 6e65 6420 6279 2074 656e  s defined by ten
+000159d0: 736f 722e 200a 2020 2020 2020 2020 2020  sor. .          
+000159e0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+000159f0: 685d 2c20 7369 7a65 4031 2c20 7369 7a65  h], size@1, size
+00015a00: 4032 2c20 2e2e 2e2c 2073 697a 6540 6e5f  @2, ..., size@n_
+00015a10: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+00015a20: 206f 7220 7468 6520 6465 7269 7661 7469   or the derivati
+00015a30: 7665 2066 6f72 2074 6865 2069 6e74 6572  ve for the inter
+00015a40: 706f 6c61 7469 6f6e 2e20 2869 6620 6064  polation. (if `d
+00015a50: 6572 6976 6174 6976 6520 3d20 5472 7565  erivative = True
+00015a60: 6029 0a20 2020 2020 2020 2020 2020 2073  `).            s
+00015a70: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
+00015a80: 207b 6e5f 6469 6d7d 2c20 7369 7a65 4031   {n_dim}, size@1
+00015a90: 2c20 7369 7a65 4032 2c20 2e2e 2e2c 2073  , size@2, ..., s
+00015aa0: 697a 6540 6e5f 6469 6d29 0a0a 2020 2020  ize@n_dim)..    
+00015ab0: 4578 616d 706c 6573 3a0a 2020 2020 2d2d  Examples:.    --
+00015ac0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e  --------.    >>>
+00015ad0: 2049 6d61 6765 203d 2062 742e 7261 6e64   Image = bt.rand
+00015ae0: 2833 2c20 3130 302c 2031 3230 2c20 3830  (3, 100, 120, 80
+00015af0: 290a 2020 2020 3e3e 3e20 414d 203d 2062  ).    >>> AM = b
+00015b00: 742e 7261 6e64 2834 2c20 3429 0a20 2020  t.rand(4, 4).   
+00015b10: 203e 3e3e 2041 4d5b 332c 203a 5d20 3d20   >>> AM[3, :] = 
+00015b20: 6274 2e6f 6e65 5f68 6f74 282d 312c 2034  bt.one_hot(-1, 4
+00015b30: 290a 2020 2020 3e3e 3e20 696e 7465 7270  ).    >>> interp
+00015b40: 6f6c 6174 696f 6e28 496d 6167 652c 2041  olation(Image, A
+00015b50: 6666 696e 6528 414d 292c 206d 6574 686f  ffine(AM), metho
+00015b60: 643d 274c 696e 6561 7227 290a 2020 2020  d='Linear').    
+00015b70: 2727 270a 2020 2020 6966 2074 7261 6e73  '''.    if trans
+00015b80: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00015b90: 2074 7261 6e73 2e62 6163 6b77 6172 643a   trans.backward:
+00015ba0: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
+00015bb0: 7474 7228 7472 616e 732c 2027 696e 7627  ttr(trans, 'inv'
+00015bc0: 293a 2074 7261 6e73 203d 2074 7261 6e73  ): trans = trans
+00015bd0: 2e69 6e76 2829 2e66 616b 655f 696e 7628  .inv().fake_inv(
+00015be0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00015bf0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00015c00: 7428 2257 6172 6e69 6e67 3a20 4261 636b  t("Warning: Back
+00015c10: 7761 7264 2074 7261 6e73 666f 726d 6174  ward transformat
+00015c20: 696f 6e20 666f 756e 6420 696e 206d 6574  ion found in met
+00015c30: 686f 6420 6069 6e74 6572 706f 6c61 7469  hod `interpolati
+00015c40: 6f6e 5f66 6f72 7761 7264 602e 2055 7369  on_forward`. Usi
+00015c50: 6e67 2060 696e 7465 7270 6f6c 6174 696f  ng `interpolatio
+00015c60: 6e60 2069 6e73 7465 6164 2e20 2229 0a20  n` instead. "). 
+00015c70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00015c80: 6e20 696e 7465 7270 6f6c 6174 696f 6e28  n interpolation(
+00015c90: 696d 6167 652c 2074 7261 6e73 2c20 6d65  image, trans, me
+00015ca0: 7468 6f64 203d 206d 6574 686f 642c 2074  thod = method, t
+00015cb0: 6172 6765 745f 7370 6163 6520 3d20 7461  arget_space = ta
+00015cc0: 7267 6574 5f73 7061 6365 2c20 6669 6c6c  rget_space, fill
+00015cd0: 203d 2066 696c 6c29 0a20 2020 2072 6574   = fill).    ret
+00015ce0: 7572 6e20 4e6f 7449 6d70 6c65 6d65 6e74  urn NotImplement
+00015cf0: 6564 0a0a 2323 2323 2323 2323 2323 2323  ed..############
+00015d00: 2049 6d61 6765 2054 7261 6e73 666f 726d   Image Transform
+00015d10: 6174 696f 6e73 2023 2323 2323 2323 2323  ations #########
+00015d20: 2323 230a 0a63 6c61 7373 2049 6d61 6765  ###..class Image
+00015d30: 5472 616e 7366 6f72 6d61 7469 6f6e 2854  Transformation(T
+00015d40: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
+00015d50: 2020 2020 2020 2020 0a20 2020 2064 6566          .    def
+00015d60: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
+00015d70: 5829 3a0a 2020 2020 2020 2020 2727 270a  X):.        '''.
+00015d80: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
+00015d90: 6e73 6f72 5d3a 2049 6d61 6765 2074 6f20  nsor]: Image to 
+00015da0: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
+00015db0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00015dc0: 3a20 285b 6e5f 6261 7463 683a 6f70 7469  : ([n_batch:opti
+00015dd0: 6f6e 616c 5d2c 207b 6e5f 6368 616e 6e65  onal], {n_channe
+00015de0: 6c3a 6f70 7469 6f6e 616c 7d2c 206e 4031  l:optional}, n@1
+00015df0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+00015e00: 6469 6d29 0a20 2020 2020 2020 206f 7574  dim).        out
+00015e10: 7075 7420 5b62 742e 5465 6e73 6f72 5d3a  put [bt.Tensor]:
+00015e20: 2054 6865 2074 7261 6e73 666f 726d 6564   The transformed
+00015e30: 2069 6d61 6765 2e0a 2020 2020 2020 2020   image..        
+00015e40: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+00015e50: 7463 685d 2c20 7b6e 5f63 6861 6e6e 656c  tch], {n_channel
+00015e60: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
+00015e70: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
+00015e80: 2020 2027 2727 0a20 2020 2020 2020 2058     '''.        X
+00015e90: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
+00015ea0: 7228 5829 0a20 2020 2020 2020 2069 6620  r(X).        if 
+00015eb0: 7365 6c66 2e6e 5f64 696d 2069 7320 4e6f  self.n_dim is No
+00015ec0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00015ed0: 6966 206e 6f74 2058 2e68 6173 5f62 6174  if not X.has_bat
+00015ee0: 6368 3a20 5820 3d20 582e 756e 7371 7565  ch: X = X.unsque
+00015ef0: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
+00015f00: 2020 2020 6966 206e 6f74 2058 2e68 6173      if not X.has
+00015f10: 5f63 6861 6e6e 656c 3a20 5820 3d20 582e  _channel: X = X.
+00015f20: 7374 616e 6461 7264 2829 2e75 6e73 7175  standard().unsqu
+00015f30: 6565 7a65 287b 317d 290a 2020 2020 2020  eeze({1}).      
+00015f40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00015f50: 2020 2020 6966 2058 2e6e 5f64 696d 203d      if X.n_dim =
+00015f60: 3d20 7365 6c66 2e6e 5f64 696d 3a20 5820  = self.n_dim: X 
+00015f70: 3d20 582e 7265 6d6f 7665 5f73 7065 6369  = X.remove_speci
+00015f80: 616c 5f28 292e 756e 7371 7565 657a 6528  al_().unsqueeze(
+00015f90: 5b5d 292e 756e 7371 7565 657a 6528 7b31  []).unsqueeze({1
+00015fa0: 7d29 0a20 2020 2020 2020 2020 2020 2065  }).            e
+00015fb0: 6c69 6620 582e 6e5f 6469 6d20 3d3d 2073  lif X.n_dim == s
+00015fc0: 656c 662e 6e5f 6469 6d20 2b20 313a 0a20  elf.n_dim + 1:. 
+00015fd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015fe0: 6620 582e 6861 735f 6261 7463 683a 2058  f X.has_batch: X
+00015ff0: 2e63 6861 6e6e 656c 5f64 696d 656e 7369  .channel_dimensi
+00016000: 6f6e 203d 204e 6f6e 653b 2058 203d 2058  on = None; X = X
+00016010: 2e75 6e73 7175 6565 7a65 287b 3020 6966  .unsqueeze({0 if
+00016020: 2058 2e62 6174 6368 5f64 696d 656e 7369   X.batch_dimensi
+00016030: 6f6e 203e 2030 2065 6c73 6520 317d 290a  on > 0 else 1}).
+00016040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016050: 656c 6966 2058 2e68 6173 5f63 6861 6e6e  elif X.has_chann
+00016060: 656c 3a20 5820 3d20 582e 756e 7371 7565  el: X = X.unsque
+00016070: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
+00016080: 2020 2020 2020 2020 656c 7365 3a20 5820          else: X 
+00016090: 3d20 582e 6261 7463 685f 6469 6d65 6e73  = X.batch_dimens
+000160a0: 696f 6e5f 2830 292e 756e 7371 7565 657a  ion_(0).unsqueez
+000160b0: 6528 7b31 7d29 0a20 2020 2020 2020 2020  e({1}).         
+000160c0: 2020 2065 6c69 6620 582e 6e5f 6469 6d20     elif X.n_dim 
+000160d0: 3d3d 2073 656c 662e 6e5f 6469 6d20 2b20  == self.n_dim + 
+000160e0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+000160f0: 2020 2023 205f 6368 616e 6e61 6c2f 6261     # _channal/ba
+00016100: 7463 6820 6469 6d65 6e73 696f 6e73 2075  tch dimensions u
+00016110: 7365 6420 6865 7265 2061 7320 7468 6579  sed here as they
+00016120: 2061 7265 206e 5f64 696d 2077 6865 6e20   are n_dim when 
+00016130: 6e6f 7420 6578 6973 7465 642e 200a 2020  not existed. .  
+00016140: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00016150: 206e 6f74 2058 2e68 6173 5f62 6174 6368   not X.has_batch
+00016160: 3a20 582e 6261 7463 685f 6469 6d65 6e73  : X.batch_dimens
+00016170: 696f 6e20 3d20 3020 6966 2058 2e5f 6368  ion = 0 if X._ch
+00016180: 616e 6e65 6c5f 6469 6d65 6e73 696f 6e20  annel_dimension 
+00016190: 3e20 3020 656c 7365 2031 0a20 2020 2020  > 0 else 1.     
+000161a0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000161b0: 7420 582e 6861 735f 6368 616e 6e65 6c3a  t X.has_channel:
+000161c0: 2058 2e63 6861 6e6e 656c 5f64 696d 656e   X.channel_dimen
+000161d0: 7369 6f6e 203d 2030 2069 6620 582e 5f62  sion = 0 if X._b
+000161e0: 6174 6368 5f64 696d 656e 7369 6f6e 203e  atch_dimension >
+000161f0: 2030 2065 6c73 6520 310a 2020 2020 2020   0 else 1.      
+00016200: 2020 6176 6f75 6368 2858 2e68 6173 5f62    avouch(X.has_b
+00016210: 6174 6368 2061 6e64 2058 2e68 6173 5f63  atch and X.has_c
+00016220: 6861 6e6e 656c 2c20 6622 506c 6561 7365  hannel, f"Please
+00016230: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+00016240: 736f 7220 6f66 2073 697a 6520 5c0a 2020  sor of size \.  
+00016250: 2020 2020 2020 2020 2020 285b 6e5f 6261            ([n_ba
+00016260: 7463 685d 2c20 7b7b 6e5f 6368 616e 6e65  tch], {{n_channe
+00016270: 6c2f 6e5f 6665 6174 7572 653a 6f70 7469  l/n_feature:opti
+00016280: 6f6e 616c 7d7d 2c20 6d5f 312c 206d 5f32  onal}}, m_1, m_2
+00016290: 2c20 2e2e 2e2c 206d 5f72 2920 5b72 3d6e  , ..., m_r) [r=n
+000162a0: 5f64 696d 5d20 666f 7220 5c0a 2020 2020  _dim] for \.    
+000162b0: 2020 2020 2020 2020 2020 2020 7b73 656c              {sel
+000162c0: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
+000162d0: 6d65 5f5f 2e73 706c 6974 2827 2e27 295b  me__.split('.')[
+000162e0: 2d31 5d7d 2054 7261 6e73 666f 726d 6174  -1]} Transformat
+000162f0: 696f 6e2c 2069 6e73 7465 6164 206f 6620  ion, instead of 
+00016300: 7b58 2e73 6861 7065 7d2e 2022 290a 2020  {X.shape}. ").  
+00016310: 2020 2020 2020 7265 7475 726e 2058 2e63        return X.c
+00016320: 6c6f 6e65 2829 0a0a 636c 6173 7320 4e6f  lone()..class No
+00016330: 726d 616c 697a 6528 496d 6167 6554 7261  rmalize(ImageTra
+00016340: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
+00016350: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00016360: 656c 662c 202a 5f72 616e 6765 293a 0a20  elf, *_range):. 
+00016370: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00016380: 2020 204e 6f72 6d61 6c69 7a65 2074 6865     Normalize the
+00016390: 2069 6e74 656e 7369 7479 206f 6620 616e   intensity of an
+000163a0: 2069 6d61 6765 2e0a 2020 2020 2020 2020   image..        
+000163b0: 0a20 2020 2020 2020 2050 6172 616d 733a  .        Params:
+000163c0: 0a20 2020 2020 2020 2020 2020 205f 7261  .            _ra
+000163d0: 6e67 6520 3d20 286c 6f77 2c20 6869 6768  nge = (low, high
+000163e0: 2920 5b69 6e74 206f 7220 666c 6f61 7420  ) [int or float 
+000163f0: 6f72 2062 742e 5465 6e73 6f72 5d3a 2054  or bt.Tensor]: T
+00016400: 6865 206c 6f77 6573 7420 2861 6e64 2068  he lowest (and h
+00016410: 6967 6865 7374 2920 696e 7465 6e73 6974  ighest) intensit
+00016420: 792e 200a 2020 2020 2020 2020 2020 2020  y. .            
+00016430: 2020 2020 7369 7a65 3a20 6c65 6e67 7468      size: length
+00016440: 2832 2920 6f72 2028 5b6e 5f62 6174 6368  (2) or ([n_batch
+00016450: 5d2c 207b 327d 290a 2020 2020 2020 2020  ], {2}).        
+00016460: 2020 2020 0a20 2020 2020 2020 2057 6865      .        Whe
+00016470: 6e20 6974 2069 7320 6361 6c6c 6564 3a0a  n it is called:.
+00016480: 2020 2020 2020 2020 2020 2020 5820 5b62              X [b
+00016490: 742e 5465 6e73 6f72 5d3a 2049 6d61 6765  t.Tensor]: Image
+000164a0: 2074 6f20 6265 2074 7261 6e73 666f 726d   to be transform
+000164b0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+000164c0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+000164d0: 7463 683a 6f70 7469 6f6e 616c 5d2c 207b  tch:optional], {
+000164e0: 6e5f 6368 616e 6e65 6c3a 6f70 7469 6f6e  n_channel:option
+000164f0: 616c 7d2c 206e 4031 2c20 6e40 322c 202e  al}, n@1, n@2, .
+00016500: 2e2e 2c20 6e40 6e5f 6469 6d29 0a20 2020  .., n@n_dim).   
+00016510: 2020 2020 2020 2020 206f 7574 7075 7420           output 
+00016520: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
+00016530: 2074 7261 6e73 666f 726d 6564 2069 6d61   transformed ima
+00016540: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
+00016550: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+00016560: 7463 685d 2c20 7b6e 5f63 6861 6e6e 656c  tch], {n_channel
+00016570: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
+00016580: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
+00016590: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+000165a0: 6620 6c65 6e28 5f72 616e 6765 2920 3d3d  f len(_range) ==
+000165b0: 2030 3a20 5f72 616e 6765 203d 204e 6f6e   0: _range = Non
+000165c0: 650a 2020 2020 2020 2020 656c 6966 206c  e.        elif l
+000165d0: 656e 285f 7261 6e67 6529 203d 3d20 3120  en(_range) == 1 
+000165e0: 616e 6420 6973 696e 7374 616e 6365 285f  and isinstance(_
+000165f0: 7261 6e67 655b 305d 2c20 286c 6973 742c  range[0], (list,
+00016600: 2074 7570 6c65 2929 3a20 5f72 616e 6765   tuple)): _range
+00016610: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
+00016620: 7228 6c69 7374 285f 7261 6e67 655b 305d  r(list(_range[0]
+00016630: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
+00016640: 6c65 6e28 5f72 616e 6765 2920 3d3d 2031  len(_range) == 1
+00016650: 2061 6e64 2069 7369 6e73 7461 6e63 6528   and isinstance(
+00016660: 5f72 616e 6765 5b30 5d2c 2062 742e 5465  _range[0], bt.Te
+00016670: 6e73 6f72 293a 205f 7261 6e67 6520 3d20  nsor): _range = 
+00016680: 5f72 616e 6765 5b30 5d0a 2020 2020 2020  _range[0].      
+00016690: 2020 656c 6966 206c 656e 285f 7261 6e67    elif len(_rang
+000166a0: 6529 203d 3d20 313a 205f 7261 6e67 6520  e) == 1: _range 
+000166b0: 3d20 6274 2e63 6861 6e6e 656c 5f74 656e  = bt.channel_ten
+000166c0: 736f 7228 2830 2c20 5f72 616e 6765 2929  sor((0, _range))
+000166d0: 0a20 2020 2020 2020 2065 6c69 6620 6c65  .        elif le
+000166e0: 6e28 5f72 616e 6765 2920 3d3d 2032 3a20  n(_range) == 2: 
+000166f0: 5f72 616e 6765 203d 2062 742e 6368 616e  _range = bt.chan
+00016700: 6e65 6c5f 7465 6e73 6f72 285f 7261 6e67  nel_tensor(_rang
+00016710: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+00016720: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+00016730: 2866 2249 6e76 616c 6964 2072 616e 6765  (f"Invalid range
+00016740: 2066 6f72 204e 6f72 6d61 6c69 7a65 3a20   for Normalize: 
+00016750: 7b5f 7261 6e67 657d 2e20 2229 0a20 2020  {_range}. ").   
+00016760: 2020 2020 2069 6620 5f72 616e 6765 2069       if _range i
+00016770: 7320 4e6f 6e65 3a20 7061 7373 0a20 2020  s None: pass.   
+00016780: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00016790: 2020 2020 2020 2069 6620 5f72 616e 6765         if _range
+000167a0: 2e6e 5f64 696d 203c 2032 3a20 5f72 616e  .n_dim < 2: _ran
+000167b0: 6765 203d 205f 7261 6e67 652e 756e 7371  ge = _range.unsq
+000167c0: 7565 657a 6528 5b5d 290a 2020 2020 2020  ueeze([]).      
+000167d0: 2020 2020 2020 6966 206e 6f74 205f 7261        if not _ra
+000167e0: 6e67 652e 6861 735f 6261 7463 683a 205f  nge.has_batch: _
+000167f0: 7261 6e67 652e 6261 7463 685f 6469 6d65  range.batch_dime
+00016800: 6e73 696f 6e20 3d20 300a 2020 2020 2020  nsion = 0.      
+00016810: 2020 2020 2020 6966 206e 6f74 205f 7261        if not _ra
+00016820: 6e67 652e 6861 735f 6368 616e 6e65 6c3a  nge.has_channel:
+00016830: 205f 7261 6e67 652e 6368 616e 6e65 6c5f   _range.channel_
+00016840: 6469 6d65 6e73 696f 6e20 3d20 310a 2020  dimension = 1.  
+00016850: 2020 2020 2020 2020 2020 6176 6f75 6368            avouch
+00016860: 285f 7261 6e67 652e 6861 735f 6261 7463  (_range.has_batc
+00016870: 6820 616e 6420 5f72 616e 6765 2e68 6173  h and _range.has
+00016880: 5f63 6861 6e6e 656c 2c20 6622 506c 6561  _channel, f"Plea
+00016890: 7365 2075 7365 2062 6174 6f72 6368 2074  se use batorch t
+000168a0: 656e 736f 7220 6f66 2073 697a 6520 5c0a  ensor of size \.
+000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168c0: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
+000168d0: 616c 5d2c 207b 7b32 7d7d 2920 666f 7220  al], {{2}}) for 
+000168e0: 4e6f 726d 616c 697a 696e 6720 7061 7261  Normalizing para
+000168f0: 6d65 7465 7273 2c20 696e 7374 6561 6420  meters, instead 
+00016900: 6f66 207b 5f72 616e 6765 2e73 6861 7065  of {_range.shape
+00016910: 7d2e 2022 290a 2020 2020 2020 2020 7375  }. ").        su
+00016920: 7065 7228 292e 5f5f 696e 6974 5f5f 285f  per().__init__(_
+00016930: 7261 6e67 6529 0a20 2020 2020 2020 2073  range).        s
+00016940: 656c 662e 7261 6e67 6520 3d20 5f72 616e  elf.range = _ran
+00016950: 6765 0a20 2020 2020 2020 2073 656c 662e  ge.        self.
+00016960: 5f72 616e 6765 203d 204e 6f6e 650a 0a20  _range = None.. 
+00016970: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
+00016980: 7365 6c66 2c20 5829 3a0a 2020 2020 2020  self, X):.      
+00016990: 2020 5820 3d20 7375 7065 7228 292e 5f5f    X = super().__
+000169a0: 6361 6c6c 5f5f 2858 290a 2020 2020 2020  call__(X).      
+000169b0: 2020 5f72 616e 6765 203d 2073 656c 662e    _range = self.
+000169c0: 7261 6e67 650a 2020 2020 2020 2020 6966  range.        if
+000169d0: 205f 7261 6e67 6520 6973 204e 6f6e 653a   _range is None:
+000169e0: 0a20 2020 2020 2020 2020 2020 205f 7261  .            _ra
+000169f0: 6e67 6520 3d20 6274 2e71 7561 6e74 696c  nge = bt.quantil
+00016a00: 6528 582e 666c 6174 7465 6e28 292e 666c  e(X.flatten().fl
+00016a10: 6f61 7428 292c 2062 6174 6f72 6368 5f74  oat(), batorch_t
+00016a20: 656e 736f 7228 5b30 2e30 3235 2c20 302e  ensor([0.025, 0.
+00016a30: 3937 355d 292c 2061 7869 733d 2d31 292e  975]), axis=-1).
+00016a40: 6d6f 7665 6469 6d28 302c 202d 3129 2e73  movedim(0, -1).s
+00016a50: 7065 6369 616c 5f66 726f 6d5f 2858 290a  pecial_from_(X).
+00016a60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016a70: 2e5f 7261 6e67 6520 3d20 5f72 616e 6765  ._range = _range
+00016a80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00016a90: 2828 5820 2d20 5f72 616e 6765 5b2e 2e2e  ((X - _range[...
+00016aa0: 2c20 305d 2920 2f20 285f 7261 6e67 655b  , 0]) / (_range[
+00016ab0: 2e2e 2e2c 2031 5d20 2d20 5f72 616e 6765  ..., 1] - _range
+00016ac0: 5b2e 2e2e 2c20 305d 2929 2e63 6c61 6d70  [..., 0])).clamp
+00016ad0: 2830 2e2c 2031 2e29 0a20 2020 200a 2020  (0., 1.).    .  
+00016ae0: 2020 6465 6620 696e 7628 7365 6c66 293a    def inv(self):
+00016af0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00016b00: 2e72 616e 6765 2069 7320 6e6f 7420 4e6f  .range is not No
+00016b10: 6e65 3a20 5f72 616e 6765 203d 2073 656c  ne: _range = sel
+00016b20: 662e 7261 6e67 650a 2020 2020 2020 2020  f.range.        
+00016b30: 656c 6966 2073 656c 662e 5f72 616e 6765  elif self._range
+00016b40: 2069 7320 6e6f 7420 4e6f 6e65 3a20 5f72   is not None: _r
+00016b50: 616e 6765 203d 2073 656c 662e 5f72 616e  ange = self._ran
+00016b60: 6765 0a20 2020 2020 2020 2065 6c73 653a  ge.        else:
+00016b70: 2072 6574 7572 6e20 4e6f 726d 616c 697a   return Normaliz
+00016b80: 6528 4e6f 6e65 290a 2020 2020 2020 2020  e(None).        
+00016b90: 6465 6e20 3d20 5f72 616e 6765 5b2e 2e2e  den = _range[...
+00016ba0: 2c20 315d 202d 205f 7261 6e67 655b 2e2e  , 1] - _range[..
+00016bb0: 2e2c 2030 5d0a 2020 2020 2020 2020 5f72  ., 0].        _r
+00016bc0: 616e 6765 203d 2062 742e 7374 6163 6b28  ange = bt.stack(
+00016bd0: 2d5f 7261 6e67 655b 2e2e 2e2c 2030 5d2c  -_range[..., 0],
+00016be0: 2031 2d5f 7261 6e67 655b 2e2e 2e2c 2030   1-_range[..., 0
+00016bf0: 5d2c 202d 3129 202f 2064 656e 0a20 2020  ], -1) / den.   
+00016c00: 2020 2020 2072 6574 7572 6e20 4e6f 726d       return Norm
+00016c10: 616c 697a 6528 5f72 616e 6765 290a 0a23  alize(_range)..#
+00016c20: 2323 2323 2323 2323 2323 2323 2053 7570  ############ Sup
+00016c30: 706f 7274 696e 6720 4675 6e63 7469 6f6e  porting Function
+00016c40: 7320 2323 2323 2323 2323 2323 2323 0a0a  s ############..
+00016c50: 6465 6620 4273 706c 696e 6528 692c 2055  def Bspline(i, U
+00016c60: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
+00016c70: 7562 6963 2042 2d73 706c 696e 6520 6675  ubic B-spline fu
+00016c80: 6e63 7469 6f6e 2e20 0a20 2020 204e 6f74  nction. .    Not
+00016c90: 653a 2041 7320 6c6f 6e67 2061 7320 6920  e: As long as i 
+00016ca0: 616e 6420 5520 6861 7665 2074 6865 2073  and U have the s
+00016cb0: 616d 6520 7369 7a65 2c20 616e 7920 7368  ame size, any sh
+00016cc0: 6170 6520 6f66 2074 656e 736f 7273 2077  ape of tensors w
+00016cd0: 6f75 6c64 2064 6f2e 0a20 2020 200a 2020  ould do..    .  
+00016ce0: 2020 5061 7261 6d73 3a0a 2020 2020 2020    Params:.      
+00016cf0: 2020 6920 5b62 742e 5465 6e73 6f72 5d3a    i [bt.Tensor]:
+00016d00: 2074 6865 2069 6e64 6578 206f 6620 7365   the index of se
+00016d10: 676d 656e 7420 6675 6e63 7469 6f6e 206f  gment function o
+00016d20: 6620 422d 7370 6c69 6e65 2e0a 2020 2020  f B-spline..    
+00016d30: 2020 2020 2020 2020 5468 6520 7661 6c75          The valu
+00016d40: 6520 6f66 2065 6163 6820 656c 656d 656e  e of each elemen
+00016d50: 7420 6361 6e20 6265 2063 686f 7365 6e20  t can be chosen 
+00016d60: 696e 2028 2d31 2c20 302c 2031 2c20 3229  in (-1, 0, 1, 2)
+00016d70: 2e20 0a20 2020 2020 2020 2055 205b 6274  . .        U [bt
+00016d80: 2e54 656e 736f 725d 3a20 7468 6520 6465  .Tensor]: the de
+00016d90: 6369 6d61 6c20 6172 6775 6d65 6e74 206f  cimal argument o
+00016da0: 6620 422d 7370 6c69 6e65 2066 756e 6374  f B-spline funct
+00016db0: 696f 6e2e 2049 7420 7368 6f75 6c64 2062  ion. It should b
+00016dc0: 6520 7769 7468 696e 2072 616e 6765 205b  e within range [
+00016dd0: 302c 2031 292e 0a20 2020 2022 2222 0a20  0, 1)..    """. 
+00016de0: 2020 2069 203d 2062 6174 6f72 6368 5f74     i = batorch_t
+00016df0: 656e 736f 7228 6929 3b20 5520 3d20 6261  ensor(i); U = ba
+00016e00: 746f 7263 685f 7465 6e73 6f72 2855 290a  torch_tensor(U).
+00016e10: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+00016e20: 2020 2020 2062 742e 7768 6572 6528 6920       bt.where(i 
+00016e30: 3d3d 202d 312c 2028 3120 2d20 5529 202a  == -1, (1 - U) *
+00016e40: 2a20 3320 2f20 362c 0a20 2020 2020 2020  * 3 / 6,.       
+00016e50: 2062 742e 7768 6572 6528 6920 3d3d 2030   bt.where(i == 0
+00016e60: 2c20 5520 2a2a 2033 202f 2032 202d 2055  , U ** 3 / 2 - U
+00016e70: 202a 2055 202b 2032 202f 2033 2c0a 2020   * U + 2 / 3,.  
+00016e80: 2020 2020 2020 6274 2e77 6865 7265 2869        bt.where(i
+00016e90: 203d 3d20 312c 2028 2d20 3320 2a20 5520   == 1, (- 3 * U 
+00016ea0: 2a2a 2033 202b 2033 202a 2055 202a 2055  ** 3 + 3 * U * U
+00016eb0: 202b 2033 202a 2055 202b 2031 2920 2f20   + 3 * U + 1) / 
+00016ec0: 362c 0a20 2020 2020 2020 2062 742e 7768  6,.        bt.wh
+00016ed0: 6572 6528 6920 3d3d 2032 2c20 5520 2a2a  ere(i == 2, U **
+00016ee0: 2033 202f 2036 2c0a 2020 2020 2020 2020   3 / 6,.        
+00016ef0: 6274 2e7a 6572 6f73 5f6c 696b 6528 5529  bt.zeros_like(U)
+00016f00: 2929 2929 0a20 2020 2029 0a0a 6465 6620  )))).    )..def 
+00016f10: 6442 7370 6c69 6e65 2869 2c20 5529 3a0a  dBspline(i, U):.
+00016f20: 2020 2020 2222 220a 2020 2020 5468 6520      """.    The 
+00016f30: 6465 7269 7661 7469 7665 206f 6620 422d  derivative of B-
+00016f40: 7370 6c69 6e65 2066 756e 6374 696f 6e2c  spline function,
+00016f50: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
+00016f60: 2055 2e20 0a20 2020 204e 6f74 653a 2041   U. .    Note: A
+00016f70: 7320 6c6f 6e67 2061 7320 6920 616e 6420  s long as i and 
+00016f80: 5520 6861 7665 2074 6865 2073 616d 6520  U have the same 
+00016f90: 7369 7a65 2c20 616e 7920 7368 6170 6520  size, any shape 
+00016fa0: 6f66 2074 656e 736f 7273 2077 6f75 6c64  of tensors would
+00016fb0: 2064 6f2e 0a20 2020 200a 2020 2020 5061   do..    .    Pa
+00016fc0: 7261 6d73 3a0a 2020 2020 2020 2020 6920  rams:.        i 
+00016fd0: 5b62 742e 5465 6e73 6f72 5d3a 2074 6865  [bt.Tensor]: the
+00016fe0: 2069 6e64 6578 206f 6620 7365 676d 656e   index of segmen
+00016ff0: 7420 6675 6e63 7469 6f6e 206f 6620 422d  t function of B-
+00017000: 7370 6c69 6e65 2e0a 2020 2020 2020 2020  spline..        
+00017010: 2020 2020 5468 6520 7661 6c75 6520 6f66      The value of
+00017020: 2065 6163 6820 656c 656d 656e 7420 6361   each element ca
+00017030: 6e20 6265 2063 686f 7365 6e20 696e 2028  n be chosen in (
+00017040: 2d31 2c20 302c 2031 2c20 3229 2e20 0a20  -1, 0, 1, 2). . 
+00017050: 2020 2020 2020 2055 205b 6274 2e54 656e         U [bt.Ten
+00017060: 736f 725d 3a20 7468 6520 6465 6369 6d61  sor]: the decima
+00017070: 6c20 6172 6775 6d65 6e74 206f 6620 422d  l argument of B-
+00017080: 7370 6c69 6e65 2066 756e 6374 696f 6e2e  spline function.
+00017090: 2049 7420 7368 6f75 6c64 2062 6520 7769   It should be wi
+000170a0: 7468 696e 2072 616e 6765 205b 302c 2031  thin range [0, 1
+000170b0: 292e 0a20 2020 2022 2222 0a20 2020 2069  )..    """.    i
+000170c0: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
+000170d0: 7228 6929 3b20 5520 3d20 6261 746f 7263  r(i); U = batorc
+000170e0: 685f 7465 6e73 6f72 2855 290a 2020 2020  h_tensor(U).    
+000170f0: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
+00017100: 2062 742e 7768 6572 6528 6920 3d3d 202d   bt.where(i == -
+00017110: 312c 202d 2033 202a 2028 3120 2d20 5529  1, - 3 * (1 - U)
+00017120: 202a 2a20 3220 2f20 362c 0a20 2020 2020   ** 2 / 6,.     
+00017130: 2020 2062 742e 7768 6572 6528 6920 3d3d     bt.where(i ==
+00017140: 2030 2c20 3320 2a20 5520 2a2a 2032 202f   0, 3 * U ** 2 /
+00017150: 2032 202d 2032 202a 2055 2c0a 2020 2020   2 - 2 * U,.    
+00017160: 2020 2020 6274 2e77 6865 7265 2869 203d      bt.where(i =
+00017170: 3d20 312c 2028 2d20 3320 2a20 5520 2a2a  = 1, (- 3 * U **
+00017180: 2032 202b 2032 202a 2055 202b 2031 2920   2 + 2 * U + 1) 
+00017190: 2f20 322c 0a20 2020 2020 2020 2062 742e  / 2,.        bt.
+000171a0: 7768 6572 6528 6920 3d3d 2032 2c20 3320  where(i == 2, 3 
+000171b0: 2a20 5520 2a2a 2032 202f 2036 2c0a 2020  * U ** 2 / 6,.  
+000171c0: 2020 2020 2020 6274 2e7a 6572 6f73 5f6c        bt.zeros_l
+000171d0: 696b 6528 5529 2929 2929 0a20 2020 2029  ike(U))))).    )
+000171e0: 0a0a 6465 6620 6642 7370 6c69 6e65 2863  ..def fBspline(c
+000171f0: 2c20 7829 3a0a 2020 2020 6320 3d20 6261  , x):.    c = ba
+00017200: 746f 7263 685f 7465 6e73 6f72 2863 293b  torch_tensor(c);
+00017210: 2078 203d 2062 6174 6f72 6368 5f74 656e   x = batorch_ten
+00017220: 736f 7228 7829 0a20 2020 2064 203d 2078  sor(x).    d = x
+00017230: 202d 2063 0a20 2020 2072 6574 7572 6e20   - c.    return 
+00017240: 280a 2020 2020 2020 2020 6274 2e77 6865  (.        bt.whe
+00017250: 7265 2828 2d32 203c 3d20 6429 202a 2028  re((-2 <= d) * (
+00017260: 6420 3c20 2d31 292c 2064 202a 2a20 3320  d < -1), d ** 3 
+00017270: 2b20 3620 2a20 6420 2a2a 2032 202b 2031  + 6 * d ** 2 + 1
+00017280: 3220 2a20 6420 2b20 382c 0a20 2020 2020  2 * d + 8,.     
+00017290: 2020 2062 742e 7768 6572 6528 282d 3120     bt.where((-1 
+000172a0: 3c3d 2064 2920 2a20 2864 203c 2030 292c  <= d) * (d < 0),
+000172b0: 202d 2033 202a 2064 202a 2a20 3320 2d20   - 3 * d ** 3 - 
+000172c0: 3620 2a20 6420 2a2a 2032 202b 2034 2c0a  6 * d ** 2 + 4,.
+000172d0: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
+000172e0: 2828 3020 3c3d 2064 2920 2a20 2864 203c  ((0 <= d) * (d <
+000172f0: 2031 292c 2033 202a 2064 202a 2a20 3320   1), 3 * d ** 3 
+00017300: 2d20 3620 2a20 6420 2a2a 2032 202b 2034  - 6 * d ** 2 + 4
+00017310: 2c0a 2020 2020 2020 2020 6274 2e77 6865  ,.        bt.whe
+00017320: 7265 2828 3120 3c3d 2064 2920 2a20 2864  re((1 <= d) * (d
+00017330: 203c 2032 292c 202d 2064 202a 2a20 3320   < 2), - d ** 3 
+00017340: 2b20 3620 2a20 6420 2a2a 2032 202d 2031  + 6 * d ** 2 - 1
+00017350: 3220 2a20 6420 2b20 382c 0a20 2020 2020  2 * d + 8,.     
+00017360: 2020 2062 742e 7a65 726f 735f 6c69 6b65     bt.zeros_like
+00017370: 2864 2929 2929 2920 2f20 360a 2020 2020  (d))))) / 6.    
+00017380: 290a 0a64 6566 2041 6666 696e 6532 4432  )..def Affine2D2
+00017390: 4d61 7472 6978 2870 6172 616d 7329 3a0a  Matrix(params):.
+000173a0: 2020 2020 2222 220a 2020 2020 7431 2c20      """.    t1, 
+000173b0: 7432 2c20 ceb8 2c20 7331 2c20 7332 2c20  t2, .., s1, s2, 
+000173c0: cf81 312c 20cf 8132 2069 6e20 7369 7a65  ..1, ..2 in size
+000173d0: 3a20 285b 6e5f 6261 7463 685d 2c20 7b37  : ([n_batch], {7
+000173e0: 7d29 0a20 2020 2074 312c 2074 322c 2063  }).    t1, t2, c
+000173f0: 312c 2063 322c 20ce b82c 2073 312c 2073  1, c2, .., s1, s
+00017400: 322c 20cf 8131 2c20 cf81 3220 696e 2073  2, ..1, ..2 in s
+00017410: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
+00017420: 207b 397d 290a 2020 2020 6f75 7470 7574   {9}).    output
+00017430: 2069 6e20 7369 7a65 3a20 285b 6e5f 6261   in size: ([n_ba
+00017440: 7463 685d 2c20 332c 2033 290a 2020 2020  tch], 3, 3).    
+00017450: 2222 220a 2020 2020 7061 7261 6d73 203d  """.    params =
+00017460: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+00017470: 7061 7261 6d73 290a 2020 2020 6966 2070  params).    if p
+00017480: 6172 616d 732e 6e5f 6469 6d20 3c3d 2031  arams.n_dim <= 1
+00017490: 2061 6e64 206e 6f74 2070 6172 616d 732e   and not params.
+000174a0: 6861 735f 6261 7463 683a 2070 6172 616d  has_batch: param
+000174b0: 7320 3d20 7061 7261 6d73 2e75 6e73 7175  s = params.unsqu
+000174c0: 6565 7a65 285b 5d29 0a20 2020 2069 6620  eeze([]).    if 
+000174d0: 7061 7261 6d73 2e6e 5f64 696d 203c 3d20  params.n_dim <= 
+000174e0: 3120 616e 6420 6e6f 7420 7061 7261 6d73  1 and not params
+000174f0: 2e68 6173 5f63 6861 6e6e 656c 3a20 7061  .has_channel: pa
+00017500: 7261 6d73 203d 2070 6172 616d 732e 756e  rams = params.un
+00017510: 7371 7565 657a 6528 7b31 7d29 0a20 2020  squeeze({1}).   
+00017520: 2069 6620 7061 7261 6d73 2e6e 5f64 696d   if params.n_dim
+00017530: 203d 3d20 3220 616e 6420 6e6f 7420 7061   == 2 and not pa
+00017540: 7261 6d73 2e68 6173 5f62 6174 6368 3a20  rams.has_batch: 
+00017550: 7061 7261 6d73 2e62 6174 6368 5f64 696d  params.batch_dim
+00017560: 656e 7369 6f6e 203d 2030 0a20 2020 2069  ension = 0.    i
+00017570: 6620 7061 7261 6d73 2e6e 5f64 696d 203d  f params.n_dim =
+00017580: 3d20 3220 616e 6420 6e6f 7420 7061 7261  = 2 and not para
+00017590: 6d73 2e68 6173 5f63 6861 6e6e 656c 3a20  ms.has_channel: 
+000175a0: 7061 7261 6d73 2e63 6861 6e6e 656c 5f64  params.channel_d
+000175b0: 696d 656e 7369 6f6e 203d 2031 0a20 2020  imension = 1.   
+000175c0: 2061 766f 7563 6828 7061 7261 6d73 2e68   avouch(params.h
+000175d0: 6173 5f62 6174 6368 2c20 6622 506c 6561  as_batch, f"Plea
+000175e0: 7365 2075 7365 2062 6174 6f72 6368 2074  se use batorch t
+000175f0: 656e 736f 7220 6f66 2073 697a 6520 285b  ensor of size ([
+00017600: 6e5f 6261 7463 685d 2c20 7b37 206f 7220  n_batch], {7 or 
+00017610: 397d 2920 5c0a 2020 2020 2020 2020 666f  9}) \.        fo
+00017620: 7220 4166 6669 6e65 2070 6172 616d 6574  r Affine paramet
+00017630: 6572 732c 2069 6e73 7465 6164 206f 6620  ers, instead of 
+00017640: 7b70 6172 616d 732e 7368 6170 657d 2e20  {params.shape}. 
+00017650: 2229 0a20 2020 206e 5f62 6174 6368 203d  ").    n_batch =
+00017660: 2070 6172 616d 732e 6e5f 6261 7463 680a   params.n_batch.
+00017670: 2020 2020 6966 2070 6172 616d 732e 7369      if params.si
+00017680: 7a65 2831 2920 3d3d 2037 3a0a 2020 2020  ze(1) == 7:.    
+00017690: 2020 2020 7431 2c20 7432 2c20 ceb8 2c20      t1, t2, .., 
+000176a0: 7331 2c20 7332 2c20 cf81 312c 20cf 8132  s1, s2, ..1, ..2
+000176b0: 203d 2070 6172 616d 732e 7370 6c69 7428   = params.split(
+000176c0: 290a 2020 2020 2020 2020 6331 203d 2062  ).        c1 = b
+000176d0: 742e 7a65 726f 7328 5b6e 5f62 6174 6368  t.zeros([n_batch
+000176e0: 5d2c 2031 293b 2063 3220 3d20 6274 2e7a  ], 1); c2 = bt.z
+000176f0: 6572 6f73 285b 6e5f 6261 7463 685d 2c20  eros([n_batch], 
+00017700: 3129 0a20 2020 2069 6620 7061 7261 6d73  1).    if params
+00017710: 2e73 697a 6528 3129 203d 3d20 393a 0a20  .size(1) == 9:. 
+00017720: 2020 2020 2020 2074 312c 2074 322c 2063         t1, t2, c
+00017730: 312c 2063 322c 20ce b82c 2073 312c 2073  1, c2, .., s1, s
+00017740: 322c 20cf 8131 2c20 cf81 3220 3d20 7061  2, ..1, ..2 = pa
+00017750: 7261 6d73 2e73 706c 6974 2829 0a20 2020  rams.split().   
+00017760: 2061 203d 2028 cf81 3120 2a20 cf81 3220   a = (..1 * ..2 
+00017770: 2b20 3129 202a 2073 3120 2a20 6274 2e63  + 1) * s1 * bt.c
+00017780: 6f73 28ce b829 202b 20cf 8131 202a 2073  os(..) + ..1 * s
+00017790: 3220 2a20 6274 2e73 696e 28ce b829 0a20  2 * bt.sin(..). 
+000177a0: 2020 2062 203d 202d 2028 cf81 3120 2a20     b = - (..1 * 
+000177b0: cf81 3220 2b20 3129 202a 2073 3120 2a20  ..2 + 1) * s1 * 
+000177c0: 6274 2e73 696e 28ce b829 202b 20cf 8131  bt.sin(..) + ..1
+000177d0: 202a 2073 3220 2a20 6274 2e63 6f73 28ce   * s2 * bt.cos(.
+000177e0: b829 0a20 2020 2063 203d 20cf 8132 202a  .).    c = ..2 *
+000177f0: 2073 3120 2a20 6274 2e63 6f73 28ce b829   s1 * bt.cos(..)
+00017800: 202b 2073 3220 2a20 6274 2e73 696e 28ce   + s2 * bt.sin(.
+00017810: b829 0a20 2020 2064 203d 202d 20cf 8132  .).    d = - ..2
+00017820: 202a 2073 3120 2a20 6274 2e73 696e 28ce   * s1 * bt.sin(.
+00017830: b829 202b 2073 3220 2a20 6274 2e63 6f73  .) + s2 * bt.cos
+00017840: 28ce b829 0a20 2020 2072 6574 7572 6e20  (..).    return 
+00017850: 6274 2e63 6174 280a 2020 2020 2020 2020  bt.cat(.        
+00017860: 6274 2e63 6174 2828 612c 2062 2c20 7431  bt.cat((a, b, t1
+00017870: 202d 2061 202a 2063 3120 2d20 6220 2a20   - a * c1 - b * 
+00017880: 6332 202b 2063 312c 2063 2c20 642c 2074  c2 + c1, c, d, t
+00017890: 3220 2d20 6320 2a20 6331 202d 2064 202a  2 - c * c1 - d *
+000178a0: 2063 3220 2b20 6332 292c 207b 7d29 2e76   c2 + c2), {}).v
+000178b0: 6965 7728 5b6e 5f62 6174 6368 5d2c 2032  iew([n_batch], 2
+000178c0: 2c20 3329 2c20 0a20 2020 2020 2020 2062  , 3), .        b
+000178d0: 742e 6f6e 655f 686f 7428 2d31 2c20 3329  t.one_hot(-1, 3)
+000178e0: 2e6d 756c 7469 706c 7928 6e5f 6261 7463  .multiply(n_batc
+000178f0: 682c 205b 5d29 2e76 6965 7728 5b6e 5f62  h, []).view([n_b
+00017900: 6174 6368 5d2c 2031 2c20 3329 2c20 310a  atch], 1, 3), 1.
+00017910: 2020 2020 290a 0a64 6566 2051 7561 7465      )..def Quate
+00017920: 726e 7332 4d61 7472 6978 2870 6172 616d  rns2Matrix(param
+00017930: 7329 3a0a 2020 2020 2222 220a 2020 2020  s):.    """.    
+00017940: 2020 2020 5175 6174 6572 6e3a 2071 622c      Quatern: qb,
+00017950: 2071 632c 2071 642c 2070 782c 2070 792c   qc, qd, px, py,
+00017960: 2070 7a20 696e 2073 697a 653a 2028 5b6e   pz in size: ([n
+00017970: 5f62 6174 6368 5d2c 207b 367d 290a 2020  _batch], {6}).  
+00017980: 2020 2020 2020 4d61 7472 6978 3a20 285b        Matrix: ([
+00017990: 6e5f 6261 7463 685d 2c20 342c 2034 290a  n_batch], 4, 4).
+000179a0: 2020 2020 2222 220a 2020 2020 7061 7261      """.    para
+000179b0: 6d73 203d 2062 6174 6f72 6368 5f74 656e  ms = batorch_ten
+000179c0: 736f 7228 7061 7261 6d73 290a 2020 2020  sor(params).    
+000179d0: 6966 2070 6172 616d 732e 6e5f 6469 6d20  if params.n_dim 
+000179e0: 3c3d 2031 2061 6e64 206e 6f74 2070 6172  <= 1 and not par
+000179f0: 616d 732e 6861 735f 6261 7463 683a 2070  ams.has_batch: p
+00017a00: 6172 616d 7320 3d20 7061 7261 6d73 2e75  arams = params.u
+00017a10: 6e73 7175 6565 7a65 285b 5d29 0a20 2020  nsqueeze([]).   
+00017a20: 2069 6620 7061 7261 6d73 2e6e 5f64 696d   if params.n_dim
+00017a30: 203c 3d20 3120 616e 6420 6e6f 7420 7061   <= 1 and not pa
+00017a40: 7261 6d73 2e68 6173 5f63 6861 6e6e 656c  rams.has_channel
+00017a50: 3a20 7061 7261 6d73 203d 2070 6172 616d  : params = param
+00017a60: 732e 756e 7371 7565 657a 6528 7b31 7d29  s.unsqueeze({1})
+00017a70: 0a20 2020 2069 6620 7061 7261 6d73 2e6e  .    if params.n
+00017a80: 5f64 696d 203d 3d20 3220 616e 6420 6e6f  _dim == 2 and no
+00017a90: 7420 7061 7261 6d73 2e68 6173 5f62 6174  t params.has_bat
+00017aa0: 6368 3a20 7061 7261 6d73 2e62 6174 6368  ch: params.batch
+00017ab0: 5f64 696d 656e 7369 6f6e 203d 2030 0a20  _dimension = 0. 
+00017ac0: 2020 2069 6620 7061 7261 6d73 2e6e 5f64     if params.n_d
+00017ad0: 696d 203d 3d20 3220 616e 6420 6e6f 7420  im == 2 and not 
+00017ae0: 7061 7261 6d73 2e68 6173 5f63 6861 6e6e  params.has_chann
+00017af0: 656c 3a20 7061 7261 6d73 2e63 6861 6e6e  el: params.chann
+00017b00: 656c 5f64 696d 656e 7369 6f6e 203d 2031  el_dimension = 1
+00017b10: 0a20 2020 2061 766f 7563 6828 7061 7261  .    avouch(para
+00017b20: 6d73 2e6e 5f64 696d 203d 3d20 3220 616e  ms.n_dim == 2 an
+00017b30: 6420 7061 7261 6d73 2e68 6173 5f62 6174  d params.has_bat
+00017b40: 6368 2061 6e64 2070 6172 616d 732e 6861  ch and params.ha
+00017b50: 735f 6368 616e 6e65 6c2c 200a 2020 2020  s_channel, .    
+00017b60: 2020 2020 2020 2066 2250 6c65 6173 6520         f"Please 
+00017b70: 7573 6520 6261 746f 7263 6820 7465 6e73  use batorch tens
+00017b80: 6f72 206f 6620 7369 7a65 2028 5b6e 5f62  or of size ([n_b
+00017b90: 6174 6368 5d2c 207b 7b36 7d7d 2920 666f  atch], {{6}}) fo
+00017ba0: 7220 4166 6669 6e65 2070 6172 616d 6574  r Affine paramet
+00017bb0: 6572 732c 2069 6e73 7465 6164 206f 6620  ers, instead of 
+00017bc0: 7b70 6172 616d 732e 7368 6170 657d 2e20  {params.shape}. 
+00017bd0: 2229 0a20 2020 206e 5f62 6174 6368 203d  ").    n_batch =
+00017be0: 2070 6172 616d 732e 6e5f 6261 7463 680a   params.n_batch.
+00017bf0: 2020 2020 622c 2063 2c20 642c 2078 2c20      b, c, d, x, 
+00017c00: 792c 207a 203d 2070 6172 616d 732e 7370  y, z = params.sp
+00017c10: 6c69 7428 290a 2020 2020 6120 3d20 6274  lit().    a = bt
+00017c20: 2e73 7172 7428 2831 2d62 2a62 2d63 2a63  .sqrt((1-b*b-c*c
+00017c30: 2d64 2a64 292e 636c 616d 7028 3029 290a  -d*d).clamp(0)).
+00017c40: 2020 2020 5231 3120 3d20 612a 612b 622a      R11 = a*a+b*
+00017c50: 622d 632a 632d 642a 640a 2020 2020 5231  b-c*c-d*d.    R1
+00017c60: 3220 3d20 322a 622a 632d 322a 612a 640a  2 = 2*b*c-2*a*d.
+00017c70: 2020 2020 5231 3320 3d20 322a 622a 642b      R13 = 2*b*d+
+00017c80: 322a 612a 630a 2020 2020 5232 3120 3d20  2*a*c.    R21 = 
+00017c90: 322a 622a 632b 322a 612a 640a 2020 2020  2*b*c+2*a*d.    
+00017ca0: 5232 3220 3d20 612a 612b 632a 632d 622a  R22 = a*a+c*c-b*
+00017cb0: 622d 642a 640a 2020 2020 5232 3320 3d20  b-d*d.    R23 = 
+00017cc0: 322a 632a 642d 322a 612a 620a 2020 2020  2*c*d-2*a*b.    
+00017cd0: 5233 3120 3d20 322a 622a 642d 322a 612a  R31 = 2*b*d-2*a*
+00017ce0: 630a 2020 2020 5233 3220 3d20 322a 632a  c.    R32 = 2*c*
+00017cf0: 642b 322a 612a 620a 2020 2020 5233 3320  d+2*a*b.    R33 
+00017d00: 3d20 612a 612b 642a 642d 632a 632d 622a  = a*a+d*d-c*c-b*
+00017d10: 620a 2020 2020 7265 7475 726e 2062 742e  b.    return bt.
+00017d20: 6361 7428 0a20 2020 2020 2020 2062 742e  cat(.        bt.
+00017d30: 6361 7428 2852 3131 2c20 5231 322c 2052  cat((R11, R12, R
+00017d40: 3133 2c20 782c 2052 3231 2c20 5232 322c  13, x, R21, R22,
+00017d50: 2052 3233 2c20 792c 2052 3331 2c20 5233   R23, y, R31, R3
+00017d60: 322c 2052 3333 2c20 7a29 2c20 3129 2e76  2, R33, z), 1).v
+00017d70: 6965 7728 5b6e 5f62 6174 6368 5d2c 2033  iew([n_batch], 3
+00017d80: 2c20 3429 2c0a 2020 2020 2020 2020 6274  , 4),.        bt
+00017d90: 2e6f 6e65 5f68 6f74 282d 312c 2034 292e  .one_hot(-1, 4).
+00017da0: 6d75 6c74 6970 6c79 286e 5f62 6174 6368  multiply(n_batch
+00017db0: 2c20 5b5d 292e 7669 6577 285b 6e5f 6261  , []).view([n_ba
+00017dc0: 7463 685d 2c20 312c 2034 292c 2031 0a20  tch], 1, 4), 1. 
+00017dd0: 2020 2029 0a0a 6465 6620 4d61 7472 6978     )..def Matrix
+00017de0: 3251 7561 7465 726e 7328 7061 7261 6d73  2Quaterns(params
+00017df0: 293a 0a20 2020 2022 2222 0a20 2020 2020  ):.    """.     
+00017e00: 2020 204d 6174 7269 783a 2028 5b6e 5f62     Matrix: ([n_b
+00017e10: 6174 6368 5d2c 2034 2c20 3429 0a20 2020  atch], 4, 4).   
+00017e20: 2020 2020 2051 7561 7465 726e 3a20 7162       Quatern: qb
+00017e30: 2c20 7163 2c20 7164 2c20 7078 2c20 7079  , qc, qd, px, py
+00017e40: 2c20 707a 2069 6e20 7369 7a65 3a20 285b  , pz in size: ([
+00017e50: 6e5f 6261 7463 685d 2c20 7b36 7d29 0a20  n_batch], {6}). 
+00017e60: 2020 2022 2222 0a20 2020 2070 6172 616d     """.    param
+00017e70: 7320 3d20 6261 746f 7263 685f 7465 6e73  s = batorch_tens
+00017e80: 6f72 2870 6172 616d 7329 0a20 2020 2069  or(params).    i
+00017e90: 6620 7061 7261 6d73 2e6e 5f64 696d 203c  f params.n_dim <
+00017ea0: 3d20 3220 616e 6420 6e6f 7420 7061 7261  = 2 and not para
+00017eb0: 6d73 2e68 6173 5f62 6174 6368 3a20 7061  ms.has_batch: pa
+00017ec0: 7261 6d73 203d 2070 6172 616d 732e 756e  rams = params.un
+00017ed0: 7371 7565 657a 6528 5b5d 290a 2020 2020  squeeze([]).    
+00017ee0: 6966 2070 6172 616d 732e 6e5f 6469 6d20  if params.n_dim 
+00017ef0: 3d3d 2033 2061 6e64 206e 6f74 2070 6172  == 3 and not par
+00017f00: 616d 732e 6861 735f 6261 7463 683a 2070  ams.has_batch: p
+00017f10: 6172 616d 732e 6261 7463 685f 6469 6d65  arams.batch_dime
+00017f20: 6e73 696f 6e20 3d20 300a 2020 2020 6966  nsion = 0.    if
+00017f30: 2070 6172 616d 732e 6e5f 6469 6d20 3d3d   params.n_dim ==
+00017f40: 2033 2061 6e64 2070 6172 616d 732e 6861   3 and params.ha
+00017f50: 735f 6368 616e 6e65 6c3a 2070 6172 616d  s_channel: param
+00017f60: 732e 6368 616e 6e65 6c5f 6469 6d65 6e73  s.channel_dimens
+00017f70: 696f 6e20 3d20 4e6f 6e65 0a20 2020 2061  ion = None.    a
+00017f80: 766f 7563 6828 7061 7261 6d73 2e6e 5f64  vouch(params.n_d
+00017f90: 696d 203d 3d20 3320 616e 6420 7061 7261  im == 3 and para
+00017fa0: 6d73 2e68 6173 5f62 6174 6368 2061 6e64  ms.has_batch and
+00017fb0: 206e 6f74 2070 6172 616d 732e 6861 735f   not params.has_
+00017fc0: 6368 616e 6e65 6c2c 200a 2020 2020 2020  channel, .      
+00017fd0: 2020 2020 2066 2250 6c65 6173 6520 7573       f"Please us
+00017fe0: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
+00017ff0: 206f 6620 7369 7a65 2028 5b6e 5f62 6174   of size ([n_bat
+00018000: 6368 5d2c 2034 2c20 3429 2066 6f72 2041  ch], 4, 4) for A
+00018010: 6666 696e 6520 6d61 7472 6978 2c20 696e  ffine matrix, in
+00018020: 7374 6561 6420 6f66 207b 7061 7261 6d73  stead of {params
+00018030: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+00018040: 6e5f 6261 7463 6820 3d20 7061 7261 6d73  n_batch = params
+00018050: 2e6e 5f62 6174 6368 0a20 2020 2078 2c20  .n_batch.    x, 
+00018060: 792c 207a 203d 2070 6172 616d 735b 2e2e  y, z = params[..
+00018070: 2e2c 203a 332c 202d 315d 2e63 6861 6e6e  ., :3, -1].chann
+00018080: 656c 5f64 696d 5f28 3129 2e73 706c 6974  el_dim_(1).split
+00018090: 2831 2c20 3129 0a20 2020 2061 3220 3d20  (1, 1).    a2 = 
+000180a0: 2862 742e 6469 6167 2870 6172 616d 7329  (bt.diag(params)
+000180b0: 2e73 756d 2829 2e75 6e73 7175 6565 7a65  .sum().unsqueeze
+000180c0: 287b 7d29 202b 2031 2920 2f20 340a 2020  ({}) + 1) / 4.  
+000180d0: 2020 6120 3d20 6274 2e73 7172 7428 6132    a = bt.sqrt(a2
+000180e0: 290a 2020 2020 6232 203d 2061 3220 2d20  ).    b2 = a2 - 
+000180f0: 2870 6172 616d 735b 2e2e 2e2c 2031 2c20  (params[..., 1, 
+00018100: 315d 202b 2070 6172 616d 735b 2e2e 2e2c  1] + params[...,
+00018110: 2032 2c20 325d 2920 2f20 320a 2020 2020   2, 2]) / 2.    
+00018120: 6332 203d 2061 3220 2d20 2870 6172 616d  c2 = a2 - (param
+00018130: 735b 2e2e 2e2c 2032 2c20 325d 202b 2070  s[..., 2, 2] + p
+00018140: 6172 616d 735b 2e2e 2e2c 2030 2c20 305d  arams[..., 0, 0]
+00018150: 2920 2f20 320a 2020 2020 6432 203d 2061  ) / 2.    d2 = a
+00018160: 3220 2d20 2870 6172 616d 735b 2e2e 2e2c  2 - (params[...,
+00018170: 2030 2c20 305d 202b 2070 6172 616d 735b   0, 0] + params[
+00018180: 2e2e 2e2c 2031 2c20 315d 2920 2f20 320a  ..., 1, 1]) / 2.
+00018190: 2020 2020 4420 3d20 7061 7261 6d73 202d      D = params -
+000181a0: 2070 6172 616d 732e 540a 2020 2020 6220   params.T.    b 
+000181b0: 3d20 6274 2e73 6967 6e28 445b 2e2e 2e2c  = bt.sign(D[...,
+000181c0: 2032 2c20 315d 2920 2a20 6274 2e73 7172   2, 1]) * bt.sqr
+000181d0: 7428 6232 290a 2020 2020 6320 3d20 2d20  t(b2).    c = - 
+000181e0: 6274 2e73 6967 6e28 445b 2e2e 2e2c 2032  bt.sign(D[..., 2
+000181f0: 2c20 305d 2920 2a20 6274 2e73 7172 7428  , 0]) * bt.sqrt(
+00018200: 6332 290a 2020 2020 6420 3d20 6274 2e73  c2).    d = bt.s
+00018210: 6967 6e28 445b 2e2e 2e2c 2031 2c20 305d  ign(D[..., 1, 0]
+00018220: 2920 2a20 6274 2e73 7172 7428 6432 290a  ) * bt.sqrt(d2).
+00018230: 2020 2020 7265 7475 726e 2062 742e 6361      return bt.ca
+00018240: 7428 622c 2063 2c20 642c 2078 2c20 792c  t(b, c, d, x, y,
+00018250: 207a 2c20 7b7d 290a                       z, {}).
```

### Comparing `pycamia-1.0.36/micomputing/zxhtools/TRS.py` & `pycamia-1.0.37/micomputing/zxhtools/TRS.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc` & `pycamia-1.0.37/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc` & `pycamia-1.0.37/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc` & `pycamia-1.0.37/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc` & `pycamia-1.0.37/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/zxhtools/exec.py` & `pycamia-1.0.37/micomputing/zxhtools/exec.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/micomputing/zxhtools/image2.FFD` & `pycamia-1.0.37/micomputing/zxhtools/image2.FFD`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/__init__.py` & `pycamia-1.0.37/pycamia/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from .manager import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = '<main>',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.0.35',
-    update = '2023-07-05 16:28:39',
+    version = '1.0.36',
+    update = '2023-07-05 17:06:00',
     contact = 'bertiezhou@163.com',
     keywords = ['environment', 'path', 'touch'],
     description = 'The main package and a background support of project PyCAMIA. ',
     requires = []
 ).check()
 
 from .environment import get_environ_vars, get_environ_globals, get_environ_locals, update_locals_by_environ, get_args_expression, get_declaration, EnvironVars #*
```

### Comparing `pycamia-1.0.36/pycamia/decorators.py` & `pycamia-1.0.37/pycamia/decorators.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/environment.py` & `pycamia-1.0.37/pycamia/environment.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/exception.py` & `pycamia-1.0.37/pycamia/exception.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/functions.py` & `pycamia-1.0.37/pycamia/functions.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/inout.py` & `pycamia-1.0.37/pycamia/inout.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/listop.py` & `pycamia-1.0.37/pycamia/listop.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/logging.py` & `pycamia-1.0.37/pycamia/logging.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/manager.py` & `pycamia-1.0.37/pycamia/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 update_format = "%Y-%m-%d %H:%M:%S"
 
 class Version(tuple):
     def __new__(cls, string):
         matches = re.findall(r"[0-9\.]+", string)
         if len(matches) == 0: raise TypeError(f"{string} is not a version")
-        return super().__new__(cls, [eval(x) for x in matches[0].split('.')])
+        return super().__new__(cls, [eval(x) for x in matches[0].split('.') if x])
     for op in "gt lt ge le eq ne".split():
         exec(f"def __{op}__(self, x): return super(Version, self).__{op}__(Version(x) if isinstance(x, str) else x)")
 
 class info_manager:
     """
     info_manager() -> info_object
 
@@ -79,19 +79,19 @@
         not_found_packages = []
         for r in self.requires:
             tokens = tokenize(r, ['<', '>', '='], strip=None, keep_empty=False)
             if len(tokens) == 2: rname, rversion = tokens
             else: rname, rversion = tokens[0], None
             try:
                 package = __import__(rname)
-                if rversion is not None:
-                    op = r.replace(rname, '').replace(rversion, '').strip()
-                    if not eval("Version(package.__version__)" + op + "'" + rversion + "'"):
-                        not_found_packages.append(r)
             except ModuleNotFoundError: not_found_packages.append(rname)
+            if rversion is not None:
+                op = r.replace(rname, '').replace(rversion, '').strip()
+                if not eval("Version(package.__version__)" + op + "'" + rversion + "'"):
+                    not_found_packages.append(r)
         if len(not_found_packages) > 0:
             raise ModuleNotFoundError(f"'{self.name}' cannot be used without dependencies {repr(not_found_packages)}.")
             
     def check(self):
         self.check_requires()
         return self
```

### Comparing `pycamia-1.0.36/pycamia/math.py` & `pycamia-1.0.37/pycamia/math.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/more.py` & `pycamia-1.0.37/pycamia/more.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/numpyop.py` & `pycamia-1.0.37/pycamia/numpyop.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/strop.py` & `pycamia-1.0.37/pycamia/strop.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/system.py` & `pycamia-1.0.37/pycamia/system.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia/timing.py` & `pycamia-1.0.37/pycamia/timing.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pycamia.egg-info/PKG-INFO` & `pycamia-1.0.37/pycamia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycamia
-Version: 1.0.36
+Version: 1.0.37
 Summary: The main package and a background support of project PyCAMIA. 
 Home-page: https://github.com/Bertie97/PyZMyc/pycamia
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # pycamia
```

### Comparing `pycamia-1.0.36/pycamia.egg-info/SOURCES.txt` & `pycamia-1.0.37/pycamia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pyoverload/__init__.py` & `pycamia-1.0.37/pyoverload/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'pyoverload',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.29',
+    version = '1.1.30',
     contact = 'bertiezhou@163.com',
     keywords = ['overload'],
     description = "'pyoverload' overloads the functions by simply using typehints and adding decorator '@overload'. ",
     requires = ['pycamia'],
-    update = '2023-07-05 16:28:39'
+    update = '2023-07-05 17:05:59'
 ).check()
 
 from .typehint import isofsubclass, inheritable, isitertype, iterable, isarray, isdtype, isatype, isoftype, isclassmethod, typename, Type, params, Bool, Int, Float, Str, Set, List, Tuple, Dict, Class, Callable, Function, Method, Lambda, Functional, Real, real, Null, null, Sequence, sequence, Array, Iterable, Scalar, IntScalar, FloatScalar #*
 from .override import override, overload, params #*
```

### Comparing `pycamia-1.0.36/pyoverload/override.py` & `pycamia-1.0.37/pyoverload/override.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pyoverload/typehint.py` & `pycamia-1.0.37/pyoverload/typehint.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/pyoverload/utils.py` & `pycamia-1.0.37/pyoverload/utils.py`

 * *Files identical despite different names*

### Comparing `pycamia-1.0.36/setup_pycamia.py` & `pycamia-1.0.37/setup_pycamia.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'pycamia',
-	version = '1.0.36',
+	version = '1.0.37',
 	keywords = ['pip', 'pymyc', 'pycamia', 'environment', 'path', 'touch'],
 	description = 'The main package and a background support of project PyCAMIA. ',
 	long_description = '# pycamia\n\n## Introduction\n\n[`pycamia`](https://github.com/Bertie97/pycamia/tree/main/pycamia) is the base package affiliated to project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It is a collection of different useful tools necessary in python programming. `pycamia` was designed for `python v3.6+`. It is consist of the following sub-packages. \n\n1. **environment** is a package containing functions to inspect the context. e.g. get the local variables in the context that calls a function. \n2. **strop** is a collection of advanced functions for strings. e.g. tokenize a string by spliting outside brackets OR find all indices for matched sub-strings.\n3. **listop** is a collection of advanced functions for lists. e.g. flatten a nested list.\n4. **manager** is a package to manage file and package infos. e.g. easily check the dependencies OR easy update the version. \n5. **functions** is a package of special (and commonly trivial) functions. e.g. empty functions. \n6. **exceptions** is a package to handle exceptions. e.g. touch a function and suppress the error OR assert with comment OR quickly create an Error.\n7. **inout** is a package to extend the input/output. e.g. printing to a string OR suppressing the console output. \n8. **timing** is a package to time the executions. e.g. use `with` structure to record time spent for a set of commands. \n9. **more** is a collection of uncategorized functions, one need to import them from `pycamia.more`.\n\n## Installation\n\nThis package can be installed by `pip install pycamia` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/pyoverload/)). \n\n```shell\npip install pycamia\n```\n\n## Package `environment`\n\nThis package fetches the surrounding environment of the call. It is likely that no more functions would be added to it. If there\'s any suggestion, please contact the developer. \n1. Use `v = get_environ_locals()` or `v = get_environ_globals()` to get the dictionary of local or global variables in the parent environment. If the result is out of expectations, please contact the developer. \n2. Use `v[\'name\']` to read variable `name` and `v[\'name\'] = value` to add variable to the environment. \n\n## Package `strop`\n\nThis package cope with str objects. \n1. Use `str_len` to find the ASCII length for a string, with a length `2` for wide characters.\n2. Use `str_slice` to slice a string by given indices.\n3. Use `find_all` to obtain all the indices of a given string. `str_slice(s, find_all(s, k))` is equivalent to `s.split(k)`. \n4. Use `sorted_dict_repr` to create a repr string for a dictionary with ordered key.\n5. Use `enclosed_object` to find the first object enclosed by brackets. \n6. Use `tokenize` to split a string without breaking enclosed objects. This is useful in breaking text of dictionary structures or arguments. e.g. one can use `tokenize(args, sep=[\',\', \'=\'])[::2]` to find the argument names if `args` is a string in the format `key1=value1, key2 = value2, ...`.\n\n## Package `listop`\n\nThis package cope with list objects. More useful functions will be added to it in the future. \n1. Use `argmin(list, domain)` to find the indices for the minimal value in list. The function only search in the indices `domain`. A list is output as there may be multiple entries. \n2. Use `argmax` to find the indices for the maximal value, similar to `argmin`. \n3. Use `flatten_list` to unwrap the list elements to create a list with no element in type `list`. \n4. Use `prod` to obtain the product of all numbers in the list. \n5. Use `item` to fetch the only element in the list. An error will be raised if there isn\'t any or are more than 1 elements. \n\n## Package `manager`\n\nThis package manages the info of packages and files. One can use it to organize the project. \n1. Use `__info__ = info_manager(project="PyCAMIA", ...)` to list the properties at the front of files. This serve as a brief introduction to readers.\n2. Use `info_manager` at the beginning of `__init__.py`, `pack.py` uses it to create the portrait of a package. \n3. Use `__info__.check_requires()` to automatically check if the dependencies in attribute `requires` exist or not. This is commonly used in `__init__.py`. One can use `__info__ = info_manager(...).check()` to perform an in-place check.\n4. Use `with __info__:` before importing required dependencies as well to perform a double check. \n\n## Package `functions`\n\nThis package contains simple functions. It is the simplest package in the project so far. \n1. Use `empty_function` for a function that does nothing. One can put any argument to the function but nothing would happen. \n2. Use `const_function(a)` for a function that accepts any argument but does nothing and always return `a`.\n\n## Package `exceptions`\n\nThis package handles exceptions. \n1. Use `touch(function)` to try a function and suppress the error in the mean time. e.g. `touch(lambda: 1/a)` returns `None` to tell you that an exception occurs when `a=0`, but returns `1` when `a=1`. \n2. Use `crashed(function)` to check whether a function fails or not. \n3. Use `avouch(bool_to_be_tested, assertion_text)` to avouch that the given expression is true and output your designed `assertion_text` when the test fails. \n4. Use `Error("name")` to creat a new error type. It is the same as creating an Error tag by `class nameError(Exception): pass`.\n\n## Package `inout`\n\nThis package manipulates the input/output. Currently, it only deal with print. Shell handler or other inout functions will be added here in the future. \n1. Use `with no_print:` to suppress the console output. Although not recommended, one can use `with no_print as out_stream:` and `output = str(out_stream)` inside the `with` structure to fetch the output. \n2. Use `sprint = SPrint()` to create a function `sprint` that collects the printed text. Use `out = sprint()` or `sprint.text` to get the results.\n\n## Package `timing`\n\nThis package use the time spent of commands to perform useful inspection or organization of the codes.\n1. Use `@time_this` to time a function.\n2. Use `with Timer("name"):` to time a series of commands.\n3. Use `with scope("name"):` to nest a series of commands. It is an alias of `Timer`. \n4. Use `with scope("name"), jump:` to jump a series of commands. \n5. Use `with scope("name"), Jump(False):` to disable the jump.\n6. Use `wf = Workflow("step1", "step2")` and `with wf("step1(2)"), wf.jump:` before commands of "step1(2)" to create a workflow. One can change the arguments in the init function to decide which steps to run. \n7. Use `@periodic(seconds, max_repeat)` to run a function repeatedly. \n\n## Package `more`\n\nCurrently, only `once` is contained in the `more` package. \nAdding it in a function to check if the function is run once or not. \n\n## Waiting to Be Imroved\n\n1. More functions will be added in the future, including path handler, tools for shell and so on. \n2. Contact us to make suggestions. \n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/pycamia',
 	author = 'Yuncheng Zhou',
```


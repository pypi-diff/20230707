# Comparing `tmp/tvdcn-0.3.2.tar.gz` & `tmp/tvdcn-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.3.2.tar", last modified: Sun Jul  2 23:41:12 2023, max compression
+gzip compressed data, was "tvdcn-0.3.3.tar", last modified: Fri Jul  7 18:51:30 2023, max compression
```

## Comparing `tvdcn-0.3.2.tar` & `tvdcn-0.3.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.557254 tvdcn-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 23:39:04.000000 tvdcn-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 23:39:04.000000 tvdcn-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-02 23:41:12.557254 tvdcn-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-02 23:39:04.000000 tvdcn-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-02 23:39:04.000000 tvdcn-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 23:39:04.000000 tvdcn-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-02 23:41:12.557254 tvdcn-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-02 23:39:04.000000 tvdcn-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.541253 tvdcn-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.541253 tvdcn-0.3.2/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.545253 tvdcn-0.3.2/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.549254 tvdcn-0.3.2/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.549254 tvdcn-0.3.2/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27298 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35673 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.549254 tvdcn-0.3.2/tvdcn/csrc/ops/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)    23593 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    30423 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    38849 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    26564 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30412 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27339 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.553254 tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.553254 tvdcn-0.3.2/tvdcn/csrc/ops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/ops/utils/tensor_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.553254 tvdcn-0.3.2/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.557254 tvdcn-0.3.2/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    33905 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-02 23:39:04.000000 tvdcn-0.3.2/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 23:41:12.545253 tvdcn-0.3.2/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 23:41:12.000000 tvdcn-0.3.2/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.094404 tvdcn-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 18:49:18.000000 tvdcn-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 18:49:18.000000 tvdcn-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-07 18:51:30.094404 tvdcn-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-07 18:49:18.000000 tvdcn-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-07 18:49:18.000000 tvdcn-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 18:49:18.000000 tvdcn-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-07 18:51:30.094404 tvdcn-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-07 18:49:18.000000 tvdcn-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.074403 tvdcn-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.074403 tvdcn-0.3.3/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.078403 tvdcn-0.3.3/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.082404 tvdcn-0.3.3/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.082404 tvdcn-0.3.3/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27299 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35674 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.086404 tvdcn-0.3.3/tvdcn/csrc/ops/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    30424 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    38850 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    26564 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30412 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27339 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.086404 tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.090404 tvdcn-0.3.3/tvdcn/csrc/ops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/utils/tensor_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.090404 tvdcn-0.3.3/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.094404 tvdcn-0.3.3/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33905 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.078403 tvdcn-0.3.3/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.3.2/LICENSE.txt` & `tvdcn-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/PKG-INFO` & `tvdcn-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.3.2
+Version: 0.3.3
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.3.2/README.md` & `tvdcn-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/pyproject.toml` & `tvdcn-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/setup.cfg` & `tvdcn-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/setup.py` & `tvdcn-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.3.3/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tests/test_grad.py` & `tvdcn-0.3.3/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include <ATen/ATen.h>
+
 #include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
             template<typename scalar_t, typename index_t>
```

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include <ATen/ATen.h>
+
 #include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
             template<typename scalar_t, typename index_t>
```

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include <ATen/ATen.h>
+
 #include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
             template<typename scalar_t, typename index_t>
```

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu` & `tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include <ATen/ATen.h>
+
 #include "cuda_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
             constexpr float threadsFraction = 1.0;
```

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu` & `tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include <ATen/ATen.h>
+
 #include "cuda_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
             constexpr float threadsFraction = 0.75;
```

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu` & `tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include <ATen/ATen.h>
+
 #include "cuda_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
         namespace {
             constexpr float threadsFraction = 0.5;
```

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/ops/utils/tensor_utils.cpp` & `tvdcn-0.3.3/tvdcn/csrc/ops/utils/tensor_utils.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.3.3/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/extension.py` & `tvdcn-0.3.3/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.3.3/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.3.3/tvdcn/ops/activations/mask_softmax.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn/ops/deform_conv.py` & `tvdcn-0.3.3/tvdcn/ops/deform_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,31 +692,31 @@
                 3 * self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.offset_groups,
                 kernel_size=self.kernel_size,  # type: ignore[arg-type]
                 stride=self.stride,  # type: ignore[arg-type]
                 padding=self.padding,
                 dilation=self.dilation,  # type: ignore[arg-type]
                 groups=self.offset_groups,
                 bias=generator_bias,
-                device=dtype,
-                dtype=device)
+                device=device,
+                dtype=dtype)
         else:
             self.register_module('offset_generator', None)
 
         if self.modulated:
             self.mask_generator = nn.Conv3d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.mask_groups,
                 kernel_size=self.kernel_size,  # type: ignore[arg-type]
                 stride=self.stride,  # type: ignore[arg-type]
                 padding=self.padding,
                 dilation=self.dilation,  # type: ignore[arg-type]
                 groups=self.mask_groups,
                 bias=generator_bias,
-                device=dtype,
-                dtype=device)
+                device=device,
+                dtype=dtype)
         else:
             self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
```

### Comparing `tvdcn-0.3.2/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.3.3/tvdcn/ops/deform_conv_transpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,28 +502,28 @@
         if self.deformable:
             self.offset_generator = nn.Conv1d(
                 self.in_channels,
                 self.kernel_size[0] * self.offset_groups,
                 kernel_size=1,
                 groups=self.offset_groups,
                 bias=generator_bias,
-                device=dtype,
-                dtype=device)
+                device=device,
+                dtype=dtype)
         else:
             self.register_module('offset_generator', None)
 
         if self.modulated:
             self.mask_generator = nn.Conv1d(
                 self.in_channels,
                 self.kernel_size[0] * self.mask_groups,
                 kernel_size=1,
                 groups=self.mask_groups,
                 bias=generator_bias,
-                device=dtype,
-                dtype=device)
+                device=device,
+                dtype=dtype)
         else:
             self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
@@ -618,28 +618,28 @@
         if self.deformable:
             self.offset_generator = nn.Conv2d(
                 self.in_channels,
                 2 * self.kernel_size[0] * self.kernel_size[1] * self.offset_groups,
                 kernel_size=1,
                 groups=self.offset_groups,
                 bias=generator_bias,
-                device=dtype,
-                dtype=device)
+                device=device,
+                dtype=dtype)
         else:
             self.register_module('offset_generator', None)
 
         if self.modulated:
             self.mask_generator = nn.Conv2d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.mask_groups,
                 kernel_size=1,
                 groups=self.mask_groups,
                 bias=generator_bias,
-                device=dtype,
-                dtype=device)
+                device=device,
+                dtype=dtype)
         else:
             self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
@@ -734,28 +734,28 @@
         if self.deformable:
             self.offset_generator = nn.Conv3d(
                 self.in_channels,
                 3 * self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.offset_groups,
                 kernel_size=1,
                 groups=self.offset_groups,
                 bias=generator_bias,
-                device=dtype,
-                dtype=device)
+                device=device,
+                dtype=dtype)
         else:
             self.register_module('offset_generator', None)
 
         if self.modulated:
             self.mask_generator = nn.Conv3d(
                 self.in_channels,
                 self.kernel_size[0] * self.kernel_size[1] * self.kernel_size[2] * self.mask_groups,
                 kernel_size=1,
                 groups=self.mask_groups,
                 bias=generator_bias,
-                device=dtype,
-                dtype=device)
+                device=device,
+                dtype=dtype)
         else:
             self.register_module('mask_generator', None)
 
         self.offset_activation = offset_activation
         self.mask_activation = mask_activation
 
         self.reset_parameters()
```

### Comparing `tvdcn-0.3.2/tvdcn/utils.py` & `tvdcn-0.3.3/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.2/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.3.3/tvdcn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.3.2
+Version: 0.3.3
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.3.2/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.3.3/tvdcn.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/x-dgcnn-0.1.2.tar.gz` & `tmp/x-dgcnn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-dgcnn-0.1.2.tar", last modified: Tue May 23 17:31:51 2023, max compression
+gzip compressed data, was "x-dgcnn-0.2.0.tar", last modified: Fri Jul  7 06:02:15 2023, max compression
```

## Comparing `x-dgcnn-0.1.2.tar` & `x-dgcnn-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:51.239447 x-dgcnn-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 17:31:51.239447 x-dgcnn-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:31:51.239447 x-dgcnn-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:51.235447 x-dgcnn-0.1.2/x_dgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/x_dgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/x_dgcnn/dgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-23 17:31:38.000000 x-dgcnn-0.1.2/x_dgcnn/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:51.239447 x-dgcnn-0.1.2/x_dgcnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 17:31:51.000000 x-dgcnn-0.1.2/x_dgcnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/x_dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/x_dgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/x_dgcnn/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 06:02:05.000000 x-dgcnn-0.2.0/x_dgcnn/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:02:15.470608 x-dgcnn-0.2.0/x_dgcnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 06:02:15.000000 x-dgcnn-0.2.0/x_dgcnn.egg-info/top_level.txt
```

### Comparing `x-dgcnn-0.1.2/LICENSE` & `x-dgcnn-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.1.2/PKG-INFO` & `x-dgcnn-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.1.2
+Version: 0.2.0
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-dgcnn-0.1.2/README.md` & `x-dgcnn-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 <img src="./dgcnn.jpg" width="1200px"></img>
 
+[![PyPI version](https://badge.fury.io/py/x-dgcnn.svg)](https://badge.fury.io/py/x-dgcnn)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 # x_dgcnn
 
 A pytorch implementation of [DGCNN](https://arxiv.org/abs/1801.07829), more efficient and memory-saving than
 [dgcnn.pytorch](https://github.com/antao97/dgcnn.pytorch).
 
 The performance in comparison with [dgcnn.pytorch](https://github.com/antao97/dgcnn.pytorch) could be found in
 the [comparison_with_dgcnn.pytorch](https://github.com/kentechx/x-dgcnn/tree/comparison_with_dgcnn.pytorch) branch.
 
+Update2: use [keops](https://github.com/getkeops/keops) to accelerate the computation of the pairwise distance matrix.
+It is memory-efficient, thus can handle larger point clouds.
+
 Update: use GELU rather than LeakyReLU. Rewrite the message passing part to make it more efficient. Move the
 normalization and activation after the max pooling in all instances. Make the categorical embedding learnable.
 We try LayerNorm and InstanceNorm, and find that BatchNorm beats them by a large margin.
 
-[![PyPI version](https://badge.fury.io/py/x-dgcnn.svg)](https://badge.fury.io/py/x-dgcnn)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
 ## Installation
 
 ```bash
 pip install x-dgcnn
 ```
 
 If you suffer from the error `No matching distribution found for x-dgcnn` using a mirror source, try the following
 (if you know how to solve this problem, please open an issue):
+
 ```bash
 pip install x-dgcnn -i https://pypi.org/simple
 ```
 
 ## Usage
 
 Classification.
@@ -65,15 +69,24 @@
 model = DGCNN_Seg(k=40, in_dim=9, out_dim=4, n_category=10, stn=stn)
 x = torch.randn(8, 9, 2048)  # keep xyz at the first 3 channels if using stn
 xyz = x[:, :3].clone()
 category = torch.randint(0, 10, (10,))
 out = model(x, xyz, category)
 ```
 
+You can disable keops by calling `disable_keops()` when exporting the model to onnx.
+
+```python
+from x_dgcnn import disable_keops
+disable_keops()
+```
+
+
 ## TODO
+
 - [ ] Add differentiable subset operator and coordinate descent as another option to fuse features.
 - [ ] Scale up model size and test.
 - [ ] Add sampling to get hierarchical features.
 - [ ] Do tasks on other tasks, e.x. rotation prediction, normal prediction, etc.
 
 ## References
```

### Comparing `x-dgcnn-0.1.2/setup.py` & `x-dgcnn-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='x-dgcnn',
     packages=find_packages(),
-    version='0.1.2',
+    version='0.2.0',
     license='MIT',
     description='X-DGCNN - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/x-dgcnn',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
         '3D classification',
         'point cloud understanding',
     ],
     install_requires=[
         'torch>=1.10',
-        'einops>=0.6.1'
+        'einops>=0.6.1',
+        'pykeops>=2.1.2',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
```

### Comparing `x-dgcnn-0.1.2/x_dgcnn/dgcnn.py` & `x-dgcnn-0.2.0/x_dgcnn/dgcnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+from pykeops.torch import LazyTensor
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from einops import repeat, rearrange, einsum, reduce
 from .route import subset_topk
 
+__KEOPS__ = True
+
+
+def disable_keops():
+    global __KEOPS__
+    __KEOPS__ = False
+
 
 def exists(val):
     return val is not None
 
 
 def cdist(x, y=None):
     # perform cdist in dimension 1
@@ -19,14 +27,27 @@
         y = rearrange(y, 'b d m -> b m d')
         return torch.cdist(x, y)
     else:
         x = rearrange(x, 'b d n -> b n d')
         return torch.cdist(x, x)
 
 
+def knn(x, y=None, k=1):
+    # x: (b, d, n)
+    # y: (b, d, m)
+    if __KEOPS__:
+        x_i = LazyTensor(rearrange(x, 'b d n -> b n 1 d').contiguous())
+        y_j = LazyTensor(rearrange(y, 'b d m -> b 1 m d').contiguous() if exists(y) else rearrange(x, 'b d n -> b 1 n d').contiguous())
+        D_ij = ((x_i - y_j) ** 2).sum(-1)  # (b, n, m)
+        neighbor_ind = D_ij.argKmin(k, axis=2)  # (b, n, k)
+    else:
+        neighbor_ind = cdist(x, y).topk(k, dim=-1, largest=False)[1]  # (b, n, k)
+    return neighbor_ind
+
+
 class EdgeConv(nn.Module):
     def __init__(self, k, dims=(64, 64)):
         super().__init__()
         self.k = k
 
         dims = (dims[0] * 2, *dims[1:])
         if len(dims) > 2:
@@ -42,15 +63,15 @@
         self.norm = nn.BatchNorm1d(dims[-1])
         self.act = nn.GELU()
 
     def route(self, x, neighbor_ind=None):
         # x: (b, d, n)
         d = x.size(1)
         if not exists(neighbor_ind):
-            neighbor_ind = cdist(x).topk(self.k, dim=-1, largest=False)[1]  # (b, n, k)
+            neighbor_ind = knn(x, k=self.k)  # (b, n, k)
 
         x = repeat(x, 'b d n -> b d n k', k=self.k)
         neighbor_ind = repeat(neighbor_ind, 'b n k -> b d n k', d=d)
         neighbor_x = x.gather(2, neighbor_ind)  # (b, d, n, k)
 
         # (b, d, n, k) -> (b, 2*d, n, k)
         graph_feature = torch.cat([neighbor_x - x, x], dim=1)
@@ -151,15 +172,15 @@
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
             nn.Linear(256, out_dim),
         )
 
     def forward(self, x, xyz):
         # x: (b, d, n)
         # xyz: (b, 3, n), spatial coordinates
-        neighbor_ind = cdist(xyz).topk(self.k, dim=-1, largest=False)[1]  # (b, n, k)
+        neighbor_ind = knn(xyz, k=self.k)  # (b, n, k)
 
         # go through all EdgeConv blocks
         xs = [self.blocks[0](x, neighbor_ind)]
         for block in self.blocks[1:]:
             x = block(xs[-1], None if self.dynamic else neighbor_ind)
             xs.append(x)
         x = torch.cat(xs, dim=1)  # (b, sum(dims), n)
@@ -233,15 +254,15 @@
             self.category_emb = nn.Embedding(n_category, 128)
         self.head = nn.Conv1d(128, out_dim, 1)
 
     def forward(self, x, xyz, category=None):
         # x: (b, d, n)
         # xyz: (b, 3, n), spatial coordinates
         n = x.size(2)
-        neighbor_ind = cdist(xyz).topk(self.k, dim=-1, largest=False)[1]  # (b, n, k)
+        neighbor_ind = knn(xyz, k=self.k)  # (b, n, k)
 
         if exists(self.stn):
             transform = self.stn(x, neighbor_ind).reshape(-1, 3, 3)
             if x.size(1) > 3:
                 x = torch.cat([torch.bmm(transform, x[:, :3]), x[:, 3:]], dim=1)
             else:
                 assert x.size(1) == 3
```

### Comparing `x-dgcnn-0.1.2/x_dgcnn/route.py` & `x-dgcnn-0.2.0/x_dgcnn/route.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.1.2/x_dgcnn.egg-info/PKG-INFO` & `x-dgcnn-0.2.0/x_dgcnn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.1.2
+Version: 0.2.0
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


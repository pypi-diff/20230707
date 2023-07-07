# Comparing `tmp/pygmtools-0.3.8a0.tar.gz` & `tmp/pygmtools-0.3.8a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.3.8a0.tar", last modified: Fri Jul  7 09:24:04 2023, max compression
+gzip compressed data, was "pygmtools-0.3.8a2.tar", last modified: Fri Jul  7 11:53:26 2023, max compression
```

## Comparing `pygmtools-0.3.8a0.tar` & `pygmtools-0.3.8a2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 09:24:04.001748 pygmtools-0.3.8a0/
--rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a0/LICENSE
--rw-rw-rw-   0        0        0       18 2023-05-03 08:07:01.000000 pygmtools-0.3.8a0/MANIFEST.in
--rw-rw-rw-   0        0        0    13827 2023-07-07 09:24:04.001748 pygmtools-0.3.8a0/PKG-INFO
--rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 09:24:03.995376 pygmtools-0.3.8a0/pygmtools/
--rw-rw-rw-   0        0        0     2119 2023-07-07 09:23:15.000000 pygmtools-0.3.8a0/pygmtools/__init__.py
--rw-rw-rw-   0        0        0    58368 2023-07-07 09:20:08.000000 pygmtools-0.3.8a0/pygmtools/a_star.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    27000 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/benchmark.py
--rw-rw-rw-   0        0        0    58667 2023-06-24 14:15:49.000000 pygmtools-0.3.8a0/pygmtools/classic_solvers.py
--rw-rw-rw-   0        0        0    59231 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/dataset.py
--rw-rw-rw-   0        0        0     3112 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/dataset_config.py
--rw-rw-rw-   0        0        0    58908 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/jittor_backend.py
--rw-rw-rw-   0        0        0    12371 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/jittor_modules.py
--rw-rw-rw-   0        0        0    77128 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/linear_solvers.py
--rw-rw-rw-   0        0        0    21736 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/mindspore_backend.py
--rw-rw-rw-   0        0        0    44038 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/multi_graph_solvers.py
--rw-rw-rw-   0        0        0    70477 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/neural_solvers.py
--rw-rw-rw-   0        0        0    60669 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/numpy_backend.py
--rw-rw-rw-   0        0        0    15282 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/numpy_modules.py
--rw-rw-rw-   0        0        0    57860 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/paddle_backend.py
--rw-rw-rw-   0        0        0    11899 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/paddle_modules.py
--rw-rw-rw-   0        0        0    21475 2023-07-02 09:29:01.000000 pygmtools-0.3.8a0/pygmtools/pytorch_astar_modules.py
--rw-rw-rw-   0        0        0    68324 2023-07-02 06:13:41.000000 pygmtools-0.3.8a0/pygmtools/pytorch_backend.py
--rw-rw-rw-   0        0        0    12329 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/pytorch_modules.py
--rw-rw-rw-   0        0        0    23046 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/tensorflow_backend.py
--rw-rw-rw-   0        0        0      508 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/tensorflow_modules.py
--rw-rw-rw-   0        0        0    51707 2023-06-19 13:47:03.000000 pygmtools-0.3.8a0/pygmtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:24:03.997585 pygmtools-0.3.8a0/pygmtools.egg-info/
--rw-rw-rw-   0        0        0    13827 2023-07-07 09:24:03.000000 pygmtools-0.3.8a0/pygmtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      978 2023-07-07 09:24:03.000000 pygmtools-0.3.8a0/pygmtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 09:24:03.000000 pygmtools-0.3.8a0/pygmtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-07-07 09:24:03.000000 pygmtools-0.3.8a0/pygmtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 09:24:03.000000 pygmtools-0.3.8a0/pygmtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 09:24:04.002797 pygmtools-0.3.8a0/setup.cfg
--rw-rw-rw-   0        0        0     5818 2023-07-07 09:10:43.000000 pygmtools-0.3.8a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 09:24:04.001748 pygmtools-0.3.8a0/tests/
--rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a0/tests/test_classic_solvers.py
--rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a0/tests/test_dataset.py
--rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a0/tests/test_misc.py
--rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a0/tests/test_multi_graph_solvers.py
--rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a0/tests/test_neural_solvers.py
--rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:53:26.219340 pygmtools-0.3.8a2/
+-rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/MANIFEST.in
+-rw-rw-rw-   0        0        0    13827 2023-07-07 11:53:26.218337 pygmtools-0.3.8a2/PKG-INFO
+-rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 11:53:26.212757 pygmtools-0.3.8a2/pygmtools/
+-rw-rw-rw-   0        0        0     2120 2023-07-07 11:53:18.000000 pygmtools-0.3.8a2/pygmtools/__init__.py
+-rw-rw-rw-   0        0        0    58368 2023-07-07 11:50:59.000000 pygmtools-0.3.8a2/pygmtools/a_star.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0    27000 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/benchmark.py
+-rw-rw-rw-   0        0        0    58667 2023-06-24 14:15:49.000000 pygmtools-0.3.8a2/pygmtools/classic_solvers.py
+-rw-rw-rw-   0        0        0    59231 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/dataset.py
+-rw-rw-rw-   0        0        0     3112 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/dataset_config.py
+-rw-rw-rw-   0        0        0    58908 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/jittor_backend.py
+-rw-rw-rw-   0        0        0    12371 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/jittor_modules.py
+-rw-rw-rw-   0        0        0    77128 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/linear_solvers.py
+-rw-rw-rw-   0        0        0    21736 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/mindspore_backend.py
+-rw-rw-rw-   0        0        0    44038 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/multi_graph_solvers.py
+-rw-rw-rw-   0        0        0    70477 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/neural_solvers.py
+-rw-rw-rw-   0        0        0    60669 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/numpy_backend.py
+-rw-rw-rw-   0        0        0    15282 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/numpy_modules.py
+-rw-rw-rw-   0        0        0    57860 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/paddle_backend.py
+-rw-rw-rw-   0        0        0    11899 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/paddle_modules.py
+-rw-rw-rw-   0        0        0    15470 2023-07-07 11:46:26.000000 pygmtools-0.3.8a2/pygmtools/pytorch_astar_modules.py
+-rw-rw-rw-   0        0        0    74399 2023-07-07 11:49:03.000000 pygmtools-0.3.8a2/pygmtools/pytorch_backend.py
+-rw-rw-rw-   0        0        0    12329 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/pytorch_modules.py
+-rw-rw-rw-   0        0        0    23046 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/tensorflow_backend.py
+-rw-rw-rw-   0        0        0      508 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/tensorflow_modules.py
+-rw-rw-rw-   0        0        0    51707 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:53:26.215158 pygmtools-0.3.8a2/pygmtools.egg-info/
+-rw-rw-rw-   0        0        0    13827 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:53:26.219340 pygmtools-0.3.8a2/setup.cfg
+-rw-rw-rw-   0        0        0     5818 2023-07-07 09:10:43.000000 pygmtools-0.3.8a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:53:26.218337 pygmtools-0.3.8a2/tests/
+-rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a2/tests/test_classic_solvers.py
+-rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_misc.py
+-rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_multi_graph_solvers.py
+-rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_neural_solvers.py
+-rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_utils.py
```

### Comparing `pygmtools-0.3.8a0/PKG-INFO` & `pygmtools-0.3.8a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a0
+Version: 0.3.8a2
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a0/README.md` & `pygmtools-0.3.8a2/README.md`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/__init__.py` & `pygmtools-0.3.8a2/pygmtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .benchmark import Benchmark
 from .linear_solvers import sinkhorn, hungarian
 from .classic_solvers import rrwm, sm, ipfp, a_star
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm
 import pygmtools.utils as utils
 BACKEND = 'numpy'
-__version__ = '0.3.8-alpha'
+__version__ = '0.3.8-alpha2'
 __author__ = 'ThinkLab at SJTU'
 
 
 def env_report():
     """
     Print environment report
     """
```

### Comparing `pygmtools-0.3.8a0/pygmtools/benchmark.py` & `pygmtools-0.3.8a2/pygmtools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/classic_solvers.py` & `pygmtools-0.3.8a2/pygmtools/classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/dataset.py` & `pygmtools-0.3.8a2/pygmtools/dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/dataset_config.py` & `pygmtools-0.3.8a2/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/jittor_backend.py` & `pygmtools-0.3.8a2/pygmtools/jittor_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/jittor_modules.py` & `pygmtools-0.3.8a2/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/linear_solvers.py` & `pygmtools-0.3.8a2/pygmtools/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/mindspore_backend.py` & `pygmtools-0.3.8a2/pygmtools/mindspore_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/multi_graph_solvers.py` & `pygmtools-0.3.8a2/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/neural_solvers.py` & `pygmtools-0.3.8a2/pygmtools/neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/numpy_backend.py` & `pygmtools-0.3.8a2/pygmtools/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/numpy_modules.py` & `pygmtools-0.3.8a2/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/paddle_backend.py` & `pygmtools-0.3.8a2/pygmtools/paddle_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/paddle_modules.py` & `pygmtools-0.3.8a2/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/pytorch_backend.py` & `pygmtools-0.3.8a2/pygmtools/pytorch_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import numpy as np
 from multiprocessing import Pool
 from torch import Tensor
 import os
 import pygmtools.utils
 from pytorch_astar_modules import *
 import warnings
-from typing import Optional, Tuple
 from torch import Tensor
 
 #############################################
 #     Linear Assignment Problem Solvers     #
 #############################################
 
 from pygmtools.numpy_backend import _hung_kernel
@@ -843,14 +842,316 @@
 astar_pretrain_path = {
     'AIDS700nef': ('https://drive.google.com/u/0/uc?export=download&confirm=Z-AR&id=1QWGgpt4C4XjFZSEcIZmQF-84XtpfXope',
                'b2516aea4c8d730704a48653a5ca94ba'),
     'LINUX': ('https://drive.google.com/u/0/uc?export=download&confirm=Z-AR&id=1EGVSejxsgSefIBquZtDftpe3Ize1Vw1P',
             'fd3b2a8dfa3edb20607da2e2b96d2e96'),
 }
 
+class GENN(torch.nn.Module):
+    def __init__(self, args):
+        """
+        :param args: Arguments object.
+        :param number_of_labels: Number of node labels.
+        """
+        super(GENN, self).__init__()
+        self.args = args
+        if self.args['use_net']:
+            self.number_labels = self.args['feature_num']
+            self.setup_layers()
+
+        self.reset_cache()
+
+    def reset_cache(self):
+        self.gnn_1_cache = dict()
+        self.gnn_2_cache = dict()
+        self.heuristic_cache = dict()
+
+    def calculate_bottleneck_features(self):
+        """
+        Deciding the shape of the bottleneck layer.
+        """
+        if self.args['histogram']:
+            self.feature_count = self.args['tensor_neurons'] + self.args['bins']
+        else:
+            self.feature_count = self.args['tensor_neurons']
+
+    def setup_layers(self):
+        """
+        Creating the layers.
+        """
+        self.calculate_bottleneck_features()
+        self.convolution_1 = GCNConv(self.number_labels, self.args['filters_1'])
+        self.convolution_2 = GCNConv(self.args['filters_1'], self.args['filters_2'])
+        self.convolution_3 = GCNConv(self.args['filters_2'], self.args['filters_3'])
+        
+        self.attention = AttentionModule(self.args)
+
+        self.tensor_network = TensorNetworkModule(self.args)
+        self.scoring_layer = torch.nn.Sequential(
+            torch.nn.Linear(self.feature_count, 16),
+            torch.nn.ReLU(),
+            torch.nn.Linear(16, 1),
+            torch.nn.Sigmoid()
+        )
+
+    def calculate_histogram(self, abstract_features_1, abstract_features_2, batch_1, batch_2):
+        """
+        Calculate histogram from similarity matrix.
+        :param abstract_features_1: Feature matrix for target graphs.
+        :param abstract_features_2: Feature matrix for source graphs.
+        :param batch_1: Batch vector for source graphs, which assigns each node to a specific example
+        :param batch_1: Batch vector for target graphs, which assigns each node to a specific example
+        :return hist: Histogram of similarity scores.
+        """
+        abstract_features_1, mask_1 = to_dense_batch(abstract_features_1, batch_1)
+        abstract_features_2, mask_2 = to_dense_batch(abstract_features_2, batch_2)
+
+        B1, N1, _ = abstract_features_1.size()
+        B2, N2, _ = abstract_features_2.size()
+
+        mask_1 = mask_1.view(B1, N1)
+        mask_2 = mask_2.view(B2, N2)
+        num_nodes = torch.max(mask_1.sum(dim=1), mask_2.sum(dim=1))
+
+        scores = torch.matmul(abstract_features_1, abstract_features_2.permute([0, 2, 1])).detach()
+
+        hist_list = []
+        for i, mat in enumerate(scores):
+            mat = torch.sigmoid(mat[:num_nodes[i], :num_nodes[i]]).view(-1)
+            hist = torch.histc(mat, bins=self.args['bins'])
+            hist = hist / torch.sum(hist)
+            hist = hist.view(1, -1)
+            hist_list.append(hist)
+
+        return torch.stack(hist_list).view(-1, self.args['bins'])
+
+    def convolutional_pass(self, A, x, edge_weight=None):
+        """
+        Making convolutional pass.
+        :param edge_index: Edge indices.
+        :param features: Feature matrix.
+        :return features: Abstract feature matrix.
+        """
+
+        features = self.convolution_1(A, x, edge_weight)
+        features = F.relu(features)
+        features = F.dropout(features, p=self.args['dropout'], training=self.training)
+        features = self.convolution_2(A, features, edge_weight)
+        features = F.relu(features)
+        features = F.dropout(features, p=self.args['dropout'], training=self.training)
+        features = self.convolution_3(A, features, edge_weight)
+        return features
+
+    def diffpool(self, abstract_features, edge_index, batch):
+        """
+        Making differentiable pooling.
+        :param abstract_features: Node feature matrix.
+        :param batch: Batch vector, which assigns each node to a specific example
+        :return pooled_features: Graph feature matrix.
+        """
+        x, mask = to_dense_batch(abstract_features, batch)
+        adj = to_dense_adj(edge_index, batch)
+        return self.attention(x, adj, mask)
+
+    def forward(self,data:Graph_pair):
+        """
+        Forward pass with graphs.
+        :param data: Data dictionary.
+        :return score: Similarity score.
+        """
+        num = data.g1.num_graphs
+        for i in range(num):
+            cur_data = Graph_pair(data.g1.x[i],data.g2.x[i],data.g1.Adj[i],data.g2.Adj[i],
+                                data.g1.nodes_num[i],data.g2.nodes_num[i])   
+            if(i == 0):
+                x_pred = self.A_star(cur_data)
+            else:
+                x_pred = torch.cat([x_pred,self.A_star(cur_data)],dim=0)
+        return x_pred[:,:-1,:-1]
+
+    def A_star(self,data:Graph_pair):
+        if self.args['cuda']:
+            device = "cuda" if torch.cuda.is_available() else "cpu"
+        else:
+            device = "cpu"
+        edge_index_1 = data.g1.edge_index.squeeze()
+        edge_index_2 = data.g2.edge_index.squeeze()
+        edge_attr_1 = data.g1.edge_weight
+        edge_attr_2 = data.g2.edge_weight
+        node_1 = data.g1.x.squeeze()
+        node_2 = data.g2.x.squeeze()
+        batch_1 = data.g1.batch
+        batch_2 = data.g2.batch
+        batch_num = data.g1.num_graphs
+
+        ns_1 = torch.bincount(data.g1.batch)
+        ns_2 = torch.bincount(data.g2.batch)
+        
+        adj_1 = to_dense_adj(edge_index_1, batch=batch_1, edge_attr=edge_attr_1)
+        
+        dummy_adj_1 = torch.zeros(adj_1.shape[0], adj_1.shape[1] + 1, adj_1.shape[2] + 1, device=device)
+        dummy_adj_1[:, :-1, :-1] = adj_1
+        adj_2 = to_dense_adj(edge_index_2, batch=batch_2, edge_attr=edge_attr_2)
+        dummy_adj_2 = torch.zeros(adj_2.shape[0], adj_2.shape[1] + 1, adj_2.shape[2] + 1, device=device)
+        dummy_adj_2[:, :-1, :-1] = adj_2
+        
+        node_1, _ = to_dense_batch(node_1, batch=batch_1)
+        node_2, _ = to_dense_batch(node_2, batch=batch_2)
+        
+        dummy_node_1 = torch.zeros(adj_1.shape[0], node_1.shape[1] + 1, node_1.shape[-1], device=device)
+        dummy_node_1[:, :-1, :] = node_1
+        dummy_node_2 = torch.zeros(adj_2.shape[0], node_2.shape[1] + 1, node_2.shape[-1], device=device)
+        dummy_node_2[:, :-1, :] = node_2
+        k_diag = self.node_metric(dummy_node_1, dummy_node_2)
+        
+        mask_1 = torch.zeros_like(dummy_adj_1)
+        mask_2 = torch.zeros_like(dummy_adj_2)
+        for b in range(batch_num):
+            mask_1[b, :ns_1[b] + 1, :ns_1[b] + 1] = 1
+            mask_1[b, :ns_1[b], :ns_1[b]] -= torch.eye(ns_1[b], device=mask_1.device)
+            mask_2[b, :ns_2[b] + 1, :ns_2[b] + 1] = 1
+            mask_2[b, :ns_2[b], :ns_2[b]] -= torch.eye(ns_2[b], device=mask_2.device)
+        
+        a1 = dummy_adj_1.reshape(batch_num, -1, 1)
+        a2 = dummy_adj_2.reshape(batch_num, 1, -1)
+        m1 = mask_1.reshape(batch_num, -1, 1)
+        m2 = mask_2.reshape(batch_num, 1, -1)
+        k = torch.abs(a1 - a2) * torch.bmm(m1, m2)
+        k[torch.logical_not(torch.bmm(m1, m2).to(dtype=torch.bool))] = VERY_LARGE_INT
+        k = k.reshape(batch_num, dummy_adj_1.shape[1], dummy_adj_1.shape[2], dummy_adj_2.shape[1], dummy_adj_2.shape[2])
+        k = k.permute([0, 1, 3, 2, 4])
+        k = k.reshape(batch_num, dummy_adj_1.shape[1] * dummy_adj_2.shape[1], dummy_adj_1.shape[2] * dummy_adj_2.shape[2])
+        k = k / 2
+        
+        for b in range(batch_num):
+            k_diag_view = torch.diagonal(k[b])
+            k_diag_view[:] = k_diag[b].reshape(-1)
+
+        self.reset_cache()
+        
+        x_pred, _ = a_star(
+            data, k, ns_1.cpu().numpy(), ns_2.cpu().numpy(),
+            self.net_prediction_cache,
+            self.heuristic_prediction_hun,
+            net_pred=self.args['use_net'],
+            beam_width=self.args['astar_beamwidth'],
+            trust_fact=self.args['astar_trustfact'],
+            no_pred_size=self.args['astar_nopred'],
+        )
+        
+        return x_pred
+    
+    def node_metric(self,node1,node2):
+        
+        encoding = torch.sum(torch.abs(node1.unsqueeze(2) - node2.unsqueeze(1)), dim=-1)
+        non_zero = torch.nonzero(encoding)
+        for i in range(non_zero.shape[0]):
+            encoding[non_zero[i][0],non_zero[i][1],non_zero[i][2]] = 1
+        return encoding
+  
+    def net_prediction_cache(self, data:Graph_pair, partial_pmat=None, return_ged_norm=False):
+        """
+        Forward pass with graphs.
+        :param data: Data dictionary.
+        :return score: Similarity score.
+        """
+        edge_index_1 = data.g1.edge_index.squeeze()
+        edge_index_2 = data.g2.edge_index.squeeze()
+        features_1 = data.g1.x.squeeze()
+        features_2 = data.g2.x.squeeze()
+        batch_1 = data.g1.batch
+        batch_2 = data.g2.batch
+        Adj1 = data.g1.Adj.squeeze()
+        Adj2 = data.g2.Adj.squeeze()
+        if 'gnn_feat' not in self.gnn_1_cache:
+            abstract_features_1 = self.convolutional_pass(Adj1,features_1)
+            self.gnn_1_cache['gnn_feat'] = abstract_features_1
+        else:
+            abstract_features_1 = self.gnn_1_cache['gnn_feat']
+        if 'gnn_feat' not in self.gnn_2_cache:
+            abstract_features_2 = self.convolutional_pass(Adj2,features_2)
+            self.gnn_2_cache['gnn_feat'] = abstract_features_2
+        else:
+            abstract_features_2 = self.gnn_2_cache['gnn_feat']
+    
+        graph_1_mask = torch.ones_like(batch_1)
+        graph_2_mask = torch.ones_like(batch_2)
+        graph_1_matched = partial_pmat.sum(dim=-1).to(dtype=torch.bool)[:graph_1_mask.shape[0]]
+        graph_2_matched = partial_pmat.sum(dim=-2).to(dtype=torch.bool)[:graph_2_mask.shape[0]]
+        graph_1_mask = torch.logical_not(graph_1_matched)
+        graph_2_mask = torch.logical_not(graph_2_matched)
+        abstract_features_1 = abstract_features_1[graph_1_mask]
+        abstract_features_2 = abstract_features_2[graph_2_mask]
+        
+        batch_1 = batch_1[graph_1_mask]
+        batch_2 = batch_2[graph_2_mask]
+        
+        if self.args['histogram']:
+            hist = self.calculate_histogram(abstract_features_1, abstract_features_2, batch_1, batch_2)
+
+        if self.args['diffpool']:
+            pooled_features_1 = self.diffpool(abstract_features_1, edge_index_1, batch_1)
+            pooled_features_2 = self.diffpool(abstract_features_2, edge_index_2, batch_2)
+        else:
+            pooled_features_1 = self.attention(abstract_features_1, batch_1)
+            pooled_features_2 = self.attention(abstract_features_2, batch_2)
+
+        scores = self.tensor_network(pooled_features_1, pooled_features_2)
+        
+        if self.args['histogram']:
+            scores = torch.cat((scores, hist), dim=1)
+
+        score = self.scoring_layer(scores).view(-1)
+        
+        if return_ged_norm:
+            return score
+        else:
+            ged = - torch.log(score) * (batch_1.shape[0] + batch_2.shape[0]) / 2
+            return ged
+
+    def heuristic_prediction_hun(self, k, n1, n2, partial_pmat):
+        k_prime = k.reshape(-1, n1+1, n2+1)
+        node_costs = torch.empty(k_prime.shape[0])
+        for i in range(k_prime.shape[0]):
+            _, node_costs[i] = hungarian_ged(k_prime[i], n1, n2)
+        node_cost_mat = node_costs.reshape(n1+1, n2+1)
+        self.heuristic_cache['node_cost'] = node_cost_mat
+
+        graph_1_mask = ~partial_pmat.sum(dim=-1).to(dtype=torch.bool)
+        graph_2_mask = ~partial_pmat.sum(dim=-2).to(dtype=torch.bool)
+        graph_1_mask[-1] = 1
+        graph_2_mask[-1] = 1
+        node_cost_mat = node_cost_mat[graph_1_mask, :]
+        node_cost_mat = node_cost_mat[:, graph_2_mask]
+
+        _, ged = hungarian_ged(node_cost_mat, torch.sum(graph_1_mask[:-1]), torch.sum(graph_2_mask[:-1]))
+    
+        return ged
+def hungarian_ged(node_cost_mat, n1, n2):
+    assert node_cost_mat.shape[-2] == n1+1
+    assert node_cost_mat.shape[-1] == n2+1
+    device = node_cost_mat.device
+    upper_left = node_cost_mat[:n1, :n2]
+    upper_right = torch.full((n1, n1), float('inf'), device=device)
+    torch.diagonal(upper_right)[:] = node_cost_mat[:-1, -1]
+    lower_left = torch.full((n2, n2), float('inf'), device=device)
+    torch.diagonal(lower_left)[:] = node_cost_mat[-1, :-1]
+    lower_right = torch.zeros((n2, n1), device=device)
+    large_cost_mat = torch.cat((torch.cat((upper_left, upper_right), dim=1),
+                                torch.cat((lower_left, lower_right), dim=1)), dim=0)
+    
+    large_pred_x = hungarian(-large_cost_mat.unsqueeze(dim=0)).squeeze()
+    pred_x = torch.zeros_like(node_cost_mat)
+    pred_x[:n1, :n2] = large_pred_x[:n1, :n2]
+    pred_x[:-1, -1] = torch.sum(large_pred_x[:n1, n2:], dim=1)
+    pred_x[-1, :-1] = torch.sum(large_pred_x[n1:, :n2], dim=0)
+
+    ged_lower_bound = torch.sum(pred_x * node_cost_mat)
+    return pred_x, ged_lower_bound
+
 def a_star(feat1,feat2,A1,A2,n1,n2,network,pretrain,**kwargs):
     args = default_parameter()
     if pretrain == 'LINUX':
         args['feature_num'] = 8
     elif pretrain == 'AIDS700nef':
         args['feature_num'] = 36
     args['pretrain'] = pretrain
@@ -890,202 +1191,14 @@
         assert A1.shape[0] == A2.shape[0]
         data = Graph_pair(feat1,feat2,A1,A2,n1,n2)
         result = network(data) 
     else:
         result = None
     return result, network
 
-def default_parameter():
-    params = {}
-    params['cuda'] = False
-    params['pretrain'] = False
-    params['feature_num'] = 36
-    params['filters_1'] = 64
-    params['filters_2'] = 32
-    params['filters_3'] = 16
-    params['tensor_neurons'] = 16
-    params['bottle_neck_neurons'] = 16
-    params['bins'] = 16
-    params['dropout'] = 0
-    params['astar_beamwidth'] = 0
-    params['astar_trustfact'] = 1
-    params['astar_nopred'] = 0
-    params['use_net'] = True
-    params['histogram'] = False
-    params['diffpool'] = False 
-    return params
-
-def check_layer_parameter(params):
-    if(params['pretrain'] == 'AIDS700nef'):
-        if params['feature_num'] != 36:
-            return False
-    elif(params['pretrain'] == 'LINUX'):
-        if params['feature_num'] != 8:
-            return False
-    if params['filters_1'] != 64:
-        return False
-    if params['filters_2'] != 32:
-        return False
-    if params['filters_3'] != 16:
-        return False
-    if params['tensor_neurons'] != 16:
-        return False
-    if params['bottle_neck_neurons'] != 16:
-        return False
-    return True
-
-def hungarian_ged(node_cost_mat, n1, n2):
-    assert node_cost_mat.shape[-2] == n1+1
-    assert node_cost_mat.shape[-1] == n2+1
-    device = node_cost_mat.device
-    upper_left = node_cost_mat[:n1, :n2]
-    upper_right = torch.full((n1, n1), float('inf'), device=device)
-    torch.diagonal(upper_right)[:] = node_cost_mat[:-1, -1]
-    lower_left = torch.full((n2, n2), float('inf'), device=device)
-    torch.diagonal(lower_left)[:] = node_cost_mat[-1, :-1]
-    lower_right = torch.zeros((n2, n1), device=device)
-    large_cost_mat = torch.cat((torch.cat((upper_left, upper_right), dim=1),
-                                torch.cat((lower_left, lower_right), dim=1)), dim=0)
-    
-    large_pred_x = hungarian(-large_cost_mat.unsqueeze(dim=0)).squeeze()
-    pred_x = torch.zeros_like(node_cost_mat)
-    pred_x[:n1, :n2] = large_pred_x[:n1, :n2]
-    pred_x[:-1, -1] = torch.sum(large_pred_x[:n1, n2:], dim=1)
-    pred_x[-1, :-1] = torch.sum(large_pred_x[n1:, :n2], dim=0)
-
-    ged_lower_bound = torch.sum(pred_x * node_cost_mat)
-    return pred_x, ged_lower_bound
-
-def broadcast(src: torch.Tensor, other: torch.Tensor, dim: int):
-    if dim < 0:
-        dim = other.dim() + dim
-    if src.dim() == 1:
-        for _ in range(0, dim):
-            src = src.unsqueeze(0)
-    for _ in range(src.dim(), other.dim()):
-        src = src.unsqueeze(-1)
-    src = src.expand(other.size())
-    return src
-
-def scatter_sum(src: torch.Tensor, index: torch.Tensor, dim: int = -1,
-                out: Optional[torch.Tensor] = None,
-                dim_size: Optional[int] = None) -> torch.Tensor:
-    index = broadcast(index, src, dim)
-    if out is None:
-        size = list(src.size())
-        if dim_size is not None:
-            size[dim] = dim_size
-        elif index.numel() == 0:
-            size[dim] = 0
-        else:
-            size[dim] = int(index.max()) + 1
-        out = torch.zeros(size, dtype=src.dtype, device=src.device)
-        return out.scatter_add_(dim, index, src)
-    else:
-        return out.scatter_add_(dim, index, src)
-
-def scatter_mean(src: torch.Tensor, index: torch.Tensor, dim: int = -1,
-                 out: Optional[torch.Tensor] = None,
-                 dim_size: Optional[int] = None) -> torch.Tensor:
-    out = scatter_sum(src, index, dim, out, dim_size)
-    dim_size = out.size(dim)
-
-    index_dim = dim
-    if index_dim < 0:
-        index_dim = index_dim + src.dim()
-    if index.dim() <= index_dim:
-        index_dim = index.dim() - 1
-
-    ones = torch.ones(index.size(), dtype=src.dtype, device=src.device)
-    count = scatter_sum(ones, index, index_dim, None, dim_size)
-    count[count < 1] = 1
-    count = broadcast(count, out, dim)
-    if out.is_floating_point():
-        out.true_divide_(count)
-    else:
-        out.div_(count, rounding_mode='floor')
-    return out 
-
-def to_dense_batch(x: Tensor, batch: Optional[Tensor] = None,
-                   fill_value: float = 0., max_num_nodes: Optional[int] = None,
-                   batch_size: Optional[int] = None) -> Tuple[Tensor, Tensor]:
-    if batch is None and max_num_nodes is None:
-        mask = torch.ones(1, x.size(0), dtype=torch.bool, device=x.device)
-        return x.unsqueeze(0), mask
-
-    if batch is None:
-        batch = x.new_zeros(x.size(0), dtype=torch.long)
-
-    if batch_size is None:
-        batch_size = int(batch.max()) + 1
-
-    num_nodes = scatter_sum(batch.new_ones(x.size(0)), batch, dim=0,
-                            dim_size=batch_size)
-    cum_nodes = torch.cat([batch.new_zeros(1), num_nodes.cumsum(dim=0)])
-
-    if max_num_nodes is None:
-        max_num_nodes = int(num_nodes.max())
-
-    idx = torch.arange(batch.size(0), dtype=torch.long, device=x.device)
-    idx = (idx - cum_nodes[batch]) + (batch * max_num_nodes)
-
-    size = [batch_size * max_num_nodes] + list(x.size())[1:]
-    out = x.new_full(size, fill_value)
-    out[idx] = x
-    out = out.view([batch_size, max_num_nodes] + list(x.size())[1:])
-
-    mask = torch.zeros(batch_size * max_num_nodes, dtype=torch.bool,
-                       device=x.device)
-    mask[idx] = 1
-    mask = mask.view(batch_size, max_num_nodes)
-
-    return out, mask
-
-def to_dense_adj(edge_index: Tensor,batch=None,edge_attr=None,max_num_nodes: Optional[int] = None) -> Tensor:
-    if batch is None:
-        num_nodes = int(edge_index.max()) + 1 if edge_index.numel() > 0 else 0
-        batch = edge_index.new_zeros(num_nodes)
-
-    batch_size = int(batch.max()) + 1 if batch.numel() > 0 else 1
-    one = batch.new_ones(batch.size(0))
-    num_nodes = scatter_sum(one, batch, dim=0, dim_size=batch_size)
-    cum_nodes = torch.cat([batch.new_zeros(1), num_nodes.cumsum(dim=0)])
-
-    idx0 = batch[edge_index[0]]
-    idx1 = edge_index[0] - cum_nodes[batch][edge_index[0]]
-    idx2 = edge_index[1] - cum_nodes[batch][edge_index[1]]
-
-    if max_num_nodes is None:
-        max_num_nodes = num_nodes.max().item()
-
-    elif ((idx1.numel() > 0 and idx1.max() >= max_num_nodes)
-          or (idx2.numel() > 0 and idx2.max() >= max_num_nodes)):
-        mask = (idx1 < max_num_nodes) & (idx2 < max_num_nodes)
-        idx0 = idx0[mask]
-        idx1 = idx1[mask]
-        idx2 = idx2[mask]
-        edge_attr = None if edge_attr is None else edge_attr[mask]
-
-    if edge_attr is None:
-        edge_attr = torch.ones(idx0.numel(), device=edge_index.device)
-
-    size = [batch_size, max_num_nodes, max_num_nodes]
-    size += list(edge_attr.size())[1:]
-    adj = torch.zeros(size, dtype=edge_attr.dtype, device=edge_index.device)
-
-    flattened_size = batch_size * max_num_nodes * max_num_nodes
-    adj = adj.view([flattened_size] + list(adj.size())[3:])
-    idx = idx0 * max_num_nodes * max_num_nodes + idx1 * max_num_nodes + idx2
-    adj = scatter_sum(edge_attr, idx, dim=0, dim_size=flattened_size)
-    adj = adj.view(size)
-
-    return adj
-
-
-
 ############################################
 #          Neural Network Solvers          #
 ############################################
 
 from pygmtools.pytorch_modules import *
```

### Comparing `pygmtools-0.3.8a0/pygmtools/pytorch_modules.py` & `pygmtools-0.3.8a2/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/tensorflow_backend.py` & `pygmtools-0.3.8a2/pygmtools/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools/utils.py` & `pygmtools-0.3.8a2/pygmtools/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.3.8a2/pygmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a0
+Version: 0.3.8a2
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a0/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.3.8a2/pygmtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/setup.py` & `pygmtools-0.3.8a2/setup.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/tests/test_classic_solvers.py` & `pygmtools-0.3.8a2/tests/test_classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/tests/test_dataset.py` & `pygmtools-0.3.8a2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/tests/test_misc.py` & `pygmtools-0.3.8a2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/tests/test_multi_graph_solvers.py` & `pygmtools-0.3.8a2/tests/test_multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/tests/test_neural_solvers.py` & `pygmtools-0.3.8a2/tests/test_neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a0/tests/test_utils.py` & `pygmtools-0.3.8a2/tests/test_utils.py`

 * *Files identical despite different names*


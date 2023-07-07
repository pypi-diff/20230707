# Comparing `tmp/pygmtools-0.3.8a2.tar.gz` & `tmp/pygmtools-0.3.8a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.3.8a2.tar", last modified: Fri Jul  7 11:53:26 2023, max compression
+gzip compressed data, was "pygmtools-0.3.8a3.tar", last modified: Fri Jul  7 12:51:51 2023, max compression
```

## Comparing `pygmtools-0.3.8a2.tar` & `pygmtools-0.3.8a3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 11:53:26.219340 pygmtools-0.3.8a2/
--rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/LICENSE
--rw-rw-rw-   0        0        0       18 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/MANIFEST.in
--rw-rw-rw-   0        0        0    13827 2023-07-07 11:53:26.218337 pygmtools-0.3.8a2/PKG-INFO
--rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 11:53:26.212757 pygmtools-0.3.8a2/pygmtools/
--rw-rw-rw-   0        0        0     2120 2023-07-07 11:53:18.000000 pygmtools-0.3.8a2/pygmtools/__init__.py
--rw-rw-rw-   0        0        0    58368 2023-07-07 11:50:59.000000 pygmtools-0.3.8a2/pygmtools/a_star.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    27000 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/benchmark.py
--rw-rw-rw-   0        0        0    58667 2023-06-24 14:15:49.000000 pygmtools-0.3.8a2/pygmtools/classic_solvers.py
--rw-rw-rw-   0        0        0    59231 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/dataset.py
--rw-rw-rw-   0        0        0     3112 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/dataset_config.py
--rw-rw-rw-   0        0        0    58908 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/jittor_backend.py
--rw-rw-rw-   0        0        0    12371 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/jittor_modules.py
--rw-rw-rw-   0        0        0    77128 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/linear_solvers.py
--rw-rw-rw-   0        0        0    21736 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/mindspore_backend.py
--rw-rw-rw-   0        0        0    44038 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/multi_graph_solvers.py
--rw-rw-rw-   0        0        0    70477 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/neural_solvers.py
--rw-rw-rw-   0        0        0    60669 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/numpy_backend.py
--rw-rw-rw-   0        0        0    15282 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/numpy_modules.py
--rw-rw-rw-   0        0        0    57860 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/paddle_backend.py
--rw-rw-rw-   0        0        0    11899 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/paddle_modules.py
--rw-rw-rw-   0        0        0    15470 2023-07-07 11:46:26.000000 pygmtools-0.3.8a2/pygmtools/pytorch_astar_modules.py
--rw-rw-rw-   0        0        0    74399 2023-07-07 11:49:03.000000 pygmtools-0.3.8a2/pygmtools/pytorch_backend.py
--rw-rw-rw-   0        0        0    12329 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/pytorch_modules.py
--rw-rw-rw-   0        0        0    23046 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/tensorflow_backend.py
--rw-rw-rw-   0        0        0      508 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/tensorflow_modules.py
--rw-rw-rw-   0        0        0    51707 2023-06-19 13:47:03.000000 pygmtools-0.3.8a2/pygmtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:53:26.215158 pygmtools-0.3.8a2/pygmtools.egg-info/
--rw-rw-rw-   0        0        0    13827 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      978 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 11:53:26.000000 pygmtools-0.3.8a2/pygmtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 11:53:26.219340 pygmtools-0.3.8a2/setup.cfg
--rw-rw-rw-   0        0        0     5818 2023-07-07 09:10:43.000000 pygmtools-0.3.8a2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:53:26.218337 pygmtools-0.3.8a2/tests/
--rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a2/tests/test_classic_solvers.py
--rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_dataset.py
--rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_misc.py
--rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_multi_graph_solvers.py
--rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_neural_solvers.py
--rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:51:51.425459 pygmtools-0.3.8a3/
+-rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a3/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-05-03 08:07:01.000000 pygmtools-0.3.8a3/MANIFEST.in
+-rw-rw-rw-   0        0        0    13827 2023-07-07 12:51:51.425459 pygmtools-0.3.8a3/PKG-INFO
+-rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 12:51:51.420207 pygmtools-0.3.8a3/pygmtools/
+-rw-rw-rw-   0        0        0     2120 2023-07-07 12:51:46.000000 pygmtools-0.3.8a3/pygmtools/__init__.py
+-rw-rw-rw-   0        0        0    58368 2023-07-07 12:51:51.000000 pygmtools-0.3.8a3/pygmtools/a_star.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0    27000 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/benchmark.py
+-rw-rw-rw-   0        0        0    58666 2023-07-07 12:42:20.000000 pygmtools-0.3.8a3/pygmtools/classic_solvers.py
+-rw-rw-rw-   0        0        0    59231 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/dataset.py
+-rw-rw-rw-   0        0        0     3112 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/dataset_config.py
+-rw-rw-rw-   0        0        0    58908 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/jittor_backend.py
+-rw-rw-rw-   0        0        0    12371 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/jittor_modules.py
+-rw-rw-rw-   0        0        0    77128 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/linear_solvers.py
+-rw-rw-rw-   0        0        0    21736 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/mindspore_backend.py
+-rw-rw-rw-   0        0        0    44038 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/multi_graph_solvers.py
+-rw-rw-rw-   0        0        0    70477 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/neural_solvers.py
+-rw-rw-rw-   0        0        0    60669 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/numpy_backend.py
+-rw-rw-rw-   0        0        0    15282 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/numpy_modules.py
+-rw-rw-rw-   0        0        0    57860 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/paddle_backend.py
+-rw-rw-rw-   0        0        0    11899 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/paddle_modules.py
+-rw-rw-rw-   0        0        0    15443 2023-07-07 12:38:50.000000 pygmtools-0.3.8a3/pygmtools/pytorch_astar_modules.py
+-rw-rw-rw-   0        0        0    74570 2023-07-07 12:48:54.000000 pygmtools-0.3.8a3/pygmtools/pytorch_backend.py
+-rw-rw-rw-   0        0        0    12329 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/pytorch_modules.py
+-rw-rw-rw-   0        0        0    23046 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/tensorflow_backend.py
+-rw-rw-rw-   0        0        0      508 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/tensorflow_modules.py
+-rw-rw-rw-   0        0        0    51707 2023-07-07 11:54:30.000000 pygmtools-0.3.8a3/pygmtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:51:51.422263 pygmtools-0.3.8a3/pygmtools.egg-info/
+-rw-rw-rw-   0        0        0    13827 2023-07-07 12:51:51.000000 pygmtools-0.3.8a3/pygmtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2023-07-07 12:51:51.000000 pygmtools-0.3.8a3/pygmtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 12:51:51.000000 pygmtools-0.3.8a3/pygmtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-07 12:51:51.000000 pygmtools-0.3.8a3/pygmtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 12:51:51.000000 pygmtools-0.3.8a3/pygmtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 12:51:51.425459 pygmtools-0.3.8a3/setup.cfg
+-rw-rw-rw-   0        0        0     5818 2023-07-07 09:10:43.000000 pygmtools-0.3.8a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 12:51:51.425459 pygmtools-0.3.8a3/tests/
+-rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a3/tests/test_classic_solvers.py
+-rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a3/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a3/tests/test_misc.py
+-rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a3/tests/test_multi_graph_solvers.py
+-rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a3/tests/test_neural_solvers.py
+-rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a3/tests/test_utils.py
```

### Comparing `pygmtools-0.3.8a2/PKG-INFO` & `pygmtools-0.3.8a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a2
+Version: 0.3.8a3
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a2/README.md` & `pygmtools-0.3.8a3/README.md`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/__init__.py` & `pygmtools-0.3.8a3/pygmtools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .benchmark import Benchmark
 from .linear_solvers import sinkhorn, hungarian
 from .classic_solvers import rrwm, sm, ipfp, a_star
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm
 import pygmtools.utils as utils
 BACKEND = 'numpy'
-__version__ = '0.3.8-alpha2'
+__version__ = '0.3.8-alpha3'
 __author__ = 'ThinkLab at SJTU'
 
 
 def env_report():
     """
     Print environment report
     """
```

### Comparing `pygmtools-0.3.8a2/pygmtools/benchmark.py` & `pygmtools-0.3.8a3/pygmtools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/classic_solvers.py` & `pygmtools-0.3.8a3/pygmtools/classic_solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1226,15 +1226,15 @@
                 f'feat2:{_get_shape(feat2, backend)}, A1:{_get_shape(A1, backend)}, A2:{_get_shape(A2, backend)}!')
     if n1 is not None: _check_data_type(n1, 'n1', backend)
     if n2 is not None: _check_data_type(n2, 'n2', backend)
 
     args = (feat1, feat2, A1, A2, n1, n2, network, pretrain)
     try:
         mod = importlib.import_module(f'pygmtools.{backend}_backend')
-        fn = mod.a_star
+        fn = mod.astar
     except (ModuleNotFoundError, AttributeError):
         raise NotImplementedError(
             NOT_IMPLEMENTED_MSG.format(backend)
         )
 
     result = fn(*args,**kwargs)
     match_mat = _squeeze(result[0], 0, backend) if non_batched_input else result[0]
```

### Comparing `pygmtools-0.3.8a2/pygmtools/dataset.py` & `pygmtools-0.3.8a3/pygmtools/dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/dataset_config.py` & `pygmtools-0.3.8a3/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/jittor_backend.py` & `pygmtools-0.3.8a3/pygmtools/jittor_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/jittor_modules.py` & `pygmtools-0.3.8a3/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/linear_solvers.py` & `pygmtools-0.3.8a3/pygmtools/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/mindspore_backend.py` & `pygmtools-0.3.8a3/pygmtools/mindspore_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/multi_graph_solvers.py` & `pygmtools-0.3.8a3/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/neural_solvers.py` & `pygmtools-0.3.8a3/pygmtools/neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/numpy_backend.py` & `pygmtools-0.3.8a3/pygmtools/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/numpy_modules.py` & `pygmtools-0.3.8a3/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/paddle_backend.py` & `pygmtools-0.3.8a3/pygmtools/paddle_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/paddle_modules.py` & `pygmtools-0.3.8a3/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/pytorch_astar_modules.py` & `pygmtools-0.3.8a3/pygmtools/pytorch_astar_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pygmtools.utils
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.parameter import Parameter
 from torch import Tensor
 from typing import Optional, Tuple
 VERY_LARGE_INT = 65536
-from a_star import a_star
 
 ###############################################################
 #                      GENN-A*  Functions                     #
 ###############################################################
 
 def default_parameter():
     params = {}
```

### Comparing `pygmtools-0.3.8a2/pygmtools/pytorch_backend.py` & `pygmtools-0.3.8a3/pygmtools/pytorch_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 import functools
 import torch
 import numpy as np
 from multiprocessing import Pool
 from torch import Tensor
 import os
 import pygmtools.utils
-from pytorch_astar_modules import *
+from .a_star import a_star
+from .pytorch_astar_modules import GCNConv,AttentionModule,TensorNetworkModule,\
+    Graph_pair,VERY_LARGE_INT,to_dense_adj,to_dense_batch,default_parameter,check_layer_parameter
 import warnings
 from torch import Tensor
 
 #############################################
 #     Linear Assignment Problem Solvers     #
 #############################################
 
@@ -1144,15 +1146,15 @@
     pred_x[:n1, :n2] = large_pred_x[:n1, :n2]
     pred_x[:-1, -1] = torch.sum(large_pred_x[:n1, n2:], dim=1)
     pred_x[-1, :-1] = torch.sum(large_pred_x[n1:, :n2], dim=0)
 
     ged_lower_bound = torch.sum(pred_x * node_cost_mat)
     return pred_x, ged_lower_bound
 
-def a_star(feat1,feat2,A1,A2,n1,n2,network,pretrain,**kwargs):
+def astar(feat1,feat2,A1,A2,n1,n2,network,pretrain,**kwargs):
     args = default_parameter()
     if pretrain == 'LINUX':
         args['feature_num'] = 8
     elif pretrain == 'AIDS700nef':
         args['feature_num'] = 36
     args['pretrain'] = pretrain
```

### Comparing `pygmtools-0.3.8a2/pygmtools/pytorch_modules.py` & `pygmtools-0.3.8a3/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/tensorflow_backend.py` & `pygmtools-0.3.8a3/pygmtools/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools/utils.py` & `pygmtools-0.3.8a3/pygmtools/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.3.8a3/pygmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a2
+Version: 0.3.8a3
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a2/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.3.8a3/pygmtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/setup.py` & `pygmtools-0.3.8a3/setup.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/tests/test_classic_solvers.py` & `pygmtools-0.3.8a3/tests/test_classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/tests/test_dataset.py` & `pygmtools-0.3.8a3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/tests/test_misc.py` & `pygmtools-0.3.8a3/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/tests/test_multi_graph_solvers.py` & `pygmtools-0.3.8a3/tests/test_multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/tests/test_neural_solvers.py` & `pygmtools-0.3.8a3/tests/test_neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a2/tests/test_utils.py` & `pygmtools-0.3.8a3/tests/test_utils.py`

 * *Files identical despite different names*


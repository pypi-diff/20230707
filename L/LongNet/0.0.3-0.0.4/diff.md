# Comparing `tmp/LongNet-0.0.3.tar.gz` & `tmp/LongNet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.0.3.tar", last modified: Fri Jul  7 04:25:15 2023, max compression
+gzip compressed data, was "LongNet-0.0.4.tar", last modified: Fri Jul  7 12:11:16 2023, max compression
```

## Comparing `LongNet-0.0.3.tar` & `LongNet-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:25:15.908628 LongNet-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 04:25:05.000000 LongNet-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:25:15.904628 LongNet-0.0.3/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:25:15.908628 LongNet-0.0.3/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 04:25:15.908628 LongNet-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-07 04:25:05.000000 LongNet-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 04:25:15.908628 LongNet-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 04:25:05.000000 LongNet-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:11:16.483978 LongNet-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 12:11:02.000000 LongNet-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:11:16.483978 LongNet-0.0.4/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 12:11:02.000000 LongNet-0.0.4/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:11:16.483978 LongNet-0.0.4/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 12:11:16.000000 LongNet-0.0.4/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 12:11:16.483978 LongNet-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-07 12:11:02.000000 LongNet-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:11:16.483978 LongNet-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 12:11:02.000000 LongNet-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:11:16.483978 LongNet-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 12:11:02.000000 LongNet-0.0.4/test/test.py
```

### Comparing `LongNet-0.0.3/LICENSE` & `LongNet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.3/LongNet/attention.py` & `LongNet-0.0.4/LongNet/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
         # Scatter and concatenate 
         attn_output = attn_output.view(batch_size, -1, self.d_model)
         return attn_output
 
 
 
-class LongNet(nn.Module):
+class LongNetTransformer(nn.Module):
     def __init__(self, d_model, num_heads, dilation_rates, segment_sizes):
-        super(LongNet, self).__init__()
+        super(LongNetTransformer, self).__init__()
         assert len(dilation_rates) == len(segment_sizes), "dilation_rates and segment_sizes should have the same length"
 
 
         self.d_model = d_model
         self.num_heads = num_heads
         self.dilation_rates = dilation_rates
         self.segment_sizes = segment_sizes
```

### Comparing `LongNet-0.0.3/LongNet/model.py` & `LongNet-0.0.4/LongNet/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from LongNet.torchscale.torchscale.architecture.decoder import DecoderConfig
+from torchscale.torchscale.architecture.decoder import DecoderConfig
 import torch
 from torchscale.architecture.decoder import Decoder
 
 from torchscale.component.embedding import PositionalEmbedding
 from transformers import CLIPProcessor, CLIPModel, AutoTokenizer
 from flamingo_pytorch import PerceiverResampler
```

### Comparing `LongNet-0.0.3/LongNet/training.py` & `LongNet-0.0.4/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.3/LongNet/utils.py` & `LongNet-0.0.4/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.3/LongNet.egg-info/PKG-INFO` & `LongNet-0.0.4/LongNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.0.3
+Version: 0.0.4
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.0.3/PKG-INFO` & `LongNet-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.0.3
+Version: 0.0.4
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.0.3/README.md` & `LongNet-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 ### Method 1 
 
 * Git clone installation
 
 * Init your parameters `accelerate config`
 
-* Then `accelerate LongNet/training.py`
+* Then `accelerate launch LongNet/training.py`
 
 # Method 2
 
 * Pip install method
 
 ```python
```

### Comparing `LongNet-0.0.3/setup.py` & `LongNet-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```


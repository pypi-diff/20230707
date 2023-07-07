# Comparing `tmp/LongNet-0.0.2.tar.gz` & `tmp/LongNet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.0.2.tar", last modified: Fri Jul  7 04:19:12 2023, max compression
+gzip compressed data, was "LongNet-0.0.3.tar", last modified: Fri Jul  7 04:25:15 2023, max compression
```

## Comparing `LongNet-0.0.2.tar` & `LongNet-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:19:12.800597 LongNet-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 04:19:01.000000 LongNet-0.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:19:12.800597 LongNet-0.0.2/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-07 04:19:01.000000 LongNet-0.0.2/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-07 04:19:01.000000 LongNet-0.0.2/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-07 04:19:01.000000 LongNet-0.0.2/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-07-07 04:19:01.000000 LongNet-0.0.2/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 04:19:01.000000 LongNet-0.0.2/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:19:12.800597 LongNet-0.0.2/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 04:19:12.000000 LongNet-0.0.2/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-07 04:19:12.000000 LongNet-0.0.2/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 04:19:12.000000 LongNet-0.0.2/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 04:19:12.000000 LongNet-0.0.2/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 04:19:12.000000 LongNet-0.0.2/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 04:19:12.800597 LongNet-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-07 04:19:01.000000 LongNet-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 04:19:12.800597 LongNet-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-07 04:19:01.000000 LongNet-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:25:15.908628 LongNet-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 04:25:05.000000 LongNet-0.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:25:15.904628 LongNet-0.0.3/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-07 04:25:05.000000 LongNet-0.0.3/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 04:25:15.908628 LongNet-0.0.3/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 04:25:15.000000 LongNet-0.0.3/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 04:25:15.908628 LongNet-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-07 04:25:05.000000 LongNet-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 04:25:15.908628 LongNet-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 04:25:05.000000 LongNet-0.0.3/setup.py
```

### Comparing `LongNet-0.0.2/LICENSE` & `LongNet-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.2/LongNet/attention.py` & `LongNet-0.0.3/LongNet/attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.2/LongNet/model.py` & `LongNet-0.0.3/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.2/LongNet/training.py` & `LongNet-0.0.3/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.2/LongNet/utils.py` & `LongNet-0.0.3/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.0.2/LongNet.egg-info/PKG-INFO` & `LongNet-0.0.3/LongNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.0.2
+Version: 0.0.3
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.0.2/PKG-INFO` & `LongNet-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.0.2
+Version: 0.0.3
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.0.2/README.md` & `LongNet-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,37 @@
 # Forward pass
 outputs = attention(inputs)
 
 # Print the output shape
 print(outputs.shape)  # Expected: [batch_size, seq_len, d_model]
 ```
 
+# Training the Model
+There are 2 methods, one is `accelerate` and the other `from LongNet import Train`
+
+### Method 1 
+
+* Git clone installation
+
+* Init your parameters `accelerate config`
+
+* Then `accelerate LongNet/training.py`
+
+# Method 2
+
+* Pip install method
+
+```python
+
+from LongNet import Train
+
+Train()
+
+```
+
 In the example above, we create an instance of the `DilatedAttention` class with the specified hyperparameters. We then generate some dummy input data and pass it through the attention mechanism to obtain the outputs. Finally, we print the shape of the output tensor.
 
 ## DilatedAttention Documentation
 
 The `DilatedAttention` class implements dilated attention, which expands the attentive field exponentially as the distance between tokens grows. It inherits from `torch.nn.Module` and can be used as a drop-in replacement for standard attention mechanisms in Transformer models.
 
 ### Parameters
```

### Comparing `LongNet-0.0.2/setup.py` & `LongNet-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
@@ -16,15 +16,17 @@
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
     install_requires=[
         'torch',
         'einops',
-        'flash_attn'
+        'flash-attn',
+        'accelerate',
+        'bitsandbytes'
     ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```


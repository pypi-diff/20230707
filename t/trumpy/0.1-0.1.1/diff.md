# Comparing `tmp/trumpy-0.1.tar.gz` & `tmp/trumpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trumpy-0.1.tar", last modified: Fri Jul  7 09:40:19 2023, max compression
+gzip compressed data, was "trumpy-0.1.1.tar", last modified: Fri Jul  7 09:46:25 2023, max compression
```

## Comparing `trumpy-0.1.tar` & `trumpy-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:40:19.040876 trumpy-0.1/
--rw-r--r--   0 youkaichao   (501) staff       (20)     1067 2023-07-07 09:11:21.000000 trumpy-0.1/LICENSE
--rw-r--r--   0 youkaichao   (501) staff       (20)      451 2023-07-07 09:40:19.040763 trumpy-0.1/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)     1466 2023-07-07 09:38:56.000000 trumpy-0.1/README.md
--rw-r--r--   0 youkaichao   (501) staff       (20)       38 2023-07-07 09:40:19.040912 trumpy-0.1/setup.cfg
--rw-r--r--   0 youkaichao   (501) staff       (20)      589 2023-07-07 09:27:46.000000 trumpy-0.1/setup.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:40:19.039921 trumpy-0.1/tests/
--rw-r--r--   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:15:05.000000 trumpy-0.1/tests/__init__.py
--rw-r--r--   0 youkaichao   (501) staff       (20)      945 2023-07-07 09:37:01.000000 trumpy-0.1/tests/test.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:40:19.040116 trumpy-0.1/trumpy/
--rw-r--r--   0 youkaichao   (501) staff       (20)       74 2023-07-07 09:18:39.000000 trumpy-0.1/trumpy/__init__.py
--rw-r--r--   0 youkaichao   (501) staff       (20)     1723 2023-07-07 09:28:50.000000 trumpy-0.1/trumpy/lib.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:40:19.040600 trumpy-0.1/trumpy.egg-info/
--rw-r--r--   0 youkaichao   (501) staff       (20)      451 2023-07-07 09:40:18.000000 trumpy-0.1/trumpy.egg-info/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      240 2023-07-07 09:40:19.000000 trumpy-0.1/trumpy.egg-info/SOURCES.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)        1 2023-07-07 09:40:18.000000 trumpy-0.1/trumpy.egg-info/dependency_links.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       26 2023-07-07 09:40:18.000000 trumpy-0.1/trumpy.egg-info/requires.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       13 2023-07-07 09:40:18.000000 trumpy-0.1/trumpy.egg-info/top_level.txt
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:46:25.193021 trumpy-0.1.1/
+-rw-r--r--   0 youkaichao   (501) staff       (20)     1067 2023-07-07 09:11:21.000000 trumpy-0.1.1/LICENSE
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2516 2023-07-07 09:46:25.192910 trumpy-0.1.1/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2030 2023-07-07 09:45:54.000000 trumpy-0.1.1/README.md
+-rw-r--r--   0 youkaichao   (501) staff       (20)       38 2023-07-07 09:46:25.193058 trumpy-0.1.1/setup.cfg
+-rw-r--r--   0 youkaichao   (501) staff       (20)      890 2023-07-07 09:43:36.000000 trumpy-0.1.1/setup.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:46:25.191727 trumpy-0.1.1/tests/
+-rw-r--r--   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:15:05.000000 trumpy-0.1.1/tests/__init__.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)      945 2023-07-07 09:37:01.000000 trumpy-0.1.1/tests/test.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:46:25.192144 trumpy-0.1.1/trumpy/
+-rw-r--r--   0 youkaichao   (501) staff       (20)       74 2023-07-07 09:18:39.000000 trumpy-0.1.1/trumpy/__init__.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)     1723 2023-07-07 09:28:50.000000 trumpy-0.1.1/trumpy/lib.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:46:25.192755 trumpy-0.1.1/trumpy.egg-info/
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2516 2023-07-07 09:46:24.000000 trumpy-0.1.1/trumpy.egg-info/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      240 2023-07-07 09:46:25.000000 trumpy-0.1.1/trumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)        1 2023-07-07 09:46:24.000000 trumpy-0.1.1/trumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       26 2023-07-07 09:46:25.000000 trumpy-0.1.1/trumpy.egg-info/requires.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       13 2023-07-07 09:46:25.000000 trumpy-0.1.1/trumpy.egg-info/top_level.txt
```

### Comparing `trumpy-0.1/LICENSE` & `trumpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trumpy-0.1/README.md` & `trumpy-0.1.1/tests/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-# TRUMPY: Tracing and Reverse Understanding Memory in Pytorch
-
-Analyze how much memory is used for calculating the backward propagation (excluding parameters and gradients). This function works by tracing the computation graph used for backward propagation.
-
-The fascinating thing is that it works in both GPU and CPU. Therefore, you can **first run the code in CPU to estimate the memory usage, which will then be a decent estimation of memory consumption in GPU**!
-
-Example usage is in `tests/test.py`.
-
-```python
 import torch
 from torchvision.models.resnet import resnet50
 
 # define device and models
 device = torch.device('cpu')
 net = resnet50().to(device)
 input = torch.rand(16, 3, 224, 224).to(device)
@@ -27,9 +18,8 @@
 print(f'estimated memory usage for backward related tensors in {device}: {saved_memory / 1024 ** 3} GB')
 
 # check how much memory pytorch holds
 if device != torch.device('cpu'):
     import gc
     gc.collect()
     saved_memory = torch.cuda.memory_allocated() - current_memory
-    print(f'ground-truth memory usage for backward related tensors in gpu: {saved_memory / 1024 ** 3} GB')
-```
+    print(f'ground-truth memory usage for backward related tensors in gpu: {saved_memory / 1024 ** 3} GB')
```

### Comparing `trumpy-0.1/setup.py` & `trumpy-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from setuptools import setup, find_packages
+from os import path
+
+# Get the long description from the README file
+here = path.abspath(path.dirname(__file__))
+with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name='trumpy',
-    version='0.1',
+    version='0.1.1',
     description='TRUMPY: Tracing and Reverse Understanding Memory in Pytorch',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='Kaichao You',
     author_email='youkaichao@gmail.com',
     url='https://github.com/youkaichao/TRUMPY',
     packages=find_packages(),
     install_requires=[
         'torch',
     ],
```

### Comparing `trumpy-0.1/trumpy/lib.py` & `trumpy-0.1.1/trumpy/lib.py`

 * *Files identical despite different names*


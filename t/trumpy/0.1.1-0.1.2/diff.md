# Comparing `tmp/trumpy-0.1.1.tar.gz` & `tmp/trumpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trumpy-0.1.1.tar", last modified: Fri Jul  7 09:46:25 2023, max compression
+gzip compressed data, was "trumpy-0.1.2.tar", last modified: Fri Jul  7 09:51:34 2023, max compression
```

## Comparing `trumpy-0.1.1.tar` & `trumpy-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:46:25.193021 trumpy-0.1.1/
--rw-r--r--   0 youkaichao   (501) staff       (20)     1067 2023-07-07 09:11:21.000000 trumpy-0.1.1/LICENSE
--rw-r--r--   0 youkaichao   (501) staff       (20)     2516 2023-07-07 09:46:25.192910 trumpy-0.1.1/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)     2030 2023-07-07 09:45:54.000000 trumpy-0.1.1/README.md
--rw-r--r--   0 youkaichao   (501) staff       (20)       38 2023-07-07 09:46:25.193058 trumpy-0.1.1/setup.cfg
--rw-r--r--   0 youkaichao   (501) staff       (20)      890 2023-07-07 09:43:36.000000 trumpy-0.1.1/setup.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:46:25.191727 trumpy-0.1.1/tests/
--rw-r--r--   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:15:05.000000 trumpy-0.1.1/tests/__init__.py
--rw-r--r--   0 youkaichao   (501) staff       (20)      945 2023-07-07 09:37:01.000000 trumpy-0.1.1/tests/test.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:46:25.192144 trumpy-0.1.1/trumpy/
--rw-r--r--   0 youkaichao   (501) staff       (20)       74 2023-07-07 09:18:39.000000 trumpy-0.1.1/trumpy/__init__.py
--rw-r--r--   0 youkaichao   (501) staff       (20)     1723 2023-07-07 09:28:50.000000 trumpy-0.1.1/trumpy/lib.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:46:25.192755 trumpy-0.1.1/trumpy.egg-info/
--rw-r--r--   0 youkaichao   (501) staff       (20)     2516 2023-07-07 09:46:24.000000 trumpy-0.1.1/trumpy.egg-info/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      240 2023-07-07 09:46:25.000000 trumpy-0.1.1/trumpy.egg-info/SOURCES.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)        1 2023-07-07 09:46:24.000000 trumpy-0.1.1/trumpy.egg-info/dependency_links.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       26 2023-07-07 09:46:25.000000 trumpy-0.1.1/trumpy.egg-info/requires.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       13 2023-07-07 09:46:25.000000 trumpy-0.1.1/trumpy.egg-info/top_level.txt
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:51:34.482982 trumpy-0.1.2/
+-rw-r--r--   0 youkaichao   (501) staff       (20)     1067 2023-07-07 09:11:21.000000 trumpy-0.1.2/LICENSE
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2790 2023-07-07 09:51:34.482865 trumpy-0.1.2/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2304 2023-07-07 09:50:16.000000 trumpy-0.1.2/README.md
+-rw-r--r--   0 youkaichao   (501) staff       (20)       38 2023-07-07 09:51:34.483018 trumpy-0.1.2/setup.cfg
+-rw-r--r--   0 youkaichao   (501) staff       (20)      890 2023-07-07 09:51:05.000000 trumpy-0.1.2/setup.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:51:34.481778 trumpy-0.1.2/tests/
+-rw-r--r--   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:15:05.000000 trumpy-0.1.2/tests/__init__.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)      941 2023-07-07 09:49:31.000000 trumpy-0.1.2/tests/test.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:51:34.482077 trumpy-0.1.2/trumpy/
+-rw-r--r--   0 youkaichao   (501) staff       (20)       74 2023-07-07 09:18:39.000000 trumpy-0.1.2/trumpy/__init__.py
+-rw-r--r--   0 youkaichao   (501) staff       (20)     1723 2023-07-07 09:28:50.000000 trumpy-0.1.2/trumpy/lib.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2023-07-07 09:51:34.482664 trumpy-0.1.2/trumpy.egg-info/
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2790 2023-07-07 09:51:34.000000 trumpy-0.1.2/trumpy.egg-info/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      240 2023-07-07 09:51:34.000000 trumpy-0.1.2/trumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)        1 2023-07-07 09:51:34.000000 trumpy-0.1.2/trumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       26 2023-07-07 09:51:34.000000 trumpy-0.1.2/trumpy.egg-info/requires.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       13 2023-07-07 09:51:34.000000 trumpy-0.1.2/trumpy.egg-info/top_level.txt
```

### Comparing `trumpy-0.1.1/LICENSE` & `trumpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trumpy-0.1.1/PKG-INFO` & `trumpy-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trumpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: TRUMPY: Tracing and Reverse Understanding Memory in Pytorch
 Home-page: https://github.com/youkaichao/TRUMPY
 Author: Kaichao You
 Author-email: youkaichao@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,16 @@
 
 # Install
 
 `pip install trumpy` or clone this repository and build it yourself.
 
 # Usage
 
+The core function is just one-line: `from trumpy import memory_for_backward; saved_memory = memory_for_backward(net, loss)`. You just pass the network and the calculated loss to this function, and it will give you how much memory (in bytes) is needed for backward propagation.
+
 Example usage is in `tests/test.py`.
 
 ```python
 import torch
 from torchvision.models.resnet import resnet50
 
 # define device and models
@@ -39,15 +41,15 @@
 
 # if gpu is available, record current memory
 if device != torch.device('cpu'):
     current_memory = torch.cuda.memory_allocated()
 
 # define loss function
 loss = net(input).sum() # loss is the starting point of the backward computation graph
-from trumpy.lib import memory_for_backward
+from trumpy import memory_for_backward
 # calculate the memory used for backward
 saved_memory = memory_for_backward(net, loss)
 print(f'estimated memory usage for backward related tensors in {device}: {saved_memory / 1024 ** 3} GB')
 
 # check how much memory pytorch holds
 if device != torch.device('cpu'):
     import gc
```

### Comparing `trumpy-0.1.1/README.md` & `trumpy-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 # Install
 
 `pip install trumpy` or clone this repository and build it yourself.
 
 # Usage
 
+The core function is just one-line: `from trumpy import memory_for_backward; saved_memory = memory_for_backward(net, loss)`. You just pass the network and the calculated loss to this function, and it will give you how much memory (in bytes) is needed for backward propagation.
+
 Example usage is in `tests/test.py`.
 
 ```python
 import torch
 from torchvision.models.resnet import resnet50
 
 # define device and models
@@ -23,15 +25,15 @@
 
 # if gpu is available, record current memory
 if device != torch.device('cpu'):
     current_memory = torch.cuda.memory_allocated()
 
 # define loss function
 loss = net(input).sum() # loss is the starting point of the backward computation graph
-from trumpy.lib import memory_for_backward
+from trumpy import memory_for_backward
 # calculate the memory used for backward
 saved_memory = memory_for_backward(net, loss)
 print(f'estimated memory usage for backward related tensors in {device}: {saved_memory / 1024 ** 3} GB')
 
 # check how much memory pytorch holds
 if device != torch.device('cpu'):
     import gc
```

### Comparing `trumpy-0.1.1/setup.py` & `trumpy-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Get the long description from the README file
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='trumpy',
-    version='0.1.1',
+    version='0.1.2',
     description='TRUMPY: Tracing and Reverse Understanding Memory in Pytorch',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Kaichao You',
     author_email='youkaichao@gmail.com',
     url='https://github.com/youkaichao/TRUMPY',
     packages=find_packages(),
```

### Comparing `trumpy-0.1.1/tests/test.py` & `trumpy-0.1.2/tests/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # if gpu is available, record current memory
 if device != torch.device('cpu'):
     current_memory = torch.cuda.memory_allocated()
 
 # define loss function
 loss = net(input).sum() # loss is the starting point of the backward computation graph
-from trumpy.lib import memory_for_backward
+from trumpy import memory_for_backward
 # calculate the memory used for backward
 saved_memory = memory_for_backward(net, loss)
 print(f'estimated memory usage for backward related tensors in {device}: {saved_memory / 1024 ** 3} GB')
 
 # check how much memory pytorch holds
 if device != torch.device('cpu'):
     import gc
```

### Comparing `trumpy-0.1.1/trumpy/lib.py` & `trumpy-0.1.2/trumpy/lib.py`

 * *Files identical despite different names*

### Comparing `trumpy-0.1.1/trumpy.egg-info/PKG-INFO` & `trumpy-0.1.2/trumpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trumpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: TRUMPY: Tracing and Reverse Understanding Memory in Pytorch
 Home-page: https://github.com/youkaichao/TRUMPY
 Author: Kaichao You
 Author-email: youkaichao@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,16 @@
 
 # Install
 
 `pip install trumpy` or clone this repository and build it yourself.
 
 # Usage
 
+The core function is just one-line: `from trumpy import memory_for_backward; saved_memory = memory_for_backward(net, loss)`. You just pass the network and the calculated loss to this function, and it will give you how much memory (in bytes) is needed for backward propagation.
+
 Example usage is in `tests/test.py`.
 
 ```python
 import torch
 from torchvision.models.resnet import resnet50
 
 # define device and models
@@ -39,15 +41,15 @@
 
 # if gpu is available, record current memory
 if device != torch.device('cpu'):
     current_memory = torch.cuda.memory_allocated()
 
 # define loss function
 loss = net(input).sum() # loss is the starting point of the backward computation graph
-from trumpy.lib import memory_for_backward
+from trumpy import memory_for_backward
 # calculate the memory used for backward
 saved_memory = memory_for_backward(net, loss)
 print(f'estimated memory usage for backward related tensors in {device}: {saved_memory / 1024 ** 3} GB')
 
 # check how much memory pytorch holds
 if device != torch.device('cpu'):
     import gc
```


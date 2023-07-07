# Comparing `tmp/explainable_cnn-0.0.9.tar.gz` & `tmp/explainable_cnn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainable_cnn-0.0.9.tar", last modified: Wed Apr 13 18:39:41 2022, max compression
+gzip compressed data, was "explainable_cnn-1.0.0.tar", last modified: Fri Jul  7 06:15:08 2023, max compression
```

## Comparing `explainable_cnn-0.0.9.tar` & `explainable_cnn-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2022-04-13 18:39:41.945317 explainable_cnn-0.0.9/
--rw-r--r--   0 ashutosh1919   (501) staff       (20)     1075 2022-03-13 20:42:52.000000 explainable_cnn-0.0.9/LICENSE
--rw-r--r--   0 ashutosh1919   (501) staff       (20)     5179 2022-04-13 18:39:41.945200 explainable_cnn-0.0.9/PKG-INFO
--rw-r--r--   0 ashutosh1919   (501) staff       (20)     4547 2022-03-27 22:49:23.000000 explainable_cnn-0.0.9/README.md
--rw-r--r--   0 ashutosh1919   (501) staff       (20)       84 2022-03-24 20:36:15.000000 explainable_cnn-0.0.9/pyproject.toml
--rw-r--r--   0 ashutosh1919   (501) staff       (20)       38 2022-04-13 18:39:41.945368 explainable_cnn-0.0.9/setup.cfg
--rw-r--r--   0 ashutosh1919   (501) staff       (20)      952 2022-04-13 18:38:50.000000 explainable_cnn-0.0.9/setup.py
-drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2022-04-13 18:39:41.941101 explainable_cnn-0.0.9/src/
-drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2022-04-13 18:39:41.942081 explainable_cnn-0.0.9/src/explainable_cnn/
--rw-r--r--   0 ashutosh1919   (501) staff       (20)       41 2022-03-24 19:46:24.000000 explainable_cnn-0.0.9/src/explainable_cnn/__init__.py
-drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2022-04-13 18:39:41.944042 explainable_cnn-0.0.9/src/explainable_cnn/explainers/
--rw-r--r--   0 ashutosh1919   (501) staff       (20)      161 2022-03-24 19:11:39.000000 explainable_cnn-0.0.9/src/explainable_cnn/explainers/__init__.py
--rw-r--r--   0 ashutosh1919   (501) staff       (20)     3847 2022-03-24 19:18:34.000000 explainable_cnn-0.0.9/src/explainable_cnn/explainers/base_explainer.py
--rw-r--r--   0 ashutosh1919   (501) staff       (20)    12366 2022-04-13 18:34:33.000000 explainable_cnn-0.0.9/src/explainable_cnn/explainers/cnn_explainer.py
--rw-r--r--   0 ashutosh1919   (501) staff       (20)     6875 2022-04-13 18:28:00.000000 explainable_cnn-0.0.9/src/explainable_cnn/explainers/grad_cam.py
-drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2022-04-13 18:39:41.944826 explainable_cnn-0.0.9/src/explainable_cnn/validators/
--rw-r--r--   0 ashutosh1919   (501) staff       (20)      111 2022-03-24 18:59:36.000000 explainable_cnn-0.0.9/src/explainable_cnn/validators/__init__.py
--rw-r--r--   0 ashutosh1919   (501) staff       (20)     1004 2022-03-24 19:00:16.000000 explainable_cnn-0.0.9/src/explainable_cnn/validators/base_validator.py
--rw-r--r--   0 ashutosh1919   (501) staff       (20)     1961 2022-03-24 19:11:14.000000 explainable_cnn-0.0.9/src/explainable_cnn/validators/cnn_validator.py
-drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2022-04-13 18:39:41.943103 explainable_cnn-0.0.9/src/explainable_cnn.egg-info/
--rw-r--r--   0 ashutosh1919   (501) staff       (20)     5179 2022-04-13 18:39:41.000000 explainable_cnn-0.0.9/src/explainable_cnn.egg-info/PKG-INFO
--rw-r--r--   0 ashutosh1919   (501) staff       (20)      568 2022-04-13 18:39:41.000000 explainable_cnn-0.0.9/src/explainable_cnn.egg-info/SOURCES.txt
--rw-r--r--   0 ashutosh1919   (501) staff       (20)        1 2022-04-13 18:39:41.000000 explainable_cnn-0.0.9/src/explainable_cnn.egg-info/dependency_links.txt
--rw-r--r--   0 ashutosh1919   (501) staff       (20)       16 2022-04-13 18:39:41.000000 explainable_cnn-0.0.9/src/explainable_cnn.egg-info/top_level.txt
+drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2023-07-07 06:15:08.018237 explainable_cnn-1.0.0/
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)     1075 2022-03-13 20:42:52.000000 explainable_cnn-1.0.0/LICENSE
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)     5142 2023-07-07 06:15:08.018006 explainable_cnn-1.0.0/PKG-INFO
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)     4547 2022-03-27 22:49:23.000000 explainable_cnn-1.0.0/README.md
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)       84 2022-03-24 20:36:15.000000 explainable_cnn-1.0.0/pyproject.toml
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)       38 2023-07-07 06:15:08.018289 explainable_cnn-1.0.0/setup.cfg
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)      952 2023-07-07 06:14:41.000000 explainable_cnn-1.0.0/setup.py
+drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2023-07-07 06:15:07.969316 explainable_cnn-1.0.0/src/
+drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2023-07-07 06:15:07.972973 explainable_cnn-1.0.0/src/explainable_cnn/
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)       41 2022-03-24 19:46:24.000000 explainable_cnn-1.0.0/src/explainable_cnn/__init__.py
+drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2023-07-07 06:15:08.003918 explainable_cnn-1.0.0/src/explainable_cnn/explainers/
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)      161 2022-03-24 19:11:39.000000 explainable_cnn-1.0.0/src/explainable_cnn/explainers/__init__.py
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)     3847 2022-03-24 19:18:34.000000 explainable_cnn-1.0.0/src/explainable_cnn/explainers/base_explainer.py
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)    12366 2022-04-13 18:34:33.000000 explainable_cnn-1.0.0/src/explainable_cnn/explainers/cnn_explainer.py
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)     6879 2023-07-07 06:07:29.000000 explainable_cnn-1.0.0/src/explainable_cnn/explainers/grad_cam.py
+drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2023-07-07 06:15:08.013322 explainable_cnn-1.0.0/src/explainable_cnn/validators/
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)      111 2022-03-24 18:59:36.000000 explainable_cnn-1.0.0/src/explainable_cnn/validators/__init__.py
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)     1004 2022-03-24 19:00:16.000000 explainable_cnn-1.0.0/src/explainable_cnn/validators/base_validator.py
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)     1961 2022-03-24 19:11:14.000000 explainable_cnn-1.0.0/src/explainable_cnn/validators/cnn_validator.py
+drwxr-xr-x   0 ashutosh1919   (501) staff       (20)        0 2023-07-07 06:15:07.978889 explainable_cnn-1.0.0/src/explainable_cnn.egg-info/
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)     5142 2023-07-07 06:15:07.000000 explainable_cnn-1.0.0/src/explainable_cnn.egg-info/PKG-INFO
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)      568 2023-07-07 06:15:07.000000 explainable_cnn-1.0.0/src/explainable_cnn.egg-info/SOURCES.txt
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)        1 2023-07-07 06:15:07.000000 explainable_cnn-1.0.0/src/explainable_cnn.egg-info/dependency_links.txt
+-rw-r--r--   0 ashutosh1919   (501) staff       (20)       16 2023-07-07 06:15:07.000000 explainable_cnn-1.0.0/src/explainable_cnn.egg-info/top_level.txt
```

### Comparing `explainable_cnn-0.0.9/LICENSE` & `explainable_cnn-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `explainable_cnn-0.0.9/PKG-INFO` & `explainable_cnn-1.0.0/src/explainable_cnn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
-Name: explainable_cnn
-Version: 0.0.9
+Name: explainable-cnn
+Version: 1.0.0
 Summary: 📦 Flexible visualization package for generatinglayer-wise explanations for CNNs.
 Home-page: https://github.com/ashutosh1919/explainable-cnn
 Author: Ashutosh Hathidara
 Author-email: ashutoshhathidara98@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ashutosh1919/explainable-cnn/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -86,9 +84,7 @@
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
 ## References
 
 - [Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization](https://arxiv.org/pdf/1610.02391.pdf)
 - [Grad CAM demonstrations in PyTorch](https://github.com/kazuto1011/grad-cam-pytorch)
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: explainable_cnn Version: 0.0.9 Summary: ð¦
+Metadata-Version: 2.1 Name: explainable-cnn Version: 1.0.0 Summary: ð¦
 Flexible visualization package for generatinglayer-wise explanations for CNNs.
 Home-page: https://github.com/ashutosh1919/explainable-cnn Author: Ashutosh
-Hathidara Author-email: ashutoshhathidara98@gmail.com License: UNKNOWN Project-
-URL: Bug Tracker, https://github.com/ashutosh1919/explainable-cnn/issues
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE # Explainable CNNs [![Torch Version](https://
-img.shields.io/badge/torch>=1.10.0-61DAFB.svg?style=flat-square)](#torch) [!
-[Torchvision Version](https://img.shields.io/badge/torchvision>=0.2.2-
-yellow.svg?style=flat-square)](#torchvision) [![Python Version](https://
-img.shields.io/badge/python->=3.6-blue.svg?style=flat-square)](#python) [![test
-workflow](https://github.com/ashutosh1919/explainable-cnn/blob/main/.github/
-workflows/test_workflow.yml/badge.svg)](#test_workflow) [![Price](https://
-img.shields.io/badge/price-free-ff69b4.svg?style=flat-square)](#price) [!
-[Maintained](https://img.shields.io/badge/maintained-yes-green.svg?style=flat-
-square)](#maintained) **ð¦ Flexible visualization package for generating
-layer-wise explanations for CNNs.** It is a common notion that a Deep Learning
-model is considered as a black box. Working towards this problem, this project
-provides flexible and easy to use `pip` package `explainable-cnn` that will
-help you to create visualization for any `torch` based CNN model. Note that it
-uses one of the data centric approach. This project focusses on making the
-internal working of the Neural layers more transparent. In order to do so,
-`explainable-cnn` is a plug & play component that visualizes the layers based
-on on their gradients and builds different representations including Saliency
-Map, Guided BackPropagation, Grad CAM and Guided Grad CAM. ## Architechture
+Hathidara Author-email: ashutoshhathidara98@gmail.com Project-URL: Bug Tracker,
+https://github.com/ashutosh1919/explainable-cnn/issues Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE # Explainable
+CNNs [![Torch Version](https://img.shields.io/badge/torch>=1.10.0-
+61DAFB.svg?style=flat-square)](#torch) [![Torchvision Version](https://
+img.shields.io/badge/torchvision>=0.2.2-yellow.svg?style=flat-square)]
+(#torchvision) [![Python Version](https://img.shields.io/badge/python->=3.6-
+blue.svg?style=flat-square)](#python) [![test workflow](https://github.com/
+ashutosh1919/explainable-cnn/blob/main/.github/workflows/test_workflow.yml/
+badge.svg)](#test_workflow) [![Price](https://img.shields.io/badge/price-free-
+ff69b4.svg?style=flat-square)](#price) [![Maintained](https://img.shields.io/
+badge/maintained-yes-green.svg?style=flat-square)](#maintained) **ð¦ Flexible
+visualization package for generating layer-wise explanations for CNNs.** It is
+a common notion that a Deep Learning model is considered as a black box.
+Working towards this problem, this project provides flexible and easy to use
+`pip` package `explainable-cnn` that will help you to create visualization for
+any `torch` based CNN model. Note that it uses one of the data centric
+approach. This project focusses on making the internal working of the Neural
+layers more transparent. In order to do so, `explainable-cnn` is a plug & play
+component that visualizes the layers based on on their gradients and builds
+different representations including Saliency Map, Guided BackPropagation, Grad
+CAM and Guided Grad CAM. ## Architechture
        [https://github.com/ashutosh1919/explainable-cnn/blob/main/data/
                                architecture.png]
 :star: Star us on GitHub â it helps! ## Usage Install the package ```bash pip
 install explainable-cnn ``` To create visualizations, create an instance of
 `CNNExplainer`. ```python from explainable_cnn import CNNExplainer x_cnn =
 CNNExplainer(...) ``` The following method calls returns `numpy` arrays
 corresponding to image for different types of visualizations. ```python
```

### Comparing `explainable_cnn-0.0.9/README.md` & `explainable_cnn-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `explainable_cnn-0.0.9/setup.py` & `explainable_cnn-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="explainable_cnn",
-    version="0.0.9",
+    version="1.0.0",
     author="Ashutosh Hathidara",
     author_email="ashutoshhathidara98@gmail.com",
     description="📦 Flexible visualization package for generating" +
     "layer-wise explanations for CNNs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashutosh1919/explainable-cnn",
```

### Comparing `explainable_cnn-0.0.9/src/explainable_cnn/explainers/base_explainer.py` & `explainable_cnn-1.0.0/src/explainable_cnn/explainers/base_explainer.py`

 * *Files identical despite different names*

### Comparing `explainable_cnn-0.0.9/src/explainable_cnn/explainers/cnn_explainer.py` & `explainable_cnn-1.0.0/src/explainable_cnn/explainers/cnn_explainer.py`

 * *Files identical despite different names*

### Comparing `explainable_cnn-0.0.9/src/explainable_cnn/explainers/grad_cam.py` & `explainable_cnn-1.0.0/src/explainable_cnn/explainers/grad_cam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import Sequence
+from collections.abc import Sequence
 
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.nn import functional as F
 from tqdm import tqdm
```

### Comparing `explainable_cnn-0.0.9/src/explainable_cnn/validators/base_validator.py` & `explainable_cnn-1.0.0/src/explainable_cnn/validators/base_validator.py`

 * *Files identical despite different names*

### Comparing `explainable_cnn-0.0.9/src/explainable_cnn/validators/cnn_validator.py` & `explainable_cnn-1.0.0/src/explainable_cnn/validators/cnn_validator.py`

 * *Files identical despite different names*

### Comparing `explainable_cnn-0.0.9/src/explainable_cnn.egg-info/PKG-INFO` & `explainable_cnn-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
-Name: explainable-cnn
-Version: 0.0.9
+Name: explainable_cnn
+Version: 1.0.0
 Summary: 📦 Flexible visualization package for generatinglayer-wise explanations for CNNs.
 Home-page: https://github.com/ashutosh1919/explainable-cnn
 Author: Ashutosh Hathidara
 Author-email: ashutoshhathidara98@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ashutosh1919/explainable-cnn/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -86,9 +84,7 @@
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
 ## References
 
 - [Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization](https://arxiv.org/pdf/1610.02391.pdf)
 - [Grad CAM demonstrations in PyTorch](https://github.com/kazuto1011/grad-cam-pytorch)
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: explainable-cnn Version: 0.0.9 Summary: ð¦
+Metadata-Version: 2.1 Name: explainable_cnn Version: 1.0.0 Summary: ð¦
 Flexible visualization package for generatinglayer-wise explanations for CNNs.
 Home-page: https://github.com/ashutosh1919/explainable-cnn Author: Ashutosh
-Hathidara Author-email: ashutoshhathidara98@gmail.com License: UNKNOWN Project-
-URL: Bug Tracker, https://github.com/ashutosh1919/explainable-cnn/issues
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE # Explainable CNNs [![Torch Version](https://
-img.shields.io/badge/torch>=1.10.0-61DAFB.svg?style=flat-square)](#torch) [!
-[Torchvision Version](https://img.shields.io/badge/torchvision>=0.2.2-
-yellow.svg?style=flat-square)](#torchvision) [![Python Version](https://
-img.shields.io/badge/python->=3.6-blue.svg?style=flat-square)](#python) [![test
-workflow](https://github.com/ashutosh1919/explainable-cnn/blob/main/.github/
-workflows/test_workflow.yml/badge.svg)](#test_workflow) [![Price](https://
-img.shields.io/badge/price-free-ff69b4.svg?style=flat-square)](#price) [!
-[Maintained](https://img.shields.io/badge/maintained-yes-green.svg?style=flat-
-square)](#maintained) **ð¦ Flexible visualization package for generating
-layer-wise explanations for CNNs.** It is a common notion that a Deep Learning
-model is considered as a black box. Working towards this problem, this project
-provides flexible and easy to use `pip` package `explainable-cnn` that will
-help you to create visualization for any `torch` based CNN model. Note that it
-uses one of the data centric approach. This project focusses on making the
-internal working of the Neural layers more transparent. In order to do so,
-`explainable-cnn` is a plug & play component that visualizes the layers based
-on on their gradients and builds different representations including Saliency
-Map, Guided BackPropagation, Grad CAM and Guided Grad CAM. ## Architechture
+Hathidara Author-email: ashutoshhathidara98@gmail.com Project-URL: Bug Tracker,
+https://github.com/ashutosh1919/explainable-cnn/issues Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE # Explainable
+CNNs [![Torch Version](https://img.shields.io/badge/torch>=1.10.0-
+61DAFB.svg?style=flat-square)](#torch) [![Torchvision Version](https://
+img.shields.io/badge/torchvision>=0.2.2-yellow.svg?style=flat-square)]
+(#torchvision) [![Python Version](https://img.shields.io/badge/python->=3.6-
+blue.svg?style=flat-square)](#python) [![test workflow](https://github.com/
+ashutosh1919/explainable-cnn/blob/main/.github/workflows/test_workflow.yml/
+badge.svg)](#test_workflow) [![Price](https://img.shields.io/badge/price-free-
+ff69b4.svg?style=flat-square)](#price) [![Maintained](https://img.shields.io/
+badge/maintained-yes-green.svg?style=flat-square)](#maintained) **ð¦ Flexible
+visualization package for generating layer-wise explanations for CNNs.** It is
+a common notion that a Deep Learning model is considered as a black box.
+Working towards this problem, this project provides flexible and easy to use
+`pip` package `explainable-cnn` that will help you to create visualization for
+any `torch` based CNN model. Note that it uses one of the data centric
+approach. This project focusses on making the internal working of the Neural
+layers more transparent. In order to do so, `explainable-cnn` is a plug & play
+component that visualizes the layers based on on their gradients and builds
+different representations including Saliency Map, Guided BackPropagation, Grad
+CAM and Guided Grad CAM. ## Architechture
        [https://github.com/ashutosh1919/explainable-cnn/blob/main/data/
                                architecture.png]
 :star: Star us on GitHub â it helps! ## Usage Install the package ```bash pip
 install explainable-cnn ``` To create visualizations, create an instance of
 `CNNExplainer`. ```python from explainable_cnn import CNNExplainer x_cnn =
 CNNExplainer(...) ``` The following method calls returns `numpy` arrays
 corresponding to image for different types of visualizations. ```python
```

### Comparing `explainable_cnn-0.0.9/src/explainable_cnn.egg-info/SOURCES.txt` & `explainable_cnn-1.0.0/src/explainable_cnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*


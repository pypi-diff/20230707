# Comparing `tmp/kalman-labs-1.0.31.tar.gz` & `tmp/kalman-labs-1.0.312.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalman-labs-1.0.31.tar", last modified: Fri Jul  7 12:29:26 2023, max compression
+gzip compressed data, was "kalman-labs-1.0.312.tar", last modified: Fri Jul  7 12:36:30 2023, max compression
```

## Comparing `kalman-labs-1.0.31.tar` & `kalman-labs-1.0.312.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:29:26.911816 kalman-labs-1.0.31/
--rw-r--r--   0 serverport   (501) staff       (20)     1067 2023-04-17 18:12:27.000000 kalman-labs-1.0.31/LICENSE
--rw-r--r--   0 serverport   (501) staff       (20)      159 2023-07-07 12:29:26.911696 kalman-labs-1.0.31/PKG-INFO
--rw-r--r--   0 serverport   (501) staff       (20)       48 2023-04-17 18:12:27.000000 kalman-labs-1.0.31/README.md
--rw-r--r--   0 serverport   (501) staff       (20)       38 2023-07-07 12:29:26.911856 kalman-labs-1.0.31/setup.cfg
--rw-r--r--   0 serverport   (501) staff       (20)      514 2023-07-07 12:29:19.000000 kalman-labs-1.0.31/setup.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:29:26.909086 kalman-labs-1.0.31/signal_processing_packages/
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:29:26.909238 kalman-labs-1.0.31/signal_processing_packages/src/
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:29:26.910515 kalman-labs-1.0.31/signal_processing_packages/src/kalman/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:42:55.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman/__init__.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:29:26.910848 kalman-labs-1.0.31/signal_processing_packages/src/kalman/audio_features/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-04-17 19:01:55.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman/audio_features/__init__.py
--rw-r--r--   0 serverport   (501) staff       (20)     3598 2023-07-03 17:29:46.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman/audio_features/extract_features.py
--rw-r--r--   0 serverport   (501) staff       (20)    15473 2023-07-05 17:50:33.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman/deep_learning_training.py
--rw-r--r--   0 serverport   (501) staff       (20)     7671 2023-07-07 12:29:03.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman/machine_learning_training.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:29:26.911497 kalman-labs-1.0.31/signal_processing_packages/src/kalman_labs.egg-info/
--rw-r--r--   0 serverport   (501) staff       (20)      159 2023-07-07 12:29:26.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
--rw-r--r--   0 serverport   (501) staff       (20)      674 2023-07-07 12:29:26.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
--rw-r--r--   0 serverport   (501) staff       (20)        1 2023-07-07 12:29:26.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
--rw-r--r--   0 serverport   (501) staff       (20)       76 2023-07-07 12:29:26.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman_labs.egg-info/requires.txt
--rw-r--r--   0 serverport   (501) staff       (20)        7 2023-07-07 12:29:26.000000 kalman-labs-1.0.31/signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:36:30.409822 kalman-labs-1.0.312/
+-rw-r--r--   0 serverport   (501) staff       (20)     1067 2023-04-17 18:12:27.000000 kalman-labs-1.0.312/LICENSE
+-rw-r--r--   0 serverport   (501) staff       (20)      160 2023-07-07 12:36:30.409677 kalman-labs-1.0.312/PKG-INFO
+-rw-r--r--   0 serverport   (501) staff       (20)       48 2023-04-17 18:12:27.000000 kalman-labs-1.0.312/README.md
+-rw-r--r--   0 serverport   (501) staff       (20)       38 2023-07-07 12:36:30.409866 kalman-labs-1.0.312/setup.cfg
+-rw-r--r--   0 serverport   (501) staff       (20)      515 2023-07-07 12:36:25.000000 kalman-labs-1.0.312/setup.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:36:30.407347 kalman-labs-1.0.312/signal_processing_packages/
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:36:30.407504 kalman-labs-1.0.312/signal_processing_packages/src/
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:36:30.408522 kalman-labs-1.0.312/signal_processing_packages/src/kalman/
+-rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:42:55.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman/__init__.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:36:30.408838 kalman-labs-1.0.312/signal_processing_packages/src/kalman/audio_features/
+-rw-r--r--   0 serverport   (501) staff       (20)        0 2023-04-17 19:01:55.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman/audio_features/__init__.py
+-rw-r--r--   0 serverport   (501) staff       (20)     3598 2023-07-03 17:29:46.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman/audio_features/extract_features.py
+-rw-r--r--   0 serverport   (501) staff       (20)    15474 2023-07-07 12:36:16.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman/deep_learning_training.py
+-rw-r--r--   0 serverport   (501) staff       (20)     7634 2023-07-07 12:36:08.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman/machine_learning_training.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 12:36:30.409508 kalman-labs-1.0.312/signal_processing_packages/src/kalman_labs.egg-info/
+-rw-r--r--   0 serverport   (501) staff       (20)      160 2023-07-07 12:36:30.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
+-rw-r--r--   0 serverport   (501) staff       (20)      674 2023-07-07 12:36:30.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
+-rw-r--r--   0 serverport   (501) staff       (20)        1 2023-07-07 12:36:30.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
+-rw-r--r--   0 serverport   (501) staff       (20)       76 2023-07-07 12:36:30.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman_labs.egg-info/requires.txt
+-rw-r--r--   0 serverport   (501) staff       (20)        7 2023-07-07 12:36:30.000000 kalman-labs-1.0.312/signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
```

### Comparing `kalman-labs-1.0.31/LICENSE` & `kalman-labs-1.0.312/LICENSE`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.31/setup.py` & `kalman-labs-1.0.312/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kalman-labs',
-    version='1.0.31',
+    version='1.0.312',
     author='Aditya',
     author_email='aditya@kalman.in',
     description='The Global Kalman Package',
     packages=find_packages('signal_processing_packages/src'),
     package_dir={'': 'signal_processing_packages/src'},
     install_requires=[
         'numpy',
```

### Comparing `kalman-labs-1.0.31/signal_processing_packages/src/kalman/audio_features/extract_features.py` & `kalman-labs-1.0.312/signal_processing_packages/src/kalman/audio_features/extract_features.py`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.31/signal_processing_packages/src/kalman/deep_learning_training.py` & `kalman-labs-1.0.312/signal_processing_packages/src/kalman/deep_learning_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from audio_features.extract_features import generate_feature_file
+from .audio_features.extract_features import generate_feature_file
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import precision_score, recall_score
 from imblearn.over_sampling import SMOTE, ADASYN
 from imblearn.under_sampling import NearMiss
 
 import tensorflow as tf
 import keras
```

### Comparing `kalman-labs-1.0.31/signal_processing_packages/src/kalman/machine_learning_training.py` & `kalman-labs-1.0.312/signal_processing_packages/src/kalman/machine_learning_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from signal_processing_packages.src.kalman.audio_features.extract_features import generate_feature_file
+from .audio_features.extract_features import generate_feature_file
 from sklearn.model_selection import train_test_split, cross_val_score
 from sklearn.metrics import classification_report
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier, AdaBoostClassifier
 from sklearn.neural_network import MLPClassifier
```

### Comparing `kalman-labs-1.0.31/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt` & `kalman-labs-1.0.312/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


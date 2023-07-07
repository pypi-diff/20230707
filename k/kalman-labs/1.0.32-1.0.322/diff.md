# Comparing `tmp/kalman-labs-1.0.32.tar.gz` & `tmp/kalman-labs-1.0.322.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalman-labs-1.0.32.tar", last modified: Fri Jul  7 15:17:43 2023, max compression
+gzip compressed data, was "kalman-labs-1.0.322.tar", last modified: Fri Jul  7 17:06:38 2023, max compression
```

## Comparing `kalman-labs-1.0.32.tar` & `kalman-labs-1.0.322.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 15:17:43.301294 kalman-labs-1.0.32/
--rw-r--r--   0 serverport   (501) staff       (20)     1067 2023-04-17 18:12:27.000000 kalman-labs-1.0.32/LICENSE
--rw-r--r--   0 serverport   (501) staff       (20)     9447 2023-07-07 15:17:43.301057 kalman-labs-1.0.32/PKG-INFO
--rw-r--r--   0 serverport   (501) staff       (20)     9247 2023-07-07 15:15:03.000000 kalman-labs-1.0.32/README.md
--rw-r--r--   0 serverport   (501) staff       (20)       38 2023-07-07 15:17:43.301345 kalman-labs-1.0.32/setup.cfg
--rw-r--r--   0 serverport   (501) staff       (20)      691 2023-07-07 15:17:34.000000 kalman-labs-1.0.32/setup.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 15:17:43.298871 kalman-labs-1.0.32/signal_processing_packages/
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 15:17:43.299023 kalman-labs-1.0.32/signal_processing_packages/src/
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 15:17:43.299883 kalman-labs-1.0.32/signal_processing_packages/src/kalman/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:42:55.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman/__init__.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 15:17:43.300209 kalman-labs-1.0.32/signal_processing_packages/src/kalman/audio_features/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-04-17 19:01:55.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman/audio_features/__init__.py
--rw-r--r--   0 serverport   (501) staff       (20)     3598 2023-07-03 17:29:46.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman/audio_features/extract_features.py
--rw-r--r--   0 serverport   (501) staff       (20)    15474 2023-07-07 12:36:16.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman/deep_learning_training.py
--rw-r--r--   0 serverport   (501) staff       (20)     7634 2023-07-07 12:36:08.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman/machine_learning_training.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 15:17:43.300850 kalman-labs-1.0.32/signal_processing_packages/src/kalman_labs.egg-info/
--rw-r--r--   0 serverport   (501) staff       (20)     9447 2023-07-07 15:17:43.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
--rw-r--r--   0 serverport   (501) staff       (20)      674 2023-07-07 15:17:43.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
--rw-r--r--   0 serverport   (501) staff       (20)        1 2023-07-07 15:17:43.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
--rw-r--r--   0 serverport   (501) staff       (20)       76 2023-07-07 15:17:43.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman_labs.egg-info/requires.txt
--rw-r--r--   0 serverport   (501) staff       (20)        7 2023-07-07 15:17:43.000000 kalman-labs-1.0.32/signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 17:06:38.910915 kalman-labs-1.0.322/
+-rw-r--r--   0 serverport   (501) staff       (20)     1067 2023-04-17 18:12:27.000000 kalman-labs-1.0.322/LICENSE
+-rw-r--r--   0 serverport   (501) staff       (20)     9229 2023-07-07 17:06:38.910551 kalman-labs-1.0.322/PKG-INFO
+-rw-r--r--   0 serverport   (501) staff       (20)     9028 2023-07-07 17:04:34.000000 kalman-labs-1.0.322/README.md
+-rw-r--r--   0 serverport   (501) staff       (20)       38 2023-07-07 17:06:38.910952 kalman-labs-1.0.322/setup.cfg
+-rw-r--r--   0 serverport   (501) staff       (20)      692 2023-07-07 17:04:57.000000 kalman-labs-1.0.322/setup.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 17:06:38.907112 kalman-labs-1.0.322/signal_processing_packages/
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 17:06:38.907278 kalman-labs-1.0.322/signal_processing_packages/src/
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 17:06:38.909299 kalman-labs-1.0.322/signal_processing_packages/src/kalman/
+-rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:42:55.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman/__init__.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 17:06:38.909743 kalman-labs-1.0.322/signal_processing_packages/src/kalman/audio_features/
+-rw-r--r--   0 serverport   (501) staff       (20)        0 2023-04-17 19:01:55.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman/audio_features/__init__.py
+-rw-r--r--   0 serverport   (501) staff       (20)     3598 2023-07-03 17:29:46.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman/audio_features/extract_features.py
+-rw-r--r--   0 serverport   (501) staff       (20)    15474 2023-07-07 12:36:16.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman/deep_learning_training.py
+-rw-r--r--   0 serverport   (501) staff       (20)     7634 2023-07-07 12:36:08.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman/machine_learning_training.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-07 17:06:38.910365 kalman-labs-1.0.322/signal_processing_packages/src/kalman_labs.egg-info/
+-rw-r--r--   0 serverport   (501) staff       (20)     9229 2023-07-07 17:06:38.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
+-rw-r--r--   0 serverport   (501) staff       (20)      674 2023-07-07 17:06:38.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
+-rw-r--r--   0 serverport   (501) staff       (20)        1 2023-07-07 17:06:38.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
+-rw-r--r--   0 serverport   (501) staff       (20)       76 2023-07-07 17:06:38.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman_labs.egg-info/requires.txt
+-rw-r--r--   0 serverport   (501) staff       (20)        7 2023-07-07 17:06:38.000000 kalman-labs-1.0.322/signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
```

### Comparing `kalman-labs-1.0.32/LICENSE` & `kalman-labs-1.0.322/LICENSE`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.32/PKG-INFO` & `kalman-labs-1.0.322/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: kalman-labs
-Version: 1.0.32
-Summary: The Global Kalman Package
-Author: Aditya
-Author-email: aditya@kalman.in
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # kalman-labs
 
 The `kalman-labs` package provides a set of tools and functionalities for audio signal processing and machine learning tasks. It includes features for feature extraction, machine learning model training, and deep learning model training.
 
 ## Features
 
 ### 1. Audio Feature Extraction
@@ -81,17 +72,16 @@
 
 # The resulting model_details dictionary contains information about the trained model
 # The classification_report contains precision, recall, f1-score, and support for each class
 ```
 
 **Parameter Descriptions:**
 
-- `ml_model` (str): The machine learning model to train. Supported options are: "random_forest", "svm", "knn", "logistic_regression".
+- `ml_model` (str): The machine learning model to train. Supported options are: "random_forest", "svm", "knn", "logistic_regression","gradient_boosting", "adaboost", "xgboost".
 - `folder_path` (str): Path to the folder containing audio files. This parameter should be used when the audio data is stored in separate files.
-- `audio_feature_extraction` (str): The audio feature extraction technique to use. Supported options are: "mfcc", "chroma", "mel".
 - `x_train` (array-like): Training data features. This should be a 2D array-like object.
 - `y_train` (array-like): Training data labels. This should be a 1D array-like object.
 - `x_test` (array-like, optional): Testing data features. This should be a 2D array-like object. (default: None)
 - `y_test` (array-like, optional): Testing data labels. This should be a 1D array-like object. (default: None)
 - `test_size` (float, optional): The proportion of the testing data when `x_test` and `y_test` are not provided. This parameter is used for splitting the training data into training and testing sets. (default: 0.2)
 - `undersampling` (bool, optional): Whether to perform undersampling to balance the class distribution. (default: False)
 - `oversampling` (str, optional): The oversampling technique to use. Supported options are: "smote", "adasyn". (default: None)
@@ -131,15 +121,14 @@
 # The resulting results dictionary contains evaluation metrics such as accuracy, precision, recall, and AUC
 ```
 
 **Parameter Descriptions:**
 
 - `dl_model` (str): The deep learning model to train. Supported options are: "DNN", "DNN-CNN", "DNN-BiLSTM", "DNN-convLSTM".
 - `folder_path` (str): Path to the folder containing audio files. This parameter should be used when the audio data is stored in separate files.
-- `audio_feature_extraction` (str): The audio feature extraction technique to use. Supported options are: "mfcc", "chroma", "mel".
 - `x_train` (array-like): Training data features. This should be a 2D array-like object.
 - `y_train` (array-like): Training data labels. This should be a 1D array-like object.
 - `x_val` (array-like): Validation data features. This should be a 2D array-like object.
 - `y_val` (array-like): Validation data labels. This should be a 1D array-like object.
 - `val_size` (float, optional): The proportion of the validation data when `x_val` and `y_val` are not provided. (default: 0.3)
 - `oversampling` (str, optional): The oversampling technique to use. Supported options are: "smote", "adasyn". (default: None)
 - `undersampling` (bool, optional): Whether to perform undersampling to balance the class distribution. (default: False)
```

### Comparing `kalman-labs-1.0.32/README.md` & `kalman-labs-1.0.322/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: kalman-labs
+Version: 1.0.322
+Summary: The Global Kalman Package
+Author: Aditya
+Author-email: aditya@kalman.in
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # kalman-labs
 
 The `kalman-labs` package provides a set of tools and functionalities for audio signal processing and machine learning tasks. It includes features for feature extraction, machine learning model training, and deep learning model training.
 
 ## Features
 
 ### 1. Audio Feature Extraction
@@ -72,17 +81,16 @@
 
 # The resulting model_details dictionary contains information about the trained model
 # The classification_report contains precision, recall, f1-score, and support for each class
 ```
 
 **Parameter Descriptions:**
 
-- `ml_model` (str): The machine learning model to train. Supported options are: "random_forest", "svm", "knn", "logistic_regression".
+- `ml_model` (str): The machine learning model to train. Supported options are: "random_forest", "svm", "knn", "logistic_regression","gradient_boosting", "adaboost", "xgboost".
 - `folder_path` (str): Path to the folder containing audio files. This parameter should be used when the audio data is stored in separate files.
-- `audio_feature_extraction` (str): The audio feature extraction technique to use. Supported options are: "mfcc", "chroma", "mel".
 - `x_train` (array-like): Training data features. This should be a 2D array-like object.
 - `y_train` (array-like): Training data labels. This should be a 1D array-like object.
 - `x_test` (array-like, optional): Testing data features. This should be a 2D array-like object. (default: None)
 - `y_test` (array-like, optional): Testing data labels. This should be a 1D array-like object. (default: None)
 - `test_size` (float, optional): The proportion of the testing data when `x_test` and `y_test` are not provided. This parameter is used for splitting the training data into training and testing sets. (default: 0.2)
 - `undersampling` (bool, optional): Whether to perform undersampling to balance the class distribution. (default: False)
 - `oversampling` (str, optional): The oversampling technique to use. Supported options are: "smote", "adasyn". (default: None)
@@ -122,15 +130,14 @@
 # The resulting results dictionary contains evaluation metrics such as accuracy, precision, recall, and AUC
 ```
 
 **Parameter Descriptions:**
 
 - `dl_model` (str): The deep learning model to train. Supported options are: "DNN", "DNN-CNN", "DNN-BiLSTM", "DNN-convLSTM".
 - `folder_path` (str): Path to the folder containing audio files. This parameter should be used when the audio data is stored in separate files.
-- `audio_feature_extraction` (str): The audio feature extraction technique to use. Supported options are: "mfcc", "chroma", "mel".
 - `x_train` (array-like): Training data features. This should be a 2D array-like object.
 - `y_train` (array-like): Training data labels. This should be a 1D array-like object.
 - `x_val` (array-like): Validation data features. This should be a 2D array-like object.
 - `y_val` (array-like): Validation data labels. This should be a 1D array-like object.
 - `val_size` (float, optional): The proportion of the validation data when `x_val` and `y_val` are not provided. (default: 0.3)
 - `oversampling` (str, optional): The oversampling technique to use. Supported options are: "smote", "adasyn". (default: None)
 - `undersampling` (bool, optional): Whether to perform undersampling to balance the class distribution. (default: False)
```

### Comparing `kalman-labs-1.0.32/setup.py` & `kalman-labs-1.0.322/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='kalman-labs',
-    version='1.0.32',
+    version='1.0.322',
     author='Aditya',
     author_email='aditya@kalman.in',
     description='The Global Kalman Package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages('signal_processing_packages/src'),
     package_dir={'': 'signal_processing_packages/src'},
```

### Comparing `kalman-labs-1.0.32/signal_processing_packages/src/kalman/audio_features/extract_features.py` & `kalman-labs-1.0.322/signal_processing_packages/src/kalman/audio_features/extract_features.py`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.32/signal_processing_packages/src/kalman/deep_learning_training.py` & `kalman-labs-1.0.322/signal_processing_packages/src/kalman/deep_learning_training.py`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.32/signal_processing_packages/src/kalman/machine_learning_training.py` & `kalman-labs-1.0.322/signal_processing_packages/src/kalman/machine_learning_training.py`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.32/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO` & `kalman-labs-1.0.322/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalman-labs
-Version: 1.0.32
+Version: 1.0.322
 Summary: The Global Kalman Package
 Author: Aditya
 Author-email: aditya@kalman.in
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kalman-labs
@@ -81,17 +81,16 @@
 
 # The resulting model_details dictionary contains information about the trained model
 # The classification_report contains precision, recall, f1-score, and support for each class
 ```
 
 **Parameter Descriptions:**
 
-- `ml_model` (str): The machine learning model to train. Supported options are: "random_forest", "svm", "knn", "logistic_regression".
+- `ml_model` (str): The machine learning model to train. Supported options are: "random_forest", "svm", "knn", "logistic_regression","gradient_boosting", "adaboost", "xgboost".
 - `folder_path` (str): Path to the folder containing audio files. This parameter should be used when the audio data is stored in separate files.
-- `audio_feature_extraction` (str): The audio feature extraction technique to use. Supported options are: "mfcc", "chroma", "mel".
 - `x_train` (array-like): Training data features. This should be a 2D array-like object.
 - `y_train` (array-like): Training data labels. This should be a 1D array-like object.
 - `x_test` (array-like, optional): Testing data features. This should be a 2D array-like object. (default: None)
 - `y_test` (array-like, optional): Testing data labels. This should be a 1D array-like object. (default: None)
 - `test_size` (float, optional): The proportion of the testing data when `x_test` and `y_test` are not provided. This parameter is used for splitting the training data into training and testing sets. (default: 0.2)
 - `undersampling` (bool, optional): Whether to perform undersampling to balance the class distribution. (default: False)
 - `oversampling` (str, optional): The oversampling technique to use. Supported options are: "smote", "adasyn". (default: None)
@@ -131,15 +130,14 @@
 # The resulting results dictionary contains evaluation metrics such as accuracy, precision, recall, and AUC
 ```
 
 **Parameter Descriptions:**
 
 - `dl_model` (str): The deep learning model to train. Supported options are: "DNN", "DNN-CNN", "DNN-BiLSTM", "DNN-convLSTM".
 - `folder_path` (str): Path to the folder containing audio files. This parameter should be used when the audio data is stored in separate files.
-- `audio_feature_extraction` (str): The audio feature extraction technique to use. Supported options are: "mfcc", "chroma", "mel".
 - `x_train` (array-like): Training data features. This should be a 2D array-like object.
 - `y_train` (array-like): Training data labels. This should be a 1D array-like object.
 - `x_val` (array-like): Validation data features. This should be a 2D array-like object.
 - `y_val` (array-like): Validation data labels. This should be a 1D array-like object.
 - `val_size` (float, optional): The proportion of the validation data when `x_val` and `y_val` are not provided. (default: 0.3)
 - `oversampling` (str, optional): The oversampling technique to use. Supported options are: "smote", "adasyn". (default: None)
 - `undersampling` (bool, optional): Whether to perform undersampling to balance the class distribution. (default: False)
```

### Comparing `kalman-labs-1.0.32/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt` & `kalman-labs-1.0.322/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


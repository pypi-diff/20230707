# Comparing `tmp/tf_nightly-2.14.0.dev20230706-cp39-cp39-win_amd64.whl.zip` & `tmp/tf_nightly-2.14.0.dev20230707-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2229 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     3408 b- defN 23-Jul-06 09:15 tf_nightly-2.14.0.dev20230706.dist-info/METADATA
--rw-rw-r--  2.0 unx       99 b- defN 23-Jul-06 09:15 tf_nightly-2.14.0.dev20230706.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-06 09:15 tf_nightly-2.14.0.dev20230706.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      361 b- defN 23-Jul-06 09:15 tf_nightly-2.14.0.dev20230706.dist-info/RECORD
-4 files, 3869 bytes uncompressed, 1519 bytes compressed:  60.7%
+Zip file size: 2226 bytes, number of entries: 4
+-rw-rw-r--  2.0 unx     3358 b- defN 23-Jul-07 09:15 tf_nightly-2.14.0.dev20230707.dist-info/METADATA
+-rw-rw-r--  2.0 unx       99 b- defN 23-Jul-07 09:15 tf_nightly-2.14.0.dev20230707.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-07 09:15 tf_nightly-2.14.0.dev20230707.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      361 b- defN 23-Jul-07 09:15 tf_nightly-2.14.0.dev20230707.dist-info/RECORD
+4 files, 3819 bytes uncompressed, 1516 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: tf_nightly-2.14.0.dev20230706.dist-info/METADATA
+Filename: tf_nightly-2.14.0.dev20230707.dist-info/METADATA
 Comment: 
 
-Filename: tf_nightly-2.14.0.dev20230706.dist-info/WHEEL
+Filename: tf_nightly-2.14.0.dev20230707.dist-info/WHEEL
 Comment: 
 
-Filename: tf_nightly-2.14.0.dev20230706.dist-info/top_level.txt
+Filename: tf_nightly-2.14.0.dev20230707.dist-info/top_level.txt
 Comment: 
 
-Filename: tf_nightly-2.14.0.dev20230706.dist-info/RECORD
+Filename: tf_nightly-2.14.0.dev20230707.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tf_nightly-2.14.0.dev20230706.dist-info/METADATA` & `tf_nightly-2.14.0.dev20230707.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-nightly
-Version: 2.14.0.dev20230706
+Version: 2.14.0.dev20230707
 Summary: TensorFlow is an open source machine learning framework for everyone.
 Home-page: https://www.tensorflow.org/
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/tensorflow/tags
 Keywords: tensorflow tensor machine learning
@@ -15,27 +15,26 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: tf-nightly-macos (==2.14.0-dev20230706) ; platform_system == "Darwin" and platform_machine == "arm64"
-Requires-Dist: tf-nightly-cpu-aws (==2.14.0-dev20230706) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
-Requires-Dist: tf-nightly-intel (==2.14.0-dev20230706) ; platform_system == "Windows"
+Requires-Dist: tf-nightly-macos (==2.14.0-dev20230707) ; platform_system == "Darwin" and platform_machine == "arm64"
+Requires-Dist: tf-nightly-cpu-aws (==2.14.0-dev20230707) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
+Requires-Dist: tf-nightly-intel (==2.14.0-dev20230707) ; platform_system == "Windows"
 Provides-Extra: and-cuda
 Requires-Dist: nvidia-cublas-cu11 (==11.11.3.6) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-cupti-cu11 (==11.8.87) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-nvcc-cu11 (==11.8.89) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-runtime-cu11 (==11.8.89) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cudnn-cu11 (==8.7.0.84) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cufft-cu11 (==10.9.0.58) ; extra == 'and-cuda'
```


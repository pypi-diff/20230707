# Comparing `tmp/ezsmdeploy-1.1.4.tar.gz` & `tmp/ezsmdeploy-1.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ezsmdeploy-1.1.4.tar", last modified: Wed Sep  1 03:07:08 2021, max compression
+gzip compressed data, was "dist/ezsmdeploy-1.6.dev0.tar", last modified: Fri Jul  7 19:16:00 2023, max compression
```

## Comparing `ezsmdeploy-1.1.4.tar` & `ezsmdeploy-1.6.dev0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxr-x   0 ec2-user   (500) ec2-user   (500)        0 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)       38 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/setup.cfg
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     1271 2021-09-01 03:03:22.000000 ezsmdeploy-1.1.4/setup.py
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)    15535 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/README.rst
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)       26 2021-08-31 21:51:34.000000 ezsmdeploy-1.1.4/MANIFEST.in
-drwxrwxr-x   0 ec2-user   (500) ec2-user   (500)        0 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/ezsmdeploy/
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)    29884 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/__init__.py
-drwxrwxr-x   0 ec2-user   (500) ec2-user   (500)        0 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     1390 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/build-docker.sh
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     1797 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/model_handler.py
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)      202 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/wsgi.py
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     1924 2021-09-01 03:06:05.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/Dockerfile_flask
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     2429 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/serve
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)      884 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/dockerd-entrypoint.py
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)      432 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/train
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     2090 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/predictor.py
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     2090 2021-09-01 03:05:48.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/Dockerfile
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)      719 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/nginx.conf
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)      576 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/instancetypes.csv
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     1202 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/cost.csv
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)     1409 2021-08-31 21:32:28.000000 ezsmdeploy-1.1.4/ezsmdeploy/data/smlocust.py
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)    18956 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/PKG-INFO
-drwxrwxr-x   0 ec2-user   (500) ec2-user   (500)        0 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/ezsmdeploy.egg-info/
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)      630 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/ezsmdeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)        1 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/ezsmdeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)       11 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/ezsmdeploy.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)    18956 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/ezsmdeploy.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)        1 2021-08-31 21:37:13.000000 ezsmdeploy-1.1.4/ezsmdeploy.egg-info/not-zip-safe
--rw-rw-r--   0 ec2-user   (500) ec2-user   (500)      128 2021-09-01 03:07:08.000000 ezsmdeploy-1.1.4/ezsmdeploy.egg-info/requires.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16024 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    15535 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/README.rst
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    44466 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/Dockerfile
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/Dockerfile_flask
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/build-docker.sh
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/conversation.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/cost.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/dockerd-entrypoint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/instancetypes.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/model_handler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/nginx.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/predictor.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/serve
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/smlocust.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/train
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/data/wsgi.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-07 19:11:22.000000 ezsmdeploy-1.6.dev0/ezsmdeploy/modelscript_sklearn.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16024 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy.egg-info/not-zip-safe
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/ezsmdeploy.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-07 19:15:59.000000 ezsmdeploy-1.6.dev0/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1273 2023-07-07 19:11:59.000000 ezsmdeploy-1.6.dev0/setup.py
```

### Comparing `ezsmdeploy-1.1.4/setup.py` & `ezsmdeploy-1.6.dev0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 extras = {
     'locust': [
         'locustio==0.14.5'
     ]
 }
 
 setup(name='ezsmdeploy',
-      version='1.1.4',
+      version='1.6dev',
       description='SageMaker custom deployments made easy',
       url='https://pypi.python.org/pypi/ezsmdeploy',
       #scripts=['Dockerfile','dockerd-entrypoint.py','model_handler.py','build-docker.sh'],
       author='Shreyas Subramanian',
       author_email='subshrey@amazon.com',
       license='MIT',
       packages=['ezsmdeploy'],
       package_data={'ezsmdeploy': ['data/*']},
       include_package_data=True,
       extras_require = extras,
-      install_requires=["sagemaker==2.16.1","yaspin==0.16.0","shortuuid==1.0.1","sagemaker-studio-image-build==0.5.0", "boto3>=1.14.12"],
+      install_requires=["sagemaker==2.171.0","yaspin==0.16.0","shortuuid==1.0.1","sagemaker-studio-image-build==0.5.0", "boto3>=1.14.12"],
       zip_safe=False,
       classifiers=['Development Status :: 3 - Alpha',
                    "Intended Audience :: Developers",
                    "Natural Language :: English",
                    "License :: OSI Approved :: Apache Software License",
                    "Programming Language :: Python"],
       long_description=read("README.rst")
```

### Comparing `ezsmdeploy-1.1.4/README.rst` & `ezsmdeploy-1.6.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/build-docker.sh` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/build-docker.sh`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/model_handler.py` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/model_handler.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/Dockerfile_flask` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/Dockerfile_flask`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Build an image that can do training and inference in SageMaker
 # This is a Python 3 image that uses the nginx, gunicorn, flask stack
 # for serving inferences in a stable way.
 
-FROM ubuntu:18.04
+FROM ubuntu:22.04
 
 RUN apt -y update && apt -y upgrade && \
     apt-get -y install curl && \
-    curl -sL https://deb.nodesource.com/setup_12.x | bash - && \
+    curl -sL https://deb.nodesource.com/setup_18.x | bash - && \
     apt install nodejs -y && \
     npm install -g @bazel/bazelisk
 
 RUN apt-get update && \
     apt-get -y install --no-install-recommends \
     build-essential \
     ca-certificates \
     openjdk-8-jdk-headless \
-    python3-dev \
+    python3 \
     python3-pip \
     python3-setuptools \
     nginx \
     ca-certificates \
     curl \
     wget \
     vim \
     gcc \
     libpq-dev \
     python3-wheel \
     && rm -rf /var/lib/apt/lists/* 
 
 RUN pip3 install --upgrade pip
-
+RUN python3 -V
 # Here we get all python packages.
 RUN pip3 install wheel
 
 RUN pip3 --no-cache-dir install setuptools \
                                 numpy \
                                 pandas \
                                 flask gevent gunicorn \
```

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/serve` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/serve`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/dockerd-entrypoint.py` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/dockerd-entrypoint.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/predictor.py` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/predictor.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/Dockerfile` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-FROM ubuntu:18.04
+FROM ubuntu:22.04
 
 # Set a docker label to advertise multi-model support on the container
 LABEL com.amazonaws.sagemaker.capabilities.multi-models=true
 # Set a docker label to enable container to use SAGEMAKER_BIND_TO_PORT environment variable if present
 LABEL com.amazonaws.sagemaker.capabilities.accept-bind-to-port=true
 
 RUN apt -y update && apt -y upgrade && \
     apt-get -y install curl && \
-    curl -sL https://deb.nodesource.com/setup_12.x | bash - && \
+    curl -sL https://deb.nodesource.com/setup_18.x | bash - && \
     apt install nodejs -y && \
     npm install -g @bazel/bazelisk
     
 # Install necessary dependencies for MMS and SageMaker Inference Toolkit
 
 RUN apt-get update && \
     apt-get -y install --no-install-recommends \
     build-essential \
     ca-certificates \
     openjdk-8-jdk-headless \
-    python3-dev \
+    python3 \
     python3-pip \
     python3-setuptools \
     nginx \
     ca-certificates \
     curl \
     wget \
     vim \
     && rm -rf /var/lib/apt/lists/* 
 
-
+RUN python3 -V
 RUN update-alternatives --install /usr/bin/python python /usr/bin/python3 1
 RUN update-alternatives --install /usr/local/bin/pip pip /usr/local/bin/pip3 1
 
 RUN pip3 install --upgrade pip
 
 # Install MXNet, MMS, and SageMaker Inference Toolkit to set up MMS
 RUN pip3 --no-cache-dir install mxnet \
```

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/nginx.conf` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/nginx.conf`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/instancetypes.csv` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/instancetypes.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/cost.csv` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/cost.csv`

 * *Files 6% similar despite different names*

```diff
@@ -54,8 +54,16 @@
 ml.p3.8xlarge,18.508
 ml.p3.16xlarge,37.016
 ml.g4dn.xlarge,0.821
 ml.g4dn.2xlarge,1.174
 ml.g4dn.4xlarge,1.879
 ml.g4dn.8xlarge,3.397
 ml.g4dn.12xlarge,6.107
-ml.g4dn.16xlarge,6.793
+ml.g4dn.16xlarge,6.793
+ml.g5.xlarge,1.408
+ml.g5.2xlarge,1.515
+ml.g5.4xlarge,2.03
+ml.g5.8xlarge,3.06
+ml.g5.12xlarge,7.09
+ml.g5.16xlarge,5.12
+ml.g5.24xlarge,10.18
+ml.g5.48xlarge,20.36
```

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy/data/smlocust.py` & `ezsmdeploy-1.6.dev0/ezsmdeploy/data/smlocust.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.1.4/PKG-INFO` & `ezsmdeploy-1.6.dev0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,379 +1,378 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.1.4
+Version: 1.6.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
-Description: ====================================================
-        Ezsmdeploy - SageMaker custom deployments made easy
-        ====================================================
-        
-        .. image:: https://img.shields.io/pypi/v/ezsmdeploy.svg
-           :target: https://pypi.python.org/pypi/ezsmdeploy
-           :alt: Latest Version
-        
-        .. image:: https://img.shields.io/badge/code_style-black-000000.svg
-           :target: https://github.com/python/black
-           :alt: Code style: black
-        
-        .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
-           :target: https://opensource.org/licenses/MIT
-           :alt: License: MIT
-        
-        .. image:: https://img.shields.io/badge/Made%20With-Love-orange.svg
-           :target: https://pypi.python.org/pypi/ezsmdeploy
-           :alt: Made With Love
-           
-        
-        **Ezsmdeploy** python SDK helps you easily deploy Machine learning models and provides a rich set of features such as passing one or more model files (yes, through multi-model deployments), automatically choosing an instance based on model size or based on a budget, and load testing endpoints using an intuitive API. **Ezsmdeploy** uses the SageMaker Python SDK, which is an open source library for training and deploying machine learning models on Amazon SageMaker. This SDK however focuses on simplifying deployment from existing models, and as such, this is for you if:
-        
-        1. you have a serialized model (a pickle / joblib/ json/ TF saved model/ Pytorch .pth/ etc) file and you want to deploy and test your model as an API endpoint
-        2. you have a model or multiple models stored as local files, in local folders, or in S3 as tar files (model.tar.gz)
-        3. you don't want to create a custom docker container for deployment and/or don't want to deal with docker
-        4. you want to make use of advanced features such as autoscaling, elastic inference, multi-model endpoints, model inference data capture, and locust.io based load testing, without any of the heavy lifting
-        5. you want to still have control of how do perform inference by passing in a python script
-        
-        Note for some Sagemaker estimators, deployment from pretrained models is easy; consider the Tensorflow savedmodel format. You can very easily tar your save_model.pb and variables file and use the sagemaker.tensorflow.serving.Model to register and deploy your model. Nevertheless, if your TF model is saved as checkpoints, HDF5 file, or as Tflite file, or if you have deployments needs accross multiple types of serialized model files, this may help standardize your deployment pipeline and avoid the need for building new containers for each model.
-        
-        V 1.x release notes
-        -------------------
-        1. Updated to use >v2.x of SageMaker SDK
-        2. Fixed failing docker builds
-        3. Tested with test notebook
-        
-        
-        Table of Contents
-        -----------------
-        1. `Installing Ezsmdeploy Python SDK <#installing-the-ezsmdeploy-python-sdk>`__
-        2. `Key Features <#key-features>`__
-        3. `Other Features <#other-features>`__
-        4. `Model script requirements <#model-script-requirements>`__
-        5. `Sample notebooks <#sample-notebooks>`__
-        6. `Known gotchas <#known-gotchas>`__
-        
-        Installing the Ezsmdeploy Python SDK
-        ------------------------------------
-        
-        
-        The Ezsmdeploy Python SDK is built to PyPI and has the following dependencies sagemaker>=1.55.3, cyaspin==0.16.0,  shortuuid==1.0.1 and locustio==0.14.5. Ezsmdeploy can be installed with pip as follows:
-        
-        ::
-        
-            pip install ezsmdeploy
-        
-        To install locustio for testing, do:
-        
-        
-        ::
-        
-            pip install ezsmdeploy[locust]
-        
-        Cleanest way to install this package is within a virtualenv:
-        
-        
-        ::
-        
-            python -m venv env
-            
-            source env/bin/activate
-        
-            pip install ezsmdeploy[locust]
-        
-        
-        In some cases, installs fail due to an existing package installed called "greenlet". This is not a direct dependency of ezsmdeploy but interferes with the installation. To fix this, either install in a virtualenv as seen above, or do:
-        
-        ::
-        
-            pip install ezsmdeploy[locust] --ignore-installed greenlet
-            
-            
-        If you have another way to test the endpoint, or want to manage locust on your own, just do:
-        
-        ::
-        
-            pip install ezsmdeploy
-            
-           
-        
-        Key Features
-        ~~~~~~~~~~~~
-        
-        At minimum, **ezsmdeploy** requires you to provide:
-        
-        1. one or more model files
-        2. a python script with two functions: i) *load_model(modelpath)* - loads a model from a modelpath and returns a model object and ii) *predict(model,input)* - performs inference based on a model object and input data
-        3. a list of requirements or a requirements.txt file
-        
-        For example, you can do:
-        
-        ::
-        
-            ezonsm = ezsmdeploy.Deploy(model = 'model.pth',
-                          script = 'modelscript_pytorch.py',
-                          requirements = ['numpy','torch','joblib'])
-        
-        
-        You can also load multiple models ...
-        
-        ::
-        
-            ezonsm = ezsmdeploy.Deploy(model = ['model1.pth','model2.pth'],
-                          script = 'modelscript_pytorch.py',
-                          requirements = ['numpy','torch','joblib'])    
-        
-        ...  or download tar.gz models from S3
-        :: 
-            
-            ezonsm = ezsmdeploy.Deploy(model = ['s3://ezsmdeploy/pytorchmnist/model.tar.gz'],
-                          script = 'modelscript_pytorch.py',
-                          requirements = 'path/to/requirements.txt')
-        
-        
-        Other Features
-        ~~~~~~~~~~~~~~~
-        
-        The **Deploy** class is initialized with these parameters:
-        
-        ::
-        
-            class Deploy(object):
-            def __init__(
-                self,
-                model,
-                script,
-                framework=None,
-                requirements=None,
-                name=None,
-                autoscale=False,
-                autoscaletarget=1000,
-                wait=True,
-                bucket=None,
-                session=None,
-                image=None,
-                dockerfilepath=None,
-                instance_type=None,
-                instance_count=1,
-                budget=100,
-                ei=None,
-                monitor=False,
-            ):
-        
-        
-        Let's take a look at each of these parameters and what they do:
-        
-        * You can skip passing in requirements through a file or a list if you choose a **"framework"** in ["tensorflow", "pytorch", "mxnet", "sklearn"]. If you do, these libraries are installed automatically. However it is expected that most people will not use this, given the limited installs, and will usually pass in a custom set of requirements.
-        
-         :: 
-        
-            ezonsm = ezsmdeploy.Deploy(model = ... ,
-                          script = ... ,
-                          framework = 'sklearn')
-        
-        * Pass in a **"name"** if you want to override the random name generated by ezsmdeploy that is used to name your custom ECR image and the endpoint.
-        
-         :: 
-        
-            ezonsm = ezsmdeploy.Deploy(model = ... ,
-                          script = ... ,
-                          framework = 'sklearn',
-                          name = 'randomname')
-                              
-                              
-        * Set **"autoscale"** to True if required to switch on autoscaling for your endpoint. By default, this sets up endpoint autoscaling with the metric *SageMakerVariantInvocationsPerInstance* and a target value of 1000. You can override this value by also passing in a value for autoscaletarget
-        
-        |
-        
-        * **"wait**" is set to True by default and can be set to False if you don't want to wait for the endpoint to deploy.
-        
-        |
-        
-        * Passing a valid **"bucket"** name will force ezsmdeploy to use this bucket rather than the Sagemaker default session bucket
-        
-        |
-        
-        * Pass in a sagemaker **"session"** to override the default session; for most cases this is not necessary. Also, this may interfere with local deployments as the same session cannot be used for tasks such as downloading and uploading files, and for local and remote deployments.
-        
-        |
-        
-        * If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in. 
-        
-        |
-        
-        * If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe. 
-        
-        |
-        
-        * Passing in an **"instance_count"** > 1 will change the initial number of instances that the model(s) is(are) deployed on.
-        
-        |
-        
-        * Pass in a value for **"ei"** or Elastic Inference from this list - ["ml.eia2.medium","ml.eia2.large","ml.eia2.xlarge","ml.eia.medium","ml.eia.large","ml.eia.xlarge"] to add an accelerator to your deployed instance. Read more about Elastic Inference here - https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html
-        
-        |
-        
-        * Set **"monitor"** to True if you would like to turn on Datacapture for this endpoint. Currently, a sampling_percentage of 100 is used. Read more about Model monitor here - https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor.html
-        
-        |
-        
-        * You should see an output as follows for a typical deployment:
-            
-         ::
-        
-           0:00:00.143132 | compressed model(s)
-           0:00:00.403894 | uploaded model tarball(s) ; check returned modelpath
-           0:00:00.404948 | added requirements file
-           0:00:00.406745 | added source file
-           0:00:00.408180 | added Dockerfile
-           0:00:00.409959 | added model_handler and docker utils
-           0:00:00.410072 | building docker container
-           0:01:59.298091 | built docker container
-           0:01:59.647986 | created model(s). Now deploying on ml.m5.xlarge
-           0:09:31.904897 | deployed model
-           0:09:31.905450 | estimated cost is $0.3 per hour
-           0:09:31.905805 | Done! ✔ 
-        
-        
-        * Once your model is deployed, you can use locust.io to load test your endpoint. The test reports the number of requests, number of failures, average, min, max response time in milliseconds and requests per second reached based on the number of parallel users and hatch rate entered. To load test your model (make sure you have deployed it remotely first), try:
-         
-         ::
-        
-             ezonsm.test(input_data, target_model='model1.tar.gz')
-         
-         or 
-        
-         ::
-        
-             ezonsm.test(input_data, target_model='model1.tar.gz',usercount=20,hatchrate=10,timeoutsecs=10)
-             
-         ... to override default arguments. Read more about locust.io here https://docs.locust.io/en/stable/
-        
-        
-        Model Script requirements
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Make sure your model script has a load_model() and predict() function. While you can still use sagemaker's serializers and deserializers, assume that you will get a payload in bytes, and that you have to return a prediction in bytes. What you do in between is up to you. For example, your model script may look like:
-        
-        ::
-        
-            def load_model(modelpath):
-                clf = load(os.path.join(modelpath,'model.joblib'))
-                return clf
-        
-            def predict(model, payload):
-                try:
-                    # in remote / container based deployment, payload comes in as a stream of bytes
-                    out = [str(model.predict(np.frombuffer(payload[0]['body']).reshape((1,64))))]
-                except Exception as e:
-                   out = [type(payload),str(e)] #useful for debugging!
-            
-            return out
-        
-        
-        Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
-        
-        
-        Supported Operating Systems
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Ezsmdeploy SDK has been tested on Unix/Linux.
-        
-        Supported Python Versions
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Ezsmdeploy SDK has been tested on Python 3.6; should run in higher versions!
-        
-        AWS Permissions
-        ~~~~~~~~~~~~~~~
-        Ezsmdeploy uses the  Sagemaker python SDK.
-        
-        As a managed service, Amazon SageMaker performs operations on your behalf on the AWS hardware that is managed by Amazon SageMaker.
-        Amazon SageMaker can perform only operations that the user permits.
-        You can read more about which permissions are necessary in the `AWS Documentation <https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html>`__.
-        
-        The SageMaker Python SDK should not require any additional permissions aside from what is required for using SageMaker.
-        However, if you are using an IAM role with a path in it, you should grant permission for ``iam:GetRole``.
-        
-        Licensing
-        ~~~~~~~~~
-        Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/ 
-        
-        Sample Notebooks
-        ~~~~~~~~~~~~~~~~~
-        https://github.com/aws-samples/easy-amazon-sagemaker-deployments/tree/master/notebooks
-        
-        Known Gotchas
-        ~~~~~~~~~~~~~~~~~~
-        * Ezsmdeploy uses the sagemaker python sdk under the hood, so any limitations / limits / restrictions are expected to be carried over
-        
-        |
-        
-        * Ezsmdeploy builds your docker container on the fly, and uses two types of base containers - a flask-nginx deployment stack or the Multi model server. Sending in a single model, or choosing to use a GPU instance will default to the flask-nginx stack. You can force the use of the MMS stack if you pass in a single model as a list, for example, ['model1.joblib']
-        
-        |
-        
-        * Ezsmdeploy uses a local 'src' folder as a staging folder which is reset at the beginning of every deploy. So consider using the package in separate project folders so there is no overlap/ overwriting  of staging files.
-        
-        |
-        
-        * Ezsmdeploy uses Locust to do endpoint testing - any restrictions of the locustio package are also expected to be seen here.
-        
-        |
-        
-        * Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU). 
-        
-        |
-        
-        * The payload comes in as bytes; you can also use Sagemaker's serializer and deserializers to send in other formats of input data
-        
-        |
-        
-        * Not all feature combinations are tested; any contributions testing, for example, budget constraints are welcome!
-        
-        |
-        
-        * If you are doing local testing in a container, make sure you kill any running containers, since any invocations hit the same port. to do this, run:
-        
-        ::
-        
-            docker container stop $(docker container ls -aq) >/dev/nul
-        
-        * If your docker push fails, chances are that your disk is full. Try. clearing some docker images:
-        
-        ::
-        
-            docker system prune -a
-        
-        * If you encounter an "image does not exist" error, try running this script that exists after an unsuccessful run, but manually. For this, do:
-        
-        ::
-        
-           ./src/build-docker.sh 
-        
-        * Locust load testing on local endpoint has not been tested (and may not make much sense). Please use the .test() for remote deployment
-        
-        |
-        
-        * Use instance_type "local" if you would like to test locally (this lets you test using the MMS stack). If you intend to finally deploy your model to a GPU instance, use "local_gpu" - this launches the flask-nginx stack locally and the same stack when you deploy to a GPU.
-        
-        |
-        
-        * At the time of writing this guide, launching a multi-model server from sagemaker does not support GPUs (but the open source MMS repository has no such restrictions). Ezsmdeploy checks the number of models passed in, the instance type and other parameters to decide which stack to build for your endpoint.
-        
-        
-        CONTRIBUTING
-        ------------
-        
-        Please submit a pull request to the packages git repo
-        
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Provides-Extra: locust
+
+====================================================
+Ezsmdeploy - SageMaker custom deployments made easy
+====================================================
+
+.. image:: https://img.shields.io/pypi/v/ezsmdeploy.svg
+   :target: https://pypi.python.org/pypi/ezsmdeploy
+   :alt: Latest Version
+
+.. image:: https://img.shields.io/badge/code_style-black-000000.svg
+   :target: https://github.com/python/black
+   :alt: Code style: black
+
+.. image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: License: MIT
+
+.. image:: https://img.shields.io/badge/Made%20With-Love-orange.svg
+   :target: https://pypi.python.org/pypi/ezsmdeploy
+   :alt: Made With Love
+   
+
+**Ezsmdeploy** python SDK helps you easily deploy Machine learning models and provides a rich set of features such as passing one or more model files (yes, through multi-model deployments), automatically choosing an instance based on model size or based on a budget, and load testing endpoints using an intuitive API. **Ezsmdeploy** uses the SageMaker Python SDK, which is an open source library for training and deploying machine learning models on Amazon SageMaker. This SDK however focuses on simplifying deployment from existing models, and as such, this is for you if:
+
+1. you have a serialized model (a pickle / joblib/ json/ TF saved model/ Pytorch .pth/ etc) file and you want to deploy and test your model as an API endpoint
+2. you have a model or multiple models stored as local files, in local folders, or in S3 as tar files (model.tar.gz)
+3. you don't want to create a custom docker container for deployment and/or don't want to deal with docker
+4. you want to make use of advanced features such as autoscaling, elastic inference, multi-model endpoints, model inference data capture, and locust.io based load testing, without any of the heavy lifting
+5. you want to still have control of how do perform inference by passing in a python script
+
+Note for some Sagemaker estimators, deployment from pretrained models is easy; consider the Tensorflow savedmodel format. You can very easily tar your save_model.pb and variables file and use the sagemaker.tensorflow.serving.Model to register and deploy your model. Nevertheless, if your TF model is saved as checkpoints, HDF5 file, or as Tflite file, or if you have deployments needs accross multiple types of serialized model files, this may help standardize your deployment pipeline and avoid the need for building new containers for each model.
+
+V 1.x release notes
+-------------------
+1. Updated to use >v2.x of SageMaker SDK
+2. Fixed failing docker builds
+3. Tested with test notebook
+
+
+Table of Contents
+-----------------
+1. `Installing Ezsmdeploy Python SDK <#installing-the-ezsmdeploy-python-sdk>`__
+2. `Key Features <#key-features>`__
+3. `Other Features <#other-features>`__
+4. `Model script requirements <#model-script-requirements>`__
+5. `Sample notebooks <#sample-notebooks>`__
+6. `Known gotchas <#known-gotchas>`__
+
+Installing the Ezsmdeploy Python SDK
+------------------------------------
+
+
+The Ezsmdeploy Python SDK is built to PyPI and has the following dependencies sagemaker>=1.55.3, cyaspin==0.16.0,  shortuuid==1.0.1 and locustio==0.14.5. Ezsmdeploy can be installed with pip as follows:
+
+::
+
+    pip install ezsmdeploy
+
+To install locustio for testing, do:
+
+
+::
+
+    pip install ezsmdeploy[locust]
+
+Cleanest way to install this package is within a virtualenv:
+
+
+::
+
+    python -m venv env
+    
+    source env/bin/activate
+
+    pip install ezsmdeploy[locust]
+
+
+In some cases, installs fail due to an existing package installed called "greenlet". This is not a direct dependency of ezsmdeploy but interferes with the installation. To fix this, either install in a virtualenv as seen above, or do:
+
+::
+
+    pip install ezsmdeploy[locust] --ignore-installed greenlet
+    
+    
+If you have another way to test the endpoint, or want to manage locust on your own, just do:
+
+::
+
+    pip install ezsmdeploy
+    
+   
+
+Key Features
+~~~~~~~~~~~~
+
+At minimum, **ezsmdeploy** requires you to provide:
+
+1. one or more model files
+2. a python script with two functions: i) *load_model(modelpath)* - loads a model from a modelpath and returns a model object and ii) *predict(model,input)* - performs inference based on a model object and input data
+3. a list of requirements or a requirements.txt file
+
+For example, you can do:
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = 'model.pth',
+                  script = 'modelscript_pytorch.py',
+                  requirements = ['numpy','torch','joblib'])
+
+
+You can also load multiple models ...
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = ['model1.pth','model2.pth'],
+                  script = 'modelscript_pytorch.py',
+                  requirements = ['numpy','torch','joblib'])    
+
+...  or download tar.gz models from S3
+:: 
+    
+    ezonsm = ezsmdeploy.Deploy(model = ['s3://ezsmdeploy/pytorchmnist/model.tar.gz'],
+                  script = 'modelscript_pytorch.py',
+                  requirements = 'path/to/requirements.txt')
+
+
+Other Features
+~~~~~~~~~~~~~~~
+
+The **Deploy** class is initialized with these parameters:
+
+::
+
+    class Deploy(object):
+    def __init__(
+        self,
+        model,
+        script,
+        framework=None,
+        requirements=None,
+        name=None,
+        autoscale=False,
+        autoscaletarget=1000,
+        wait=True,
+        bucket=None,
+        session=None,
+        image=None,
+        dockerfilepath=None,
+        instance_type=None,
+        instance_count=1,
+        budget=100,
+        ei=None,
+        monitor=False,
+    ):
+
+
+Let's take a look at each of these parameters and what they do:
+
+* You can skip passing in requirements through a file or a list if you choose a **"framework"** in ["tensorflow", "pytorch", "mxnet", "sklearn"]. If you do, these libraries are installed automatically. However it is expected that most people will not use this, given the limited installs, and will usually pass in a custom set of requirements.
+
+ :: 
+
+    ezonsm = ezsmdeploy.Deploy(model = ... ,
+                  script = ... ,
+                  framework = 'sklearn')
+
+* Pass in a **"name"** if you want to override the random name generated by ezsmdeploy that is used to name your custom ECR image and the endpoint.
+
+ :: 
+
+    ezonsm = ezsmdeploy.Deploy(model = ... ,
+                  script = ... ,
+                  framework = 'sklearn',
+                  name = 'randomname')
+                      
+                      
+* Set **"autoscale"** to True if required to switch on autoscaling for your endpoint. By default, this sets up endpoint autoscaling with the metric *SageMakerVariantInvocationsPerInstance* and a target value of 1000. You can override this value by also passing in a value for autoscaletarget
+
+|
+
+* **"wait**" is set to True by default and can be set to False if you don't want to wait for the endpoint to deploy.
+
+|
+
+* Passing a valid **"bucket"** name will force ezsmdeploy to use this bucket rather than the Sagemaker default session bucket
+
+|
+
+* Pass in a sagemaker **"session"** to override the default session; for most cases this is not necessary. Also, this may interfere with local deployments as the same session cannot be used for tasks such as downloading and uploading files, and for local and remote deployments.
+
+|
+
+* If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in. 
+
+|
+
+* If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe. 
+
+|
+
+* Passing in an **"instance_count"** > 1 will change the initial number of instances that the model(s) is(are) deployed on.
+
+|
+
+* Pass in a value for **"ei"** or Elastic Inference from this list - ["ml.eia2.medium","ml.eia2.large","ml.eia2.xlarge","ml.eia.medium","ml.eia.large","ml.eia.xlarge"] to add an accelerator to your deployed instance. Read more about Elastic Inference here - https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html
+
+|
+
+* Set **"monitor"** to True if you would like to turn on Datacapture for this endpoint. Currently, a sampling_percentage of 100 is used. Read more about Model monitor here - https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor.html
+
+|
+
+* You should see an output as follows for a typical deployment:
+    
+ ::
+
+   0:00:00.143132 | compressed model(s)
+   0:00:00.403894 | uploaded model tarball(s) ; check returned modelpath
+   0:00:00.404948 | added requirements file
+   0:00:00.406745 | added source file
+   0:00:00.408180 | added Dockerfile
+   0:00:00.409959 | added model_handler and docker utils
+   0:00:00.410072 | building docker container
+   0:01:59.298091 | built docker container
+   0:01:59.647986 | created model(s). Now deploying on ml.m5.xlarge
+   0:09:31.904897 | deployed model
+   0:09:31.905450 | estimated cost is $0.3 per hour
+   0:09:31.905805 | Done! ✔ 
+
+
+* Once your model is deployed, you can use locust.io to load test your endpoint. The test reports the number of requests, number of failures, average, min, max response time in milliseconds and requests per second reached based on the number of parallel users and hatch rate entered. To load test your model (make sure you have deployed it remotely first), try:
+ 
+ ::
+
+     ezonsm.test(input_data, target_model='model1.tar.gz')
+ 
+ or 
+
+ ::
+
+     ezonsm.test(input_data, target_model='model1.tar.gz',usercount=20,hatchrate=10,timeoutsecs=10)
+     
+ ... to override default arguments. Read more about locust.io here https://docs.locust.io/en/stable/
+
+
+Model Script requirements
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Make sure your model script has a load_model() and predict() function. While you can still use sagemaker's serializers and deserializers, assume that you will get a payload in bytes, and that you have to return a prediction in bytes. What you do in between is up to you. For example, your model script may look like:
+
+::
+
+    def load_model(modelpath):
+        clf = load(os.path.join(modelpath,'model.joblib'))
+        return clf
+
+    def predict(model, payload):
+        try:
+            # in remote / container based deployment, payload comes in as a stream of bytes
+            out = [str(model.predict(np.frombuffer(payload[0]['body']).reshape((1,64))))]
+        except Exception as e:
+           out = [type(payload),str(e)] #useful for debugging!
+    
+    return out
+
+
+Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
+
+
+Supported Operating Systems
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Ezsmdeploy SDK has been tested on Unix/Linux.
+
+Supported Python Versions
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Ezsmdeploy SDK has been tested on Python 3.6; should run in higher versions!
+
+AWS Permissions
+~~~~~~~~~~~~~~~
+Ezsmdeploy uses the  Sagemaker python SDK.
+
+As a managed service, Amazon SageMaker performs operations on your behalf on the AWS hardware that is managed by Amazon SageMaker.
+Amazon SageMaker can perform only operations that the user permits.
+You can read more about which permissions are necessary in the `AWS Documentation <https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html>`__.
+
+The SageMaker Python SDK should not require any additional permissions aside from what is required for using SageMaker.
+However, if you are using an IAM role with a path in it, you should grant permission for ``iam:GetRole``.
+
+Licensing
+~~~~~~~~~
+Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/ 
+
+Sample Notebooks
+~~~~~~~~~~~~~~~~~
+https://github.com/aws-samples/easy-amazon-sagemaker-deployments/tree/master/notebooks
+
+Known Gotchas
+~~~~~~~~~~~~~~~~~~
+* Ezsmdeploy uses the sagemaker python sdk under the hood, so any limitations / limits / restrictions are expected to be carried over
+
+|
+
+* Ezsmdeploy builds your docker container on the fly, and uses two types of base containers - a flask-nginx deployment stack or the Multi model server. Sending in a single model, or choosing to use a GPU instance will default to the flask-nginx stack. You can force the use of the MMS stack if you pass in a single model as a list, for example, ['model1.joblib']
+
+|
+
+* Ezsmdeploy uses a local 'src' folder as a staging folder which is reset at the beginning of every deploy. So consider using the package in separate project folders so there is no overlap/ overwriting  of staging files.
+
+|
+
+* Ezsmdeploy uses Locust to do endpoint testing - any restrictions of the locustio package are also expected to be seen here.
+
+|
+
+* Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU). 
+
+|
+
+* The payload comes in as bytes; you can also use Sagemaker's serializer and deserializers to send in other formats of input data
+
+|
+
+* Not all feature combinations are tested; any contributions testing, for example, budget constraints are welcome!
+
+|
+
+* If you are doing local testing in a container, make sure you kill any running containers, since any invocations hit the same port. to do this, run:
+
+::
+
+    docker container stop $(docker container ls -aq) >/dev/nul
+
+* If your docker push fails, chances are that your disk is full. Try. clearing some docker images:
+
+::
+
+    docker system prune -a
+
+* If you encounter an "image does not exist" error, try running this script that exists after an unsuccessful run, but manually. For this, do:
+
+::
+
+   ./src/build-docker.sh 
+
+* Locust load testing on local endpoint has not been tested (and may not make much sense). Please use the .test() for remote deployment
+
+|
+
+* Use instance_type "local" if you would like to test locally (this lets you test using the MMS stack). If you intend to finally deploy your model to a GPU instance, use "local_gpu" - this launches the flask-nginx stack locally and the same stack when you deploy to a GPU.
+
+|
+
+* At the time of writing this guide, launching a multi-model server from sagemaker does not support GPUs (but the open source MMS repository has no such restrictions). Ezsmdeploy checks the number of models passed in, the instance type and other parameters to decide which stack to build for your endpoint.
+
+
+CONTRIBUTING
+------------
+
+Please submit a pull request to the packages git repo
+
+
+
```

### Comparing `ezsmdeploy-1.1.4/ezsmdeploy.egg-info/PKG-INFO` & `ezsmdeploy-1.6.dev0/ezsmdeploy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,379 +1,378 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.1.4
+Version: 1.6.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
-Description: ====================================================
-        Ezsmdeploy - SageMaker custom deployments made easy
-        ====================================================
-        
-        .. image:: https://img.shields.io/pypi/v/ezsmdeploy.svg
-           :target: https://pypi.python.org/pypi/ezsmdeploy
-           :alt: Latest Version
-        
-        .. image:: https://img.shields.io/badge/code_style-black-000000.svg
-           :target: https://github.com/python/black
-           :alt: Code style: black
-        
-        .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
-           :target: https://opensource.org/licenses/MIT
-           :alt: License: MIT
-        
-        .. image:: https://img.shields.io/badge/Made%20With-Love-orange.svg
-           :target: https://pypi.python.org/pypi/ezsmdeploy
-           :alt: Made With Love
-           
-        
-        **Ezsmdeploy** python SDK helps you easily deploy Machine learning models and provides a rich set of features such as passing one or more model files (yes, through multi-model deployments), automatically choosing an instance based on model size or based on a budget, and load testing endpoints using an intuitive API. **Ezsmdeploy** uses the SageMaker Python SDK, which is an open source library for training and deploying machine learning models on Amazon SageMaker. This SDK however focuses on simplifying deployment from existing models, and as such, this is for you if:
-        
-        1. you have a serialized model (a pickle / joblib/ json/ TF saved model/ Pytorch .pth/ etc) file and you want to deploy and test your model as an API endpoint
-        2. you have a model or multiple models stored as local files, in local folders, or in S3 as tar files (model.tar.gz)
-        3. you don't want to create a custom docker container for deployment and/or don't want to deal with docker
-        4. you want to make use of advanced features such as autoscaling, elastic inference, multi-model endpoints, model inference data capture, and locust.io based load testing, without any of the heavy lifting
-        5. you want to still have control of how do perform inference by passing in a python script
-        
-        Note for some Sagemaker estimators, deployment from pretrained models is easy; consider the Tensorflow savedmodel format. You can very easily tar your save_model.pb and variables file and use the sagemaker.tensorflow.serving.Model to register and deploy your model. Nevertheless, if your TF model is saved as checkpoints, HDF5 file, or as Tflite file, or if you have deployments needs accross multiple types of serialized model files, this may help standardize your deployment pipeline and avoid the need for building new containers for each model.
-        
-        V 1.x release notes
-        -------------------
-        1. Updated to use >v2.x of SageMaker SDK
-        2. Fixed failing docker builds
-        3. Tested with test notebook
-        
-        
-        Table of Contents
-        -----------------
-        1. `Installing Ezsmdeploy Python SDK <#installing-the-ezsmdeploy-python-sdk>`__
-        2. `Key Features <#key-features>`__
-        3. `Other Features <#other-features>`__
-        4. `Model script requirements <#model-script-requirements>`__
-        5. `Sample notebooks <#sample-notebooks>`__
-        6. `Known gotchas <#known-gotchas>`__
-        
-        Installing the Ezsmdeploy Python SDK
-        ------------------------------------
-        
-        
-        The Ezsmdeploy Python SDK is built to PyPI and has the following dependencies sagemaker>=1.55.3, cyaspin==0.16.0,  shortuuid==1.0.1 and locustio==0.14.5. Ezsmdeploy can be installed with pip as follows:
-        
-        ::
-        
-            pip install ezsmdeploy
-        
-        To install locustio for testing, do:
-        
-        
-        ::
-        
-            pip install ezsmdeploy[locust]
-        
-        Cleanest way to install this package is within a virtualenv:
-        
-        
-        ::
-        
-            python -m venv env
-            
-            source env/bin/activate
-        
-            pip install ezsmdeploy[locust]
-        
-        
-        In some cases, installs fail due to an existing package installed called "greenlet". This is not a direct dependency of ezsmdeploy but interferes with the installation. To fix this, either install in a virtualenv as seen above, or do:
-        
-        ::
-        
-            pip install ezsmdeploy[locust] --ignore-installed greenlet
-            
-            
-        If you have another way to test the endpoint, or want to manage locust on your own, just do:
-        
-        ::
-        
-            pip install ezsmdeploy
-            
-           
-        
-        Key Features
-        ~~~~~~~~~~~~
-        
-        At minimum, **ezsmdeploy** requires you to provide:
-        
-        1. one or more model files
-        2. a python script with two functions: i) *load_model(modelpath)* - loads a model from a modelpath and returns a model object and ii) *predict(model,input)* - performs inference based on a model object and input data
-        3. a list of requirements or a requirements.txt file
-        
-        For example, you can do:
-        
-        ::
-        
-            ezonsm = ezsmdeploy.Deploy(model = 'model.pth',
-                          script = 'modelscript_pytorch.py',
-                          requirements = ['numpy','torch','joblib'])
-        
-        
-        You can also load multiple models ...
-        
-        ::
-        
-            ezonsm = ezsmdeploy.Deploy(model = ['model1.pth','model2.pth'],
-                          script = 'modelscript_pytorch.py',
-                          requirements = ['numpy','torch','joblib'])    
-        
-        ...  or download tar.gz models from S3
-        :: 
-            
-            ezonsm = ezsmdeploy.Deploy(model = ['s3://ezsmdeploy/pytorchmnist/model.tar.gz'],
-                          script = 'modelscript_pytorch.py',
-                          requirements = 'path/to/requirements.txt')
-        
-        
-        Other Features
-        ~~~~~~~~~~~~~~~
-        
-        The **Deploy** class is initialized with these parameters:
-        
-        ::
-        
-            class Deploy(object):
-            def __init__(
-                self,
-                model,
-                script,
-                framework=None,
-                requirements=None,
-                name=None,
-                autoscale=False,
-                autoscaletarget=1000,
-                wait=True,
-                bucket=None,
-                session=None,
-                image=None,
-                dockerfilepath=None,
-                instance_type=None,
-                instance_count=1,
-                budget=100,
-                ei=None,
-                monitor=False,
-            ):
-        
-        
-        Let's take a look at each of these parameters and what they do:
-        
-        * You can skip passing in requirements through a file or a list if you choose a **"framework"** in ["tensorflow", "pytorch", "mxnet", "sklearn"]. If you do, these libraries are installed automatically. However it is expected that most people will not use this, given the limited installs, and will usually pass in a custom set of requirements.
-        
-         :: 
-        
-            ezonsm = ezsmdeploy.Deploy(model = ... ,
-                          script = ... ,
-                          framework = 'sklearn')
-        
-        * Pass in a **"name"** if you want to override the random name generated by ezsmdeploy that is used to name your custom ECR image and the endpoint.
-        
-         :: 
-        
-            ezonsm = ezsmdeploy.Deploy(model = ... ,
-                          script = ... ,
-                          framework = 'sklearn',
-                          name = 'randomname')
-                              
-                              
-        * Set **"autoscale"** to True if required to switch on autoscaling for your endpoint. By default, this sets up endpoint autoscaling with the metric *SageMakerVariantInvocationsPerInstance* and a target value of 1000. You can override this value by also passing in a value for autoscaletarget
-        
-        |
-        
-        * **"wait**" is set to True by default and can be set to False if you don't want to wait for the endpoint to deploy.
-        
-        |
-        
-        * Passing a valid **"bucket"** name will force ezsmdeploy to use this bucket rather than the Sagemaker default session bucket
-        
-        |
-        
-        * Pass in a sagemaker **"session"** to override the default session; for most cases this is not necessary. Also, this may interfere with local deployments as the same session cannot be used for tasks such as downloading and uploading files, and for local and remote deployments.
-        
-        |
-        
-        * If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in. 
-        
-        |
-        
-        * If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe. 
-        
-        |
-        
-        * Passing in an **"instance_count"** > 1 will change the initial number of instances that the model(s) is(are) deployed on.
-        
-        |
-        
-        * Pass in a value for **"ei"** or Elastic Inference from this list - ["ml.eia2.medium","ml.eia2.large","ml.eia2.xlarge","ml.eia.medium","ml.eia.large","ml.eia.xlarge"] to add an accelerator to your deployed instance. Read more about Elastic Inference here - https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html
-        
-        |
-        
-        * Set **"monitor"** to True if you would like to turn on Datacapture for this endpoint. Currently, a sampling_percentage of 100 is used. Read more about Model monitor here - https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor.html
-        
-        |
-        
-        * You should see an output as follows for a typical deployment:
-            
-         ::
-        
-           0:00:00.143132 | compressed model(s)
-           0:00:00.403894 | uploaded model tarball(s) ; check returned modelpath
-           0:00:00.404948 | added requirements file
-           0:00:00.406745 | added source file
-           0:00:00.408180 | added Dockerfile
-           0:00:00.409959 | added model_handler and docker utils
-           0:00:00.410072 | building docker container
-           0:01:59.298091 | built docker container
-           0:01:59.647986 | created model(s). Now deploying on ml.m5.xlarge
-           0:09:31.904897 | deployed model
-           0:09:31.905450 | estimated cost is $0.3 per hour
-           0:09:31.905805 | Done! ✔ 
-        
-        
-        * Once your model is deployed, you can use locust.io to load test your endpoint. The test reports the number of requests, number of failures, average, min, max response time in milliseconds and requests per second reached based on the number of parallel users and hatch rate entered. To load test your model (make sure you have deployed it remotely first), try:
-         
-         ::
-        
-             ezonsm.test(input_data, target_model='model1.tar.gz')
-         
-         or 
-        
-         ::
-        
-             ezonsm.test(input_data, target_model='model1.tar.gz',usercount=20,hatchrate=10,timeoutsecs=10)
-             
-         ... to override default arguments. Read more about locust.io here https://docs.locust.io/en/stable/
-        
-        
-        Model Script requirements
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Make sure your model script has a load_model() and predict() function. While you can still use sagemaker's serializers and deserializers, assume that you will get a payload in bytes, and that you have to return a prediction in bytes. What you do in between is up to you. For example, your model script may look like:
-        
-        ::
-        
-            def load_model(modelpath):
-                clf = load(os.path.join(modelpath,'model.joblib'))
-                return clf
-        
-            def predict(model, payload):
-                try:
-                    # in remote / container based deployment, payload comes in as a stream of bytes
-                    out = [str(model.predict(np.frombuffer(payload[0]['body']).reshape((1,64))))]
-                except Exception as e:
-                   out = [type(payload),str(e)] #useful for debugging!
-            
-            return out
-        
-        
-        Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
-        
-        
-        Supported Operating Systems
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Ezsmdeploy SDK has been tested on Unix/Linux.
-        
-        Supported Python Versions
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Ezsmdeploy SDK has been tested on Python 3.6; should run in higher versions!
-        
-        AWS Permissions
-        ~~~~~~~~~~~~~~~
-        Ezsmdeploy uses the  Sagemaker python SDK.
-        
-        As a managed service, Amazon SageMaker performs operations on your behalf on the AWS hardware that is managed by Amazon SageMaker.
-        Amazon SageMaker can perform only operations that the user permits.
-        You can read more about which permissions are necessary in the `AWS Documentation <https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html>`__.
-        
-        The SageMaker Python SDK should not require any additional permissions aside from what is required for using SageMaker.
-        However, if you are using an IAM role with a path in it, you should grant permission for ``iam:GetRole``.
-        
-        Licensing
-        ~~~~~~~~~
-        Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/ 
-        
-        Sample Notebooks
-        ~~~~~~~~~~~~~~~~~
-        https://github.com/aws-samples/easy-amazon-sagemaker-deployments/tree/master/notebooks
-        
-        Known Gotchas
-        ~~~~~~~~~~~~~~~~~~
-        * Ezsmdeploy uses the sagemaker python sdk under the hood, so any limitations / limits / restrictions are expected to be carried over
-        
-        |
-        
-        * Ezsmdeploy builds your docker container on the fly, and uses two types of base containers - a flask-nginx deployment stack or the Multi model server. Sending in a single model, or choosing to use a GPU instance will default to the flask-nginx stack. You can force the use of the MMS stack if you pass in a single model as a list, for example, ['model1.joblib']
-        
-        |
-        
-        * Ezsmdeploy uses a local 'src' folder as a staging folder which is reset at the beginning of every deploy. So consider using the package in separate project folders so there is no overlap/ overwriting  of staging files.
-        
-        |
-        
-        * Ezsmdeploy uses Locust to do endpoint testing - any restrictions of the locustio package are also expected to be seen here.
-        
-        |
-        
-        * Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU). 
-        
-        |
-        
-        * The payload comes in as bytes; you can also use Sagemaker's serializer and deserializers to send in other formats of input data
-        
-        |
-        
-        * Not all feature combinations are tested; any contributions testing, for example, budget constraints are welcome!
-        
-        |
-        
-        * If you are doing local testing in a container, make sure you kill any running containers, since any invocations hit the same port. to do this, run:
-        
-        ::
-        
-            docker container stop $(docker container ls -aq) >/dev/nul
-        
-        * If your docker push fails, chances are that your disk is full. Try. clearing some docker images:
-        
-        ::
-        
-            docker system prune -a
-        
-        * If you encounter an "image does not exist" error, try running this script that exists after an unsuccessful run, but manually. For this, do:
-        
-        ::
-        
-           ./src/build-docker.sh 
-        
-        * Locust load testing on local endpoint has not been tested (and may not make much sense). Please use the .test() for remote deployment
-        
-        |
-        
-        * Use instance_type "local" if you would like to test locally (this lets you test using the MMS stack). If you intend to finally deploy your model to a GPU instance, use "local_gpu" - this launches the flask-nginx stack locally and the same stack when you deploy to a GPU.
-        
-        |
-        
-        * At the time of writing this guide, launching a multi-model server from sagemaker does not support GPUs (but the open source MMS repository has no such restrictions). Ezsmdeploy checks the number of models passed in, the instance type and other parameters to decide which stack to build for your endpoint.
-        
-        
-        CONTRIBUTING
-        ------------
-        
-        Please submit a pull request to the packages git repo
-        
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Provides-Extra: locust
+
+====================================================
+Ezsmdeploy - SageMaker custom deployments made easy
+====================================================
+
+.. image:: https://img.shields.io/pypi/v/ezsmdeploy.svg
+   :target: https://pypi.python.org/pypi/ezsmdeploy
+   :alt: Latest Version
+
+.. image:: https://img.shields.io/badge/code_style-black-000000.svg
+   :target: https://github.com/python/black
+   :alt: Code style: black
+
+.. image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: License: MIT
+
+.. image:: https://img.shields.io/badge/Made%20With-Love-orange.svg
+   :target: https://pypi.python.org/pypi/ezsmdeploy
+   :alt: Made With Love
+   
+
+**Ezsmdeploy** python SDK helps you easily deploy Machine learning models and provides a rich set of features such as passing one or more model files (yes, through multi-model deployments), automatically choosing an instance based on model size or based on a budget, and load testing endpoints using an intuitive API. **Ezsmdeploy** uses the SageMaker Python SDK, which is an open source library for training and deploying machine learning models on Amazon SageMaker. This SDK however focuses on simplifying deployment from existing models, and as such, this is for you if:
+
+1. you have a serialized model (a pickle / joblib/ json/ TF saved model/ Pytorch .pth/ etc) file and you want to deploy and test your model as an API endpoint
+2. you have a model or multiple models stored as local files, in local folders, or in S3 as tar files (model.tar.gz)
+3. you don't want to create a custom docker container for deployment and/or don't want to deal with docker
+4. you want to make use of advanced features such as autoscaling, elastic inference, multi-model endpoints, model inference data capture, and locust.io based load testing, without any of the heavy lifting
+5. you want to still have control of how do perform inference by passing in a python script
+
+Note for some Sagemaker estimators, deployment from pretrained models is easy; consider the Tensorflow savedmodel format. You can very easily tar your save_model.pb and variables file and use the sagemaker.tensorflow.serving.Model to register and deploy your model. Nevertheless, if your TF model is saved as checkpoints, HDF5 file, or as Tflite file, or if you have deployments needs accross multiple types of serialized model files, this may help standardize your deployment pipeline and avoid the need for building new containers for each model.
+
+V 1.x release notes
+-------------------
+1. Updated to use >v2.x of SageMaker SDK
+2. Fixed failing docker builds
+3. Tested with test notebook
+
+
+Table of Contents
+-----------------
+1. `Installing Ezsmdeploy Python SDK <#installing-the-ezsmdeploy-python-sdk>`__
+2. `Key Features <#key-features>`__
+3. `Other Features <#other-features>`__
+4. `Model script requirements <#model-script-requirements>`__
+5. `Sample notebooks <#sample-notebooks>`__
+6. `Known gotchas <#known-gotchas>`__
+
+Installing the Ezsmdeploy Python SDK
+------------------------------------
+
+
+The Ezsmdeploy Python SDK is built to PyPI and has the following dependencies sagemaker>=1.55.3, cyaspin==0.16.0,  shortuuid==1.0.1 and locustio==0.14.5. Ezsmdeploy can be installed with pip as follows:
+
+::
+
+    pip install ezsmdeploy
+
+To install locustio for testing, do:
+
+
+::
+
+    pip install ezsmdeploy[locust]
+
+Cleanest way to install this package is within a virtualenv:
+
+
+::
+
+    python -m venv env
+    
+    source env/bin/activate
+
+    pip install ezsmdeploy[locust]
+
+
+In some cases, installs fail due to an existing package installed called "greenlet". This is not a direct dependency of ezsmdeploy but interferes with the installation. To fix this, either install in a virtualenv as seen above, or do:
+
+::
+
+    pip install ezsmdeploy[locust] --ignore-installed greenlet
+    
+    
+If you have another way to test the endpoint, or want to manage locust on your own, just do:
+
+::
+
+    pip install ezsmdeploy
+    
+   
+
+Key Features
+~~~~~~~~~~~~
+
+At minimum, **ezsmdeploy** requires you to provide:
+
+1. one or more model files
+2. a python script with two functions: i) *load_model(modelpath)* - loads a model from a modelpath and returns a model object and ii) *predict(model,input)* - performs inference based on a model object and input data
+3. a list of requirements or a requirements.txt file
+
+For example, you can do:
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = 'model.pth',
+                  script = 'modelscript_pytorch.py',
+                  requirements = ['numpy','torch','joblib'])
+
+
+You can also load multiple models ...
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = ['model1.pth','model2.pth'],
+                  script = 'modelscript_pytorch.py',
+                  requirements = ['numpy','torch','joblib'])    
+
+...  or download tar.gz models from S3
+:: 
+    
+    ezonsm = ezsmdeploy.Deploy(model = ['s3://ezsmdeploy/pytorchmnist/model.tar.gz'],
+                  script = 'modelscript_pytorch.py',
+                  requirements = 'path/to/requirements.txt')
+
+
+Other Features
+~~~~~~~~~~~~~~~
+
+The **Deploy** class is initialized with these parameters:
+
+::
+
+    class Deploy(object):
+    def __init__(
+        self,
+        model,
+        script,
+        framework=None,
+        requirements=None,
+        name=None,
+        autoscale=False,
+        autoscaletarget=1000,
+        wait=True,
+        bucket=None,
+        session=None,
+        image=None,
+        dockerfilepath=None,
+        instance_type=None,
+        instance_count=1,
+        budget=100,
+        ei=None,
+        monitor=False,
+    ):
+
+
+Let's take a look at each of these parameters and what they do:
+
+* You can skip passing in requirements through a file or a list if you choose a **"framework"** in ["tensorflow", "pytorch", "mxnet", "sklearn"]. If you do, these libraries are installed automatically. However it is expected that most people will not use this, given the limited installs, and will usually pass in a custom set of requirements.
+
+ :: 
+
+    ezonsm = ezsmdeploy.Deploy(model = ... ,
+                  script = ... ,
+                  framework = 'sklearn')
+
+* Pass in a **"name"** if you want to override the random name generated by ezsmdeploy that is used to name your custom ECR image and the endpoint.
+
+ :: 
+
+    ezonsm = ezsmdeploy.Deploy(model = ... ,
+                  script = ... ,
+                  framework = 'sklearn',
+                  name = 'randomname')
+                      
+                      
+* Set **"autoscale"** to True if required to switch on autoscaling for your endpoint. By default, this sets up endpoint autoscaling with the metric *SageMakerVariantInvocationsPerInstance* and a target value of 1000. You can override this value by also passing in a value for autoscaletarget
+
+|
+
+* **"wait**" is set to True by default and can be set to False if you don't want to wait for the endpoint to deploy.
+
+|
+
+* Passing a valid **"bucket"** name will force ezsmdeploy to use this bucket rather than the Sagemaker default session bucket
+
+|
+
+* Pass in a sagemaker **"session"** to override the default session; for most cases this is not necessary. Also, this may interfere with local deployments as the same session cannot be used for tasks such as downloading and uploading files, and for local and remote deployments.
+
+|
+
+* If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in. 
+
+|
+
+* If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe. 
+
+|
+
+* Passing in an **"instance_count"** > 1 will change the initial number of instances that the model(s) is(are) deployed on.
+
+|
+
+* Pass in a value for **"ei"** or Elastic Inference from this list - ["ml.eia2.medium","ml.eia2.large","ml.eia2.xlarge","ml.eia.medium","ml.eia.large","ml.eia.xlarge"] to add an accelerator to your deployed instance. Read more about Elastic Inference here - https://docs.aws.amazon.com/sagemaker/latest/dg/ei.html
+
+|
+
+* Set **"monitor"** to True if you would like to turn on Datacapture for this endpoint. Currently, a sampling_percentage of 100 is used. Read more about Model monitor here - https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor.html
+
+|
+
+* You should see an output as follows for a typical deployment:
+    
+ ::
+
+   0:00:00.143132 | compressed model(s)
+   0:00:00.403894 | uploaded model tarball(s) ; check returned modelpath
+   0:00:00.404948 | added requirements file
+   0:00:00.406745 | added source file
+   0:00:00.408180 | added Dockerfile
+   0:00:00.409959 | added model_handler and docker utils
+   0:00:00.410072 | building docker container
+   0:01:59.298091 | built docker container
+   0:01:59.647986 | created model(s). Now deploying on ml.m5.xlarge
+   0:09:31.904897 | deployed model
+   0:09:31.905450 | estimated cost is $0.3 per hour
+   0:09:31.905805 | Done! ✔ 
+
+
+* Once your model is deployed, you can use locust.io to load test your endpoint. The test reports the number of requests, number of failures, average, min, max response time in milliseconds and requests per second reached based on the number of parallel users and hatch rate entered. To load test your model (make sure you have deployed it remotely first), try:
+ 
+ ::
+
+     ezonsm.test(input_data, target_model='model1.tar.gz')
+ 
+ or 
+
+ ::
+
+     ezonsm.test(input_data, target_model='model1.tar.gz',usercount=20,hatchrate=10,timeoutsecs=10)
+     
+ ... to override default arguments. Read more about locust.io here https://docs.locust.io/en/stable/
+
+
+Model Script requirements
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Make sure your model script has a load_model() and predict() function. While you can still use sagemaker's serializers and deserializers, assume that you will get a payload in bytes, and that you have to return a prediction in bytes. What you do in between is up to you. For example, your model script may look like:
+
+::
+
+    def load_model(modelpath):
+        clf = load(os.path.join(modelpath,'model.joblib'))
+        return clf
+
+    def predict(model, payload):
+        try:
+            # in remote / container based deployment, payload comes in as a stream of bytes
+            out = [str(model.predict(np.frombuffer(payload[0]['body']).reshape((1,64))))]
+        except Exception as e:
+           out = [type(payload),str(e)] #useful for debugging!
+    
+    return out
+
+
+Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
+
+
+Supported Operating Systems
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Ezsmdeploy SDK has been tested on Unix/Linux.
+
+Supported Python Versions
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Ezsmdeploy SDK has been tested on Python 3.6; should run in higher versions!
+
+AWS Permissions
+~~~~~~~~~~~~~~~
+Ezsmdeploy uses the  Sagemaker python SDK.
+
+As a managed service, Amazon SageMaker performs operations on your behalf on the AWS hardware that is managed by Amazon SageMaker.
+Amazon SageMaker can perform only operations that the user permits.
+You can read more about which permissions are necessary in the `AWS Documentation <https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html>`__.
+
+The SageMaker Python SDK should not require any additional permissions aside from what is required for using SageMaker.
+However, if you are using an IAM role with a path in it, you should grant permission for ``iam:GetRole``.
+
+Licensing
+~~~~~~~~~
+Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/ 
+
+Sample Notebooks
+~~~~~~~~~~~~~~~~~
+https://github.com/aws-samples/easy-amazon-sagemaker-deployments/tree/master/notebooks
+
+Known Gotchas
+~~~~~~~~~~~~~~~~~~
+* Ezsmdeploy uses the sagemaker python sdk under the hood, so any limitations / limits / restrictions are expected to be carried over
+
+|
+
+* Ezsmdeploy builds your docker container on the fly, and uses two types of base containers - a flask-nginx deployment stack or the Multi model server. Sending in a single model, or choosing to use a GPU instance will default to the flask-nginx stack. You can force the use of the MMS stack if you pass in a single model as a list, for example, ['model1.joblib']
+
+|
+
+* Ezsmdeploy uses a local 'src' folder as a staging folder which is reset at the beginning of every deploy. So consider using the package in separate project folders so there is no overlap/ overwriting  of staging files.
+
+|
+
+* Ezsmdeploy uses Locust to do endpoint testing - any restrictions of the locustio package are also expected to be seen here.
+
+|
+
+* Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU). 
+
+|
+
+* The payload comes in as bytes; you can also use Sagemaker's serializer and deserializers to send in other formats of input data
+
+|
+
+* Not all feature combinations are tested; any contributions testing, for example, budget constraints are welcome!
+
+|
+
+* If you are doing local testing in a container, make sure you kill any running containers, since any invocations hit the same port. to do this, run:
+
+::
+
+    docker container stop $(docker container ls -aq) >/dev/nul
+
+* If your docker push fails, chances are that your disk is full. Try. clearing some docker images:
+
+::
+
+    docker system prune -a
+
+* If you encounter an "image does not exist" error, try running this script that exists after an unsuccessful run, but manually. For this, do:
+
+::
+
+   ./src/build-docker.sh 
+
+* Locust load testing on local endpoint has not been tested (and may not make much sense). Please use the .test() for remote deployment
+
+|
+
+* Use instance_type "local" if you would like to test locally (this lets you test using the MMS stack). If you intend to finally deploy your model to a GPU instance, use "local_gpu" - this launches the flask-nginx stack locally and the same stack when you deploy to a GPU.
+
+|
+
+* At the time of writing this guide, launching a multi-model server from sagemaker does not support GPUs (but the open source MMS repository has no such restrictions). Ezsmdeploy checks the number of models passed in, the instance type and other parameters to decide which stack to build for your endpoint.
+
+
+CONTRIBUTING
+------------
+
+Please submit a pull request to the packages git repo
+
+
+
```


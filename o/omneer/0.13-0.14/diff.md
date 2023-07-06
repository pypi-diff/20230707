# Comparing `tmp/omneer-0.13.tar.gz` & `tmp/omneer-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omneer-0.13.tar", last modified: Thu Jul  6 21:08:59 2023, max compression
+gzip compressed data, was "dist/omneer-0.14.tar", last modified: Thu Jul  6 21:32:54 2023, max compression
```

## Comparing `omneer-0.13.tar` & `omneer-0.14.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:59.145809 omneer-0.13/
--rw-r--r--   0 williamblair   (501) staff       (20)     3736 2023-07-06 21:08:59.143312 omneer-0.13/PKG-INFO
--rw-r--r--   0 williamblair   (501) staff       (20)     3300 2023-07-06 04:35:57.000000 omneer-0.13/README.md
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:56.880935 omneer-0.13/omneer/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/__init__.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.285127 omneer-0.13/omneer/data/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/data/__init__.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.285625 omneer-0.13/omneer/data/external/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/data/external/__init__.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.285848 omneer-0.13/omneer/data/fusion/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/data/fusion/__init__.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.286321 omneer-0.13/omneer/data/preprocessing/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/data/preprocessing/__init__.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.298333 omneer-0.13/omneer/model/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/model/__init__.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.310876 omneer-0.13/omneer/model/deeplearning/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/model/deeplearning/__init__.py
--rw-r--r--   0 williamblair   (501) staff       (20)     8580 2023-07-06 04:35:57.000000 omneer-0.13/omneer/model/deeplearning/mlp.py
--rw-r--r--   0 williamblair   (501) staff       (20)     6212 2023-07-06 04:49:18.000000 omneer-0.13/omneer/model/train.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.349328 omneer-0.13/omneer/processing/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/processing/__init__.py
--rw-r--r--   0 williamblair   (501) staff       (20)     2036 2023-07-06 04:35:57.000000 omneer-0.13/omneer/processing/bootstrap.py
--rw-r--r--   0 williamblair   (501) staff       (20)     3563 2023-07-06 20:38:18.000000 omneer-0.13/omneer/processing/main.py
--rw-r--r--   0 williamblair   (501) staff       (20)     8847 2023-07-06 04:35:57.000000 omneer-0.13/omneer/processing/misc.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.922049 omneer-0.13/omneer/visualization/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/__init__.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:59.140179 omneer-0.13/omneer/visualization/graph/
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/__init__.py
--rw-r--r--   0 williamblair   (501) staff       (20)     4917 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/grid_search_.py
--rw-r--r--   0 williamblair   (501) staff       (20)      979 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/plot_summary.py
--rw-r--r--   0 williamblair   (501) staff       (20)     1573 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/plot_swarm.py
--rw-r--r--   0 williamblair   (501) staff       (20)      496 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/shap_1_aggregate.py
--rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/shap_2_average.py
--rw-r--r--   0 williamblair   (501) staff       (20)      744 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/shap_3_correlation.py
--rw-r--r--   0 williamblair   (501) staff       (20)      428 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/shap_4_summary.py
--rw-r--r--   0 williamblair   (501) staff       (20)     1576 2023-07-06 04:35:57.000000 omneer-0.13/omneer/visualization/graph/shap_analysis__.py
--rw-r--r--   0 williamblair   (501) staff       (20)     2955 2023-07-06 18:26:25.000000 omneer-0.13/omneer/visualization/plot.py
-drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:08:57.282722 omneer-0.13/omneer.egg-info/
--rw-r--r--   0 williamblair   (501) staff       (20)     3736 2023-07-06 21:08:54.000000 omneer-0.13/omneer.egg-info/PKG-INFO
--rw-r--r--   0 williamblair   (501) staff       (20)     1036 2023-07-06 21:08:56.000000 omneer-0.13/omneer.egg-info/SOURCES.txt
--rw-r--r--   0 williamblair   (501) staff       (20)        1 2023-07-06 21:08:54.000000 omneer-0.13/omneer.egg-info/dependency_links.txt
--rw-r--r--   0 williamblair   (501) staff       (20)       47 2023-07-06 21:08:54.000000 omneer-0.13/omneer.egg-info/entry_points.txt
--rw-r--r--   0 williamblair   (501) staff       (20)      268 2023-07-06 21:08:54.000000 omneer-0.13/omneer.egg-info/requires.txt
--rw-r--r--   0 williamblair   (501) staff       (20)        7 2023-07-06 21:08:54.000000 omneer-0.13/omneer.egg-info/top_level.txt
--rw-r--r--   0 williamblair   (501) staff       (20)       38 2023-07-06 21:08:59.145898 omneer-0.13/setup.cfg
--rw-r--r--   0 williamblair   (501) staff       (20)     1327 2023-07-06 21:06:41.000000 omneer-0.13/setup.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer.egg-info/
+-rw-r--r--   0 williamblair   (501) staff       (20)     4367 2023-07-06 21:32:54.000000 omneer-0.14/omneer.egg-info/PKG-INFO
+-rw-r--r--   0 williamblair   (501) staff       (20)     1036 2023-07-06 21:32:54.000000 omneer-0.14/omneer.egg-info/SOURCES.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)       48 2023-07-06 21:32:54.000000 omneer-0.14/omneer.egg-info/entry_points.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)      268 2023-07-06 21:32:54.000000 omneer-0.14/omneer.egg-info/requires.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)        7 2023-07-06 21:32:54.000000 omneer-0.14/omneer.egg-info/top_level.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)        1 2023-07-06 21:32:54.000000 omneer-0.14/omneer.egg-info/dependency_links.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)     4367 2023-07-06 21:32:54.000000 omneer-0.14/PKG-INFO
+-rw-r--r--   0 williamblair   (501) staff       (20)     3292 2023-07-06 21:31:26.000000 omneer-0.14/README.md
+-rw-r--r--   0 williamblair   (501) staff       (20)     1327 2023-07-06 21:32:09.000000 omneer-0.14/setup.py
+-rw-r--r--   0 williamblair   (501) staff       (20)       38 2023-07-06 21:32:54.000000 omneer-0.14/setup.cfg
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/visualization/
+-rw-r--r--   0 williamblair   (501) staff       (20)     2955 2023-07-06 18:26:25.000000 omneer-0.14/omneer/visualization/plot.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/visualization/graph/
+-rw-r--r--   0 williamblair   (501) staff       (20)      496 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/shap_1_aggregate.py
+-rw-r--r--   0 williamblair   (501) staff       (20)      428 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/shap_4_summary.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     1573 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/plot_swarm.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     4917 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/grid_search_.py
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)      979 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/plot_summary.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     1576 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/shap_analysis__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)      744 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/shap_3_correlation.py
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/graph/shap_2_average.py
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/visualization/__init__.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/processing/
+-rw-r--r--   0 williamblair   (501) staff       (20)     2036 2023-07-06 04:35:57.000000 omneer-0.14/omneer/processing/bootstrap.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     8847 2023-07-06 04:35:57.000000 omneer-0.14/omneer/processing/misc.py
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/processing/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     3563 2023-07-06 20:38:18.000000 omneer-0.14/omneer/processing/main.py
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/__init__.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/model/
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/model/deeplearning/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/model/deeplearning/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     8580 2023-07-06 04:35:57.000000 omneer-0.14/omneer/model/deeplearning/mlp.py
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/model/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     6212 2023-07-06 04:49:18.000000 omneer-0.14/omneer/model/train.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/data/
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/data/fusion/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/data/fusion/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/data/__init__.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/data/preprocessing/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/data/preprocessing/__init__.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-06 21:32:54.000000 omneer-0.14/omneer/data/external/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-06 04:35:57.000000 omneer-0.14/omneer/data/external/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `omneer-0.13/PKG-INFO` & `omneer-0.14/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: omneer
-Version: 0.13
-Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
-Home-page: http://docs.omneer.xyz
-Author: William Blair
-Author-email: william.blair0708@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-
 <div align="center">
 
 # Omneer SDK
 
 Omneer SDK is a state-of-the-art toolkit designed for the development and deployment of AI and machine learning powered personalized medicine applications in the neuroscience field. The SDK, with its Python-centric approach, provides an easy-to-use platform for developers to create and interact with their applications.
 
 Fueled by Airflow, a dynamic and highly scalable workflow orchestration engine known for its efficiency and flexibility, Omneer SDK ensures seamless processing and management of complex data workflows. Airflow's Directed Acyclic Graph (DAG) approach ensures atomicity at a task level, allowing for a comprehensive and orderly execution of tasks.
@@ -40,15 +27,15 @@
 ### Getting Started
 
 See the SDK in action by following the steps below to register your first workflow with Omneer.
 
 First, install omneer through `pip`.
 
 ```
-$ python3 pip install omneer
+$ pip install omneer
 ```
 
 Then, create some boilerplate code for your new workflow.
 
 ```
 $ omneer init diagnosis
 ```
```

### Comparing `omneer-0.13/README.md` & `omneer-0.14/omneer.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,90 @@
-<div align="center">
-
-# Omneer SDK
-
-Omneer SDK is a state-of-the-art toolkit designed for the development and deployment of AI and machine learning powered personalized medicine applications in the neuroscience field. The SDK, with its Python-centric approach, provides an easy-to-use platform for developers to create and interact with their applications.
-
-Fueled by Airflow, a dynamic and highly scalable workflow orchestration engine known for its efficiency and flexibility, Omneer SDK ensures seamless processing and management of complex data workflows. Airflow's Directed Acyclic Graph (DAG) approach ensures atomicity at a task level, allowing for a comprehensive and orderly execution of tasks.
-
-This SDK further enhances workflow execution with containerization options, offering independence in task scheduling and a vast array of scalable computing resources. As such, the Omneer SDK represents a perfect convergence of neuroscience, personalized medicine, and cutting-edge technology, promising a new era of advanced and personalized healthcare solutions.
-
-[Discord Community Community]() • [Docs](https://docs.omneer.xyz) • [Installation](#installation) •
-[Quickstart](#configuration) • [Omneer](https://omneer.xyz)
-
-</div>
-
-Utilizing the Omneer SDK, developers can deliver:
-
-- Personalized AI and machine learning tools
-- Advanced disease progression diagnosis and tracking
-- Creation of digital twins for individualized healthcare
-- Instant no-code interfaces for rapid deployment
-- High-performing, reliable cloud infrastructure
-- Flexibility to define resources (CPU, GPU, etc.) for serverless execution
-
-- Omneer SDK continues to be a ground-breaking platform for personalized healthcare solutions. Browse our collection of existing and actively maintained solutions at [Omneer Community]().
-
-### Getting Started
-
-See the SDK in action by following the steps below to register your first workflow with Omneer.
-
-First, install omneer through `pip`.
-
-```
-$ python3 pip install omneer
-```
-
-Then, create some boilerplate code for your new workflow.
-
-```
-$ omneer init diagnosis
-```
-
-The registration process, which could take a few minutes depending on your network connection, involves building a Docker image with your workflow code, serializing the code, registering it with your Omneer account, and pushing the Docker image to a managed container registry.
-
-Upon successful registration, your new workflow should be visible in your Omneer Console.
-
-For issues with registration or other queries, please raise an issue on GitHub.
-
----
-
-### Installation
-
-Omneer SDK is distributed via pip. We recommend installing it in a clean virtual environment for the best user experience.
-
-Virtualenv is our recommended tool for creating isolated Python environments.
-
-[Virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) is recommended.
-
-```
-pip install omneer
-```
-
-### Examples
-
-[Omneer Examples]() features list of well-curated workflows developed by the Omneer team. 
-* [Parkinson's Diagnosis]()
-* [Parkinson's Progression]()
-* [Parkinson's Personalized]()
-
-We'll maintain a growing list of well documented examples developed by our community members here. Please open a pull request to feature your own:
-
-**Parkinson's Diagnosis**
-  * [Early Detection]()
-
- 
-  
+Metadata-Version: 2.1
+Name: omneer
+Version: 0.14
+Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
+Home-page: http://docs.omneer.xyz
+Author: William Blair
+Author-email: william.blair0708@gmail.com
+License: MIT
+Description: <div align="center">
+        
+        # Omneer SDK
+        
+        Omneer SDK is a state-of-the-art toolkit designed for the development and deployment of AI and machine learning powered personalized medicine applications in the neuroscience field. The SDK, with its Python-centric approach, provides an easy-to-use platform for developers to create and interact with their applications.
+        
+        Fueled by Airflow, a dynamic and highly scalable workflow orchestration engine known for its efficiency and flexibility, Omneer SDK ensures seamless processing and management of complex data workflows. Airflow's Directed Acyclic Graph (DAG) approach ensures atomicity at a task level, allowing for a comprehensive and orderly execution of tasks.
+        
+        This SDK further enhances workflow execution with containerization options, offering independence in task scheduling and a vast array of scalable computing resources. As such, the Omneer SDK represents a perfect convergence of neuroscience, personalized medicine, and cutting-edge technology, promising a new era of advanced and personalized healthcare solutions.
+        
+        [Discord Community Community]() • [Docs](https://docs.omneer.xyz) • [Installation](#installation) •
+        [Quickstart](#configuration) • [Omneer](https://omneer.xyz)
+        
+        </div>
+        
+        Utilizing the Omneer SDK, developers can deliver:
+        
+        - Personalized AI and machine learning tools
+        - Advanced disease progression diagnosis and tracking
+        - Creation of digital twins for individualized healthcare
+        - Instant no-code interfaces for rapid deployment
+        - High-performing, reliable cloud infrastructure
+        - Flexibility to define resources (CPU, GPU, etc.) for serverless execution
+        
+        - Omneer SDK continues to be a ground-breaking platform for personalized healthcare solutions. Browse our collection of existing and actively maintained solutions at [Omneer Community]().
+        
+        ### Getting Started
+        
+        See the SDK in action by following the steps below to register your first workflow with Omneer.
+        
+        First, install omneer through `pip`.
+        
+        ```
+        $ pip install omneer
+        ```
+        
+        Then, create some boilerplate code for your new workflow.
+        
+        ```
+        $ omneer init diagnosis
+        ```
+        
+        The registration process, which could take a few minutes depending on your network connection, involves building a Docker image with your workflow code, serializing the code, registering it with your Omneer account, and pushing the Docker image to a managed container registry.
+        
+        Upon successful registration, your new workflow should be visible in your Omneer Console.
+        
+        For issues with registration or other queries, please raise an issue on GitHub.
+        
+        ---
+        
+        ### Installation
+        
+        Omneer SDK is distributed via pip. We recommend installing it in a clean virtual environment for the best user experience.
+        
+        Virtualenv is our recommended tool for creating isolated Python environments.
+        
+        [Virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) is recommended.
+        
+        ```
+        pip install omneer
+        ```
+        
+        ### Examples
+        
+        [Omneer Examples]() features list of well-curated workflows developed by the Omneer team. 
+        * [Parkinson's Diagnosis]()
+        * [Parkinson's Progression]()
+        * [Parkinson's Personalized]()
+        
+        We'll maintain a growing list of well documented examples developed by our community members here. Please open a pull request to feature your own:
+        
+        **Parkinson's Diagnosis**
+          * [Early Detection]()
+        
+         
+          
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
```

### Comparing `omneer-0.13/omneer/model/deeplearning/mlp.py` & `omneer-0.14/omneer/model/deeplearning/mlp.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/model/train.py` & `omneer-0.14/omneer/model/train.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/processing/bootstrap.py` & `omneer-0.14/omneer/processing/bootstrap.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/processing/main.py` & `omneer-0.14/omneer/processing/main.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/processing/misc.py` & `omneer-0.14/omneer/processing/misc.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/visualization/graph/grid_search_.py` & `omneer-0.14/omneer/visualization/graph/grid_search_.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/visualization/graph/plot_summary.py` & `omneer-0.14/omneer/visualization/graph/plot_summary.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/visualization/graph/plot_swarm.py` & `omneer-0.14/omneer/visualization/graph/plot_swarm.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/visualization/graph/shap_3_correlation.py` & `omneer-0.14/omneer/visualization/graph/shap_3_correlation.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/visualization/graph/shap_analysis__.py` & `omneer-0.14/omneer/visualization/graph/shap_analysis__.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer/visualization/plot.py` & `omneer-0.14/omneer/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `omneer-0.13/omneer.egg-info/PKG-INFO` & `omneer-0.14/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 Metadata-Version: 2.1
 Name: omneer
-Version: 0.13
+Version: 0.14
 Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
 Home-page: http://docs.omneer.xyz
 Author: William Blair
 Author-email: william.blair0708@gmail.com
 License: MIT
+Description: <div align="center">
+        
+        # Omneer SDK
+        
+        Omneer SDK is a state-of-the-art toolkit designed for the development and deployment of AI and machine learning powered personalized medicine applications in the neuroscience field. The SDK, with its Python-centric approach, provides an easy-to-use platform for developers to create and interact with their applications.
+        
+        Fueled by Airflow, a dynamic and highly scalable workflow orchestration engine known for its efficiency and flexibility, Omneer SDK ensures seamless processing and management of complex data workflows. Airflow's Directed Acyclic Graph (DAG) approach ensures atomicity at a task level, allowing for a comprehensive and orderly execution of tasks.
+        
+        This SDK further enhances workflow execution with containerization options, offering independence in task scheduling and a vast array of scalable computing resources. As such, the Omneer SDK represents a perfect convergence of neuroscience, personalized medicine, and cutting-edge technology, promising a new era of advanced and personalized healthcare solutions.
+        
+        [Discord Community Community]() • [Docs](https://docs.omneer.xyz) • [Installation](#installation) •
+        [Quickstart](#configuration) • [Omneer](https://omneer.xyz)
+        
+        </div>
+        
+        Utilizing the Omneer SDK, developers can deliver:
+        
+        - Personalized AI and machine learning tools
+        - Advanced disease progression diagnosis and tracking
+        - Creation of digital twins for individualized healthcare
+        - Instant no-code interfaces for rapid deployment
+        - High-performing, reliable cloud infrastructure
+        - Flexibility to define resources (CPU, GPU, etc.) for serverless execution
+        
+        - Omneer SDK continues to be a ground-breaking platform for personalized healthcare solutions. Browse our collection of existing and actively maintained solutions at [Omneer Community]().
+        
+        ### Getting Started
+        
+        See the SDK in action by following the steps below to register your first workflow with Omneer.
+        
+        First, install omneer through `pip`.
+        
+        ```
+        $ pip install omneer
+        ```
+        
+        Then, create some boilerplate code for your new workflow.
+        
+        ```
+        $ omneer init diagnosis
+        ```
+        
+        The registration process, which could take a few minutes depending on your network connection, involves building a Docker image with your workflow code, serializing the code, registering it with your Omneer account, and pushing the Docker image to a managed container registry.
+        
+        Upon successful registration, your new workflow should be visible in your Omneer Console.
+        
+        For issues with registration or other queries, please raise an issue on GitHub.
+        
+        ---
+        
+        ### Installation
+        
+        Omneer SDK is distributed via pip. We recommend installing it in a clean virtual environment for the best user experience.
+        
+        Virtualenv is our recommended tool for creating isolated Python environments.
+        
+        [Virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) is recommended.
+        
+        ```
+        pip install omneer
+        ```
+        
+        ### Examples
+        
+        [Omneer Examples]() features list of well-curated workflows developed by the Omneer team. 
+        * [Parkinson's Diagnosis]()
+        * [Parkinson's Progression]()
+        * [Parkinson's Personalized]()
+        
+        We'll maintain a growing list of well documented examples developed by our community members here. Please open a pull request to feature your own:
+        
+        **Parkinson's Diagnosis**
+          * [Early Detection]()
+        
+         
+          
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-
-<div align="center">
-
-# Omneer SDK
-
-Omneer SDK is a state-of-the-art toolkit designed for the development and deployment of AI and machine learning powered personalized medicine applications in the neuroscience field. The SDK, with its Python-centric approach, provides an easy-to-use platform for developers to create and interact with their applications.
-
-Fueled by Airflow, a dynamic and highly scalable workflow orchestration engine known for its efficiency and flexibility, Omneer SDK ensures seamless processing and management of complex data workflows. Airflow's Directed Acyclic Graph (DAG) approach ensures atomicity at a task level, allowing for a comprehensive and orderly execution of tasks.
-
-This SDK further enhances workflow execution with containerization options, offering independence in task scheduling and a vast array of scalable computing resources. As such, the Omneer SDK represents a perfect convergence of neuroscience, personalized medicine, and cutting-edge technology, promising a new era of advanced and personalized healthcare solutions.
-
-[Discord Community Community]() • [Docs](https://docs.omneer.xyz) • [Installation](#installation) •
-[Quickstart](#configuration) • [Omneer](https://omneer.xyz)
-
-</div>
-
-Utilizing the Omneer SDK, developers can deliver:
-
-- Personalized AI and machine learning tools
-- Advanced disease progression diagnosis and tracking
-- Creation of digital twins for individualized healthcare
-- Instant no-code interfaces for rapid deployment
-- High-performing, reliable cloud infrastructure
-- Flexibility to define resources (CPU, GPU, etc.) for serverless execution
-
-- Omneer SDK continues to be a ground-breaking platform for personalized healthcare solutions. Browse our collection of existing and actively maintained solutions at [Omneer Community]().
-
-### Getting Started
-
-See the SDK in action by following the steps below to register your first workflow with Omneer.
-
-First, install omneer through `pip`.
-
-```
-$ python3 pip install omneer
-```
-
-Then, create some boilerplate code for your new workflow.
-
-```
-$ omneer init diagnosis
-```
-
-The registration process, which could take a few minutes depending on your network connection, involves building a Docker image with your workflow code, serializing the code, registering it with your Omneer account, and pushing the Docker image to a managed container registry.
-
-Upon successful registration, your new workflow should be visible in your Omneer Console.
-
-For issues with registration or other queries, please raise an issue on GitHub.
-
----
-
-### Installation
-
-Omneer SDK is distributed via pip. We recommend installing it in a clean virtual environment for the best user experience.
-
-Virtualenv is our recommended tool for creating isolated Python environments.
-
-[Virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) is recommended.
-
-```
-pip install omneer
-```
-
-### Examples
-
-[Omneer Examples]() features list of well-curated workflows developed by the Omneer team. 
-* [Parkinson's Diagnosis]()
-* [Parkinson's Progression]()
-* [Parkinson's Personalized]()
-
-We'll maintain a growing list of well documented examples developed by our community members here. Please open a pull request to feature your own:
-
-**Parkinson's Diagnosis**
-  * [Early Detection]()
-
- 
-
```

### Comparing `omneer-0.13/omneer.egg-info/SOURCES.txt` & `omneer-0.14/omneer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omneer-0.13/setup.py` & `omneer-0.14/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='omneer',
-    version='0.13',
+    version='0.14',
     packages=find_packages(include=['omneer', 'omneer.*']),
     url='http://docs.omneer.xyz',
     license='MIT',
     author='William Blair',
     author_email='william.blair0708@gmail.com',
     description='Advanced personalized medicine diagnostics for neurodegenerative disorders',
     long_description=open('README.md').read(),
```


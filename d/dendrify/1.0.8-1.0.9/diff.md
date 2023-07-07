# Comparing `tmp/dendrify-1.0.8.tar.gz` & `tmp/dendrify-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dendrify-1.0.8.tar", last modified: Wed Jan 11 10:22:02 2023, max compression
+gzip compressed data, was "dendrify-1.0.9.tar", last modified: Fri Jul  7 13:17:28 2023, max compression
```

## Comparing `dendrify-1.0.8.tar` & `dendrify-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:22:02.855873 dendrify-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-11 10:21:54.000000 dendrify-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-11 10:22:02.855873 dendrify-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-01-11 10:21:54.000000 dendrify-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:22:02.855873 dendrify-1.0.8/dendrify/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-11 10:21:54.000000 dendrify-1.0.8/dendrify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27172 2023-01-11 10:21:54.000000 dendrify-1.0.8/dendrify/compartment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-01-11 10:21:54.000000 dendrify-1.0.8/dendrify/ephysproperties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-01-11 10:21:54.000000 dendrify-1.0.8/dendrify/equations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-01-11 10:21:54.000000 dendrify-1.0.8/dendrify/neuronmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 10:22:02.855873 dendrify-1.0.8/dendrify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-11 10:22:02.000000 dendrify-1.0.8/dendrify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-11 10:22:02.000000 dendrify-1.0.8/dendrify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 10:22:02.000000 dendrify-1.0.8/dendrify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-11 10:22:02.000000 dendrify-1.0.8/dendrify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-11 10:22:02.000000 dendrify-1.0.8/dendrify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 10:22:02.855873 dendrify-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-11 10:21:54.000000 dendrify-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:17:28.185462 dendrify-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 13:17:15.000000 dendrify-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-07 13:17:28.185462 dendrify-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-07 13:17:15.000000 dendrify-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:17:28.181461 dendrify-1.0.9/dendrify/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 13:17:15.000000 dendrify-1.0.9/dendrify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27172 2023-07-07 13:17:15.000000 dendrify-1.0.9/dendrify/compartment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-07 13:17:15.000000 dendrify-1.0.9/dendrify/ephysproperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-07 13:17:15.000000 dendrify-1.0.9/dendrify/equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-07-07 13:17:15.000000 dendrify-1.0.9/dendrify/neuronmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:17:28.185462 dendrify-1.0.9/dendrify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-07 13:17:28.000000 dendrify-1.0.9/dendrify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 13:17:28.000000 dendrify-1.0.9/dendrify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:17:28.000000 dendrify-1.0.9/dendrify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 13:17:28.000000 dendrify-1.0.9/dendrify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 13:17:28.000000 dendrify-1.0.9/dendrify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:17:28.185462 dendrify-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-07 13:17:15.000000 dendrify-1.0.9/setup.py
```

### Comparing `dendrify-1.0.8/LICENSE` & `dendrify-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dendrify-1.0.8/README.rst` & `dendrify-1.0.9/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -10,40 +10,22 @@
   :target: https://dendrify.readthedocs.io/en/stable/?badge=stable
   :alt: Documentation Status
 
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg
         :target: CODE_OF_CONDUCT.md
         :alt: Contributor Covenant
 
-Although neuronal dendrites greatly influence how single neurons process incoming
-information, their role in network-level functions remain largely unexplored.
-Current SNNs are usually quite simplistic, overlooking essential dendritic
-properties. Conversely, circuit models with morphologically detailed neuron
-models are computationally costly, thus impractical for large-network
-simulations.
-
-To bridge the gap between these two, we introduce Dendrify, a free,
-open-source Python package compatible with the
-`Brian 2 simulator <https://brian2.readthedocs.io/en/stable/>`_. Dendrify,
-through simple commands, automatically generates reduced compartmental neuron
-models with simplified yet biologically relevant dendritic and synaptic
-integrative properties. Such models strike a good balance between flexibility,
-performance, and biological accuracy, allowing us to explore dendritic
-contributions to network-level functions.
+Although neuronal dendrites greatly influence how single neurons process incoming information, their role in network-level functions remain largely unexplored. Current SNNs are usually quite simplistic, overlooking essential dendritic properties. Conversely, circuit models with morphologically detailed neuron models are computationally costly, thus impractical for large-network simulations.
+
+To bridge the gap between these two, we introduce Dendrify, a free, open-source Python package compatible with the `Brian 2 simulator <https://brian2.readthedocs.io/en/stable/>`_. Dendrify, through simple commands, automatically generates reduced compartmental neuron models with simplified yet biologically relevant dendritic and synaptic integrative properties. Such models strike a good balance between flexibility, performance, and biological accuracy, allowing us to explore dendritic contributions to network-level functions.
 
 .. image:: docs_sphinx/source/_static/intro.png
-   :width: 75 %
+   :width: 70 %
    :align: center
 
-.. tip::
-   If you use Dendrify for your published research, we kindly ask you to cite our
-   article:|br|
-   **Introducing the Dendrify framework for incorporating dendrites to spiking neural networks** |br|
-   M Pagkalos, S Chavlis, P Poirazi |br|
-   DOI: https://doi.org/10.1038/s41467-022-35747-8 |br|
-
-Documentation for Dendrify can be found at https://dendrify.readthedocs.io/en/latest/
+If you use Dendrify for your published research, we kindly ask you to cite our article:
 
+Pagkalos, M., Chavlis, S., & Poirazi, P. (2023). Introducing the Dendrify framework for incorporating dendrites to spiking neural networks. Nature Communications, 14(1), 131. https://doi.org/10.1038/s41467-022-35747-8
 
-.. |br| raw:: html
+Documentation for Dendrify can be found at https://dendrify.readthedocs.io/en/latest/
 
-     <br>
+The project presentation for the INCF/OCNS Software Working Group is available `on google drive <https://docs.google.com/presentation/d/1LUUh2ja3YSHcmByU0Vyn7vcDEnDq6fWfVxFfuK8FzE0/edit?usp=sharing>`_ and an interactive notebook with a short demo `on google colab <https://colab.research.google.com/drive/1-bGp15eWfjNuF7ETCNSsL3ovOanS_R_7?usp=sharing>`_.
```

### Comparing `dendrify-1.0.8/dendrify/compartment.py` & `dendrify-1.0.9/dendrify/compartment.py`

 * *Files identical despite different names*

### Comparing `dendrify-1.0.8/dendrify/ephysproperties.py` & `dendrify-1.0.9/dendrify/ephysproperties.py`

 * *Files identical despite different names*

### Comparing `dendrify-1.0.8/dendrify/equations.py` & `dendrify-1.0.9/dendrify/equations.py`

 * *Files identical despite different names*

### Comparing `dendrify-1.0.8/dendrify/neuronmodel.py` & `dendrify-1.0.9/dendrify/neuronmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from typing import List, Optional, Tuple, Union
 
 import __main__ as main
 from brian2 import NeuronGroup
-from brian2.units import Quantity, mV
+from brian2.units import Quantity, mV, mvolt
 
 from .compartment import Compartment, Dendrite, Soma
 
 
 class NeuronModel:
     """
     Creates a multicompartmental neuron model by connecting individual
```

### Comparing `dendrify-1.0.8/setup.py` & `dendrify-1.0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import find_packages, setup
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 DESCRIPTION = 'A package for adding dendrites to SNNs'
-LONG_DESCRIPTION = 'A package for adding dendrites to SNNs in Brian 2'
+with open("README.rst") as f:
+    LONG_DESCRIPTION = f.read()
 
 # Setting up
 setup(
     name="dendrify",
     version=VERSION,
     author="Michalis Pagkalos",
     author_email="<mpagkalos93@gmail.com>",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst; charset=UTF-8",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['brian2==2.5.1'],
     keywords=['python', 'brian2', 'dendrites', 'SNNs', 'network models'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
```


# Comparing `tmp/ElementEmbeddings-0.1.1.tar.gz` & `tmp/ElementEmbeddings-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ElementEmbeddings-0.1.1.tar", last modified: Wed Jul  5 16:30:32 2023, max compression
+gzip compressed data, was "ElementEmbeddings-0.2.0.tar", last modified: Fri Jul  7 16:35:27 2023, max compression
```

## Comparing `ElementEmbeddings-0.1.1.tar` & `ElementEmbeddings-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.387287 ElementEmbeddings-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.391287 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 16:30:32.000000 ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.391287 ElementEmbeddings-0.1.1/src/elementembeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    33383 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/src/elementembeddings/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/element_group.json
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/element_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/ordered_periodic.txt
--rw-r--r--   0 runner    (1001) docker     (123)   199959 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)   259692 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/periodic-table-lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/magpie.csv
--rw-r--r--   0 runner    (1001) docker     (123)    44406 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/magpie_sc.json
--rw-r--r--   0 runner    (1001) docker     (123)   476891 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/mat2vec.csv
--rw-r--r--   0 runner    (1001) docker     (123)   449163 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/matscholar-embedding.json
--rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/megnet16.json
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/mod_petti.json
--rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/oliynyk.json
--rw-r--r--   0 runner    (1001) docker     (123)    77531 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/oliynyk_sc.json
--rw-r--r--   0 runner    (1001) docker     (123)   487394 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/random_200.csv
--rw-r--r--   0 runner    (1001) docker     (123)   488226 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/random_200_new.csv
--rw-r--r--   0 runner    (1001) docker     (123)   356292 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/data/skipatom_20201009_induced.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/src/elementembeddings/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:30:32.395288 ElementEmbeddings-0.1.1/src/elementembeddings/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-05 16:30:21.000000 ElementEmbeddings-0.1.1/src/elementembeddings/utils/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.988227 ElementEmbeddings-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.992227 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 16:35:26.000000 ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.992227 ElementEmbeddings-0.2.0/src/elementembeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33496 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/src/elementembeddings/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/element_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/element_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/ordered_periodic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   199959 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)   259692 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/periodic-table-lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/magpie.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44406 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/magpie_sc.json
+-rw-r--r--   0 runner    (1001) docker     (123)   476891 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/mat2vec.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   449163 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/matscholar-embedding.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32012 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/megnet16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/mod_petti.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/oliynyk.json
+-rw-r--r--   0 runner    (1001) docker     (123)    77531 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/oliynyk_sc.json
+-rw-r--r--   0 runner    (1001) docker     (123)   487394 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/random_200.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   488226 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/random_200_new.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   356292 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/data/skipatom_20201009_induced.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/src/elementembeddings/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:35:26.996227 ElementEmbeddings-0.2.0/src/elementembeddings/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-07 16:35:17.000000 ElementEmbeddings-0.2.0/src/elementembeddings/utils/math.py
```

### Comparing `ElementEmbeddings-0.1.1/LICENSE.md` & `ElementEmbeddings-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/PKG-INFO` & `ElementEmbeddings-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ElementEmbeddings
-Version: 0.1.1
+Version: 0.2.0
 Summary: Element Embeddings
 Author: Anthony O. Onwuli
 Author-email: anthony.onwuli16@imperial.ac.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE.md
 
 ElementEmbeddings
 ====
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -27,15 +29,14 @@
 [![CI Status](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/WMD-group/ElementEmbeddings/branch/main/graph/badge.svg?token=OCMIM5SHL0)](https://codecov.io/gh/WMD-group/ElementEmbeddings)
 [![DOI](https://zenodo.org/badge/493285385.svg)](https://zenodo.org/badge/latestdoi/493285385)
 [![PyPI](https://img.shields.io/pypi/v/ElementEmbeddings)](https://pypi.org/project/ElementEmbeddings/)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://wmd-group.github.io/ElementEmbeddings/)
 ![python version](https://img.shields.io/pypi/pyversions/elementembeddings)
 
-
 The **Element Embeddings** package provides high-level tools for analysing elemental
 embeddings data. This primarily involves visualising the correlation between
 embedding schemes using different statistical measures.
 
 Motivation
 --------
 
@@ -52,22 +53,26 @@
 --------
 
 ElementEmbeddings's main feature, the Embedding class is accessible by
 importing the class.
 
 Installation
 --------
+
 The latest stable release can be installed via pip using:
+
 ```bash
 pip install ElementEmbeddings
 ```
-The latest version can be installed using:
+
+For installing the development or documentation dependencies via pip:
 
 ```bash
-pip install git+git://github.com/WMD-group/ElementEmbeddings.git
+pip install "ElementEmbeddings[dev]"
+pip install "ElementEmbeddings[docs]"
 ```
 
 For development, you can clone the repository and install the package in editable mode.
 To clone the repository and make a local installation, run the following commands:
 
 ```bash
 git clone https://github.com/WMD-group/ElementEmbeddings.git
@@ -95,8 +100,7 @@
 ```python
 # Print out some of the properties of the ElementEmbeddings class
 >>> print(f'The magpie representation has embeddings of dimension {magpie.dim}') 
 >>> print(magpie.element_list) # prints out all the elements considered for this representation
 The magpie representation has embeddings of dimension 22
 ['H', 'He', 'Li', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K', 'Ca', 'Sc', 'Ti', 'V', 'Cr', 'Mn', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr', 'Rb', 'Sr', 'Y', 'Zr', 'Nb', 'Mo', 'Tc', 'Ru', 'Rh', 'Pd', 'Ag', 'Cd', 'In', 'Sn', 'Sb', 'Te', 'I', 'Xe', 'Cs', 'Ba', 'La', 'Ce', 'Pr', 'Nd', 'Pm', 'Sm', 'Eu', 'Gd', 'Tb', 'Dy', 'Ho', 'Er', 'Tm', 'Yb', 'Lu', 'Hf', 'Ta', 'W', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl', 'Pb', 'Bi', 'Po', 'At', 'Rn', 'Fr', 'Ra', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm', 'Bk']
 ```
-
```

### Comparing `ElementEmbeddings-0.1.1/README.md` & `ElementEmbeddings-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 [![CI Status](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/WMD-group/ElementEmbeddings/branch/main/graph/badge.svg?token=OCMIM5SHL0)](https://codecov.io/gh/WMD-group/ElementEmbeddings)
 [![DOI](https://zenodo.org/badge/493285385.svg)](https://zenodo.org/badge/latestdoi/493285385)
 [![PyPI](https://img.shields.io/pypi/v/ElementEmbeddings)](https://pypi.org/project/ElementEmbeddings/)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://wmd-group.github.io/ElementEmbeddings/)
 ![python version](https://img.shields.io/pypi/pyversions/elementembeddings)
 
-
 The **Element Embeddings** package provides high-level tools for analysing elemental
 embeddings data. This primarily involves visualising the correlation between
 embedding schemes using different statistical measures.
 
 Motivation
 --------
 
@@ -33,22 +32,26 @@
 --------
 
 ElementEmbeddings's main feature, the Embedding class is accessible by
 importing the class.
 
 Installation
 --------
+
 The latest stable release can be installed via pip using:
+
 ```bash
 pip install ElementEmbeddings
 ```
-The latest version can be installed using:
+
+For installing the development or documentation dependencies via pip:
 
 ```bash
-pip install git+git://github.com/WMD-group/ElementEmbeddings.git
+pip install "ElementEmbeddings[dev]"
+pip install "ElementEmbeddings[docs]"
 ```
 
 For development, you can clone the repository and install the package in editable mode.
 To clone the repository and make a local installation, run the following commands:
 
 ```bash
 git clone https://github.com/WMD-group/ElementEmbeddings.git
@@ -76,8 +79,7 @@
 ```python
 # Print out some of the properties of the ElementEmbeddings class
 >>> print(f'The magpie representation has embeddings of dimension {magpie.dim}') 
 >>> print(magpie.element_list) # prints out all the elements considered for this representation
 The magpie representation has embeddings of dimension 22
 ['H', 'He', 'Li', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K', 'Ca', 'Sc', 'Ti', 'V', 'Cr', 'Mn', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr', 'Rb', 'Sr', 'Y', 'Zr', 'Nb', 'Mo', 'Tc', 'Ru', 'Rh', 'Pd', 'Ag', 'Cd', 'In', 'Sn', 'Sb', 'Te', 'I', 'Xe', 'Cs', 'Ba', 'La', 'Ce', 'Pr', 'Nd', 'Pm', 'Sm', 'Eu', 'Gd', 'Tb', 'Dy', 'Ho', 'Er', 'Tm', 'Yb', 'Lu', 'Hf', 'Ta', 'W', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl', 'Pb', 'Bi', 'Po', 'At', 'Rn', 'Fr', 'Ra', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm', 'Bk']
 ```
-
```

### Comparing `ElementEmbeddings-0.1.1/setup.py` & `ElementEmbeddings-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup script for AtomicEmbeddings."""
 import os
 
 from setuptools import find_namespace_packages, setup
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 
-VERSION = "0.1.1"
+VERSION = "0.2.0"
 DESCRIPTION = "Element Embeddings"
 with open(os.path.join(module_dir, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 
 # Setting up
 setup(
@@ -33,14 +33,34 @@
         "pymatgen>2022.9.21",
         "seaborn==0.12.1",
         "matplotlib==3.7.1",
         "scikit-learn==1.3.0",
         "umap-learn==0.5.3",
         "adjustText==0.8",
     ],
+    extras_require={
+        "dev": [
+            "pre-commit==2.20.0",
+            "black==23.3.0",
+            "isort==5.12.0",
+            "pytest==7.2.1",
+            "pytest-subtests==0.10.0",
+            "nbqa==1.5.3",
+            "pyupgrade==3.3.1",
+            "flake8==6.0.0",
+            "autopep8==2.0.1",
+            "pytest-cov==4.1.0",
+        ],
+        "docs": [
+            "mkdocs==1.4.3",
+            "mkdocs-material==9.1.17",
+            "mkdocstrings ==0.21.2",
+            "mkdocstrings-python == 1.0.0",
+        ],
+    },
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
```

### Comparing `ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/PKG-INFO` & `ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ElementEmbeddings
-Version: 0.1.1
+Version: 0.2.0
 Summary: Element Embeddings
 Author: Anthony O. Onwuli
 Author-email: anthony.onwuli16@imperial.ac.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE.md
 
 ElementEmbeddings
 ====
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -27,15 +29,14 @@
 [![CI Status](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/ElementEmbeddings/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/WMD-group/ElementEmbeddings/branch/main/graph/badge.svg?token=OCMIM5SHL0)](https://codecov.io/gh/WMD-group/ElementEmbeddings)
 [![DOI](https://zenodo.org/badge/493285385.svg)](https://zenodo.org/badge/latestdoi/493285385)
 [![PyPI](https://img.shields.io/pypi/v/ElementEmbeddings)](https://pypi.org/project/ElementEmbeddings/)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://wmd-group.github.io/ElementEmbeddings/)
 ![python version](https://img.shields.io/pypi/pyversions/elementembeddings)
 
-
 The **Element Embeddings** package provides high-level tools for analysing elemental
 embeddings data. This primarily involves visualising the correlation between
 embedding schemes using different statistical measures.
 
 Motivation
 --------
 
@@ -52,22 +53,26 @@
 --------
 
 ElementEmbeddings's main feature, the Embedding class is accessible by
 importing the class.
 
 Installation
 --------
+
 The latest stable release can be installed via pip using:
+
 ```bash
 pip install ElementEmbeddings
 ```
-The latest version can be installed using:
+
+For installing the development or documentation dependencies via pip:
 
 ```bash
-pip install git+git://github.com/WMD-group/ElementEmbeddings.git
+pip install "ElementEmbeddings[dev]"
+pip install "ElementEmbeddings[docs]"
 ```
 
 For development, you can clone the repository and install the package in editable mode.
 To clone the repository and make a local installation, run the following commands:
 
 ```bash
 git clone https://github.com/WMD-group/ElementEmbeddings.git
@@ -95,8 +100,7 @@
 ```python
 # Print out some of the properties of the ElementEmbeddings class
 >>> print(f'The magpie representation has embeddings of dimension {magpie.dim}') 
 >>> print(magpie.element_list) # prints out all the elements considered for this representation
 The magpie representation has embeddings of dimension 22
 ['H', 'He', 'Li', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K', 'Ca', 'Sc', 'Ti', 'V', 'Cr', 'Mn', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr', 'Rb', 'Sr', 'Y', 'Zr', 'Nb', 'Mo', 'Tc', 'Ru', 'Rh', 'Pd', 'Ag', 'Cd', 'In', 'Sn', 'Sb', 'Te', 'I', 'Xe', 'Cs', 'Ba', 'La', 'Ce', 'Pr', 'Nd', 'Pm', 'Sm', 'Eu', 'Gd', 'Tb', 'Dy', 'Ho', 'Er', 'Tm', 'Yb', 'Lu', 'Hf', 'Ta', 'W', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl', 'Pb', 'Bi', 'Po', 'At', 'Rn', 'Fr', 'Ra', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm', 'Bk']
 ```
-
```

### Comparing `ElementEmbeddings-0.1.1/src/ElementEmbeddings.egg-info/SOURCES.txt` & `ElementEmbeddings-0.2.0/src/ElementEmbeddings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/composition.py` & `ElementEmbeddings-0.2.0/src/elementembeddings/composition.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/core.py` & `ElementEmbeddings-0.2.0/src/elementembeddings/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,19 +147,14 @@
                 # Remove 'Null' key from megnet embedding
                 del embedding_data["Null"]
 
             elif embedding_name in _cbfv_names_others:
                 _json = path.join(data_directory, _cbfv_files[embedding_name])
                 with open(_json) as f:
                     embedding_data = json.load(f)
-
-            # Load a json file from a file specified in the input
-            else:
-                with open(embedding_name) as f:
-                    embedding_data = json.load(f)
         else:
             raise (
                 ValueError(
                     f"{embedding_name} not in the data directory or not in directory."
                 )
             )
         return Embedding(embedding_data, embedding_name)
@@ -849,14 +844,18 @@
             figsize (tuple): A tuple of (width, height)
             points_size (float): The marker size
 
         Returns:
             ax (matplotlib.axes.Axes): An Axes object with the PCA plot
 
         """
+        warnings.warn(
+            "This method is deprecated and will be removed in a future release. ",
+            DeprecationWarning,
+        )
         embeddings_array = np.array(list(self.embeddings.values()))
         element_array = np.array(self.element_list)
 
         pca = decomposition.PCA(n_components=2)  # project to 2 dimensions
 
         pca.fit(embeddings_array)
         X = pca.transform(embeddings_array)
@@ -909,14 +908,18 @@
             points_size (float): The marker size
 
         Returns:
             ax (matplotlib.axes.Axes): An Axes object with the PCA plot
 
 
         """
+        warnings.warn(
+            "This method is deprecated and will be removed in a future release. ",
+            DeprecationWarning,
+        )
         embeddings_array = np.array(list(self.embeddings.values()))
         element_array = np.array(self.element_list)
 
         tsne = TSNE(n_components)
         tsne_result = tsne.fit_transform(embeddings_array)
 
         tsne_df = pd.DataFrame(
```

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/element_group.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/element_group.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/element_symbols.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/element_symbols.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/periodic-table-lookup-symbols.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/element_data/periodic-table-lookup.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/element_data/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/magpie.csv` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/magpie.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/magpie_sc.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/magpie_sc.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/mat2vec.csv` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/mat2vec.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/matscholar-embedding.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/matscholar-embedding.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/megnet16.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/megnet16.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/mod_petti.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/mod_petti.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/oliynyk.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/oliynyk.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/oliynyk_sc.json` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/oliynyk_sc.json`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/random_200.csv` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/random_200.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/random_200_new.csv` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/random_200_new.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/data/skipatom_20201009_induced.csv` & `ElementEmbeddings-0.2.0/src/elementembeddings/data/skipatom_20201009_induced.csv`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/plotter.py` & `ElementEmbeddings-0.2.0/src/elementembeddings/plotter.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/tests/test_utils.py` & `ElementEmbeddings-0.2.0/src/elementembeddings/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ElementEmbeddings-0.1.1/src/elementembeddings/utils/math.py` & `ElementEmbeddings-0.2.0/src/elementembeddings/utils/math.py`

 * *Files identical despite different names*


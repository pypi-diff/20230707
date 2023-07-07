# Comparing `tmp/pygmtools-0.3.8a4.tar.gz` & `tmp/pygmtools-0.3.8a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.3.8a4.tar", last modified: Fri Jul  7 12:56:58 2023, max compression
+gzip compressed data, was "pygmtools-0.3.8a5.tar", last modified: Fri Jul  7 17:10:52 2023, max compression
```

## Comparing `pygmtools-0.3.8a4.tar` & `pygmtools-0.3.8a5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 12:56:58.062524 pygmtools-0.3.8a4/
--rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a4/LICENSE
--rw-rw-rw-   0        0        0       18 2023-05-03 08:07:01.000000 pygmtools-0.3.8a4/MANIFEST.in
--rw-rw-rw-   0        0        0    13827 2023-07-07 12:56:58.062524 pygmtools-0.3.8a4/PKG-INFO
--rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 12:56:58.057419 pygmtools-0.3.8a4/pygmtools/
--rw-rw-rw-   0        0        0     2120 2023-07-07 12:56:01.000000 pygmtools-0.3.8a4/pygmtools/__init__.py
--rw-rw-rw-   0        0        0    58368 2023-07-07 12:56:57.000000 pygmtools-0.3.8a4/pygmtools/a_star.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    27000 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/benchmark.py
--rw-rw-rw-   0        0        0    58666 2023-07-07 12:42:20.000000 pygmtools-0.3.8a4/pygmtools/classic_solvers.py
--rw-rw-rw-   0        0        0    59231 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/dataset.py
--rw-rw-rw-   0        0        0     3112 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/dataset_config.py
--rw-rw-rw-   0        0        0    58908 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/jittor_backend.py
--rw-rw-rw-   0        0        0    12371 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/jittor_modules.py
--rw-rw-rw-   0        0        0    77128 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/linear_solvers.py
--rw-rw-rw-   0        0        0    21736 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/mindspore_backend.py
--rw-rw-rw-   0        0        0    44038 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/multi_graph_solvers.py
--rw-rw-rw-   0        0        0    70477 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/neural_solvers.py
--rw-rw-rw-   0        0        0    60669 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/numpy_backend.py
--rw-rw-rw-   0        0        0    15282 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/numpy_modules.py
--rw-rw-rw-   0        0        0    57860 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/paddle_backend.py
--rw-rw-rw-   0        0        0    11899 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/paddle_modules.py
--rw-rw-rw-   0        0        0    15443 2023-07-07 12:38:50.000000 pygmtools-0.3.8a4/pygmtools/pytorch_astar_modules.py
--rw-rw-rw-   0        0        0    74579 2023-07-07 12:56:18.000000 pygmtools-0.3.8a4/pygmtools/pytorch_backend.py
--rw-rw-rw-   0        0        0    12329 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/pytorch_modules.py
--rw-rw-rw-   0        0        0    23046 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/tensorflow_backend.py
--rw-rw-rw-   0        0        0      508 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/tensorflow_modules.py
--rw-rw-rw-   0        0        0    51707 2023-07-07 11:54:30.000000 pygmtools-0.3.8a4/pygmtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:56:58.059456 pygmtools-0.3.8a4/pygmtools.egg-info/
--rw-rw-rw-   0        0        0    13827 2023-07-07 12:56:57.000000 pygmtools-0.3.8a4/pygmtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      978 2023-07-07 12:56:58.000000 pygmtools-0.3.8a4/pygmtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 12:56:57.000000 pygmtools-0.3.8a4/pygmtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-07-07 12:56:57.000000 pygmtools-0.3.8a4/pygmtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 12:56:57.000000 pygmtools-0.3.8a4/pygmtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 12:56:58.062524 pygmtools-0.3.8a4/setup.cfg
--rw-rw-rw-   0        0        0     5818 2023-07-07 09:10:43.000000 pygmtools-0.3.8a4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:56:58.062524 pygmtools-0.3.8a4/tests/
--rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a4/tests/test_classic_solvers.py
--rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a4/tests/test_dataset.py
--rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a4/tests/test_misc.py
--rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a4/tests/test_multi_graph_solvers.py
--rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a4/tests/test_neural_solvers.py
--rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.193519 pygmtools-0.3.8a5/
+-rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/LICENSE
+-rw-rw-rw-   0        0        0    13827 2023-07-07 17:10:52.193519 pygmtools-0.3.8a5/PKG-INFO
+-rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.182234 pygmtools-0.3.8a5/pygmtools/
+-rw-rw-rw-   0        0        0     2120 2023-07-07 16:55:51.000000 pygmtools-0.3.8a5/pygmtools/__init__.py
+-rw-rw-rw-   0        0        0    27000 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/benchmark.py
+-rw-rw-rw-   0        0        0    58666 2023-07-07 12:42:20.000000 pygmtools-0.3.8a5/pygmtools/classic_solvers.py
+-rw-rw-rw-   0        0        0    59231 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/dataset.py
+-rw-rw-rw-   0        0        0     3112 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/dataset_config.py
+-rw-rw-rw-   0        0        0    58908 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/jittor_backend.py
+-rw-rw-rw-   0        0        0    12371 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/jittor_modules.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.187364 pygmtools-0.3.8a5/pygmtools/lib/
+-rw-rw-rw-   0        0        0  1138391 2023-07-02 08:40:47.000000 pygmtools-0.3.8a5/pygmtools/lib/a_star.tar.gz
+-rw-rw-rw-   0        0        0  3203980 2023-07-02 08:39:54.000000 pygmtools-0.3.8a5/pygmtools/lib/a_star.zip
+-rw-rw-rw-   0        0        0    77128 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/linear_solvers.py
+-rw-rw-rw-   0        0        0    21736 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/mindspore_backend.py
+-rw-rw-rw-   0        0        0    44038 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/multi_graph_solvers.py
+-rw-rw-rw-   0        0        0    70477 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/neural_solvers.py
+-rw-rw-rw-   0        0        0    60669 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/numpy_backend.py
+-rw-rw-rw-   0        0        0    15282 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/numpy_modules.py
+-rw-rw-rw-   0        0        0    57860 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/paddle_backend.py
+-rw-rw-rw-   0        0        0    11899 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/paddle_modules.py
+-rw-rw-rw-   0        0        0    15443 2023-07-07 12:38:50.000000 pygmtools-0.3.8a5/pygmtools/pytorch_astar_modules.py
+-rw-rw-rw-   0        0        0    74579 2023-07-07 12:56:18.000000 pygmtools-0.3.8a5/pygmtools/pytorch_backend.py
+-rw-rw-rw-   0        0        0    12329 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/pytorch_modules.py
+-rw-rw-rw-   0        0        0    23046 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/tensorflow_backend.py
+-rw-rw-rw-   0        0        0      508 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/tensorflow_modules.py
+-rw-rw-rw-   0        0        0    51707 2023-07-07 11:54:30.000000 pygmtools-0.3.8a5/pygmtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.184291 pygmtools-0.3.8a5/pygmtools.egg-info/
+-rw-rw-rw-   0        0        0    13827 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      982 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 17:10:52.000000 pygmtools-0.3.8a5/pygmtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 17:10:52.194543 pygmtools-0.3.8a5/setup.cfg
+-rw-rw-rw-   0        0        0     5922 2023-07-07 17:10:41.000000 pygmtools-0.3.8a5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 17:10:52.192516 pygmtools-0.3.8a5/tests/
+-rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a5/tests/test_classic_solvers.py
+-rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_misc.py
+-rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_multi_graph_solvers.py
+-rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_neural_solvers.py
+-rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a5/tests/test_utils.py
```

### Comparing `pygmtools-0.3.8a4/PKG-INFO` & `pygmtools-0.3.8a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a4
+Version: 0.3.8a5
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a4/README.md` & `pygmtools-0.3.8a5/README.md`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/__init__.py` & `pygmtools-0.3.8a5/pygmtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .benchmark import Benchmark
 from .linear_solvers import sinkhorn, hungarian
 from .classic_solvers import rrwm, sm, ipfp, a_star
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm
 import pygmtools.utils as utils
 BACKEND = 'numpy'
-__version__ = '0.3.8-alpha4'
+__version__ = '0.3.8-alpha5'
 __author__ = 'ThinkLab at SJTU'
 
 
 def env_report():
     """
     Print environment report
     """
```

### Comparing `pygmtools-0.3.8a4/pygmtools/benchmark.py` & `pygmtools-0.3.8a5/pygmtools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/classic_solvers.py` & `pygmtools-0.3.8a5/pygmtools/classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/dataset.py` & `pygmtools-0.3.8a5/pygmtools/dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/dataset_config.py` & `pygmtools-0.3.8a5/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/jittor_backend.py` & `pygmtools-0.3.8a5/pygmtools/jittor_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/jittor_modules.py` & `pygmtools-0.3.8a5/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/linear_solvers.py` & `pygmtools-0.3.8a5/pygmtools/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/mindspore_backend.py` & `pygmtools-0.3.8a5/pygmtools/mindspore_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/multi_graph_solvers.py` & `pygmtools-0.3.8a5/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/neural_solvers.py` & `pygmtools-0.3.8a5/pygmtools/neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/numpy_backend.py` & `pygmtools-0.3.8a5/pygmtools/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/numpy_modules.py` & `pygmtools-0.3.8a5/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/paddle_backend.py` & `pygmtools-0.3.8a5/pygmtools/paddle_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/paddle_modules.py` & `pygmtools-0.3.8a5/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/pytorch_astar_modules.py` & `pygmtools-0.3.8a5/pygmtools/pytorch_astar_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/pytorch_backend.py` & `pygmtools-0.3.8a5/pygmtools/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/pytorch_modules.py` & `pygmtools-0.3.8a5/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/tensorflow_backend.py` & `pygmtools-0.3.8a5/pygmtools/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools/utils.py` & `pygmtools-0.3.8a5/pygmtools/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.3.8a5/pygmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a4
+Version: 0.3.8a5
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a4/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.3.8a5/pygmtools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
-MANIFEST.in
 README.md
 setup.py
 pygmtools/__init__.py
-pygmtools/a_star.cp310-win_amd64.pyd
 pygmtools/benchmark.py
 pygmtools/classic_solvers.py
 pygmtools/dataset.py
 pygmtools/dataset_config.py
 pygmtools/jittor_backend.py
 pygmtools/jittor_modules.py
 pygmtools/linear_solvers.py
@@ -25,13 +23,15 @@
 pygmtools/tensorflow_modules.py
 pygmtools/utils.py
 pygmtools.egg-info/PKG-INFO
 pygmtools.egg-info/SOURCES.txt
 pygmtools.egg-info/dependency_links.txt
 pygmtools.egg-info/requires.txt
 pygmtools.egg-info/top_level.txt
+pygmtools/lib/a_star.tar.gz
+pygmtools/lib/a_star.zip
 tests/test_classic_solvers.py
 tests/test_dataset.py
 tests/test_misc.py
 tests/test_multi_graph_solvers.py
 tests/test_neural_solvers.py
 tests/test_utils.py
```

### Comparing `pygmtools-0.3.8a4/setup.py` & `pygmtools-0.3.8a5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import re
 import platform
 from setuptools import find_packages, setup, Command
 import tarfile
 import zipfile
 import os
 import distro
+import shutil
 
 def unzip_file(zip_file_path, extract_folder_path):
     with zipfile.ZipFile(zip_file_path, 'r') as zipObj:
         zipObj.extractall(extract_folder_path)
 
 def untar_file(tar_file_path, extract_folder_path):
     with tarfile.open(tar_file_path, 'r:gz') as tarObj:
@@ -76,40 +77,33 @@
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
     with open(os.path.join(here, project_slug, '__version__.py')) as f:
         exec(f.read(), about)
 else:
     about['__version__'] = VERSION
 
-
-os_version, python_version = get_os_and_python_version()
-
-filename={  'windows':{ '3.7':'a_star.cp37-win_amd64.pyd',
-                        '3.8':'a_star.cp38-win_amd64.pyd',
-                        '3.9':'a_star.cp37-win_amd64.pyd',
-                        '3.10':'a_star.cp310-win_amd64.pyd'},
-            'macos'  :{ '3.7':'a_star.cpython-37m-darwin.so',
-                        '3.8':'a_star.cpython-38-darwin.so',
-                        '3.9':'a_star.cpython-39-darwin.so'},
-            'ubuntu' :{ '3.7':'a_star.cpython-37m-x86_64-linux-gnu.so',
-                        '3.8':'a_star.cpython-38-x86_64-linux-gnu.so',
-                        '3.9':'a_star.cpython-39-x86_64-linux-gnu.so'}}
-
-dynamic_link = filename[os_version][python_version]
-if not os.path.exists(os.path.join(NAME,dynamic_link)):
-    if os_version == 'windows':
-        try:
-            unzip_file(os.path.join(NAME,'a_star.zip'),NAME)
-        except:
-            pass
-    else:
-        try:
-            untar_file(os.path.join(NAME,'a_star.tar.gz'),NAME)
-        except:
-            pass
+def post_install():
+    os_version, python_version = get_os_and_python_version()
+    filename={  'windows':{ '3.7':'a_star.cp37-win_amd64.pyd',
+                            '3.8':'a_star.cp38-win_amd64.pyd',
+                            '3.9':'a_star.cp37-win_amd64.pyd',
+                            '3.10':'a_star.cp310-win_amd64.pyd'},
+                'macos'  :{ '3.7':'a_star.cpython-37m-darwin.so',
+                            '3.8':'a_star.cpython-38-darwin.so',
+                            '3.9':'a_star.cpython-39-darwin.so'},
+                'ubuntu' :{ '3.7':'a_star.cpython-37m-x86_64-linux-gnu.so',
+                            '3.8':'a_star.cpython-38-x86_64-linux-gnu.so',
+                            '3.9':'a_star.cpython-39-x86_64-linux-gnu.so'}}
+    dynamic_link = filename[os_version][python_version]
+    if not os.path.exists(os.path.join(NAME,dynamic_link)):
+        if os_version == 'windows':
+            unzip_file(os.path.join(NAME,'lib/a_star.zip'),os.path.join(NAME,'lib'))
+        else:
+            untar_file(os.path.join(NAME,'lib/a_star.tar.gz'),os.path.join(NAME,'lib'))
+        shutil.copy2(dynamic_link, NAME)
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
 
@@ -149,15 +143,15 @@
     version=about['__version__'],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    package_data={NAME:[dynamic_link]},
+    package_data={NAME: ['lib/*.zip', 'lib/*.tar.gz']},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='Mulan PSL v2',
     python_requires='>=3.7',
     classifiers=(
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
```

### Comparing `pygmtools-0.3.8a4/tests/test_classic_solvers.py` & `pygmtools-0.3.8a5/tests/test_classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/tests/test_dataset.py` & `pygmtools-0.3.8a5/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/tests/test_misc.py` & `pygmtools-0.3.8a5/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/tests/test_multi_graph_solvers.py` & `pygmtools-0.3.8a5/tests/test_multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/tests/test_neural_solvers.py` & `pygmtools-0.3.8a5/tests/test_neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a4/tests/test_utils.py` & `pygmtools-0.3.8a5/tests/test_utils.py`

 * *Files identical despite different names*


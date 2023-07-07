# Comparing `tmp/SPLayout-0.4.9.tar.gz` & `tmp/SPLayout-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPLayout-0.4.9.tar", last modified: Tue Jul  4 01:34:46 2023, max compression
+gzip compressed data, was "SPLayout-0.5.0.tar", last modified: Fri Jul  7 11:25:31 2023, max compression
```

## Comparing `SPLayout-0.4.9.tar` & `SPLayout-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.863259 SPLayout-0.4.9/
--rw-rw-rw-   0        0        0    35803 2023-06-20 10:20:16.000000 SPLayout-0.4.9/LICENSE
--rw-rw-rw-   0        0        0     1719 2023-07-04 01:34:46.862264 SPLayout-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     1473 2023-06-20 10:20:16.000000 SPLayout-0.4.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.507701 SPLayout-0.4.9/SPLayout.egg-info/
--rw-rw-rw-   0        0        0     1719 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1578 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 01:34:46.000000 SPLayout-0.4.9/SPLayout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 01:34:46.863259 SPLayout-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-06-20 10:20:16.000000 SPLayout-0.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.508717 SPLayout-0.4.9/splayout/
--rw-rw-rw-   0        0        0     2120 2023-07-04 01:26:34.000000 SPLayout-0.4.9/splayout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.583254 SPLayout-0.4.9/splayout/adjointmethod/
--rw-rw-rw-   0        0        0      398 2023-07-03 08:15:18.000000 SPLayout-0.4.9/splayout/adjointmethod/__init__.py
--rw-rw-rw-   0        0        0    13624 2023-07-04 01:33:39.000000 SPLayout-0.4.9/splayout/adjointmethod/adjointmultitoopt.py
--rw-rw-rw-   0        0        0    10984 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/adjointshapeopt.py
--rw-rw-rw-   0        0        0    11728 2023-07-03 09:59:25.000000 SPLayout-0.4.9/splayout/adjointmethod/adjointtopologyopt.py
--rw-rw-rw-   0        0        0    15991 2023-07-04 00:55:42.000000 SPLayout-0.4.9/splayout/adjointmethod/scalabletotegion3d.py
--rw-rw-rw-   0        0        0    10586 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/shaperegion2d.py
--rw-rw-rw-   0        0        0    10652 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/shaperegion3d.py
--rw-rw-rw-   0        0        0    11374 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/topologyregion2d.py
--rw-rw-rw-   0        0        0    11304 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/adjointmethod/topologyregion3d.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.642426 SPLayout-0.4.9/splayout/algorithms/
--rw-rw-rw-   0        0        0      312 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5781 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/binarybatalgorithm.py
--rw-rw-rw-   0        0        0     6360 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/binarygeneticalgorithm.py
--rw-rw-rw-   0        0        0     5831 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/binaryparticleswarmalgorithm.py
--rw-rw-rw-   0        0        0     4305 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/directbinarysearchalgorithm.py
--rw-rw-rw-   0        0        0     7326 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/algorithms/particleswarmalgorithm.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.802861 SPLayout-0.4.9/splayout/components/
--rw-rw-rw-   0        0        0     3728 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/AEMDgrating.py
--rw-rw-rw-   0        0        0      714 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/__init__.py
--rw-rw-rw-   0        0        0     4403 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/bend.py
--rw-rw-rw-   0        0        0     9026 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/doubleconnector.py
--rw-rw-rw-   0        0        0     6092 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/filledpattern.py
--rw-rw-rw-   0        0        0    49359 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/microring.py
--rw-rw-rw-   0        0        0    21403 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/pixelsregion.py
--rw-rw-rw-   0        0        0     7433 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/polygon.py
--rw-rw-rw-   0        0        0    14219 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/quarbend.py
--rw-rw-rw-   0        0        0    18098 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/sbend.py
--rw-rw-rw-   0        0        0    13136 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/selfdefinecomponent.py
--rw-rw-rw-   0        0        0    28052 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/simpleasymmetricdirectionalcoupler.py
--rw-rw-rw-   0        0        0     7270 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/slowlyvaryingtaper.py
--rw-rw-rw-   0        0        0     6668 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/taper.py
--rw-rw-rw-   0        0        0     1269 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/text.py
--rw-rw-rw-   0        0        0     8908 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/components/waveguide.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.841989 SPLayout-0.4.9/splayout/lumericalcommun/
--rw-rw-rw-   0        0        0       72 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/lumericalcommun/__init__.py
--rw-rw-rw-   0        0        0    78118 2023-06-20 11:33:12.000000 SPLayout-0.4.9/splayout/lumericalcommun/fdtdapi.py
--rw-rw-rw-   0        0        0    44213 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/lumericalcommun/modeapi.py
-drwxrwxrwx   0        0        0        0 2023-07-04 01:34:46.860203 SPLayout-0.4.9/splayout/utils/
--rw-rw-rw-   0        0        0       20 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/utils/__init__.py
--rw-rw-rw-   0        0        0    14788 2023-06-20 10:20:16.000000 SPLayout-0.4.9/splayout/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:25:31.752839 SPLayout-0.5.0/
+-rw-rw-rw-   0        0        0    35803 2023-06-20 10:20:16.000000 SPLayout-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1719 2023-07-07 11:25:31.750580 SPLayout-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1473 2023-06-20 10:20:16.000000 SPLayout-0.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-07 11:25:31.489313 SPLayout-0.5.0/SPLayout.egg-info/
+-rw-rw-rw-   0        0        0     1719 2023-07-07 11:25:31.000000 SPLayout-0.5.0/SPLayout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1578 2023-07-07 11:25:31.000000 SPLayout-0.5.0/SPLayout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 11:25:31.000000 SPLayout-0.5.0/SPLayout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-07 11:25:31.000000 SPLayout-0.5.0/SPLayout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-07 11:25:31.000000 SPLayout-0.5.0/SPLayout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:25:31.752839 SPLayout-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-06-20 10:20:16.000000 SPLayout-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:25:31.490314 SPLayout-0.5.0/splayout/
+-rw-rw-rw-   0        0        0     2120 2023-07-07 11:20:26.000000 SPLayout-0.5.0/splayout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:25:31.530665 SPLayout-0.5.0/splayout/adjointmethod/
+-rw-rw-rw-   0        0        0      398 2023-07-07 11:19:52.000000 SPLayout-0.5.0/splayout/adjointmethod/__init__.py
+-rw-rw-rw-   0        0        0    13750 2023-07-07 11:23:24.000000 SPLayout-0.5.0/splayout/adjointmethod/adjointmultitoopt.py
+-rw-rw-rw-   0        0        0    11110 2023-07-07 11:23:24.000000 SPLayout-0.5.0/splayout/adjointmethod/adjointshapeopt.py
+-rw-rw-rw-   0        0        0    11854 2023-07-07 11:23:24.000000 SPLayout-0.5.0/splayout/adjointmethod/adjointtopologyopt.py
+-rw-rw-rw-   0        0        0    15991 2023-07-04 00:55:42.000000 SPLayout-0.5.0/splayout/adjointmethod/scalabletoregion3d.py
+-rw-rw-rw-   0        0        0    10586 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/adjointmethod/shaperegion2d.py
+-rw-rw-rw-   0        0        0    10652 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/adjointmethod/shaperegion3d.py
+-rw-rw-rw-   0        0        0    11374 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/adjointmethod/topologyregion2d.py
+-rw-rw-rw-   0        0        0    11304 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/adjointmethod/topologyregion3d.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:25:31.569617 SPLayout-0.5.0/splayout/algorithms/
+-rw-rw-rw-   0        0        0      312 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5781 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/algorithms/binarybatalgorithm.py
+-rw-rw-rw-   0        0        0     6360 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/algorithms/binarygeneticalgorithm.py
+-rw-rw-rw-   0        0        0     5831 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/algorithms/binaryparticleswarmalgorithm.py
+-rw-rw-rw-   0        0        0     4305 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/algorithms/directbinarysearchalgorithm.py
+-rw-rw-rw-   0        0        0     7326 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/algorithms/particleswarmalgorithm.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:25:31.701865 SPLayout-0.5.0/splayout/components/
+-rw-rw-rw-   0        0        0     3728 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/AEMDgrating.py
+-rw-rw-rw-   0        0        0      714 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/__init__.py
+-rw-rw-rw-   0        0        0     4403 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/bend.py
+-rw-rw-rw-   0        0        0     9026 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/doubleconnector.py
+-rw-rw-rw-   0        0        0     6092 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/filledpattern.py
+-rw-rw-rw-   0        0        0    49359 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/microring.py
+-rw-rw-rw-   0        0        0    21403 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/pixelsregion.py
+-rw-rw-rw-   0        0        0     7433 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/polygon.py
+-rw-rw-rw-   0        0        0    14219 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/quarbend.py
+-rw-rw-rw-   0        0        0    18098 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/sbend.py
+-rw-rw-rw-   0        0        0    13136 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/selfdefinecomponent.py
+-rw-rw-rw-   0        0        0    28052 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/simpleasymmetricdirectionalcoupler.py
+-rw-rw-rw-   0        0        0     7270 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/slowlyvaryingtaper.py
+-rw-rw-rw-   0        0        0     6668 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/taper.py
+-rw-rw-rw-   0        0        0     1269 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/text.py
+-rw-rw-rw-   0        0        0     8908 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/components/waveguide.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:25:31.733098 SPLayout-0.5.0/splayout/lumericalcommun/
+-rw-rw-rw-   0        0        0       72 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/lumericalcommun/__init__.py
+-rw-rw-rw-   0        0        0    78118 2023-06-20 11:33:12.000000 SPLayout-0.5.0/splayout/lumericalcommun/fdtdapi.py
+-rw-rw-rw-   0        0        0    44213 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/lumericalcommun/modeapi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 11:25:31.750580 SPLayout-0.5.0/splayout/utils/
+-rw-rw-rw-   0        0        0       20 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/utils/__init__.py
+-rw-rw-rw-   0        0        0    14788 2023-06-20 10:20:16.000000 SPLayout-0.5.0/splayout/utils/utils.py
```

### Comparing `SPLayout-0.4.9/LICENSE` & `SPLayout-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/PKG-INFO` & `SPLayout-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.4.9
+Version: 0.5.0
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License-File: LICENSE
 
 SPLayout
```

### Comparing `SPLayout-0.4.9/README.rst` & `SPLayout-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/SPLayout.egg-info/PKG-INFO` & `SPLayout-0.5.0/SPLayout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.4.9
+Version: 0.5.0
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License-File: LICENSE
 
 SPLayout
```

### Comparing `SPLayout-0.4.9/SPLayout.egg-info/SOURCES.txt` & `SPLayout-0.5.0/SPLayout.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 SPLayout.egg-info/requires.txt
 SPLayout.egg-info/top_level.txt
 splayout/__init__.py
 splayout/adjointmethod/__init__.py
 splayout/adjointmethod/adjointmultitoopt.py
 splayout/adjointmethod/adjointshapeopt.py
 splayout/adjointmethod/adjointtopologyopt.py
-splayout/adjointmethod/scalabletotegion3d.py
+splayout/adjointmethod/scalabletoregion3d.py
 splayout/adjointmethod/shaperegion2d.py
 splayout/adjointmethod/shaperegion3d.py
 splayout/adjointmethod/topologyregion2d.py
 splayout/adjointmethod/topologyregion3d.py
 splayout/algorithms/__init__.py
 splayout/algorithms/binarybatalgorithm.py
 splayout/algorithms/binarygeneticalgorithm.py
```

### Comparing `SPLayout-0.4.9/setup.py` & `SPLayout-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/__init__.py` & `SPLayout-0.5.0/splayout/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.9"
+__version__ = "0.5.0"
 
 ## Submodules
 from . import utils
 from . import components
 from . import algorithms
 from . import lumericalcommun
 from . import adjointmethod
@@ -29,15 +29,15 @@
 from .lumericalcommun.modeapi import MODESimulation
 
 ## Adjoint Method
 from .adjointmethod.shaperegion2d import ShapeOptRegion2D
 from .adjointmethod.shaperegion3d import ShapeOptRegion3D
 from .adjointmethod.topologyregion2d import TopologyOptRegion2D
 from .adjointmethod.topologyregion3d import TopologyOptRegion3D
-from .adjointmethod.scalabletotegion3d import ScalableToOptRegion3D
+from .adjointmethod.scalabletoregion3d import ScalableToOptRegion3D
 from .adjointmethod.adjointshapeopt import AdjointForShapeOpt
 from .adjointmethod.adjointtopologyopt import AdjointForTO
 from .adjointmethod.adjointmultitoopt import AdjointForMultiTO
 
 ## Algorithms
 from .algorithms.binarybatalgorithm import BinaryBatAlgorithm
 from .algorithms.directbinarysearchalgorithm import  DirectBinarySearchAlgorithm
```

### Comparing `SPLayout-0.4.9/splayout/adjointmethod/adjointmultitoopt.py` & `SPLayout-0.5.0/splayout/adjointmethod/adjointmultitoopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..utils.utils import *
 from .topologyregion3d import TopologyOptRegion3D
 from .topologyregion2d import TopologyOptRegion2D
-from .scalabletotegion3d import ScalableToOptRegion3D
+from .scalabletoregion3d import ScalableToOptRegion3D
 import numpy as np
 import scipy.constants
 
 class AdjointForMultiTO:
     """
     Adjoint Method for Multiple Topology Optimization Regions.
 
@@ -241,51 +241,51 @@
             # T_fwd_partial_derivs_regions = []
             # for i in range(0, self.design_region_num):
             #     T_fwd_partial_derivs_regions.append(
             #         T_fwd_partial_derivs[:, self.params_indices_start[i]:self.params_indices_end[i]])
 
         return T_fwd_partial_derivs
 
-    def reset_fom_monitor_name(self, fom_monitor_name):
+    def reset_T_monitor_names(self, T_monitor_names):
         """
         Rest fom monitor for deriving FoM.
 
         Parameters
         ----------
-        fom_monitor_name : String or List of String
+        T_monitor_names : String or List of String
             Monitor names for deriving FoM.
         """
-        self.fom_monitor_name = fom_monitor_name
+        self.T_monitor_names = np.array([T_monitor_names]).flatten()
 
-    def reset_forward_source_name(self, forward_source_name):
+    def reset_forward_source_names(self, forward_source_names):
         """
         Rest source for Forward simulation.
 
         Parameters
         ----------
-        forward_source_name : String or List of String
+        forward_source_names : String or List of String
             Source names for Forward simulation.
         """
-        self.forward_source_name = forward_source_name
+        self.forward_source_names = np.array([forward_source_names]).flatten()
 
-    def reset_backward_source_name(self, backward_source_name):
+    def reset_backward_source_names(self, backward_source_names):
         """
         Rest source for Adjoint simulation.
 
         Parameters
         ----------
-        backward_source_name : String or List of String
+        backward_source_names : String or List of String
             Source names for Adjoint simulation.
 
         """
-        self.backward_source_name = backward_source_name
+        self.backward_source_names = np.array([backward_source_names]).flatten()
 
-    def reset_target_fom(self, target_fom):
+    def reset_target_T(self, target_T):
         """
         Rest target FoMs at different frequencies.
 
         Parameters
         ----------
-        target_fom : Array or List of Array
+        target_T : Array or List of Array
             Target FoMs at different frequencies.
         """
-        self.target_fom = target_fom
+        self.target_T = np.reshape(np.array([target_T]), (np.shape(self.T_monitor_names)[0], -1))
```

### Comparing `SPLayout-0.4.9/splayout/adjointmethod/adjointshapeopt.py` & `SPLayout-0.5.0/splayout/adjointmethod/adjointshapeopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,51 +200,51 @@
         d = np.diff(wavelength)
 
         quad_weight = np.append(np.append(d[0], d[0:-1] + d[1:]), d[-1]) / 2
         v = const_factor * integral_kernel.flatten() * quad_weight
         T_fwd_partial_derivs = partial_fom.transpose().dot(v).flatten().real
         return - T_fwd_partial_derivs / 1e6
 
-    def reset_fom_monitor_name(self, fom_monitor_name):
+    def reset_T_monitor_names(self, T_monitor_names):
         """
         Rest fom monitor for deriving FoM.
 
         Parameters
         ----------
-        fom_monitor_name : String or List of String
+        T_monitor_names : String or List of String
             Monitor names for deriving FoM.
         """
-        self.fom_monitor_name = fom_monitor_name
+        self.T_monitor_names = np.array([T_monitor_names]).flatten()
 
-    def reset_forward_source_name(self, forward_source_name):
+    def reset_forward_source_names(self, forward_source_names):
         """
         Rest source for Forward simulation.
 
         Parameters
         ----------
-        forward_source_name : String or List of String
+        forward_source_names : String or List of String
             Source names for Forward simulation.
         """
-        self.forward_source_name = forward_source_name
+        self.forward_source_names = np.array([forward_source_names]).flatten()
 
-    def reset_backward_source_name(self, backward_source_name):
+    def reset_backward_source_names(self, backward_source_names):
         """
         Rest source for Adjoint simulation.
 
         Parameters
         ----------
-        backward_source_name : String or List of String
+        backward_source_names : String or List of String
             Source names for Adjoint simulation.
 
         """
-        self.backward_source_name = backward_source_name
+        self.backward_source_names = np.array([backward_source_names]).flatten()
 
-    def reset_target_fom(self, target_fom):
+    def reset_target_T(self, target_T):
         """
         Rest target FoMs at different frequencies.
 
         Parameters
         ----------
-        target_fom : Array or List of Array
+        target_T : Array or List of Array
             Target FoMs at different frequencies.
         """
-        self.target_fom = target_fom
+        self.target_T = np.reshape(np.array([target_T]), (np.shape(self.T_monitor_names)[0], -1))
```

### Comparing `SPLayout-0.4.9/splayout/adjointmethod/adjointtopologyopt.py` & `SPLayout-0.5.0/splayout/adjointmethod/adjointtopologyopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..utils.utils import *
 from .topologyregion3d import TopologyOptRegion3D
 from .topologyregion2d import TopologyOptRegion2D
-from .scalabletotegion3d import ScalableToOptRegion3D
+from .scalabletoregion3d import ScalableToOptRegion3D
 import numpy as np
 import scipy.constants
 
 class AdjointForTO:
     """
     Adjoint Method for Topology Optimization.
 
@@ -207,51 +207,51 @@
         if (self.if_default_fom == 1):
             T_fwd_partial_derivs = - np.sum(np.array(T_fwd_partial_derivs), axis=0)
         else:
             T_fwd_partial_derivs = np.array(T_fwd_partial_derivs)
 
         return T_fwd_partial_derivs
 
-    def reset_fom_monitor_name(self, fom_monitor_name):
+    def reset_T_monitor_names(self, T_monitor_names):
         """
         Rest fom monitor for deriving FoM.
 
         Parameters
         ----------
-        fom_monitor_name : String or List of String
+        T_monitor_names : String or List of String
             Monitor names for deriving FoM.
         """
-        self.fom_monitor_name = fom_monitor_name
+        self.T_monitor_names = np.array([T_monitor_names]).flatten()
 
-    def reset_forward_source_name(self, forward_source_name):
+    def reset_forward_source_names(self, forward_source_names):
         """
         Rest source for Forward simulation.
 
         Parameters
         ----------
-        forward_source_name : String or List of String
+        forward_source_names : String or List of String
             Source names for Forward simulation.
         """
-        self.forward_source_name = forward_source_name
+        self.forward_source_names = np.array([forward_source_names]).flatten()
 
-    def reset_backward_source_name(self, backward_source_name):
+    def reset_backward_source_names(self, backward_source_names):
         """
         Rest source for Adjoint simulation.
 
         Parameters
         ----------
-        backward_source_name : String or List of String
+        backward_source_names : String or List of String
             Source names for Adjoint simulation.
 
         """
-        self.backward_source_name = backward_source_name
+        self.backward_source_names = np.array([backward_source_names]).flatten()
 
-    def reset_target_fom(self, target_fom):
+    def reset_target_T(self, target_T):
         """
         Rest target FoMs at different frequencies.
 
         Parameters
         ----------
-        target_fom : Array or List of Array
+        target_T : Array or List of Array
             Target FoMs at different frequencies.
         """
-        self.target_fom = target_fom
+        self.target_T = np.reshape(np.array([target_T]), (np.shape(self.T_monitor_names)[0], -1))
```

### Comparing `SPLayout-0.4.9/splayout/adjointmethod/scalabletotegion3d.py` & `SPLayout-0.5.0/splayout/adjointmethod/scalabletoregion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/adjointmethod/shaperegion2d.py` & `SPLayout-0.5.0/splayout/adjointmethod/shaperegion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/adjointmethod/shaperegion3d.py` & `SPLayout-0.5.0/splayout/adjointmethod/shaperegion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/adjointmethod/topologyregion2d.py` & `SPLayout-0.5.0/splayout/adjointmethod/topologyregion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/adjointmethod/topologyregion3d.py` & `SPLayout-0.5.0/splayout/adjointmethod/topologyregion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/algorithms/binarybatalgorithm.py` & `SPLayout-0.5.0/splayout/algorithms/binarybatalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/algorithms/binarygeneticalgorithm.py` & `SPLayout-0.5.0/splayout/algorithms/binarygeneticalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/algorithms/binaryparticleswarmalgorithm.py` & `SPLayout-0.5.0/splayout/algorithms/binaryparticleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/algorithms/directbinarysearchalgorithm.py` & `SPLayout-0.5.0/splayout/algorithms/directbinarysearchalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/algorithms/particleswarmalgorithm.py` & `SPLayout-0.5.0/splayout/algorithms/particleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/AEMDgrating.py` & `SPLayout-0.5.0/splayout/components/AEMDgrating.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/__init__.py` & `SPLayout-0.5.0/splayout/components/__init__.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/bend.py` & `SPLayout-0.5.0/splayout/components/bend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/doubleconnector.py` & `SPLayout-0.5.0/splayout/components/doubleconnector.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/filledpattern.py` & `SPLayout-0.5.0/splayout/components/filledpattern.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/microring.py` & `SPLayout-0.5.0/splayout/components/microring.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/pixelsregion.py` & `SPLayout-0.5.0/splayout/components/pixelsregion.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/polygon.py` & `SPLayout-0.5.0/splayout/components/polygon.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/quarbend.py` & `SPLayout-0.5.0/splayout/components/quarbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/sbend.py` & `SPLayout-0.5.0/splayout/components/sbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/selfdefinecomponent.py` & `SPLayout-0.5.0/splayout/components/selfdefinecomponent.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/simpleasymmetricdirectionalcoupler.py` & `SPLayout-0.5.0/splayout/components/simpleasymmetricdirectionalcoupler.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/slowlyvaryingtaper.py` & `SPLayout-0.5.0/splayout/components/slowlyvaryingtaper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/taper.py` & `SPLayout-0.5.0/splayout/components/taper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/text.py` & `SPLayout-0.5.0/splayout/components/text.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/components/waveguide.py` & `SPLayout-0.5.0/splayout/components/waveguide.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/lumericalcommun/fdtdapi.py` & `SPLayout-0.5.0/splayout/lumericalcommun/fdtdapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/lumericalcommun/modeapi.py` & `SPLayout-0.5.0/splayout/lumericalcommun/modeapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.9/splayout/utils/utils.py` & `SPLayout-0.5.0/splayout/utils/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/sphractal-0.7.1.tar.gz` & `tmp/sphractal-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.7.1.tar", max compression
+gzip compressed data, was "sphractal-0.8.0.tar", max compression
```

## Comparing `sphractal-0.7.1.tar` & `sphractal-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-05 01:38:59.307865 sphractal-0.7.1/LICENSE
--rw-r--r--   0        0        0     4015 2023-07-05 01:38:59.307865 sphractal-0.7.1/README.md
--rw-r--r--   0        0        0     2056 2023-07-05 01:39:39.072186 sphractal-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      736 2023-07-05 01:39:39.072186 sphractal-0.7.1/setup.py
--rw-r--r--   0        0        0     1429 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/__init__.py
--rw-r--r--   0        0        0    23019 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     4384 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      278 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/datasets.py
--rw-r--r--   0        0        0     8749 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8119 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11513 2023-07-05 01:38:59.363866 sphractal-0.7.1/src/sphractal/utils.py
--rw-r--r--   0        0        0    94032 2023-07-05 01:38:59.363866 sphractal-0.7.1/tests/fixtures.py
--rw-r--r--   0        0        0    17618 2023-07-05 01:38:59.363866 sphractal-0.7.1/tests/test_sphractal.py
--rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 sphractal-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-07 09:11:28.347972 sphractal-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4017 2023-07-07 09:11:28.347972 sphractal-0.8.0/README.md
+-rw-r--r--   0        0        0     2056 2023-07-07 09:12:06.575822 sphractal-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      736 2023-07-07 09:12:06.575822 sphractal-0.8.0/setup.py
+-rw-r--r--   0        0        0     1429 2023-07-07 09:11:28.411972 sphractal-0.8.0/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    23050 2023-07-07 09:11:28.411972 sphractal-0.8.0/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4382 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      264 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8750 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8121 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11515 2023-07-07 09:11:28.415972 sphractal-0.8.0/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94032 2023-07-07 09:11:28.415972 sphractal-0.8.0/tests/fixtures.py
+-rw-r--r--   0        0        0    17618 2023-07-07 09:11:28.415972 sphractal-0.8.0/tests/test_sphractal.py
+-rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 sphractal-0.8.0/PKG-INFO
```

### Comparing `sphractal-0.7.1/LICENSE` & `sphractal-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.1/README.md` & `sphractal-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Sphractal
 
 [![ci-cd](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml)
 
 ## Description
 
-`Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
+`Sphractal` is a package that provides functionalities to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
 ### Aims
 * Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
```

### Comparing `sphractal-0.7.1/pyproject.toml` & `sphractal-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.7.1"
+version = "0.8.0"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
```

### Comparing `sphractal-0.7.1/setup.py` & `sphractal-0.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.7.1'
+__version__ = '0.8.0'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphractal",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `sphractal-0.7.1/src/sphractal/__init__.py` & `sphractal-0.8.0/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.1/src/sphractal/boxCnt.py` & `sphractal-0.8.0/src/sphractal/boxCnt.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 import numpy as np
 from statsmodels.api import OLS, add_constant
 
 from sphractal.constants import PLT_PARAMS
-from sphractal.utils import findNN, findSurf, readXYZ
-# from sphractal.utils import estDuration, annotate
 from sphractal.surfPointClouds import genSurfPoints
 from sphractal.surfExact import findTargetAtoms, MIN_VAL_FROM_BOUND, scanAllAtoms, writeBoxCoords
+from sphractal.utils import findNN, findSurf, readXYZ
+# from sphractal.utils import estDuration, annotate
 
 
 # @annotate('getVoxelBoxCnts', color='blue')
 def getVoxelBoxCnts(atomsEle, atomsRad, atomsSurfIdxs, atomsXYZ, atomsNeighIdxs,
                     npName, writeFileDir='boxCntOutputs', exePath='$FASTBC_EXE',
                     radType='atomic', numPoint=300, gridNum=1024,
                     rmInSurf=True, vis=True, verbose=False, genPCD=False):
@@ -163,16 +163,16 @@
     numCPUs = cpu_count()
     boxLenScanMaxWorkers = ceil(numCPUs * numBoxLenSample / len(atomsIdxs))
     boxLenConc = False if boxLenScanMaxWorkers < 2 else True
     atomScanMaxWorkers = numCPUs - boxLenScanMaxWorkers if boxLenConc else numCPUs
 
     if verbose:
         print(f"  Representing the surface by treating each atom as exact spheres...")
-        print(f"  Parallelised with {atomScanMaxWorkers} out of {numCPUs} cores for scanning over atoms, "
-              f"the rest over box lengths...")
+        print(f"    Parallelised with {atomScanMaxWorkers} out of {numCPUs} cores for scanning over {len(atomsIdxs)} "
+              f"atoms, the rest over {numBoxLenSample} box lengths...")
         print(f"    (1/eps)    (# bulk)    (# surf)")
     if writeBox:
         if not isdir(writeFileDir):
             mkdir(writeFileDir)
 
     overallBoxLen = maxRange + MIN_VAL_FROM_BOUND * 2
     allLensSurfBoxs, allLensBulkBoxs, allLensSurfCnts, allLensBulkCnts = [], [], [], []
@@ -210,15 +210,15 @@
         writeBoxCoords(atomsEle, atomsXYZ, allLensSurfBoxs, allLensBulkBoxs, minXYZ, scanBoxLens, writeFileDir, npName)
     return scales, counts
 
 
 # @annotate('findSlope', color='green')
 def findSlope(scales, counts, npName='', writeFileDir='boxCntOutputs', lenRange='trim',
               minSampleNum=5, confLvl=95, 
-              visReg=True, figType='article', saveFig=False, showPlot=False):
+              visReg=True, figType='paper', saveFig=False, showPlot=False):
     """
     Compute the slope (box counting dimension) from the box-counting data collected.
 
     Parameters
     ----------
     scales : list
         Box lengths.
@@ -233,15 +233,15 @@
         coefficient of determination by iteratively removing the box counts obtained using boxes of extreme sizes.
     minSampleNum : int, optional
         Minimum number of box count data points to be retained for slope estimation from the linear regression fitting.
     confLvl : Union[int, float]
         Confidence level of confidence interval in percentage.
     visReg : bool, optional
         Whether to generate figures from the linear regression fitting process.
-    figType : {'article', 'poster', 'ppt'}
+    figType : {'paper', 'poster', 'talk'}
         Type of figures to be generated.
     saveFig : bool, optional
         Whether to save the plots generated, only works when 'visReg' is True.
     showPlot : bool, optional
         Whether to show the plots generated, only works when 'visReg' is True.
     
     Returns
@@ -347,15 +347,15 @@
 
 
 # @annotate('runCase', color='cyan')
 # @estDuration
 def runBoxCnt(xyzFilePath, 
               radType='atomic', calcBL=False, findSurfOption='alphaShape', alphaMult=2.0,
               writeFileDir='boxCntOutputs', lenRange='trim', minSampleNum=5, confLvl=95, 
-              rmInSurf=True, vis=True, figType='article', saveFig=False, showPlot=False, verbose=False,
+              rmInSurf=True, vis=True, figType='paper', saveFig=False, showPlot=False, verbose=False,
               runPointCloudBoxCnt=True, numPoints=300, gridNum=1024, exePath='$FASTBC_EXE', genPCD=False,
               runExactSphereBoxCnt=True, minLenMult=0.25, maxLenMult=1, numBoxLenSample=10, writeBox=True): 
     """
     Run box-counting algorithm on the surface of a given object consisting of a set of spheres represented as either
     point clouds or exact spherical surface.
     
     Parameters
@@ -380,15 +380,15 @@
         Minimum number of box count data points to be retained for slope estimation from the linear regression fitting.
     confLvl : Union[int, float], optional
         Confidence level of confidence interval in percentage.
     rmInSurf : bool, optional
         Whether to remove the surface points on the inner surface.
     vis : bool, optional
         Whether to generate output files for visualisation.
-    figType : {'article', 'poster', 'ppt'}
+    figType : {'paper', 'poster', 'talk'}
         Type of figures to be generated.
     saveFig : bool, optional
         Whether to save the plots generated, only used if 'vis' is True.
     showPlot : bool, optional
         Whether to show the plots generated, only used if 'vis' is True.
     verbose : bool, optional
         Whether to display the details.
```

### Comparing `sphractal-0.7.1/src/sphractal/constants.py` & `sphractal-0.8.0/src/sphractal/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,13 +35,13 @@
     'Hf': 1.59, 'Ta': 1.46, 'W': 1.39, 'Re': 1.37, 'Os': 1.35, 'Ir': 1.355, 'Pt': 1.385, 'Au': 1.44, 'Hg': 1.51,
     'Tl': 1.70, 'Pb': defRad, 'Bi': defRad, 'Po': defRad, 'At': defRad, 'Rn': defRad, 'Fr': defRad, 'Ra': defRad,
     'Ac': defRad, 'Th': 1.79, 'Pa': 1.63, 'U': 1.56, 'Np': 1.55, 'Pu': 1.59, 'Am': 1.73, 'Cm': 1.74, 'Bk': 1.70,
     'Cf': 1.86, 'Es': 1.86, 'Fm': defRad, 'Md': defRad, 'No': defRad, 'Lr': defRad, 'Rf': defRad, 'Db': defRad,
     'Sg': defRad, 'Bh': defRad, 'Hs': defRad, 'Mt': defRad, 'Ds': defRad, 'Rg': defRad, 'Cn': defRad, 'Nh': defRad,
     'Fl': defRad, 'Mc': defRad, 'Lv': defRad, 'Ts': defRad, 'Og': defRad
 }
-PLT_PARAMS = {'article': {'figSize': (3.5, 2.5), 'dpi': 300, 'fontSize': 'medium', 'labelSize': 'small',
-                          'legendSize': 'x-small', 'lineWidth': 0.5, 'markerSize': 24},
+PLT_PARAMS = {'paper': {'figSize': (3.5, 2.5), 'dpi': 300, 'fontSize': 'medium', 'labelSize': 'small',
+                        'legendSize': 'x-small', 'lineWidth': 0.5, 'markerSize': 24},
               'poster': {'figSize': (4.5, 3.5), 'dpi': 600, 'fontSize': 'x-large', 'labelSize': 'large',
                          'legendSize': 'medium', 'lineWidth': 1.0, 'markerSize': 48},
-              'ppt': {'figSize': (4, 3), 'dpi': 144, 'fontSize': 'large', 'labelSize': 'medium', 'legendSize': 'small',
-                      'lineWidth': 1.0, 'markerSize': 36}}
+              'talk': {'figSize': (4, 3), 'dpi': 144, 'fontSize': 'large', 'labelSize': 'medium', 'legendSize': 'small',
+                       'lineWidth': 1.0, 'markerSize': 36}}
```

### Comparing `sphractal-0.7.1/src/sphractal/data/example.xyz` & `sphractal-0.8.0/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.1/src/sphractal/surfExact.py` & `sphractal-0.8.0/src/sphractal/surfExact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from concurrent.futures import ProcessPoolExecutor as Pool
 from math import ceil
-from numba import njit
-import numpy as np
 from os import mkdir
 from os.path import isdir
 
+from numba import njit
+import numpy as np
+
 from sphractal.utils import calcDist, oppositeInnerAtoms
 # from sphractal.utils import annotate
 
 
 MIN_VAL_FROM_BOUND = 5.0  # Angstrom
```

### Comparing `sphractal-0.7.1/src/sphractal/surfPointClouds.py` & `sphractal-0.8.0/src/sphractal/surfPointClouds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from math import cos, pi, sin, sqrt
-from numba import njit
-import numpy as np
 from os import mkdir
 from os.path import isdir
 
+from numba import njit
+import numpy as np
+
 from sphractal.constants import ATOMIC_RAD_DICT, METALLIC_RAD_DICT
 from sphractal.utils import calcDist, oppositeInnerAtoms
 # from sphractal.utils import annotate
 
 
 @njit(fastmath=True, cache=True)
 def fibonacciSphere(numPoint, sphereRad):
```

### Comparing `sphractal-0.7.1/src/sphractal/utils.py` & `sphractal-0.8.0/src/sphractal/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from time import time
 # from warnings import warn
 
 from numba import njit, prange
 import numpy as np
 # from nvtx import annotate
 from scipy.spatial import ConvexHull, Delaunay
+
 from sphractal.constants import ATOMIC_RAD_DICT, BULK_CN, METALLIC_RAD_DICT
 
 
 def estDuration(func):
     """Return time taken to run a function."""
     def wrap(*arg, **kwargs):
         start = time()
```

### Comparing `sphractal-0.7.1/tests/fixtures.py` & `sphractal-0.8.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.1/tests/test_sphractal.py` & `sphractal-0.8.0/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.7.1/PKG-INFO` & `sphractal-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.7.1
+Version: 0.8.0
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
@@ -29,15 +29,15 @@
 
 # Sphractal
 
 [![ci-cd](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml)
 
 ## Description
 
-`Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
+`Sphractal` is a package that provides functionalities to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
 ### Aims
 * Representation of the surface as either point clouds or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
```


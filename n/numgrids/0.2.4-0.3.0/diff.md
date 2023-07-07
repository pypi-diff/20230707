# Comparing `tmp/numgrids-0.2.4.tar.gz` & `tmp/numgrids-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numgrids-0.2.4.tar", last modified: Tue Jul  4 14:43:10 2023, max compression
+gzip compressed data, was "numgrids-0.3.0.tar", last modified: Fri Jul  7 13:44:31 2023, max compression
```

## Comparing `numgrids-0.2.4.tar` & `numgrids-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-04 14:43:10.157045 numgrids-0.2.4/
--rw-r--r--   0 mbaer    (671849960) 579947404     1069 2023-07-03 11:28:15.000000 numgrids-0.2.4/LICENSE
--rw-r--r--   0 mbaer    (671849960) 579947404      989 2023-07-04 14:43:10.156410 numgrids-0.2.4/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404     4203 2023-07-01 06:53:26.000000 numgrids-0.2.4/README.md
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-04 14:43:10.152349 numgrids-0.2.4/numgrids/
--rw-r--r--   0 mbaer    (671849960) 579947404      169 2023-07-04 14:37:32.000000 numgrids-0.2.4/numgrids/__init__.py
--rw-r--r--   0 mbaer    (671849960) 579947404     4402 2023-07-03 12:45:13.000000 numgrids-0.2.4/numgrids/api.py
--rw-r--r--   0 mbaer    (671849960) 579947404     7127 2023-06-30 13:37:54.000000 numgrids-0.2.4/numgrids/axes.py
--rw-r--r--   0 mbaer    (671849960) 579947404     5157 2023-06-28 14:34:51.000000 numgrids-0.2.4/numgrids/diff.py
--rw-r--r--   0 mbaer    (671849960) 579947404     4311 2023-07-04 14:37:13.000000 numgrids-0.2.4/numgrids/grids.py
--rw-r--r--   0 mbaer    (671849960) 579947404     1995 2023-07-04 14:37:13.000000 numgrids-0.2.4/numgrids/integration.py
--rw-r--r--   0 mbaer    (671849960) 579947404     2001 2023-07-03 11:10:56.000000 numgrids-0.2.4/numgrids/interpol.py
--rw-r--r--   0 mbaer    (671849960) 579947404      957 2023-07-04 14:37:13.000000 numgrids-0.2.4/numgrids/plots.py
--rw-r--r--   0 mbaer    (671849960) 579947404      163 2023-06-30 06:18:32.000000 numgrids-0.2.4/numgrids/utils.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-04 14:43:10.155679 numgrids-0.2.4/numgrids.egg-info/
--rw-r--r--   0 mbaer    (671849960) 579947404      989 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404      355 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/SOURCES.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/dependency_links.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       39 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/requires.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        9 2023-07-04 14:43:10.000000 numgrids-0.2.4/numgrids.egg-info/top_level.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       38 2023-07-04 14:43:10.157191 numgrids-0.2.4/setup.cfg
--rw-r--r--   0 mbaer    (671849960) 579947404     1282 2023-07-04 14:42:04.000000 numgrids-0.2.4/setup.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-07 13:44:31.182646 numgrids-0.3.0/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1069 2023-07-03 11:28:15.000000 numgrids-0.3.0/LICENSE
+-rw-r--r--   0 mbaer    (671849960) 579947404      989 2023-07-07 13:44:31.182109 numgrids-0.3.0/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404     4248 2023-07-07 13:42:56.000000 numgrids-0.3.0/README.md
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-07 13:44:31.178844 numgrids-0.3.0/numgrids/
+-rw-r--r--   0 mbaer    (671849960) 579947404      210 2023-07-07 13:43:04.000000 numgrids-0.3.0/numgrids/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     5040 2023-07-06 09:32:05.000000 numgrids-0.3.0/numgrids/api.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     7127 2023-06-30 13:37:54.000000 numgrids-0.3.0/numgrids/axes.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     5157 2023-06-28 14:34:51.000000 numgrids-0.3.0/numgrids/diff.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     8225 2023-07-07 13:42:56.000000 numgrids-0.3.0/numgrids/grids.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     1995 2023-07-04 14:37:13.000000 numgrids-0.3.0/numgrids/integration.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     2354 2023-07-07 13:42:56.000000 numgrids-0.3.0/numgrids/interpol.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      957 2023-07-06 09:08:38.000000 numgrids-0.3.0/numgrids/plots.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      163 2023-07-06 09:08:38.000000 numgrids-0.3.0/numgrids/utils.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-07 13:44:31.181192 numgrids-0.3.0/numgrids.egg-info/
+-rw-r--r--   0 mbaer    (671849960) 579947404      989 2023-07-07 13:44:31.000000 numgrids-0.3.0/numgrids.egg-info/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      355 2023-07-07 13:44:31.000000 numgrids-0.3.0/numgrids.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-07 13:44:31.000000 numgrids-0.3.0/numgrids.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       39 2023-07-07 13:44:31.000000 numgrids-0.3.0/numgrids.egg-info/requires.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        9 2023-07-07 13:44:31.000000 numgrids-0.3.0/numgrids.egg-info/top_level.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       38 2023-07-07 13:44:31.182829 numgrids-0.3.0/setup.cfg
+-rw-r--r--   0 mbaer    (671849960) 579947404     1282 2023-07-04 14:42:04.000000 numgrids-0.3.0/setup.py
```

### Comparing `numgrids-0.2.4/LICENSE` & `numgrids-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.4/PKG-INFO` & `numgrids-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numgrids
-Version: 0.2.4
+Version: 0.3.0
 Summary: Working with numerical grids made easy.
 Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Platform: ALL
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: numgrids Version: 0.2.4 Summary: Working with
+Metadata-Version: 2.1 Name: numgrids Version: 0.3.0 Summary: Working with
 numerical grids made easy. Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer Author-email: matthias.r.baer@googlemail.com License: MIT
 Platform: ALL Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
                             ****** numgrids ******
                     Working with numerical grids made easy.
```

### Comparing `numgrids-0.2.4/README.md` & `numgrids-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 **Main Features**
 
 - Quickly define numerical grids for any rectangular or curvilinear coordinate system
 - Differentiation and integration
 - Interpolation
 - Easy manipulation of meshed functions
 - Using high precision spectral methods (FFT + Chebyshev) wherever possible
+- Includes multigrid functionality
 - Fully compatible with *numpy*
 
 ## Installation
 
 ```shell
-pip install numgrids
+pip install --upgrade numgrids
 ```
 
 ## Quick Start
 
 As a quick example, here is how you define a grid on the unit disk using polar coordinates.
 Along the azimuthal (angular) direction, choose an equidistant spacing with periodic boundary conditions:
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
                             ****** numgrids ******
                     Working with numerical grids made easy.
                             [PyPI_version] [build]
    [docs/assets/torus.png] [docs/assets/disk320.png] [docs/assets/cubic.png]
 **Main Features** - Quickly define numerical grids for any rectangular or
 curvilinear coordinate system - Differentiation and integration - Interpolation
 - Easy manipulation of meshed functions - Using high precision spectral methods
-(FFT + Chebyshev) wherever possible - Fully compatible with *numpy* ##
-Installation ```shell pip install numgrids ``` ## Quick Start As a quick
-example, here is how you define a grid on the unit disk using polar
-coordinates. Along the azimuthal (angular) direction, choose an equidistant
-spacing with periodic boundary conditions: ```python from numgrids import *
-from numpy import pi axis_phi = Axis(AxisType.EQUIDISTANT, 50, 0, 2*pi,
-periodic=True) ``` [docs/assets/equi_periodic.png] Along the radial axis, let's
-choose a non-equidistant spacing: ```python axis_radial = Axis
-(AxisType.CHEBYSHEV, 20, 0, 1) ``` [docs/assets/cheby.png] Now combine the axes
-to a **grid**: ```python grid = Grid(axis_radial, axis_phi) ``` [docs/assets/
-disk320.png] **Sample** a meshed function on this grid: ```python from numpy
-import exp, sin R, Phi = grid.meshed_coords f = R**2 * sin(Phi)**2 ``` Define
-**partial derivatives** $\partial/\partial r$ and $\partial/\partial \varphi$
-and apply them: ```python # second argument means derivative order, third
-argument means axis index: d_dr = Diff(grid, 1, 0) d_dphi = Diff(grid, 1, 1)
-df_dr = d_dr(f) df_dphi = d_dphi(f) ``` Obtain the **matrix representation** of
-the differential operators: ```python d_dr.as_matrix() Out: <1000x1000 sparse
-matrix of type '
+(FFT + Chebyshev) wherever possible - Includes multigrid functionality - Fully
+compatible with *numpy* ## Installation ```shell pip install --upgrade numgrids
+``` ## Quick Start As a quick example, here is how you define a grid on the
+unit disk using polar coordinates. Along the azimuthal (angular) direction,
+choose an equidistant spacing with periodic boundary conditions: ```python from
+numgrids import * from numpy import pi axis_phi = Axis(AxisType.EQUIDISTANT,
+50, 0, 2*pi, periodic=True) ``` [docs/assets/equi_periodic.png] Along the
+radial axis, let's choose a non-equidistant spacing: ```python axis_radial =
+Axis(AxisType.CHEBYSHEV, 20, 0, 1) ``` [docs/assets/cheby.png] Now combine the
+axes to a **grid**: ```python grid = Grid(axis_radial, axis_phi) ``` [docs/
+assets/disk320.png] **Sample** a meshed function on this grid: ```python from
+numpy import exp, sin R, Phi = grid.meshed_coords f = R**2 * sin(Phi)**2 ```
+Define **partial derivatives** $\partial/\partial r$ and $\partial/\partial
+\varphi$ and apply them: ```python # second argument means derivative order,
+third argument means axis index: d_dr = Diff(grid, 1, 0) d_dphi = Diff(grid, 1,
+1) df_dr = d_dr(f) df_dphi = d_dphi(f) ``` Obtain the **matrix representation**
+of the differential operators: ```python d_dr.as_matrix() Out: <1000x1000
+sparse matrix of type '
 numpy.float64'>' with 20000 stored elements in COOrdinate format> ``` Define
 **integration operator** $$ \int \dots dr d\varphi $$ ```python I = Integral
 (grid) ``` Calculate the area integral $$ \int f(r, \varphi) r dr d\varphi $$
 (taking into account the appropriate integration measure $r$ for polar
 coordinates): ```python I(f * R) ``` Setting **boundary** values to zero
 ```python f[grid.boundary] = 0 # grid.boundary is boolean mask selecting
 boundary grid points ``` or to something more complicated: ```python f
```

### Comparing `numgrids-0.2.4/numgrids/api.py` & `numgrids-0.3.0/numgrids/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -136,7 +136,32 @@
                    1 / (R ** 2 * np.sin(Theta) ** 2) * dphi2(f)
 
         self._laplacian = laplacian
 
     def laplacian(self, f):
         """Returns the laplacian in spherical coordinates as a callable."""
         return self._laplacian(f)
+
+
+def diff(grid, f, order=1, axis_index=0):
+    if (order, axis_index) in grid.cache.get("diffs"):
+        d = grid.cache["diffs"][order, axis_index]
+    else:
+        d = Diff(grid, order, axis_index)
+        grid.cache["diffs"][order, axis_index] = d
+    return d(f)
+
+
+def interpolate(grid, f, locations):
+    from numgrids import Interpolator
+    inter = Interpolator(grid, f)
+    return inter(locations)
+
+
+def integrate(grid, f):
+    from numgrids.integration import Integral
+    if grid.cache.get("integral"):
+        I = grid.cache["integral"]
+    else:
+        I = Integral(grid)
+        grid.cache["integral"] = I
+    return I(f)
```

### Comparing `numgrids-0.2.4/numgrids/axes.py` & `numgrids-0.3.0/numgrids/axes.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.4/numgrids/diff.py` & `numgrids-0.3.0/numgrids/diff.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.4/numgrids/integration.py` & `numgrids-0.3.0/numgrids/integration.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.4/numgrids/interpol.py` & `numgrids-0.3.0/numgrids/interpol.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 import numpy as np
-from scipy.interpolate import RegularGridInterpolator, CubicSpline
+from scipy.interpolate import RegularGridInterpolator, CubicSpline, UnivariateSpline, interp1d
 
 from numgrids import Grid
 
 
 class Interpolator:
 
-    def __init__(self, grid, f):
+    def __init__(self, grid, f, method="cubic"):
         """
         Create an interpolating function for the array data.
 
         Call the Interpolator object like a normal function to interpolate.
 
         Parameters
         ----------
         grid: Grid
             The grid on which the array f is meshed.
         f: numpy.ndarray
             The data to interpolate.
+        method: str
+            Interpolation order. May be 'linear', 'quadratic' or 'cubic'.
         """
         self.grid = grid
         if grid.ndims > 1:
-            self._inter = RegularGridInterpolator(grid.coords, f, method="cubic")
+            self._inter = RegularGridInterpolator(grid.coords, f, method=method)
         else:
-            self._inter = CubicSpline(grid.coords, f)
+            methods = {
+                "linear": 1,
+                "quadratic": 2,
+                "cubic": 3
+            }
+            # self._inter = UnivariateSpline(grid.coords, f, k=methods[method])
+            self._inter = interp1d(grid.coords, f, kind=method)
 
     def __call__(self, locations):
         """
         Return the interpolation for one or more points.
 
         Parameters
         ----------
```

### Comparing `numgrids-0.2.4/numgrids/plots.py` & `numgrids-0.3.0/numgrids/plots.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.4/numgrids.egg-info/PKG-INFO` & `numgrids-0.3.0/numgrids.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numgrids
-Version: 0.2.4
+Version: 0.3.0
 Summary: Working with numerical grids made easy.
 Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Platform: ALL
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: numgrids Version: 0.2.4 Summary: Working with
+Metadata-Version: 2.1 Name: numgrids Version: 0.3.0 Summary: Working with
 numerical grids made easy. Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer Author-email: matthias.r.baer@googlemail.com License: MIT
 Platform: ALL Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
                             ****** numgrids ******
                     Working with numerical grids made easy.
```

### Comparing `numgrids-0.2.4/setup.py` & `numgrids-0.3.0/setup.py`

 * *Files identical despite different names*


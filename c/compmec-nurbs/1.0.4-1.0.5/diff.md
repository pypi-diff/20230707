# Comparing `tmp/compmec_nurbs-1.0.4.tar.gz` & `tmp/compmec_nurbs-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compmec_nurbs-1.0.4.tar", max compression
+gzip compressed data, was "compmec_nurbs-1.0.5.tar", max compression
```

## Comparing `compmec_nurbs-1.0.4.tar` & `compmec_nurbs-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    35142 2023-07-05 10:35:21.767464 compmec_nurbs-1.0.4/LICENSE.md
--rw-r--r--   0        0        0     2142 2023-07-05 10:35:21.767464 compmec_nurbs-1.0.4/README.md
--rw-r--r--   0        0        0      543 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3316 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/__classes__.py
--rw-r--r--   0        0        0      175 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/__init__.py
--rw-r--r--   0        0        0    10541 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/algorithms.py
--rw-r--r--   0        0        0    12888 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/curves.py
--rw-r--r--   0        0        0     8153 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/functions.py
--rw-r--r--   0        0        0     8362 2023-07-05 10:35:21.771464 compmec_nurbs-1.0.4/src/compmec/nurbs/knotspace.py
--rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 compmec_nurbs-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35142 2023-07-07 20:30:37.558810 compmec_nurbs-1.0.5/LICENSE.md
+-rw-r--r--   0        0        0     2241 2023-07-07 20:30:37.558810 compmec_nurbs-1.0.5/README.md
+-rw-r--r--   0        0        0      543 2023-07-07 20:30:37.562810 compmec_nurbs-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2997 2023-07-07 20:30:37.562810 compmec_nurbs-1.0.5/src/compmec/nurbs/__classes__.py
+-rw-r--r--   0        0        0      212 2023-07-07 20:30:37.562810 compmec_nurbs-1.0.5/src/compmec/nurbs/__init__.py
+-rw-r--r--   0        0        0     2350 2023-07-07 20:30:37.562810 compmec_nurbs-1.0.5/src/compmec/nurbs/advanced.py
+-rw-r--r--   0        0        0     1787 2023-07-07 20:30:37.562810 compmec_nurbs-1.0.5/src/compmec/nurbs/calculus.py
+-rw-r--r--   0        0        0    11147 2023-07-07 20:30:37.562810 compmec_nurbs-1.0.5/src/compmec/nurbs/curves.py
+-rw-r--r--   0        0        0     6816 2023-07-07 20:30:37.570810 compmec_nurbs-1.0.5/src/compmec/nurbs/functions.py
+-rw-r--r--   0        0        0    12732 2023-07-07 20:30:37.570810 compmec_nurbs-1.0.5/src/compmec/nurbs/heavy.py
+-rw-r--r--   0        0        0     9752 2023-07-07 20:30:37.570810 compmec_nurbs-1.0.5/src/compmec/nurbs/knotspace.py
+-rw-r--r--   0        0        0     2734 1970-01-01 00:00:00.000000 compmec_nurbs-1.0.5/PKG-INFO
```

### Comparing `compmec_nurbs-1.0.4/LICENSE.md` & `compmec_nurbs-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `compmec_nurbs-1.0.4/README.md` & `compmec_nurbs-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,59 +3,60 @@
 [![Lint with Black][lintblack-img]][lintblack-url]
 [![Code Coverage][coverage-img]][coverage-url]
 
 [![PyPI Version][pypi-img]][pypi-url]
 [![Python Versions][pyversions-img]][pyversions-url]
 [![License: MIT][license-img]][license-url]
 
-A python package for [Non-Uniform rational B-Spline], parametrized geometry.
+A python package for [Non-Uniform rational B-Spline][nurbswiki-url], parametrized geometry.
 
 
 #### Features
 
 * [X] Knot Vector
 * [X] Base Functions
 * [X] Curves
-* [] Surface
 
 Operations
 
 * Knots
-    * Insertion
-    * Removal
-    * Clean
+    * [X] Insertion
+    * [X] Removal
+    * [X] Clean
 * Degree
-    * Increase
-    * Decrease
-    * Clean
-* Split and unite
+    * [X] Increase
+    * [X] Decrease
+    * [X] Clean
+* [X] Split curves
+* [X] Unite curves
 
 ## Install
 
-This library is available in [PyPI][pypilink]. To install it
+This library is available in [PyPI][pypi-url]. To install it
 
 ```
 pip install compmec-nurbs
 ```
 
 For more details, refer to the [documentation][docs-url].
 
 ### Documentation
 
 The documentation can be found at [compmec-nurbs.readthedocs.io][docs-url]
 
 
 ## Contribute
 
-Please use the [Issues][issueslink] or refer to the email ```compmecgit@gmail.com```
+Please use the [Issues][issues-url] or refer to the email ```compmecgit@gmail.com```
 
 <!-- Badges: -->
 
 <!-- Badges: -->
 
+[nurbswiki-url]: https://pt.wikipedia.org/wiki/NURBS
 [lintblack-img]: https://github.com/compmec/nurbs/actions/workflows/black.yaml/badge.svg
 [lintblack-url]: https://github.com/compmec/nurbs/actions/workflows/black.yaml
 [docs-img]: https://readthedocs.org/projects/compmec-nurbs/badge/?version=latest
 [docs-url]: https://compmec-nurbs.readthedocs.io/en/latest/?badge=latest
 [pypi-img]: https://img.shields.io/pypi/v/compmec-nurbs
 [pypi-url]: https://pypi.org/project/compmec-nurbs/
 [build-img]: https://github.com/compmec/nurbs/actions/workflows/build.yaml/badge.svg
```

### Comparing `compmec_nurbs-1.0.4/pyproject.toml` & `compmec_nurbs-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compmec-nurbs"
-version = "1.0.4"
+version = "1.0.5"
 description = ""
 readme = "README.md"
 authors = ["Carlos Adir <carlos.adir@gmail.com>"]
 packages = [{ include = "compmec/nurbs", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `compmec_nurbs-1.0.4/src/compmec/nurbs/__classes__.py` & `compmec_nurbs-1.0.5/src/compmec/nurbs/__classes__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import abc
-from typing import Any, Optional, Tuple, Union
+from typing import Tuple, Union
 
 import numpy as np
 
 
 class Intface_KnotVector(abc.ABC):
     @abc.abstractproperty
     def degree(self) -> int:
         raise NotImplementedError
 
     @abc.abstractproperty
     def npts(self) -> int:
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def verify_input_init(self, knotvector: Tuple[float]):
+    @abc.abstractproperty
+    def knots(self) -> Tuple[float]:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def verify_valid_span(self, u: Tuple[float]):
+    def __iter__(self):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def span(self, knot: np.ndarray) -> np.ndarray:
+    def __eq__(self, obj: object) -> bool:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def insert_knot(self, knot: float, times: Optional[int] = 1):
+    def __ne__(self, obj: object) -> bool:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def remove_knot(self, knot: float, times: Optional[int] = 1):
+    def shift(self, value: float):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __eq__(self, obj: object) -> bool:
+    def span(self, nodes: Union[float, np.ndarray]) -> Union[int, np.ndarray]:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __ne__(self, obj: object) -> bool:
+    def mult(self, nodes: Union[float, np.ndarray]) -> Union[int, np.ndarray]:
         raise NotImplementedError
 
 
 class Intface_Evaluator(abc.ABC):
     @abc.abstractproperty
-    def evalf(self) -> Union[int, slice]:
+    def eval(self) -> Union[int, slice]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def __call__(self, u: np.ndarray) -> np.ndarray:
         raise NotImplementedError
 
 
@@ -70,57 +70,49 @@
         raise NotImplementedError
 
     @abc.abstractproperty
     def npts(self) -> int:
         raise NotImplementedError
 
     @abc.abstractproperty
-    def knots(self) -> int:
+    def knots(self) -> Tuple[float]:
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def knot_insert(self, knot: float, times: Optional[int] = 1):
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def knot_remove(self, knot: float, times: Optional[int] = 1):
+    @abc.abstractproperty
+    def weights(self) -> Tuple[float]:
         raise NotImplementedError
 
-    @abc.abstractmethod
-    def degree_increase(self, times: Optional[int] = 1):
-        raise NotImplementedError
 
+class Intface_BaseFunction(Intface_BaseFunction_BaseCurve):
     @abc.abstractmethod
-    def degree_decrease(self, times: Optional[int] = 1):
+    def __init__(self, knotvector: Intface_KnotVector):
         raise NotImplementedError
 
-
-class Intface_BaseFunction(Intface_BaseFunction_BaseCurve):
     @abc.abstractmethod
-    def __init__(self, knotvector: Intface_KnotVector):
+    def eval(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __getitem__(self, tup: Any) -> Union[float, np.ndarray]:
+    def __getitem__(self, index) -> Intface_Evaluator:
         raise NotImplementedError
 
 
 class Intface_BaseCurve(Intface_BaseFunction_BaseCurve):
     @abc.abstractmethod
     def __init__(self, knotvector: Intface_KnotVector, ctrlpoints: np.ndarray):
         raise NotImplementedError
 
     @abc.abstractproperty
-    def F(self) -> Intface_BaseFunction:
-        raise NotImplementedError
-
-    @abc.abstractproperty
     def ctrlpoints(self) -> np.ndarray:
         raise NotImplementedError
 
     @abc.abstractmethod
     def knot_clean(self):
         raise NotImplementedError
 
     @abc.abstractmethod
     def degree_clean(self):
         raise NotImplementedError
+
+    @abc.abstractmethod
+    def eval(self):
+        raise NotImplementedError
```

### Comparing `compmec_nurbs-1.0.4/src/compmec/nurbs/algorithms.py` & `compmec_nurbs-1.0.5/src/compmec/nurbs/heavy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from typing import List, Tuple
+from typing import Tuple
 
 import numpy as np
 
-# from compmec.nurbs.functions import SplineFunction
-
 
 def N(i: int, j: int, k: int, u: float, U: Tuple[float]) -> float:
     """
     Returns the value of N_{ij}(u) in the interval [u_{k}, u_{k+1}]
     Remember that N_{i, j}(u) = 0   if  ( u not in [U[i], U[i+j+1]] )
     """
 
@@ -187,22 +185,42 @@
             for i in range(npts1):
                 for j, uj in enumerate(chebynodes):
                     Mvalues[i, j] = N(i, degree1, k1, uj, knotvect1)
             A += np.einsum("k,ik,jk->ij", integrator, Nvalues, Nvalues)
             B += np.einsum("k,ik,jk->ij", integrator, Nvalues, Mvalues)
             C += np.einsum("k,ik,jk->ij", integrator, Mvalues, Mvalues)
 
-        Cinv = np.linalg.inv(C)
-        T = Cinv @ B.T
+        T = np.linalg.solve(C, B.T)
         E = A - B @ T
         return T, E
 
 
 class KnotVector:
     @staticmethod
+    def is_valid_vector(knotvector: Tuple[float]) -> bool:
+        lenght = len(knotvector)
+        for i in range(lenght - 1):
+            if knotvector[i] > knotvector[i + 1]:
+                return False
+        knots = []
+        mults = []
+        for knot in knotvector:
+            if knot not in knots:
+                knots.append(knot)
+                mults.append(0)
+            ind = knots.index(knot)
+            mults[ind] += 1
+        if mults[0] != mults[-1]:
+            return False
+        for mult in mults:
+            if mult > mults[0]:
+                return False
+        return True
+
+    @staticmethod
     def find_degree(knotvector: Tuple[float]) -> int:
         degree = 0
         while knotvector[degree] == knotvector[degree + 1]:
             degree += 1
         return degree
 
     @staticmethod
@@ -227,58 +245,98 @@
             if knotvector[mid] <= node < knotvector[mid + 1]:
                 return mid
 
     @staticmethod
     def find_mult(node: float, knotvector: Tuple[float]) -> int:
         """
         #### Algorithm A2.1
-            Determine the knot span index
+            Returns how many times a knot is in knotvector
         #### Input:
-            ``npts``: int -- number of DOFs
-            ``degree``: int -- degree
-            ``u``: float -- knot value
-            ``U``: Tuple[float] -- knot vector
+            ``knotvector``: Tuple[float] -- knot vector
         #### Output:
-            ``s``: int -- Multiplicity of the knot
+            ``m``: int -- Multiplicity of the knot
         """
         mult = 0
         for knot in knotvector:
             if abs(knot - node) < 1e-9:
                 mult += 1
         return mult
 
     @staticmethod
     def find_knots(knotvector: Tuple[float]) -> Tuple[float]:
         """
-        #### Algorithm A2.1
-            Determine the knot span index
+        ####
+            Returns a tuple with non repeted knots
         #### Input:
             ``npts``: int -- number of DOFs
             ``degree``: int -- degree
             ``u``: float -- knot value
             ``U``: Tuple[float] -- knot vector
         #### Output:
             ``s``: int -- Multiplicity of the knot
         """
         knots = []
         for knot in knotvector:
             if knot not in knots:
                 knots.append(knot)
         return knots
 
-    def add_knot(node: float, knotvector: Tuple[float]):
+    @staticmethod
+    def insert_knots(knotvector: Tuple[float], addknots: Tuple[float]) -> Tuple[float]:
         """
-        Add the node inside the knotvector
+        Returns a new knotvector which contains the previous and new knots.
+        This function don't do the validation
         """
-        span = KnotVector.find_span(node, knotvector)
-        knotvector = list(knotvector)
-        knotvector.insert(span, node)
-        return tuple(knotvector)
+        newknotvector = list(knotvector) + list(addknots)
+        newknotvector.sort()
+        return tuple(newknotvector)
+
+    @staticmethod
+    def remove_knots(knotvector: Tuple[float], subknots: Tuple[float]) -> Tuple[float]:
+        newknotvector = list(knotvector)
+        for knot in subknots:
+            newknotvector.remove(knot)
+        return tuple(newknotvector)
 
-    def split(knotvector: Tuple[float], nodes: Tuple[float]) -> List[Tuple[float]]:
+    @staticmethod
+    def unite_vectors(vector0: Tuple[float], vector1: Tuple[float]) -> Tuple[float]:
+        all_knots = list(set(vector0) | set(vector1))
+        all_mults = [0] * len(all_knots)
+        for vector in [vector0, vector1]:
+            for knot in vector:
+                index = all_knots.index(knot)
+                mult = KnotVector.find_mult(knot, vector)
+                if mult > all_mults[index]:
+                    all_mults[index] = mult
+        final_vector = []
+        for knot, mult in zip(all_knots, all_mults):
+            final_vector += [knot] * mult
+        final_vector.sort()
+        return tuple(final_vector)
+
+    @staticmethod
+    def intersect_vectors(vector0: Tuple[float], vector1: Tuple[float]) -> Tuple[float]:
+        all_knots = list(set(vector0) & set(vector1))
+        all_mults = [9999] * len(all_knots)
+        for vector in [vector0, vector1]:
+            for knot in vector:
+                if knot not in all_knots:
+                    continue
+                index = all_knots.index(knot)
+                mult = KnotVector.find_mult(knot, vector)
+                if mult < all_mults[index]:
+                    all_mults[index] = mult
+        final_vector = []
+        for knot, mult in zip(all_knots, all_mults):
+            final_vector += [knot] * mult
+        final_vector.sort()
+        return tuple(final_vector)
+
+    @staticmethod
+    def split(knotvector: Tuple[float], nodes: Tuple[float]) -> Tuple[Tuple[float]]:
         """
         It splits the knotvector at nodes.
         You may put initial and final values.
         Example:
             >> U = [0, 0, 0.5, 1, 1]
             >> split(U, [0.5])
             [[0, 0, 0.5, 0.5],
@@ -298,8 +356,8 @@
         nodes = list(set(nodes))
         nodes.sort()
         degree = np.sum(knotvector == minu) - 1
         for a, b in zip(nodes[:-1], nodes[1:]):
             middle = list(knotvector[(a < knotvector) * (knotvector < b)])
             newknotvect = (degree + 1) * [a] + middle + (degree + 1) * [b]
             retorno.append(newknotvect)
-        return retorno
+        return tuple(retorno)
```

### Comparing `compmec_nurbs-1.0.4/src/compmec/nurbs/curves.py` & `compmec_nurbs-1.0.5/src/compmec/nurbs/curves.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,129 +1,52 @@
+from __future__ import annotations
+
 from typing import Optional, Tuple, Union
 
 import numpy as np
 
-from compmec.nurbs import algorithms as algo
+from compmec.nurbs import heavy
 from compmec.nurbs.__classes__ import Intface_BaseCurve
 from compmec.nurbs.functions import Function
 from compmec.nurbs.knotspace import KnotVector
 
 
 class BaseCurve(Intface_BaseCurve):
     def __init__(self, knotvector: KnotVector):
-        self.knotvector = KnotVector(knotvector)
-
-    def deepcopy(self) -> Intface_BaseCurve:
-        curve = self.__class__(self.knotvector)
-        curve.ctrlpoints = self.ctrlpoints
-        return curve
-
-    def __call__(self, u: np.ndarray) -> np.ndarray:
-        return self.evaluate(u)
-
-    def evaluate(self, u: np.ndarray) -> np.ndarray:
-        if self.ctrlpoints is None:
-            error_msg = "Cannot evaluate: There are no control points"
-            raise ValueError(error_msg)
-        L = self.F(u)
-        return np.moveaxis(L, 0, -1) @ self.ctrlpoints
-
-    @property
-    def knotvector(self):
-        return KnotVector(self.__knotvector)
-
-    @property
-    def degree(self):
-        return self.knotvector.degree
-
-    @property
-    def npts(self):
-        return self.knotvector.npts
-
-    @property
-    def knots(self):
-        return self.knotvector.knots
+        self.__ctrlpoints = None
+        self.__weights = None
+        self.__knotvector = KnotVector(knotvector)
 
-    @property
-    def ctrlpoints(self):
-        return self.__ctrlpoints
-
-    @knotvector.setter
-    def knotvector(self, value: KnotVector):
-        self.__knotvector = KnotVector(value)
-
-    @degree.setter
-    def degree(self, value: int):
-        value = int(value)
-        if value < 1:
-            raise ValueError("The degree must be 1 or higher!")
-        if value == self.degree:
-            return
-        if value > self.degree:
-            self.__degree_increase(value - self.degree)
-        else:
-            self.__degree_decrease(self.degree - value)
-
-    @ctrlpoints.setter
-    def ctrlpoints(self, value: np.ndarray):
-        if value is None:
-            self.__ctrlpoints = None
-            return
-        try:
-            iter(value)
-        except Exception:
-            raise ValueError
-        if len(value) != self.npts:
-            error_msg = "The number of control points must be the same as"
-            error_msg += " degrees of freedom of KnotVector.\n"
-            error_msg += f"  knotvector.npts = {self.npts}"
-            error_msg += f"  len(ctrlpoints) = {len(value)}"
-            raise ValueError(error_msg)
-        try:
-            1.0 * value[0] - 1.5 * value[0] + 3.1 * value[0]
-        except Exception:
-            error_msg = "For each control point P, it's needed operations"
-            error_msg = "with floats like 1.0*P - 1.5*P + 3.1*P"
-            raise ValueError(error_msg)
-        self.__ctrlpoints = value
+    def __call__(self, nodes: np.ndarray) -> np.ndarray:
+        return self.eval(nodes)
 
     def __eq__(self, other: object) -> bool:
-        if type(self) != type(other):
+        if type(self) is not type(other):
             return False
         if self.knotvector[0] != other.knotvector[0]:
             return False
         if self.knotvector[-1] != other.knotvector[-1]:
             return False
+        newknotvec = self.knotvector | other.knotvector
         selfcopy = self.deepcopy()
+        selfcopy.knotvector = newknotvec
         othercopy = other.deepcopy()
-        maxdegree = max(self.degree, other.degree)
-        selfcopy.degree = maxdegree
-        othercopy.degree = maxdegree
-        allknots = list(selfcopy.knots) + list(othercopy.knots)
-        allknots = list(set(allknots))
-        allknots.sort()
-        for knot in allknots[1:-1]:
-            multself = selfcopy.knotvector.mult(knot)
-            multother = othercopy.knotvector.mult(knot)
-            diff = multself - multother
-            if diff > 0:
-                othercopy.knot_insert(diff * [knot])
-            elif diff < 0:
-                selfcopy.knot_insert((-diff) * [knot])
-        # Now the knotvectors are equal
+        othercopy.knotvector = newknotvec
         diffctrlpoints = selfcopy.ctrlpoints - othercopy.ctrlpoints
-        if np.all(np.abs(diffctrlpoints) > 1e-9):
+        if np.any(np.abs(diffctrlpoints) > 1e-9):
             return False
         return True
 
     def __ne__(self, obj: object):
         return not self.__eq__(obj)
 
     def __neg__(self):
-        return self.__class__(self.knotvector, np.copy(-self.ctrlpoints))
+        newcurve = self.deepcopy()
+        newcurve.ctrlpoints *= -1
+        return newcurve
 
     def __add__(self, obj: object):
         if type(self) != type(obj):
             error_msg = f"Cannot sum a {type(obj)} object with"
             error_msg += f" a {self.__class__} object"
             raise TypeError(error_msg)
         if self.knotvector != obj.knotvector:
@@ -163,180 +86,218 @@
         newknotvector = KnotVector(newknotvector)
         newshape = [npts0 + npts1 - 1] + list(self.ctrlpoints.shape[1:])
         newctrlpoints = np.zeros(newshape, dtype="float64")
         newctrlpoints[:npts0] = selfcopy.ctrlpoints[:npts0]
         newctrlpoints[npts0:] = othercopy.ctrlpoints[1:]
         return self.__class__(newknotvector, newctrlpoints)
 
-    def knot_insert(self, nodes: Union[float, Tuple[float]]) -> None:
-        nodes = np.array(nodes, dtype="float64").flatten()
-        newknotvector = np.array(self.knotvector).tolist()
+    @property
+    def knotvector(self):
+        return self.__knotvector
 
-        newknotvector.extend(nodes)
-        newknotvector.sort()
-        newknotvector = KnotVector(newknotvector)
-        T, _ = algo.LeastSquare.spline(self.knotvector, newknotvector)
-        newcontrolpoints = T @ self.ctrlpoints
-        self.__knotvector = KnotVector(newknotvector)
-        self.ctrlpoints = newcontrolpoints
+    @property
+    def degree(self):
+        return self.knotvector.degree
 
-    def knot_remove(
-        self, nodes: Union[float, Tuple[float]], tolerance: float = 1e-9
-    ) -> None:
-        nodes = np.array(nodes, dtype="float64").flatten()
-        nodes_requested = list(set(list(nodes)))
-        newknotvector = list(self.knotvector)
-        for node in nodes_requested:
-            if node not in self.knots:
-                error_msg = f"Requested remove ({node:.3f}),"
-                error_msg += " which it's not in knotvector"
-                raise ValueError(error_msg)
-        times_requested = [sum(abs(nodes - node) < 1e-9) for node in nodes]
-        for node, times in zip(nodes_requested, times_requested):
-            mult = self.knotvector.mult(node)
-            if times > mult:
-                error_msg = f"Requested remove {times} times the node "
-                error_msg += f"{node:.3f}, but only {mult} available."
-                raise ValueError(error_msg)
-            for i in range(times):
-                newknotvector.remove(node)
-        newknotvector = KnotVector(newknotvector)
-        T, E = algo.LeastSquare.spline(self.knotvector, newknotvector)
+    @property
+    def npts(self):
+        return self.knotvector.npts
+
+    @property
+    def knots(self):
+        return self.knotvector.knots
+
+    @property
+    def weights(self):
+        return self.__weights
+
+    @property
+    def ctrlpoints(self):
+        return self.__ctrlpoints
+
+    @knotvector.setter
+    def knotvector(self, value: KnotVector):
+        self.update_knotvector(value)
+
+    @degree.setter
+    def degree(self, value: int):
+        newknotvector = self.knotvector.deepcopy()
+        newknotvector.degree = int(value)
+        self.knotvector = newknotvector
+
+    @weights.setter
+    def weights(self, value: Tuple[float]):
+        if value is None:
+            self.__weights = None
+            return
+        array = np.array(value, dtype="float64")
+        if not np.all(array > 0):
+            raise ValueError("All weights must be > 0")
+        if array.shape != (self.npts,):
+            error_msg = "Weights must be a 1D array with "
+            error_msg += f"{self.npts} points"
+            raise ValueError(error_msg)
+        self.__weights = tuple(value)
+
+    @ctrlpoints.setter
+    def ctrlpoints(self, value: np.ndarray):
+        if value is None:
+            self.__ctrlpoints = None
+            return
+        try:
+            iter(value)
+        except Exception:
+            raise ValueError
+        if len(value) != self.npts:
+            error_msg = "The number of control points must be the same as"
+            error_msg += " degrees of freedom of KnotVector.\n"
+            error_msg += f"  knotvector.npts = {self.npts}"
+            error_msg += f"  len(ctrlpoints) = {len(value)}"
+            raise ValueError(error_msg)
+        try:
+            1.0 * value[0] - 1.5 * value[0] + 3.1 * value[0]
+        except Exception:
+            error_msg = "For each control point P, it's needed operations"
+            error_msg += "with floats like 1.0*P - 1.5*P + 3.1*P"
+            raise ValueError(error_msg)
+        self.__ctrlpoints = value
+
+    def deepcopy(self) -> Curve:
+        curve = self.__class__(self.knotvector)
+        curve.ctrlpoints = self.ctrlpoints
+        curve.weights = self.weights
+        return curve
+
+    def update_knotvector(self, newvector: KnotVector, tolerance: float = 1e-9):
+        newvector = KnotVector(newvector)
+        if newvector == self.knotvector:
+            return
+        if self.ctrlpoints is None:
+            self.__knotvector = newvector
+            return
+        oldvec, newvec = tuple(self.knotvector), tuple(newvector)
+        T, E = heavy.LeastSquare.spline(oldvec, newvec)
         error = np.moveaxis(self.ctrlpoints, 0, -1) @ E @ self.ctrlpoints
         error = np.max(np.abs(error))
-        if error > tolerance:
-            error_msg = f"Cannot remove the nodes {nodes} cause the "
-            error_msg += f" error ({error:.1e}) is > {tolerance:.1e} "
+        if tolerance and error > tolerance:
+            error_msg = "Cannot update knotvector cause error is "
+            error_msg += f" {error} > {tolerance}"
             raise ValueError(error_msg)
         newctrlpoints = T @ self.ctrlpoints
-        self.__knotvector = KnotVector(newknotvector)
+        self.__knotvector = newvector
         self.ctrlpoints = newctrlpoints
 
-    def knot_clean(self, tolerance: float = 1e-9) -> None:
+
+class Curve(BaseCurve):
+    def __init__(
+        self,
+        knotvector: KnotVector,
+        ctrlpoints: Optional[np.ndarray] = None,
+        weights: Optional[np.ndarray] = None,
+    ):
+        super().__init__(knotvector)
+        self.ctrlpoints = ctrlpoints
+        self.weights = weights
+
+    def eval(self, nodes: np.ndarray) -> np.ndarray:
+        if self.ctrlpoints is None:
+            error_msg = "Cannot evaluate: There are no control points"
+            raise ValueError(error_msg)
+        tempfunction = Function(self.knotvector)
+        tempfunction.weights = self.weights
+        matrix = tempfunction(nodes)
+        return np.moveaxis(matrix, 0, -1) @ self.ctrlpoints
+
+    def knot_insert(self, nodes: Union[float, Tuple[float]]) -> None:
+        nodes = np.array(nodes, dtype="float64").flatten()
+        newknotvec = self.knotvector.deepcopy() + tuple(nodes)
+        self.update_knotvector(newknotvec)
+
+    def knot_remove(
+        self, nodes: Union[float, Tuple[float]], tolerance: float = 1e-9
+    ) -> None:
+        nodes = np.array(nodes, dtype="float64").flatten()
+        newknotvec = self.knotvector.deepcopy() - tuple(nodes)
+        self.update_knotvector(newknotvec, tolerance)
+
+    def knot_clean(
+        self, nodes: Optional[Tuple[float]] = None, tolerance: float = 1e-9
+    ) -> None:
         """
-        Remove all unecessary knots.
+        Remove all unnecessary knots.
+        If no nodes are given, it tries to remove all internal knots
         If removing the knot the error is bigger than the tolerance,
         nothing happens
         """
-        internal_knots = self.knotvector.knots[1:-1]
-        for knot in internal_knots:
+        if nodes is None:
+            nodes = self.knotvector.knots
+        umin, umax = self.knotvector[0], self.knotvector[1]
+        nodes = tuple(set(nodes) - set((umin, umax)))
+        for knot in nodes:
             try:
                 while True:
                     self.knot_remove(knot, tolerance)
             except ValueError:
                 pass
 
-    def __degree_increase(self, times: int):
-        newknotvector = list(self.knotvector) + times * list(self.knots)
-        newknotvector.sort()
-        T, _ = algo.LeastSquare.spline(self.knotvector, newknotvector)
-        newctrlpoints = T @ self.ctrlpoints
-        self.__knotvector = KnotVector(newknotvector)
-        self.ctrlpoints = newctrlpoints
-
-    def __degree_decrease(self, times: int = 1, tolerance: float = 1e-9):
-        newknotvector = list(self.knotvector)
-        for knot in self.knots:
-            mult = min(times, self.knotvector.mult(knot))
-            for i in range(mult):
-                newknotvector.remove(knot)
-        T, E = algo.LeastSquare.spline(self.knotvector, newknotvector)
-        error = np.moveaxis(self.ctrlpoints, 0, -1) @ E @ self.ctrlpoints
-        error = np.max(np.abs(error))
-        if error > tolerance:
-            error_msg = f"Cannot reduce degree {times} times "
-            error_msg += f"cause the error ({error:.1e}) is > {tolerance:.1e} "
-            raise ValueError(error_msg)
-        newctrlpoints = T @ self.ctrlpoints
-        self.__knotvector = newknotvector
-        self.ctrlpoints = newctrlpoints
-
-    def degree_decrease(self, times: Optional[int] = 1):
+    def degree_increase(self, times: Optional[int] = 1):
         """
-        The same as mycurve.degree -= 1
+        The same as mycurve.degree += times
         But this function forces the degree reductions without looking the error
         """
-        self.degree -= times
+        newknotvec = self.knotvector.deepcopy()
+        newknotvec.degree += times
+        self.update_knotvector(newknotvec)
 
-    def degree_increase(self, times: Optional[int] = 1):
+    def degree_decrease(
+        self, times: Optional[int] = 1, tolerance: Optional[float] = 1e-9
+    ):
         """
-        The same as mycurve.degree += times
+        The same as mycurve.degree -= 1
         But this function forces the degree reductions without looking the error
         """
-        self.degree += times
+        newknotvec = self.knotvector.deepcopy()
+        newknotvec.degree -= times
+        self.update_knotvector(newknotvec, tolerance)
 
     def degree_clean(self, tolerance: float = 1e-9):
         """
         Reduces au maximum the degree of the curve received the tolerance.
         If the reduced degree error is bigger than the tolerance, nothing happen
         """
         try:
             while True:
-                self.__degree_decrease(1, tolerance)
+                self.degree_decrease(1, tolerance)
         except ValueError:
             pass
 
-    def split(
-        self, nodes: Optional[Union[float, np.ndarray]] = None
-    ) -> Tuple[Intface_BaseCurve]:
+    def split(self, nodes: Optional[Union[float, np.ndarray]] = None) -> Tuple[Curve]:
         """
         Separate the current spline at specified knots
         If no arguments are given, it splits at every knot and
             returns a list of bezier curves
         """
         if nodes is None:  # split into beziers
             if self.degree + 1 == self.npts:  # already bezier
                 return (self.deepcopy(),)
             return self.split(self.knots)
-        nodes = np.array(nodes, dtype="float64").flatten()
-        nodes = list(nodes) + [self.knotvector[0], self.knotvector[-1]]
-        nodes = list(set(nodes))
+        nodes = set(np.array(nodes, dtype="float64").flatten())
+        nodes |= set([self.knotvector[0], self.knotvector[-1]])
+        nodes = list(nodes)
         nodes.sort()
-        copycurve = self.deepcopy()
+        newvector = self.knotvector.deepcopy()
         for node in nodes[1:-1]:
-            mult = self.knotvector.mult(node)
-            copycurve.knot_insert((self.degree - mult) * [node])
-
-        allknotvec = algo.KnotVector.split(self.knotvector, nodes)
+            mult = newvector.mult(node)
+            newvector += (self.degree - mult) * [node]
+        copycurve = self.deepcopy()
+        copycurve.update_knotvector(newvector)
+        allknotvec = heavy.KnotVector.split(tuple(self.knotvector), nodes)
         listcurves = [0] * len(allknotvec)
         for i, newknotvec in enumerate(allknotvec):
-            nodeinf, nodesup = nodes[i], nodes[i + 1]
-            lowerind = copycurve.knotvector.span(nodeinf) - self.degree
-            if nodesup < self.knotvector[-1]:
-                upperind = copycurve.knotvector.span(nodesup) - self.degree + 1
-            else:
-                upperind = None
+            lowerind = copycurve.knotvector.span(nodes[i]) - self.degree
+            upperind = lowerind + len(newknotvec) - self.degree - 1
             newctrlpts = copycurve.ctrlpoints[lowerind:upperind]
             newcurve = self.__class__(newknotvec, newctrlpts)
+            newcurve.knot_clean()
             listcurves[i] = newcurve
         del copycurve
         return tuple(listcurves)
-
-
-class Curve(BaseCurve):
-    def __init__(
-        self,
-        knotvector: KnotVector,
-        ctrlpoints: Optional[np.ndarray] = None,
-        weights: Optional[np.ndarray] = None,
-    ):
-        super().__init__(knotvector)
-        self.ctrlpoints = ctrlpoints
-        self.weights = weights
-
-    @property
-    def F(self):
-        function = Function(self.knotvector)
-        return function
-
-    def deepcopy(self):
-        curve = super().deepcopy()
-        curve.weights = self.weights
-        return curve
-
-    @property
-    def weights(self):
-        return self.__weights
-
-    @weights.setter
-    def weights(self, value: Tuple[float]):
-        self.__weights = value
```

### Comparing `compmec_nurbs-1.0.4/src/compmec/nurbs/functions.py` & `compmec_nurbs-1.0.5/src/compmec/nurbs/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,102 @@
-import abc
-from typing import Any, Optional, Tuple, Union
+from __future__ import annotations
+
+from typing import Tuple, Union
 
 import numpy as np
 
+from compmec.nurbs import heavy
 from compmec.nurbs.__classes__ import Intface_BaseFunction, Intface_Evaluator
-from compmec.nurbs.algorithms import N, R
 from compmec.nurbs.knotspace import KnotVector
 
 
 class BaseFunction(Intface_BaseFunction):
     def __init__(self, knotvector: KnotVector):
-        self.__knotvector = KnotVector(knotvector)
+        self.knotvector = knotvector
         self.weights = None
-        self.__degree = self.knotvector.degree
 
     def __eq__(self, other: Intface_BaseFunction) -> bool:
         if not isinstance(other, Intface_BaseFunction):
             return False
-        if self.degree != other.degree:
-            return False
         if self.knotvector != other.knotvector:
             return False
         weightleft = self.weights
         weightrigh = other.weights
         weightleft = np.ones(self.npts) if self.weights is None else self.weights
         weightrigh = np.ones(self.npts) if weightrigh is None else weightrigh
         return np.all(weightleft == weightrigh)
 
     def __ne__(self, other: Intface_BaseFunction) -> bool:
         return not self.__eq__(other)
 
+    def __call__(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        return self.eval(nodes)
+
     @property
     def knotvector(self) -> KnotVector:
         return self.__knotvector
 
     @property
     def degree(self) -> int:
-        return self.__degree
+        return self.knotvector.degree
 
     @property
     def npts(self) -> int:
         return self.knotvector.npts
 
     @property
     def knots(self) -> Tuple[float]:
         return self.knotvector.knots
 
     @property
     def weights(self) -> Union[Tuple[float], None]:
         return self.__weights
 
+    @degree.setter
+    def degree(self, value: int):
+        value = int(value)
+        self.knotvector.degree = value
+
+    @knotvector.setter
+    def knotvector(self, value: KnotVector):
+        self.__knotvector = KnotVector(value)
+
     @weights.setter
     def weights(self, value: Tuple[float]):
         if value is None:
             self.__weights = None
             return
         value = np.array(value, dtype="float64")
         if not np.all(value > 0):
             error_msg = "All weights must be positive!"
             raise ValueError(error_msg)
         if value.shape != (self.npts,):
             error_msg = f"Weights shape invalid! {value.shape} != ({self.npts})"
             raise ValueError(error_msg)
         self.__weights = value
 
-    @degree.setter
-    def degree(self, value: int):
-        self.__degree = int(value)
-
-    def knot_insert(self, knot: float, times: Optional[int] = 1):
-        self.knotvector.knot_insert(knot, times)
-
-    def knot_remove(self, knot: float, times: Optional[int] = 1):
-        self.knotvector.knot_remove(knot, times)
-
-    def degree_increase(self, times: Optional[int] = 1):
-        pass
-
-    def degree_decrease(self, times: Optional[int] = 1):
-        pass
-
-    @abc.abstractmethod
-    def evalf(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        raise NotImplementedError
-
-    def __call__(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        return self.evalf(nodes)
+    def deepcopy(self) -> BaseFunction:
+        newfunc = self.__class__(self.knotvector)
+        newfunc.weights = self.weights
+        return newfunc
 
 
 class FunctionEvaluator(Intface_Evaluator):
     def __init__(self, func: BaseFunction, i: Union[int, slice], j: int):
         self.__knotvector = func.knotvector
         self.__weights = func.weights
         self.__first_index = i
         self.__second_index = j
 
     def compute_one_value(self, i: int, node: float, span: int) -> float:
         j = self.__second_index
         U = tuple(self.__knotvector)
         if self.__weights is None:
-            return N(i, j, span, node, U)
-        return R(i, j, span, node, U, self.__weights)
+            return heavy.N(i, j, span, node, U)
+        return heavy.R(i, j, span, node, U, self.__weights)
 
     def compute_vector(self, node: float, span: int) -> np.ndarray:
         """
         Given a 'u' float, it returns the vector with all BasicFunctions:
         compute_vector(u, span) = [F_{0j}(u), F_{1j}(u), ..., F_{npts-1,j}(u)]
         """
         npts = self.__knotvector.npts
@@ -125,40 +117,37 @@
         nodes = np.array(nodes, dtype="float64")
         newshape = [self.__knotvector.npts] + list(nodes.shape)
         result = np.zeros(newshape, dtype="float64")
         for i, (nodei, spani) in enumerate(zip(nodes, spans)):
             result[:, i] = self.compute_vector(nodei, spani)
         return result
 
-    def __evalf(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+    def __eval(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
         """
-        If i is integer, u is float -> float
-        If i is integer, u is np.ndarray, ndim = k -> np.ndarray, ndim = k
-        If i is slice, u is float -> 1D np.ndarray
-        if i is slice, u is np.ndarray, ndim = k -> np.ndarray, ndim = k+1
+        Private and unprotected method of eval
         """
         nodes = np.array(nodes, dtype="float64")
         flat_nodes = nodes.flatten()
         flat_spans = self.__knotvector.span(flat_nodes)
         flat_spans = np.array(flat_spans, dtype="int16")
         newshape = [self.__knotvector.npts] + list(nodes.shape)
         result = self.compute_matrix(flat_nodes, flat_spans)
         return result.reshape(newshape)
 
-    def evalf(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+    def eval(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
         """
         If i is integer, u is float -> float
         If i is integer, u is np.ndarray, ndim = k -> np.ndarray, ndim = k
         If i is slice, u is float -> 1D np.ndarray
         if i is slice, u is np.ndarray, ndim = k -> np.ndarray, ndim = k+1
         """
-        return self.__evalf(nodes)[self.__first_index]
+        return self.__eval(nodes)[self.__first_index]
 
     def __call__(self, nodes: np.ndarray) -> np.ndarray:
-        return self.evalf(nodes)
+        return self.eval(nodes)
 
 
 class IndexableFunction(BaseFunction):
     def __init__(self, knotvector: KnotVector):
         super().__init__(knotvector)
 
     def __valid_first_index(self, index: Union[int, slice]):
@@ -173,58 +162,31 @@
         if not isinstance(index, int):
             raise TypeError
         if not (0 <= index <= self.degree):
             error_msg = f"Second index (={index}) "
             error_msg += f"must be in [0, {self.degree}]"
             raise IndexError(error_msg)
 
-    def __getitem__(self, tup: Any):
-        if isinstance(tup, tuple):
-            if len(tup) > 2:
+    def __getitem__(self, index) -> FunctionEvaluator:
+        if isinstance(index, tuple):
+            if len(index) > 2:
                 raise IndexError
-            i, j = tup
+            i, j = index
         else:
-            i, j = tup, self.degree
+            i, j = index, self.degree
         self.__valid_first_index(i)
         self.__valid_second_index(j)
         return FunctionEvaluator(self, i, j)
 
-
-class DerivableFunction(IndexableFunction):
-    def __init__(self, knotvector: KnotVector):
-        super().__init__(knotvector)
-        self.__matrix = np.eye(self.npts, dtype="float64")
-
-    @property
-    def matrix(self) -> np.ndarray:
-        return np.copy(self.__matrix)
-
-    def derivate(self):
-        """
-        Derivates the function once. If you want more, call it in a loop
-        """
-        avals = np.zeros(self.npts)
-        for i in range(self.npts):
-            diff = (
-                self.knotvector[i + self.degree] - self.knotvector[i]
-            )  # Maybe it's wrong
-            if diff != 0:
-                avals[i] = self.degree / diff
-        newA = np.diag(avals)
-        for i in range(self.npts - 1):
-            newA[i, i + 1] = -avals[i + 1]
-        self.__matrix = self.__matrix @ newA
-        self.degree -= 1
-
-    def evalf(self, nodes: np.ndarray) -> np.ndarray:
+    def eval(self, nodes: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
         evaluator = self[:, self.degree]
-        return self.matrix @ evaluator(nodes)
+        return evaluator(nodes)
 
 
-class Function(DerivableFunction):
+class Function(IndexableFunction):
     def __doc__(self):
         """
         Spline and rational base function
         """
 
     def __repr__(self) -> str:
         if self.npts == self.degree + 1:
```

### Comparing `compmec_nurbs-1.0.4/src/compmec/nurbs/knotspace.py` & `compmec_nurbs-1.0.5/src/compmec/nurbs/knotspace.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Optional, Tuple, Union
+from __future__ import annotations
+
+from typing import Tuple, Union
 
 import numpy as np
 
-from compmec.nurbs import algorithms
+from compmec.nurbs import heavy
 from compmec.nurbs.__classes__ import Intface_KnotVector
 
 
 class ValidationKnotVector(object):
     @staticmethod
     def array1D(knotvector: Tuple[float]):
         knotvector = np.array(knotvector, "float64")
@@ -17,214 +19,251 @@
 
     @staticmethod
     def degree_npts(degree: int, npts: int):
         if not isinstance(degree, int):
             raise TypeError("Degree must be an integer")
         if not isinstance(npts, int):
             raise TypeError("Number of points must be integer")
-        if degree <= 0:
-            raise ValueError("Degree must be >= 1")
+        if degree < 0:
+            raise ValueError("Degree must be >= 0")
         if not (npts > degree):
             raise ValueError("Must have npts > degree")
 
     @staticmethod
     def all(knotvector: Tuple[float]) -> None:
         ValidationKnotVector.array1D(knotvector)
         knotvector = np.array(knotvector, dtype="float64")
-        # Ordered
-        sorted_array = np.copy(knotvector)
-        sorted_array.sort()
-        if np.any(knotvector != sorted_array):
-            raise ValueError("Knotvector must be ordored")
-        # Multiplicity
-        set_knotvector = list(set(knotvector.tolist()))
-        set_knotvector.sort()
-        multknots = [np.sum(knotvector == u) for u in set_knotvector]
-        if multknots[0] != multknots[-1]:
-            raise ValueError("Extremities quantities are not equal")
-        if len(multknots) == 2:  # No internal knot
-            return
-        if max(multknots[1:-1]) >= multknots[0]:
-            raise ValueError("An internal knot has multiplicity too high")
+        knotvector = tuple(knotvector)
+        if not heavy.KnotVector.is_valid_vector(knotvector):
+            error_msg = f"Knot Vector is invalid: {knotvector}"
+            raise ValueError(error_msg)
 
 
-class KnotVector(Intface_KnotVector, list):
+class KnotVector(Intface_KnotVector):
     def __init__(self, knotvector: Tuple[float]):
-        ValidationKnotVector.all(knotvector)
-        knotvector = np.array(knotvector)
-        degree = algorithms.KnotVector.find_degree(knotvector)
-        npts = algorithms.KnotVector.find_npts(knotvector)
-        self.__degree = degree
-        self.__npts = npts
-        super().__init__(knotvector)
+        if not isinstance(knotvector, self.__class__):
+            ValidationKnotVector.all(knotvector)
+        self.__update_vector(knotvector)
 
-    @property
-    def degree(self) -> int:
-        return int(self.__degree)
+    def __update_vector(self, newvector: Tuple[float]):
+        """
+        Unprotected private function to set newvector
+        """
+        self.__degree = None
+        self.__npts = None
+        self.__internal_vector = tuple(newvector)
+        return self
 
-    @property
-    def npts(self) -> int:
-        return int(self.__npts)
+    def __str__(self) -> str:
+        return str(self.__internal_vector)
 
-    @property
-    def knots(self) -> Tuple[float]:
-        values = list(set(list(self)))
-        values.sort()
-        return tuple(values)
+    def __repr__(self) -> str:
+        return str(self)
 
-    def deepcopy(self):
-        return self.__class__(list(self))
+    def __iter__(self) -> float:
+        for knot in self.__internal_vector:
+            yield knot
+
+    def __getitem__(self, index):
+        return self.__internal_vector[index]
+
+    def __len__(self) -> int:
+        return len(self.__internal_vector)
+
+    def __iadd__(self, other: Union[float, Tuple[float]]):
+        try:
+            return self.shift(other)
+        except TypeError:
+            return self.__insert_knots(tuple(other))
 
-    def __valid_knot(self, u: float):
+    def __isub__(self, other: Union[float, Tuple[float]]):
         try:
-            u = float(u)
-        except Exception:
-            raise TypeError
-        minU = self[0]
-        maxU = self[-1]
-        if u < minU:
-            raise ValueError(f"Received u = {u} < minU = {minU}")
-        if maxU < u:
-            raise ValueError(f"Received u = {u} > maxU = {maxU}")
-
-    def __valid_insert_knot(self, u: float, times: float):
-        if times <= 0:
-            raise ValueError
-        mult = self.mult_onevalue(u)
-        if times > self.degree - mult:
-            raise ValueError
-
-    def __valid_remove_knot(self, u: float, times: float):
-        if times <= 0:
-            raise ValueError
-        mult = self.mult_onevalue(u)
-        if times > mult:
-            raise ValueError
-
-    def span_onevalue(self, u: float) -> int:
-        self.__valid_knot(u)
-        vector = np.array(self)
-        lower = int(np.max(np.where(vector == self[0])))
-        upper = int(np.min(np.where(vector == self[-1])))
-        if u == self[0]:
-            return lower
-        if u == self[-1]:
-            return upper
-        mid = (lower + upper) // 2
-        while True:
-            if u < vector[mid]:
-                upper = mid
-            elif vector[mid + 1] <= u:
-                lower = mid
-            else:
-                return mid
-            mid = (lower + upper) // 2
-
-    def span(self, u: Union[float, np.ndarray]) -> Union[int, np.ndarray]:
-        u = np.array(u)
-        if u.ndim == 0:
-            return self.span_onevalue(u)
-        npts = u.shape[0]
-        result = [0] * (npts)
-        for i in range(npts):
-            result[i] = self.span(u[i])
-        return np.array(result, dtype="int16")
-
-    def mult_onevalue(self, u: float) -> int:
-        if u < self[0] or self[-1] < u:
-            raise ValueError("Outside interval")
-        return algorithms.KnotVector.find_mult(u, list(self))
-
-    def mult(self, u: Union[float, np.ndarray]) -> Union[int, np.ndarray]:
-        u = np.array(u)
-        if u.ndim == 0:
-            return self.mult_onevalue(u)
-        npts = u.shape[0]
-        result = np.zeros([npts] + list(u.shape[1:]), dtype="int16")
-        for i in range(npts):
-            result[i] = self.mult(u[i])
-        return result
-
-    def __knot_insert(self, knot: float, times: int):
-        if times == 1:
-            span = self.span_onevalue(knot)
-            copylist = list(self)
-            copylist.insert(span + 1, knot)
-            ValidationKnotVector.all(copylist)
-            self.insert(span + 1, knot)
-            degree = algorithms.KnotVector.find_degree(list(self))
-            npts = algorithms.KnotVector.find_npts(list(self))
-            ValidationKnotVector.degree_npts(degree, npts)
-            self.__degree = degree
-            self.__npts = npts
-            return
-        for i in range(times):
-            self.__knot_insert(knot, 1)
-
-    def __knot_remove(self, knot: float, times: int):
-        if times == 1:
-            span = self.span_onevalue(knot)
-            self.pop(span)
-            degree = algorithms.KnotVector.find_degree(list(self))
-            npts = algorithms.KnotVector.find_npts(list(self))
-            ValidationKnotVector.degree_npts(degree, npts)
-            self.__degree = degree
-            self.__npts = npts
-            return
-        for i in range(times):
-            self.__knot_remove(knot, 1)
-
-    def knot_insert(self, knot: float, times: Optional[int] = 1):
-        self.__valid_knot(knot)
-        self.__valid_insert_knot(knot, times)
-        self.__knot_insert(knot, times)
-
-    def knot_remove(self, knot: float, times: Optional[int] = 1):
-        self.__valid_knot(knot)
-        self.__valid_remove_knot(knot, times)
-        self.__knot_remove(knot, times)
-
-    def __eq__(self, obj: object):
-        if not isinstance(obj, self.__class__):
-            # Will try to cenvert obj
+            return self.shift(-other)
+        except TypeError:
+            return self.__remove_knots(tuple(other))
+
+    def __imul__(self, other: float):
+        return self.scale(other)
+
+    def __itruediv__(self, other: float):
+        return self.scale(1 / other)
+
+    def __ior__(self, other: KnotVector) -> KnotVector:
+        newvector = heavy.KnotVector.unite_vectors(tuple(self), tuple(other))
+        if not heavy.KnotVector.is_valid_vector(newvector):
+            raise ValueError("Cannot use __or__ in this case")
+        return self.__update_vector(newvector)
+
+    def __iand__(self, other: KnotVector) -> KnotVector:
+        newvector = heavy.KnotVector.intersect_vectors(tuple(self), tuple(other))
+        if not heavy.KnotVector.is_valid_vector(newvector):
+            raise ValueError("Cannot use __and__ in this case")
+        return self.__update_vector(newvector)
+
+    def __add__(self, other: Union[float, Tuple[float]]):
+        return self.deepcopy().__iadd__(other)
+
+    def __sub__(self, other: Union[float, Tuple[float]]):
+        return self.deepcopy().__isub__(other)
+
+    def __mul__(self, other: float):
+        return self.deepcopy().__imul__(other)
+
+    def __rmul__(self, other: float):
+        return self.deepcopy().__imul__(other)
+
+    def __truediv__(self, other: float):
+        return self.deepcopy().__itruediv__(other)
+
+    def __or__(self, other: float):
+        return self.deepcopy().__ior__(other)
+
+    def __and__(self, other: float):
+        return self.deepcopy().__iand__(other)
+
+    def __eq__(self, other: object):
+        if not isinstance(other, self.__class__):
+            # Will try to cenvert other
             try:
-                obj = self.__class__(obj)
+                other = self.__class__(other)
             except ValueError:
                 return False
-        if self.npts != obj.npts:
+        if self.npts != other.npts:
             return False
-        if self.degree != obj.degree:
+        if self.degree != other.degree:
             return False
         for i, v in enumerate(self):
-            if v != obj[i]:
+            if v != other[i]:
                 return False
         return True
 
-    def __ne__(self, __obj: object) -> bool:
-        return not (self == __obj)
+    def __ne__(self, other: object) -> bool:
+        return not self == other
+
+    @property
+    def degree(self) -> int:
+        if self.__degree is None:
+            self.__degree = heavy.KnotVector.find_degree(self)
+        return int(self.__degree)
+
+    @property
+    def npts(self) -> int:
+        if self.__npts is None:
+            self.__npts = heavy.KnotVector.find_npts(self)
+        return int(self.__npts)
+
+    @property
+    def knots(self) -> Tuple[float]:
+        return heavy.KnotVector.find_knots(tuple(self))
+
+    @degree.setter
+    def degree(self, value: int):
+        value = int(value)
+        knots = self.knots
+        diff = value - self.degree
+        if diff < 0:  # Decrease degree
+            self -= (-diff) * knots
+        if 0 < diff:  # Increase degree
+            self += diff * knots
+
+    def __insert_knots(self, knots: Tuple[float]):
+        newvector = heavy.KnotVector.insert_knots(tuple(self), knots)
+        if not heavy.KnotVector.is_valid_vector(newvector):
+            error_msg = f"Cannot insert knots {knots} in knotvector {self}"
+            raise ValueError(error_msg)
+        return self.__update_vector(newvector)
+
+    def __remove_knots(self, knots: Tuple[float]):
+        try:
+            newvector = heavy.KnotVector.remove_knots(tuple(self), knots)
+            if not heavy.KnotVector.is_valid_vector(newvector):
+                raise ValueError
+        except ValueError:
+            error_msg = f"Cannot remove knots {knots} in knotvector {self}"
+            raise ValueError(error_msg)
+        return self.__update_vector(newvector)
+
+    def deepcopy(self) -> KnotVector:
+        """
+        Returns a exact object, but with different ID
+        """
+        return self.__class__(self.__internal_vector)
+
+    def shift(self, value: float):
+        """
+        Moves every knot by an amount `value`
+        """
+        value = float(value)
+        newvector = tuple([knoti + value for knoti in self])
+        return self.__update_vector(newvector)
+
+    def scale(self, value: float) -> KnotVector:
+        """
+        Multiply every knot by amount `value`
+        """
+        value = float(value)
+        newvector = tuple([knoti * value for knoti in self])
+        return self.__update_vector(newvector)
+
+    def normalize(self) -> KnotVector:
+        """
+        Shift and scale the vector to match the interval [0, 1]
+        """
+        self.shift(-self[0])
+        self.scale(1 / self[-1])
+        return self
+
+    def span(self, nodes: Union[float, np.ndarray]) -> Union[int, np.ndarray]:
+        """
+        Finds the index position of
+        """
+        nodes = np.array(nodes, dtype="float64")
+        if np.any(nodes < self[0]) or np.any(self[-1] < nodes):
+            raise ValueError("Nodes outside interval knotvector")
+        flatnodes = nodes.flatten()
+        flatspans = np.empty(flatnodes.shape, dtype="int16")
+        for i, node in enumerate(flatnodes):
+            flatspans[i] = heavy.KnotVector.find_span(node, tuple(self))
+        return flatspans.reshape(nodes.shape)
+
+    def mult(self, nodes: Union[float, np.ndarray]) -> Union[int, np.ndarray]:
+        """
+        Counts how many times a node is inside the knotvector
+        """
+        nodes = np.array(nodes, dtype="float64")
+        if np.any(nodes < self[0]) or np.any(self[-1] < nodes):
+            raise ValueError("Nodes outside interval knotvector")
+        flatnodes = nodes.flatten()
+        flatspans = np.empty(flatnodes.shape, dtype="int16")
+        for i, node in enumerate(flatnodes):
+            flatspans[i] = heavy.KnotVector.find_mult(node, tuple(self))
+        return flatspans.reshape(nodes.shape)
 
 
 class GeneratorKnotVector:
     @staticmethod
     def bezier(degree: int) -> KnotVector:
-        npts = degree + 1
-        ValidationKnotVector.degree_npts(degree, npts)
+        ValidationKnotVector.degree_npts(degree, degree + 1)
         return KnotVector((degree + 1) * [0] + (degree + 1) * [1])
 
     @staticmethod
     def uniform(degree: int, npts: int) -> KnotVector:
         ValidationKnotVector.degree_npts(degree, npts)
         weights = np.ones(npts - degree)
-        return GeneratorKnotVector.weight(degree, weights)
+        knotvector = GeneratorKnotVector.weight(degree, weights)
+        knotvector.normalize()
+        return knotvector
 
     @staticmethod
     def random(degree: int, npts: int) -> KnotVector:
         ValidationKnotVector.degree_npts(degree, npts)
         weights = np.random.rand(npts - degree)
-        return GeneratorKnotVector.weight(degree, weights)
+        knotvector = GeneratorKnotVector.weight(degree, weights)
+        knotvector.shift(np.random.uniform(-1, 1))
+        return knotvector
 
     @staticmethod
     def weight(degree: int, weights: Tuple[float]) -> KnotVector:
         """
         Creates a KnotVector with degree ```degree``` and spaced points
         depending on the ```weights``` vectors.
         The number of segments are equal to lenght of weights
@@ -232,11 +271,10 @@
         degree = 1 and weights = [1] -> [0, 0, 1, 1]
         degree = 1 and weights = [1, 1] -> [0, 0, 0.5, 1, 1]
         degree = 1 and weights = [1, 1, 2] -> [0, 0.25, 0.5, 1, 1]
         """
         ValidationKnotVector.array1D(weights)
         npts = len(weights) + degree
         ValidationKnotVector.degree_npts(degree, npts)
-        cumsum = np.cumsum(weights)
-        listknots = [knot / cumsum[-1] for knot in cumsum]
-        knotvector = (degree + 1) * [0] + listknots + degree * [1]
+        listknots = list(np.cumsum(weights))
+        knotvector = (degree + 1) * [0] + listknots + degree * [listknots[-1]]
         return KnotVector(knotvector)
```

### Comparing `compmec_nurbs-1.0.4/PKG-INFO` & `compmec_nurbs-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compmec-nurbs
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: Carlos Adir
 Author-email: carlos.adir@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,59 +18,60 @@
 [![Lint with Black][lintblack-img]][lintblack-url]
 [![Code Coverage][coverage-img]][coverage-url]
 
 [![PyPI Version][pypi-img]][pypi-url]
 [![Python Versions][pyversions-img]][pyversions-url]
 [![License: MIT][license-img]][license-url]
 
-A python package for [Non-Uniform rational B-Spline], parametrized geometry.
+A python package for [Non-Uniform rational B-Spline][nurbswiki-url], parametrized geometry.
 
 
 #### Features
 
 * [X] Knot Vector
 * [X] Base Functions
 * [X] Curves
-* [] Surface
 
 Operations
 
 * Knots
-    * Insertion
-    * Removal
-    * Clean
+    * [X] Insertion
+    * [X] Removal
+    * [X] Clean
 * Degree
-    * Increase
-    * Decrease
-    * Clean
-* Split and unite
+    * [X] Increase
+    * [X] Decrease
+    * [X] Clean
+* [X] Split curves
+* [X] Unite curves
 
 ## Install
 
-This library is available in [PyPI][pypilink]. To install it
+This library is available in [PyPI][pypi-url]. To install it
 
 ```
 pip install compmec-nurbs
 ```
 
 For more details, refer to the [documentation][docs-url].
 
 ### Documentation
 
 The documentation can be found at [compmec-nurbs.readthedocs.io][docs-url]
 
 
 ## Contribute
 
-Please use the [Issues][issueslink] or refer to the email ```compmecgit@gmail.com```
+Please use the [Issues][issues-url] or refer to the email ```compmecgit@gmail.com```
 
 <!-- Badges: -->
 
 <!-- Badges: -->
 
+[nurbswiki-url]: https://pt.wikipedia.org/wiki/NURBS
 [lintblack-img]: https://github.com/compmec/nurbs/actions/workflows/black.yaml/badge.svg
 [lintblack-url]: https://github.com/compmec/nurbs/actions/workflows/black.yaml
 [docs-img]: https://readthedocs.org/projects/compmec-nurbs/badge/?version=latest
 [docs-url]: https://compmec-nurbs.readthedocs.io/en/latest/?badge=latest
 [pypi-img]: https://img.shields.io/pypi/v/compmec-nurbs
 [pypi-url]: https://pypi.org/project/compmec-nurbs/
 [build-img]: https://github.com/compmec/nurbs/actions/workflows/build.yaml/badge.svg
```


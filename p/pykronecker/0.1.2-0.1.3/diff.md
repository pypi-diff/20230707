# Comparing `tmp/pykronecker-0.1.2.tar.gz` & `tmp/pykronecker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykronecker-0.1.2.tar", last modified: Tue Jan 24 22:24:16 2023, max compression
+gzip compressed data, was "pykronecker-0.1.3.tar", last modified: Fri Jul  7 14:32:09 2023, max compression
```

## Comparing `pykronecker-0.1.2.tar` & `pykronecker-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-01-24 22:24:16.248060 pykronecker-0.1.2/
--rw-r--r--   0 ed        (1001) ed        (1001)     1068 2022-08-15 11:33:29.000000 pykronecker-0.1.2/LICENSE
--rw-rw-r--   0 ed        (1001) ed        (1001)     9192 2023-01-24 22:24:16.248060 pykronecker-0.1.2/PKG-INFO
--rw-rw-r--   0 ed        (1001) ed        (1001)     8278 2023-01-24 22:23:05.000000 pykronecker-0.1.2/README.md
--rw-r--r--   0 ed        (1001) ed        (1001)      226 2022-08-18 15:54:24.000000 pykronecker-0.1.2/pyproject.toml
--rw-rw-r--   0 ed        (1001) ed        (1001)     1171 2023-01-24 22:24:16.248060 pykronecker-0.1.2/setup.cfg
--rw-r--r--   0 ed        (1001) ed        (1001)       69 2022-08-16 13:31:08.000000 pykronecker-0.1.2/setup.py
-drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-01-24 22:24:16.236060 pykronecker-0.1.2/src/
-drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-01-24 22:24:16.244060 pykronecker-0.1.2/src/pykronecker/
--rw-rw-r--   0 ed        (1001) ed        (1001)      200 2022-09-22 16:41:27.000000 pykronecker-0.1.2/src/pykronecker/__init__.py
--rw-rw-r--   0 ed        (1001) ed        (1001)    11794 2023-01-24 22:23:05.000000 pykronecker-0.1.2/src/pykronecker/base.py
--rw-rw-r--   0 ed        (1001) ed        (1001)    11567 2023-01-24 22:23:05.000000 pykronecker-0.1.2/src/pykronecker/block.py
--rw-r--r--   0 ed        (1001) ed        (1001)     4326 2022-09-22 22:08:17.000000 pykronecker-0.1.2/src/pykronecker/composite.py
--rw-rw-r--   0 ed        (1001) ed        (1001)     7114 2022-11-11 15:45:32.000000 pykronecker-0.1.2/src/pykronecker/fast_math.py
--rw-rw-r--   0 ed        (1001) ed        (1001)    14839 2022-10-19 10:32:51.000000 pykronecker-0.1.2/src/pykronecker/operators.py
--rw-rw-r--   0 ed        (1001) ed        (1001)     2012 2022-09-22 16:41:27.000000 pykronecker-0.1.2/src/pykronecker/utils.py
-drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-01-24 22:24:16.248060 pykronecker-0.1.2/src/pykronecker.egg-info/
--rw-r--r--   0 ed        (1001) ed        (1001)     9192 2023-01-24 22:24:16.000000 pykronecker-0.1.2/src/pykronecker.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1001) ed        (1001)      472 2023-01-24 22:24:16.000000 pykronecker-0.1.2/src/pykronecker.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1001) ed        (1001)        1 2023-01-24 22:24:16.000000 pykronecker-0.1.2/src/pykronecker.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1001) ed        (1001)        1 2022-08-15 11:32:42.000000 pykronecker-0.1.2/src/pykronecker.egg-info/not-zip-safe
--rw-r--r--   0 ed        (1001) ed        (1001)      120 2023-01-24 22:24:16.000000 pykronecker-0.1.2/src/pykronecker.egg-info/requires.txt
--rw-r--r--   0 ed        (1001) ed        (1001)       12 2023-01-24 22:24:16.000000 pykronecker-0.1.2/src/pykronecker.egg-info/top_level.txt
+drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-07-07 14:32:09.100382 pykronecker-0.1.3/
+-rw-r--r--   0 ed        (1001) ed        (1001)     1068 2022-08-15 11:33:29.000000 pykronecker-0.1.3/LICENSE
+-rw-rw-r--   0 ed        (1001) ed        (1001)     9670 2023-07-07 14:32:09.104382 pykronecker-0.1.3/PKG-INFO
+-rw-rw-r--   0 ed        (1001) ed        (1001)     8756 2023-07-07 14:25:35.000000 pykronecker-0.1.3/README.md
+-rw-r--r--   0 ed        (1001) ed        (1001)      226 2022-08-18 15:54:24.000000 pykronecker-0.1.3/pyproject.toml
+-rw-rw-r--   0 ed        (1001) ed        (1001)     1171 2023-07-07 14:32:09.104382 pykronecker-0.1.3/setup.cfg
+-rw-r--r--   0 ed        (1001) ed        (1001)       69 2022-08-16 13:31:08.000000 pykronecker-0.1.3/setup.py
+drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-07-07 14:32:09.092382 pykronecker-0.1.3/src/
+drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-07-07 14:32:09.100382 pykronecker-0.1.3/src/pykronecker/
+-rw-rw-r--   0 ed        (1001) ed        (1001)      200 2022-09-22 16:41:27.000000 pykronecker-0.1.3/src/pykronecker/__init__.py
+-rw-rw-r--   0 ed        (1001) ed        (1001)    14545 2023-07-07 14:25:35.000000 pykronecker-0.1.3/src/pykronecker/base.py
+-rw-rw-r--   0 ed        (1001) ed        (1001)    11576 2023-07-07 14:25:35.000000 pykronecker-0.1.3/src/pykronecker/block.py
+-rw-r--r--   0 ed        (1001) ed        (1001)     4326 2022-09-22 22:08:17.000000 pykronecker-0.1.3/src/pykronecker/composite.py
+-rw-rw-r--   0 ed        (1001) ed        (1001)     7114 2022-11-11 15:45:32.000000 pykronecker-0.1.3/src/pykronecker/fast_math.py
+-rw-rw-r--   0 ed        (1001) ed        (1001)    14839 2022-10-19 10:32:51.000000 pykronecker-0.1.3/src/pykronecker/operators.py
+-rw-rw-r--   0 ed        (1001) ed        (1001)     2012 2022-09-22 16:41:27.000000 pykronecker-0.1.3/src/pykronecker/utils.py
+drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-07-07 14:32:09.100382 pykronecker-0.1.3/src/pykronecker.egg-info/
+-rw-r--r--   0 ed        (1001) ed        (1001)     9670 2023-07-07 14:32:09.000000 pykronecker-0.1.3/src/pykronecker.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1001) ed        (1001)      560 2023-07-07 14:32:09.000000 pykronecker-0.1.3/src/pykronecker.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1001) ed        (1001)        1 2023-07-07 14:32:09.000000 pykronecker-0.1.3/src/pykronecker.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1001) ed        (1001)        1 2022-08-15 11:32:42.000000 pykronecker-0.1.3/src/pykronecker.egg-info/not-zip-safe
+-rw-r--r--   0 ed        (1001) ed        (1001)      120 2023-07-07 14:32:09.000000 pykronecker-0.1.3/src/pykronecker.egg-info/requires.txt
+-rw-r--r--   0 ed        (1001) ed        (1001)       12 2023-07-07 14:32:09.000000 pykronecker-0.1.3/src/pykronecker.egg-info/top_level.txt
+drwxrwxr-x   0 ed        (1001) ed        (1001)        0 2023-07-07 14:32:09.100382 pykronecker-0.1.3/tests/
+-rw-rw-r--   0 ed        (1001) ed        (1001)     6537 2022-09-22 16:41:27.000000 pykronecker-0.1.3/tests/test_block.py
+-rw-rw-r--   0 ed        (1001) ed        (1001)     4293 2022-10-06 13:10:23.000000 pykronecker-0.1.3/tests/test_composite.py
+-rw-rw-r--   0 ed        (1001) ed        (1001)     3795 2022-09-22 16:41:27.000000 pykronecker-0.1.3/tests/test_operators.py
+-rw-r--r--   0 ed        (1001) ed        (1001)      474 2022-08-18 14:13:10.000000 pykronecker-0.1.3/tests/test_utils.py
```

### Comparing `pykronecker-0.1.2/LICENSE` & `pykronecker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykronecker-0.1.2/PKG-INFO` & `pykronecker-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,10 @@
-Metadata-Version: 2.1
-Name: pykronecker
-Version: 0.1.2
-Summary: Tools for performing efficient Kronecker product-based matrix operations
-Home-page: https://github.com/nickelnine37/pykronecker
-Author: nickelnine37
-License: MIT
-Project-URL: Bug Tracker, https://github.com/nickelnine37/pykronecker/issues
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: jax
-License-File: LICENSE
-
 ![Logo](https://raw.githubusercontent.com/nickelnine37/pykronecker/main/assets/logo.png)
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04900/status.svg)](https://doi.org/10.21105/joss.04900)
 ![Tests](https://github.com/nickelnine37/pykronecker/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/nickelnine37/pykronecker/badge.svg)](https://coveralls.io/github/nickelnine37/pykronecker)
 [![Documentation Status](https://readthedocs.org/projects/pykronecker/badge/?version=latest)](https://pykronecker.readthedocs.io/en/latest/?badge=latest)
 
 Check out the full documentation and install instructions [here](https://pykronecker.readthedocs.io/en/latest/) :)
 
 # Overview
@@ -259,34 +233,49 @@
 KI = KroneckerIdentity(like=KP)
 
 # find the inverse
 M = (KP @ KD).inv()
 print(M @ x)
 ```
 
-Summing down an axis or over the whole matrix is supported for any opertor.
+Basic indexing is supported for all operators. This will return literal numpy arrays. [Advanced indexing](https://numpy.org/doc/stable/user/basics.indexing.html#advanced-indexing) is not supported.
 
 ```python
-M = KP.T + KS @ KD
+J = KP.T + KS @ KD
+
+print(J[0])
+print(J[2:5])
+print(J[2:8:3])
+print(J[:, 2])
+print(J[:, 2:5])
+print(J[:, 2:8:3])
+print(J[2, 5])
+print(J[2:5, 2:8:3])
+print(J[:])
+print(J[:, :])
+```
 
-print(M.sum(0))
-print(M.sum(1))
-print(M.sum())
+Summing down an axis or over the whole matrix is supported for any opertor.
+
+```python
+print(J.sum(0))
+print(J.sum(1))
+print(J.sum())
 ```
 
 Any operator can also be converted to a literal array. This should only be used for small test purposes, as the arrays created can be very large. 
 
 ```python
-print(M.to_array())
+print(J.to_array())
 ```
 
 The matrix diagonal of most operators can be found with `.diag()`. This returns a one-dimensional array. 
 
 ```python
-print(M.diag())
+print(J.diag())
 ```
 
 The conjugate transpose of any complex operator can be found with `.H`
 
 ```python
 
 A_ = np.random.normal(size=(5, 5)) + 1j * np.random.normal(size=(5, 5))
```

### Comparing `pykronecker-0.1.2/README.md` & `pykronecker-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,37 @@
+Metadata-Version: 2.1
+Name: pykronecker
+Version: 0.1.3
+Summary: Tools for performing efficient Kronecker product-based matrix operations
+Home-page: https://github.com/nickelnine37/pykronecker
+Author: nickelnine37
+License: MIT
+Project-URL: Bug Tracker, https://github.com/nickelnine37/pykronecker/issues
+Platform: unix
+Platform: linux
+Platform: osx
+Platform: cygwin
+Platform: win32
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: jax
+License-File: LICENSE
+
 ![Logo](https://raw.githubusercontent.com/nickelnine37/pykronecker/main/assets/logo.png)
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04900/status.svg)](https://doi.org/10.21105/joss.04900)
 ![Tests](https://github.com/nickelnine37/pykronecker/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/nickelnine37/pykronecker/badge.svg)](https://coveralls.io/github/nickelnine37/pykronecker)
 [![Documentation Status](https://readthedocs.org/projects/pykronecker/badge/?version=latest)](https://pykronecker.readthedocs.io/en/latest/?badge=latest)
 
 Check out the full documentation and install instructions [here](https://pykronecker.readthedocs.io/en/latest/) :)
 
 # Overview
@@ -232,34 +260,49 @@
 KI = KroneckerIdentity(like=KP)
 
 # find the inverse
 M = (KP @ KD).inv()
 print(M @ x)
 ```
 
-Summing down an axis or over the whole matrix is supported for any opertor.
+Basic indexing is supported for all operators. This will return literal numpy arrays. [Advanced indexing](https://numpy.org/doc/stable/user/basics.indexing.html#advanced-indexing) is not supported.
 
 ```python
-M = KP.T + KS @ KD
+J = KP.T + KS @ KD
+
+print(J[0])
+print(J[2:5])
+print(J[2:8:3])
+print(J[:, 2])
+print(J[:, 2:5])
+print(J[:, 2:8:3])
+print(J[2, 5])
+print(J[2:5, 2:8:3])
+print(J[:])
+print(J[:, :])
+```
 
-print(M.sum(0))
-print(M.sum(1))
-print(M.sum())
+Summing down an axis or over the whole matrix is supported for any opertor.
+
+```python
+print(J.sum(0))
+print(J.sum(1))
+print(J.sum())
 ```
 
 Any operator can also be converted to a literal array. This should only be used for small test purposes, as the arrays created can be very large. 
 
 ```python
-print(M.to_array())
+print(J.to_array())
 ```
 
 The matrix diagonal of most operators can be found with `.diag()`. This returns a one-dimensional array. 
 
 ```python
-print(M.diag())
+print(J.diag())
 ```
 
 The conjugate transpose of any complex operator can be found with `.H`
 
 ```python
 
 A_ = np.random.normal(size=(5, 5)) + 1j * np.random.normal(size=(5, 5))
```

### Comparing `pykronecker-0.1.2/setup.cfg` & `pykronecker-0.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = pykronecker
 description = Tools for performing efficient Kronecker product-based matrix operations
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = nickelnine37
-version = 0.1.2
+version = 0.1.3
 license = MIT
 license_file = LICENSE
 url = https://github.com/nickelnine37/pykronecker
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `pykronecker-0.1.2/src/pykronecker/base.py` & `pykronecker-0.1.3/src/pykronecker/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -114,14 +114,96 @@
         Subclasses should define their own repr
         """
         raise NotImplementedError
 
     # ----------- CONCRETE METHODS ----------
     # These define shared and default behaviours
 
+    def __getitem__(self, item: Union[int, tuple, slice]):
+        """
+        Add support for indexing a KroneckerOperator. Note that fancy indexing is not supported.
+
+        Examples:
+            KP = KroneckerProduct([A, B])
+
+            print(KP[0])
+            print(KP[2:5])
+            print(KP[2:8:3])
+            print(KP[:, 2])
+            print(KP[:, 2:5])
+            print(KP[:, 2:8:3])
+            print(KP[2:5, 2:8:3])
+            print(KP[:])
+            print(KP[:, :])
+        """
+
+        def get_one(index: int, row=True) -> ndarray:
+            """
+            Get a single row or column
+            """
+            x = np.zeros(self.shape[0])
+            x[index] = 1.0
+            if row:
+                return self.T @ x
+            else:
+                return self @ x
+
+        def get_many(index_slice: slice, row=True) -> ndarray:
+            """
+            Get multiple rows or columns
+            """
+
+            indices = list(range(*index_slice.indices(self.shape[0])))
+            x = np.zeros((self.shape[0], len(indices)))
+            x[indices, range(len(indices))] = 1
+            if row:
+                return (self.T @ x).T
+            else:
+                return self @ x
+
+        # get a single row
+        if isinstance(item, int):
+            return get_one(item, row=True)
+
+        # get many rows
+        if isinstance(item, slice):
+            return get_many(item, row=True)
+
+        # multi-indexing
+        if isinstance(item, tuple):
+
+            # operator is 2-dimensional...
+            if len(item) > 2:
+                raise IndexError(f'too many indices for array: operator is 2-dimensional, but {len(item)} were indexed')
+
+            # get a single row
+            if len(item) == 1:
+                return get_one(item[0], row=True)
+
+            # get a single element
+            if isinstance(item[0], int) and isinstance(item[1], int):
+                return get_one(item[1], row=False)[item[0]]
+
+            # get a slice of a row
+            if isinstance(item[0], int) and isinstance(item[1], slice):
+                return get_one(item[0], row=True)[item[1]]
+
+            # get a slice of a column
+            if isinstance(item[0], slice) and isinstance(item[1], int):
+                return get_one(item[1], row=False)[item[0]]
+
+            # get a slice of both
+            if isinstance(item[0], slice) and isinstance(item[1], slice):
+                return get_many(item[1], row=False)[item[0]]
+
+            else:
+                raise IndexError(f'Could not interpret indices. Got [{type(item[0])}, {type(item[1])}]. Expected both to be either and int or slice')
+
+        raise IndexError(f'Could not interpret index type. Got {type(item)}. Expected int, slice or tuple')
+
     def __add__(self, other: 'KroneckerOperator') -> 'KroneckerOperator':
         """
         Overload the addition method. This is used to sum together KroneckerOperators and as such
         `other` must be an instance of a KroneckerOperator, and not an array or other numeric type.
         """
 
         from pykronecker.composite import OperatorSum
```

### Comparing `pykronecker-0.1.2/src/pykronecker/block.py` & `pykronecker-0.1.3/src/pykronecker/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from __future__ import annotations
 from abc import abstractmethod, ABC
 from typing import Callable, List, Union
 
 import numpy as np
 from numpy import ndarray
 
+
+
 from pykronecker.base import KroneckerOperator
 from pykronecker.composite import OperatorSum
 from pykronecker.utils import numeric
 
+try:
+    import jax.numpy as jnp
+except ImportError:
+    import numpy as jnp
 
 class KroneckerBlockBase(KroneckerOperator, ABC):
     """
     Abstract class to capture shared behaviour of KroneckerBlock and KroneckerBlockDiag
     """
 
     def __init__(self, blocks: list):
@@ -52,15 +58,27 @@
 
     @staticmethod
     def check_blocks_consistent(blocks: list):
         """
         Check the blocks, which are provided as input to KroneckerBlock and KroneckerBlockDiag are consistent
         """
 
-        ndim = np.asarray(blocks, dtype='object').ndim
+        def replace(items):
+            """
+            Turn into a block of stings, so we can use numpy.block
+            """
+            out = []
+            for item in items:
+                if isinstance(item, (list, tuple)):
+                    out.append(replace(item))
+                else:
+                    out.append('a')
+            return out
+
+        ndim = np.block(replace(blocks)).ndim
 
         if ndim == 1:
             assert all(hasattr(block, 'shape') for block in blocks)
             assert all(block.shape[0] == block.shape[1] for block in blocks)
 
         elif ndim == 2:
 
@@ -129,37 +147,22 @@
 
     def get_tensor_shape(self) -> tuple:
         return tuple(self.blocks[i][i].tensor_shape if isinstance(self.blocks[i][i], KroneckerOperator) else self.blocks[i][i].shape[0] for i in range(len(self.blocks)))
 
     def operate(self, other: ndarray) -> ndarray:
 
         x = other.squeeze()
-        dtype = np.result_type(self.dtype, x)
 
         if x.shape[0] != len(self):
             raise ValueError(f'other\'s first dimension should have length {len(self)} to match the dimensions of the operator, but it has length {x.shape[0]}')
 
-        if x.ndim == 1:
-
-            out = [np.zeros_like(x[n1:n2], dtype=dtype) for n1, n2 in self.iter_edges()]
-            blocks = [x[n1:n2] for n1, n2 in self.iter_edges()]
-
-        elif x.ndim == 2:
-
-            out = [np.zeros_like(x[n1:n2, :], dtype=dtype) for n1, n2 in self.iter_edges()]
-            blocks = [x[n1:n2, :] for n1, n2 in self.iter_edges()]
-
-        else:
+        if x.ndim not in [1, 2]:
             raise ValueError(f'other must be 1 or 2d but it is {other.ndim}d')
-
-        for i in range(self.n_blocks):
-            for j in range(self.n_blocks):
-                out[i] += self.blocks[i][j] @ blocks[j]
-
-        return self.factor * np.concatenate(out, axis=0)
+ 
+        return self.factor * jnp.concatenate([sum(self.blocks[i][j] @ x[n1:n2] for j, (n1, n2) in enumerate(self.iter_edges())) for i in range(self.n_blocks)], axis=0)
 
     def __mul__(self, other: Union['KroneckerOperator', numeric]) -> KroneckerOperator:
 
         if isinstance(other, KroneckerOperator):
 
             self.check_operators_consistent(self, other)
```

### Comparing `pykronecker-0.1.2/src/pykronecker/composite.py` & `pykronecker-0.1.3/src/pykronecker/composite.py`

 * *Files identical despite different names*

### Comparing `pykronecker-0.1.2/src/pykronecker/fast_math.py` & `pykronecker-0.1.3/src/pykronecker/fast_math.py`

 * *Files identical despite different names*

### Comparing `pykronecker-0.1.2/src/pykronecker/operators.py` & `pykronecker-0.1.3/src/pykronecker/operators.py`

 * *Files identical despite different names*

### Comparing `pykronecker-0.1.2/src/pykronecker/utils.py` & `pykronecker-0.1.3/src/pykronecker/utils.py`

 * *Files identical despite different names*

### Comparing `pykronecker-0.1.2/src/pykronecker.egg-info/PKG-INFO` & `pykronecker-0.1.3/src/pykronecker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykronecker
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for performing efficient Kronecker product-based matrix operations
 Home-page: https://github.com/nickelnine37/pykronecker
 Author: nickelnine37
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nickelnine37/pykronecker/issues
 Platform: unix
 Platform: linux
@@ -23,14 +23,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: jax
 License-File: LICENSE
 
 ![Logo](https://raw.githubusercontent.com/nickelnine37/pykronecker/main/assets/logo.png)
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04900/status.svg)](https://doi.org/10.21105/joss.04900)
 ![Tests](https://github.com/nickelnine37/pykronecker/actions/workflows/tests.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/nickelnine37/pykronecker/badge.svg)](https://coveralls.io/github/nickelnine37/pykronecker)
 [![Documentation Status](https://readthedocs.org/projects/pykronecker/badge/?version=latest)](https://pykronecker.readthedocs.io/en/latest/?badge=latest)
 
 Check out the full documentation and install instructions [here](https://pykronecker.readthedocs.io/en/latest/) :)
 
 # Overview
@@ -259,34 +260,49 @@
 KI = KroneckerIdentity(like=KP)
 
 # find the inverse
 M = (KP @ KD).inv()
 print(M @ x)
 ```
 
-Summing down an axis or over the whole matrix is supported for any opertor.
+Basic indexing is supported for all operators. This will return literal numpy arrays. [Advanced indexing](https://numpy.org/doc/stable/user/basics.indexing.html#advanced-indexing) is not supported.
 
 ```python
-M = KP.T + KS @ KD
+J = KP.T + KS @ KD
+
+print(J[0])
+print(J[2:5])
+print(J[2:8:3])
+print(J[:, 2])
+print(J[:, 2:5])
+print(J[:, 2:8:3])
+print(J[2, 5])
+print(J[2:5, 2:8:3])
+print(J[:])
+print(J[:, :])
+```
 
-print(M.sum(0))
-print(M.sum(1))
-print(M.sum())
+Summing down an axis or over the whole matrix is supported for any opertor.
+
+```python
+print(J.sum(0))
+print(J.sum(1))
+print(J.sum())
 ```
 
 Any operator can also be converted to a literal array. This should only be used for small test purposes, as the arrays created can be very large. 
 
 ```python
-print(M.to_array())
+print(J.to_array())
 ```
 
 The matrix diagonal of most operators can be found with `.diag()`. This returns a one-dimensional array. 
 
 ```python
-print(M.diag())
+print(J.diag())
 ```
 
 The conjugate transpose of any complex operator can be found with `.H`
 
 ```python
 
 A_ = np.random.normal(size=(5, 5)) + 1j * np.random.normal(size=(5, 5))
```


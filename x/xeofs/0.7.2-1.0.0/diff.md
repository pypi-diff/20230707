# Comparing `tmp/xeofs-0.7.2.tar.gz` & `tmp/xeofs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeofs-0.7.2.tar", max compression
+gzip compressed data, was "xeofs-1.0.0.tar", max compression
```

## Comparing `xeofs-0.7.2.tar` & `xeofs-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,31 @@
--rw-r--r--   0        0        0     1070 2023-01-10 17:15:49.351089 xeofs-0.7.2/LICENSE
--rw-r--r--   0        0        0     9472 2023-01-10 17:15:49.351089 xeofs-0.7.2/README.rst
--rw-r--r--   0        0        0      976 2023-01-10 17:15:50.075086 xeofs-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      112 2023-01-10 17:15:50.075086 xeofs-0.7.2/xeofs/__init__.py
--rw-r--r--   0        0        0      178 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/__init__.py
--rw-r--r--   0        0        0     6290 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/_base_bootstrapper.py
--rw-r--r--   0        0        0    10918 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/_base_eof.py
--rw-r--r--   0        0        0    16839 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/_base_mca.py
--rw-r--r--   0        0        0    18694 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/_base_mca_rotator.py
--rw-r--r--   0        0        0     8928 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/_base_rock_pca.py
--rw-r--r--   0        0        0     9889 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/_base_rotator.py
--rw-r--r--   0        0        0     8916 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/_transformer.py
--rw-r--r--   0        0        0     1230 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/bootstrapper.py
--rw-r--r--   0        0        0     5177 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/eof.py
--rw-r--r--   0        0        0     6794 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/mca.py
--rw-r--r--   0        0        0     4719 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/mca_rotator.py
--rw-r--r--   0        0        0     1949 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/rock_pca.py
--rw-r--r--   0        0        0     3180 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/models/rotator.py
--rw-r--r--   0        0        0      178 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/pandas/__init__.py
--rw-r--r--   0        0        0     4096 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/pandas/_transformer.py
--rw-r--r--   0        0        0     1673 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/pandas/bootstrapper.py
--rw-r--r--   0        0        0     4928 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/pandas/eof.py
--rw-r--r--   0        0        0     6360 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/pandas/mca.py
--rw-r--r--   0        0        0     5299 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/pandas/mca_rotator.py
--rw-r--r--   0        0        0     2353 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/pandas/rock_pca.py
--rw-r--r--   0        0        0     3488 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/pandas/rotator.py
--rw-r--r--   0        0        0        0 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/utils/__init__.py
--rw-r--r--   0        0        0     1114 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/utils/distance_matrix.py
--rw-r--r--   0        0        0     5224 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/utils/rotation.py
--rw-r--r--   0        0        0     1482 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/utils/tools.py
--rw-r--r--   0        0        0      178 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/xarray/__init__.py
--rw-r--r--   0        0        0     6790 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/xarray/_transformer.py
--rw-r--r--   0        0        0     2660 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/xarray/bootstrapper.py
--rw-r--r--   0        0        0     6745 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/xarray/eof.py
--rw-r--r--   0        0        0     8091 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/xarray/mca.py
--rw-r--r--   0        0        0     5234 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/xarray/mca_rotator.py
--rw-r--r--   0        0        0     2903 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/xarray/rock_pca.py
--rw-r--r--   0        0        0     3783 2023-01-10 17:15:49.403089 xeofs-0.7.2/xeofs/xarray/rotator.py
--rw-r--r--   0        0        0    10526 1970-01-01 00:00:00.000000 xeofs-0.7.2/setup.py
--rw-r--r--   0        0        0    10440 1970-01-01 00:00:00.000000 xeofs-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-07 02:07:15.725350 xeofs-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5580 2023-07-07 02:07:15.725350 xeofs-1.0.0/README.rst
+-rw-r--r--   0        0        0     1088 2023-07-07 02:07:16.693359 xeofs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-07 02:07:16.693359 xeofs-1.0.0/xeofs/_version.py
+-rw-r--r--   0        0        0      219 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/__init__.py
+-rw-r--r--   0        0        0     5791 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/_base_cross_model.py
+-rw-r--r--   0        0        0     8790 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/_base_model.py
+-rw-r--r--   0        0        0     3398 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/_base_rotator.py
+-rw-r--r--   0        0        0     8778 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/decomposer.py
+-rw-r--r--   0        0        0     7540 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/eof.py
+-rw-r--r--   0        0        0     9859 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/eof_rotator.py
+-rw-r--r--   0        0        0    24353 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/mca.py
+-rw-r--r--   0        0        0    25201 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/mca_rotator.py
+-rw-r--r--   0        0        0     2153 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/models/rotator_factory.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/__init__.py
+-rw-r--r--   0        0        0      812 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/_base_scaler.py
+-rw-r--r--   0        0        0     3781 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/_base_stacker.py
+-rw-r--r--   0        0        0    11193 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/scaler.py
+-rw-r--r--   0        0        0    21232 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/stacker.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/constants.py
+-rw-r--r--   0        0        0      631 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/data_types.py
+-rw-r--r--   0        0        0     5179 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/rotation.py
+-rw-r--r--   0        0        0     2201 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/sanity_checks.py
+-rw-r--r--   0        0        0     4681 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/statistics.py
+-rw-r--r--   0        0        0     6514 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/xarray_utils.py
+-rw-r--r--   0        0        0       41 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/validation/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/validation/_base_bootstrapper.py
+-rw-r--r--   0        0        0     4957 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/validation/bootstrapper.py
+-rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 xeofs-1.0.0/PKG-INFO
```

### Comparing `xeofs-0.7.2/LICENSE` & `xeofs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xeofs-0.7.2/pyproject.toml` & `xeofs-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xeofs"
-version = "0.7.2"
+version = "1.0.0"
 description = "Collection of EOF analysis and related techniques for climate science"
 authors = ["Niclas Rieger <niclasrieger@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/nicrie/xeofs"
 repository = "https://github.com/nicrie/xeofs"
 documentation = "https://xeofs.readthedocs.io/en/latest/"
@@ -19,21 +19,27 @@
 tqdm = "^4.64.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 pytest = "^7.0.1"
 coverage = "^6.3.1"
 netCDF4 = "^1.5.7"
+sphinx-gallery = "^0"
+sphinxawesome-theme = "^4"
+sphinx-design = "^0"
+nbsphinx = "^0"
+sphinx-copybutton = "^0"
+
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = [
-    "xeofs/__init__.py:__version__",
+    "xeofs/_version.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "main"
 upload_to_pypi = true
 uploade_to_release = true
 build_command = "pip install poetry && poetry build"
```

### Comparing `xeofs-0.7.2/xeofs/models/rotator.py` & `xeofs-1.0.0/xeofs/models/_base_rotator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,107 @@
+from abc import ABC, abstractmethod
+from datetime import datetime
+
 import numpy as np
+import scipy as sc
+import xarray as xr
 from typing import Optional, Union, List, Tuple
 
-from .eof import EOF
-from ._base_rotator import _BaseRotator
-from ._transformer import _MultiArrayTransformer
-from ..utils.tools import squeeze
-
-Array = np.ndarray
-ArrayList = Union[Array, List[Array]]
+from ..utils.rotation import promax
+from .._version import __version__
 
 
-class Rotator(_BaseRotator):
-    '''Rotates a solution obtained from ``xe.models.EOF``.
+class _BaseRotator():
+    '''Rotates a solution obtained from an EOF model.
 
     Parameters
     ----------
-    model : xe.models.EOF
-        A EOF model solution.
-    n_rot : int
-        Number of modes to be rotated.
+    n_modes : int
+        Number of modes to be rotated (the default is 10).
     power : int
         Defines the power of Promax rotation. Choosing ``power=1`` equals
         a Varimax solution (the default is 1).
     max_iter : int
         Number of maximal iterations for obtaining the rotation matrix
         (the default is 1000).
     rtol : float
         Relative tolerance to be achieved for early stopping the iteration
         process (the default is 1e-8).
 
 
     '''
 
-    def __init__(
-        self,
-        model : EOF,
-        n_rot : int,
-        power : int = 1,
-        max_iter : int = 1000,
-        rtol : float = 1e-8
-    ):
-
-        super().__init__(
-            model=model, n_rot=n_rot, power=power, max_iter=max_iter, rtol=rtol
-        )
-
-    def explained_variance(self) -> Array:
-        return super().explained_variance()
-
-    def explained_variance_ratio(self) -> Array:
-        return super().explained_variance_ratio()
-
-    def eofs(self, scaling : int = 0) -> ArrayList:
-        eofs = super().eofs(scaling=scaling)
-        eofs = self._model._tf.back_transform_eofs(eofs)
-        return squeeze(eofs)
-
-    def pcs(self, scaling : int = 0) -> Array:
-        pcs = super().pcs(scaling=scaling)
-        return self._model._tf.back_transform_pcs(pcs)
-
-    def eofs_as_correlation(self) -> Tuple[ArrayList, ArrayList]:
-        corr, pvals = super().eofs_as_correlation()
-        corr = self._model._tf.back_transform_eofs(corr)
-        pvals = self._model._tf.back_transform_eofs(pvals)
-        return squeeze(corr), squeeze(pvals)
-
-    def reconstruct_X(
-        self,
-        mode : Optional[Union[int, List[int], slice]] = None
-    ) -> ArrayList:
-        Xrec = super().reconstruct_X(mode=mode)
-        Xrec = self._model._tf.back_transform(Xrec)
-        return squeeze(Xrec)
-
-    def project_onto_eofs(
-        self,
-        X : ArrayList,
-        scaling : int = 0
-    ) -> Array:
-        '''Project new data onto the rotated EOFs.
+    def __init__(self, n_modes: int = 10, power: int = 1, max_iter: int = 1000, rtol: float = 1e-8):
+        
+        # Define model parameters
+        self._params = {
+            'n_modes': n_modes,
+            'power': power,
+            'max_iter': max_iter,
+            'rtol': rtol,
+        }
+        
+        # Define analysis-relevant meta data
+        self.attrs = {'model': 'BaseRotator'}
+        self.attrs.update(self._params)
+        self.attrs.update({
+            'software': 'xeofs',
+            'version': __version__,
+            'date': datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        })
+
+
+    @abstractmethod
+    def fit(self, model):
+        '''Fit the model.'''
+
+        # VARIABLES TO BE DEFINED
+        # self._model
+        # self._rotation_matrix --> rotation matrix to be applied to the loadings
+        # self._idx_expvar --> order of explained variance so that modes can be reordered
+        # according to highest explained variance
+
+        # OTHER VARIABLES THAT DEPEND ON THE SPECIFIC MODEL TO BE ROTATED
+        # self._explained_variance
+        # self._explained_variance_ratio | self._squared_covariance_fraction
+        # self._components
+        # self._scores
+        raise NotImplementedError
+    
+    @abstractmethod
+    def transform(self, data):
+        '''Transform the model.'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def inverse_transform(self, mode: int | List[int] | slice = slice(None)):
+        '''Inverse transform the model.'''
+        raise NotImplementedError
+    
+    
+    def _get_rotation_matrix(self, inverse_transpose : bool = False) -> xr.DataArray:
+        '''Return the rotation matrix.
 
         Parameters
         ----------
-        X : np.ndarray
-             New data to project. Data must have same feature shape as original
-             data.
-        scaling : [0, 1, 2]
-            Projections are scaled (i) to be orthonormal (``scaling=0``), (ii) by the
-            square root of the eigenvalues (``scaling=1``) or (iii) by the
-            singular values (``scaling=2``). In case no weights were applied,
-            scaling by the singular values results in the projections having the
-            unit of the input data (the default is 0).
+        inverse_transpose : bool, default=False
+            Determines whether to return the rotation matrix or its inverse transposed. 
+            For orthogonal rotations (e.g., Varimax), the inverse transpose is equivalent 
+            to the rotation matrix itself. However, for oblique rotations (e.g., Promax), it may differ.
+
+        Returns
+        -------
+        rotation_matrix : xr.DataArray
 
         '''
-        proj = _MultiArrayTransformer()
-        X = proj.fit_transform(X, axis=self._model._tf.axis_samples)
-        pcs = super().project_onto_eofs(X=X, scaling=scaling)
-        return proj.back_transform_pcs(pcs)
+        R = self._rotation_matrix  # type: ignore
+        if inverse_transpose and self._params['power'] > 1:
+            # inverse matrix
+            R = xr.apply_ufunc(
+                np.linalg.pinv,
+                R,
+                input_core_dims=[['mode','mode1']],
+                output_core_dims=[['mode','mode1']]
+            )
+            # transpose matrix
+            R = R.conj().T
+        return R  # type: ignore
```

### Comparing `xeofs-0.7.2/xeofs/utils/rotation.py` & `xeofs-1.0.0/xeofs/utils/rotation.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,34 +50,34 @@
         err_msg = err_msg.format(n_modes)
         raise ValueError(err_msg)
 
     # Initialize rotation matrix
     R = np.eye(n_modes)
 
     # Normalize the matrix using square root of the sum of squares (Kaiser)
-    h = np.sqrt(np.sum(X * X.conjugate(), axis=1))
+    h = np.sqrt(np.sum(X * X.conj(), axis=1))
     # A = np.diag(1./h) @ A
 
     # Add a stabilizer to avoid zero communalities
     eps = 1e-9
     X = (1. / (h + eps))[:, np.newaxis] * X
 
     # Seek for rotation matrix based on varimax criteria
     delta = 0.
     converged = False
     for i in range(max_iter):
         delta_old = delta
         basis = X @ R
 
-        basis2 = basis * basis.conjugate()
+        basis2 = basis * basis.conj()
         basis3 = basis2 * basis
         W = np.diag(np.sum(basis2, axis=0))
         alpha = gamma / n_samples
 
-        transformed = X.conjugate().T @ (basis3 - (alpha * basis @ W))
+        transformed = X.conj().T @ (basis3 - (alpha * basis @ W))
         U, svals, VT = np.linalg.svd(transformed)
         R = U @ VT
         delta = np.sum(svals)
         if (abs(delta - delta_old) / delta) < rtol:
             converged = True
             break
 
@@ -136,42 +136,42 @@
     '''
     X = X.copy()
 
     # Perform varimax rotation
     X, rot_mat = varimax(X=X, max_iter=max_iter, rtol=rtol)
 
     # Pre-normalization by communalities (sum of squared rows)
-    h = np.sqrt(np.sum(X * X.conjugate(), axis=1))
+    h = np.sqrt(np.sum(X * X.conj(), axis=1))
     # Add a stabilizer to avoid zero communalities
     eps = 1e-9
     X = (1. / (h + eps))[:, np.newaxis] * X
 
     # Max-normalisation of columns
     Xnorm = X / np.max(abs(X), axis=0)
 
     # "Procustes" equation
     P = Xnorm * np.abs(Xnorm)**(power - 1)
 
     # Fit linear regression model of "Procrustes" equation
     # see Richman 1986 for derivation
-    L = np.linalg.inv(X.conjugate().T @ X) @ X.conjugate().T @ P
+    L = np.linalg.inv(X.conj().T @ X) @ X.conj().T @ P
 
     # calculate diagonal of inverse square
     try:
-        sigma_inv = np.diag(np.diag(np.linalg.inv(L.conjugate().T @ L)))
+        sigma_inv = np.diag(np.diag(np.linalg.inv(L.conj().T @ L)))
     except np.linalg.LinAlgError:
-        sigma_inv = np.diag(np.diag(np.linalg.pinv(L.conjugate().T @ L)))
+        sigma_inv = np.diag(np.diag(np.linalg.pinv(L.conj().T @ L)))
 
     # transform and calculate inner products
     L = L @ np.sqrt(sigma_inv)
     Xrot = X @ L
 
     # Post-normalization based on Kaiser
     Xrot = h[:, np.newaxis] * Xrot
 
     rot_mat = rot_mat @ L
 
     # Correlation matrix
     L_inv = np.linalg.inv(L)
-    phi = L_inv @ L_inv.conjugate().T
+    phi = L_inv @ L_inv.conj().T
 
     return Xrot, rot_mat, phi
```


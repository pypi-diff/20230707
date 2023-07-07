# Comparing `tmp/xeofs-1.0.0.tar.gz` & `tmp/xeofs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeofs-1.0.0.tar", max compression
+gzip compressed data, was "xeofs-1.0.1.tar", max compression
```

## Comparing `xeofs-1.0.0.tar` & `xeofs-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1070 2023-07-07 02:07:15.725350 xeofs-1.0.0/LICENSE
--rw-r--r--   0        0        0     5580 2023-07-07 02:07:15.725350 xeofs-1.0.0/README.rst
--rw-r--r--   0        0        0     1088 2023-07-07 02:07:16.693359 xeofs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       75 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/__init__.py
--rw-r--r--   0        0        0       70 2023-07-07 02:07:16.693359 xeofs-1.0.0/xeofs/_version.py
--rw-r--r--   0        0        0      219 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/__init__.py
--rw-r--r--   0        0        0     5791 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/_base_cross_model.py
--rw-r--r--   0        0        0     8790 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/_base_model.py
--rw-r--r--   0        0        0     3398 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/_base_rotator.py
--rw-r--r--   0        0        0     8778 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/decomposer.py
--rw-r--r--   0        0        0     7540 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/eof.py
--rw-r--r--   0        0        0     9859 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/eof_rotator.py
--rw-r--r--   0        0        0    24353 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/mca.py
--rw-r--r--   0        0        0    25201 2023-07-07 02:07:15.773351 xeofs-1.0.0/xeofs/models/mca_rotator.py
--rw-r--r--   0        0        0     2153 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/models/rotator_factory.py
--rw-r--r--   0        0        0        0 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/__init__.py
--rw-r--r--   0        0        0      812 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/_base_scaler.py
--rw-r--r--   0        0        0     3781 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/_base_stacker.py
--rw-r--r--   0        0        0    11193 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/scaler.py
--rw-r--r--   0        0        0    21232 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/preprocessing/stacker.py
--rw-r--r--   0        0        0        0 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/__init__.py
--rw-r--r--   0        0        0      301 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/constants.py
--rw-r--r--   0        0        0      631 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/data_types.py
--rw-r--r--   0        0        0     5179 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/rotation.py
--rw-r--r--   0        0        0     2201 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/sanity_checks.py
--rw-r--r--   0        0        0     4681 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/statistics.py
--rw-r--r--   0        0        0     6514 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/utils/xarray_utils.py
--rw-r--r--   0        0        0       41 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/validation/__init__.py
--rw-r--r--   0        0        0        1 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/validation/_base_bootstrapper.py
--rw-r--r--   0        0        0     4957 2023-07-07 02:07:15.777351 xeofs-1.0.0/xeofs/validation/bootstrapper.py
--rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 xeofs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-07 02:48:04.371585 xeofs-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5580 2023-07-07 02:48:04.371585 xeofs-1.0.1/README.rst
+-rw-r--r--   0        0        0     1138 2023-07-07 02:48:05.119587 xeofs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-07-07 02:48:04.415585 xeofs-1.0.1/xeofs/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-07 02:48:05.119587 xeofs-1.0.1/xeofs/_version.py
+-rw-r--r--   0        0        0      219 2023-07-07 02:48:04.415585 xeofs-1.0.1/xeofs/models/__init__.py
+-rw-r--r--   0        0        0     5791 2023-07-07 02:48:04.415585 xeofs-1.0.1/xeofs/models/_base_cross_model.py
+-rw-r--r--   0        0        0     8790 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/_base_model.py
+-rw-r--r--   0        0        0     3398 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/_base_rotator.py
+-rw-r--r--   0        0        0     8778 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/decomposer.py
+-rw-r--r--   0        0        0     7540 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/eof.py
+-rw-r--r--   0        0        0     9859 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/eof_rotator.py
+-rw-r--r--   0        0        0    24353 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/mca.py
+-rw-r--r--   0        0        0    25201 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/mca_rotator.py
+-rw-r--r--   0        0        0     2153 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/models/rotator_factory.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/__init__.py
+-rw-r--r--   0        0        0      812 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/_base_scaler.py
+-rw-r--r--   0        0        0     3781 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/_base_stacker.py
+-rw-r--r--   0        0        0    11193 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/scaler.py
+-rw-r--r--   0        0        0    21232 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/preprocessing/stacker.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/constants.py
+-rw-r--r--   0        0        0      631 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/data_types.py
+-rw-r--r--   0        0        0     5179 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/rotation.py
+-rw-r--r--   0        0        0     2201 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/sanity_checks.py
+-rw-r--r--   0        0        0     4681 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/statistics.py
+-rw-r--r--   0        0        0     6514 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/utils/xarray_utils.py
+-rw-r--r--   0        0        0       41 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/validation/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/validation/_base_bootstrapper.py
+-rw-r--r--   0        0        0     4957 2023-07-07 02:48:04.419585 xeofs-1.0.1/xeofs/validation/bootstrapper.py
+-rw-r--r--   0        0        0     6494 1970-01-01 00:00:00.000000 xeofs-1.0.1/PKG-INFO
```

### Comparing `xeofs-1.0.0/LICENSE` & `xeofs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/README.rst` & `xeofs-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/pyproject.toml` & `xeofs-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "xeofs"
-version = "1.0.0"
+version = "1.0.1"
 description = "Collection of EOF analysis and related techniques for climate science"
 authors = ["Niclas Rieger <niclasrieger@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/nicrie/xeofs"
 repository = "https://github.com/nicrie/xeofs"
 documentation = "https://xeofs.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-numpy = "^1.19.2"
-pandas = "^1.4.1"
+python = ">=3.10"
+numpy = ">=1.19.2"
+pandas = ">=1.4.1"
 xarray = ">=0.21.1"
-scikit-learn = "^1.0.2"
+scikit-learn = ">=1.0.2"
 pooch = "^1.6.0"
 tqdm = "^4.64.0"
+dask = ">=2023.0.1"
+statsmodels = ">=0.14.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 pytest = "^7.0.1"
 coverage = "^6.3.1"
 netCDF4 = "^1.5.7"
 sphinx-gallery = "^0"
```

### Comparing `xeofs-1.0.0/xeofs/models/_base_cross_model.py` & `xeofs-1.0.1/xeofs/models/_base_cross_model.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/models/_base_model.py` & `xeofs-1.0.1/xeofs/models/_base_model.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/models/_base_rotator.py` & `xeofs-1.0.1/xeofs/models/_base_rotator.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/models/decomposer.py` & `xeofs-1.0.1/xeofs/models/decomposer.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/models/eof.py` & `xeofs-1.0.1/xeofs/models/eof.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/models/eof_rotator.py` & `xeofs-1.0.1/xeofs/models/eof_rotator.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/models/mca.py` & `xeofs-1.0.1/xeofs/models/mca.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/models/mca_rotator.py` & `xeofs-1.0.1/xeofs/models/mca_rotator.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/models/rotator_factory.py` & `xeofs-1.0.1/xeofs/models/rotator_factory.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/preprocessing/_base_scaler.py` & `xeofs-1.0.1/xeofs/preprocessing/_base_scaler.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/preprocessing/_base_stacker.py` & `xeofs-1.0.1/xeofs/preprocessing/_base_stacker.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/preprocessing/scaler.py` & `xeofs-1.0.1/xeofs/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/preprocessing/stacker.py` & `xeofs-1.0.1/xeofs/preprocessing/stacker.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/utils/data_types.py` & `xeofs-1.0.1/xeofs/utils/data_types.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/utils/rotation.py` & `xeofs-1.0.1/xeofs/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/utils/sanity_checks.py` & `xeofs-1.0.1/xeofs/utils/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/utils/statistics.py` & `xeofs-1.0.1/xeofs/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/utils/xarray_utils.py` & `xeofs-1.0.1/xeofs/utils/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/xeofs/validation/bootstrapper.py` & `xeofs-1.0.1/xeofs/validation/bootstrapper.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.0/PKG-INFO` & `xeofs-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: xeofs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Collection of EOF analysis and related techniques for climate science
 Home-page: https://github.com/nicrie/xeofs
 License: MIT
 Author: Niclas Rieger
 Author-email: niclasrieger@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.19.2,<2.0.0)
-Requires-Dist: pandas (>=1.4.1,<2.0.0)
+Requires-Dist: dask (>=2023.0.1)
+Requires-Dist: numpy (>=1.19.2)
+Requires-Dist: pandas (>=1.4.1)
 Requires-Dist: pooch (>=1.6.0,<2.0.0)
-Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
+Requires-Dist: scikit-learn (>=1.0.2)
+Requires-Dist: statsmodels (>=0.14.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: xarray (>=0.21.1)
 Project-URL: Documentation, https://xeofs.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/nicrie/xeofs
 Description-Content-Type: text/x-rst
 
 .. image:: docs/logos/xeofs_logo.png
```


# Comparing `tmp/fixms-0.0.0.tar.gz` & `tmp/fixms-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixms-0.0.0.tar", max compression
+gzip compressed data, was "fixms-0.0.1.tar", max compression
```

## Comparing `fixms-0.0.0.tar` & `fixms-0.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2975 2023-07-07 07:41:47.593892 fixms-0.0.0/README.md
--rw-r--r--   0        0        0        0 2023-07-07 06:20:46.198000 fixms-0.0.0/fixms/__init__.py
--rw-r--r--   0        0        0    12138 2023-07-07 06:29:07.701736 fixms-0.0.0/fixms/fix_ms_corrs.py
--rw-r--r--   0        0        0    12457 2023-07-07 06:29:06.299265 fixms-0.0.0/fixms/fix_ms_dir.py
--rw-r--r--   0        0        0      713 2023-07-07 07:31:51.620364 fixms-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 fixms-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3216 2023-07-07 07:58:45.133732 fixms-0.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 07:58:45.133732 fixms-0.0.1/fixms/__init__.py
+-rw-r--r--   0        0        0    12138 2023-07-07 07:58:45.133732 fixms-0.0.1/fixms/fix_ms_corrs.py
+-rw-r--r--   0        0        0    12457 2023-07-07 07:58:45.133732 fixms-0.0.1/fixms/fix_ms_dir.py
+-rw-r--r--   0        0        0      713 2023-07-07 07:58:45.133732 fixms-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 fixms-0.0.1/PKG-INFO
```

### Comparing `fixms-0.0.0/README.md` & `fixms-0.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest)
+![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest) [![Python package](https://github.com/AlecThomson/FixMS/actions/workflows/main.yml/badge.svg)](https://github.com/AlecThomson/FixMS/actions/workflows/main.yml)
 
 # FixMS
 
 ASKAP utilities for updating MeasurementSets for external imagers.
 
 ASKAP MSs are produced in a way that breaks compatibility with most other imagers (e.g. CASA, WSclean). Here we provide two modules (with CLI hooks) that fix the two stages that need to be applied to produce astronomically correct imagers with non-YandaSoft imagers:
 
 1. `fix_ms_dir` : ASKAP MeasurementSets are phased towards the centre of field, but not the centre of its given beam. This utility reads the appropriate offsets to the beam centre from the `BEAM_OFFSET` and updates the `FIELD` table, as well as the phase and delay reference columns.
 
 2. `fix_ms_corrs` : ASKAP MeasurementSets, as calibrated by the obervatory, provide correlations in the instrument frame. ASKAP has a unique 'roll' axis which means, in principle, the instrument frame can be at any arbitrary rotation on the sky. This utility applies the appropriate rotation matrix to the visibilities such the 'X' is aligned North-South and 'Y' is aligned East-West (IAU convention). Further, ASKAPsoft defines Stokes I as $I=XX+YY$, whereas most other telescopes use $I=\frac{1}{2}(XX+YY)$ (note this also applies to all other Stokes paramters). This factor is also corrected for here at the same time as the rotation.
 
+Full documentation on [Read The Docs](https://fixms.readthedocs.io/en/latest/).
+
 ## Installation
 
 Obtain and install Python 3 (I recommend [Miniforge](https://github.com/conda-forge/miniforge) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)).
 
 Install the Python scripts:
 
 Latest:
```

### Comparing `fixms-0.0.0/fixms/fix_ms_corrs.py` & `fixms-0.0.1/fixms/fix_ms_corrs.py`

 * *Files identical despite different names*

### Comparing `fixms-0.0.0/fixms/fix_ms_dir.py` & `fixms-0.0.1/fixms/fix_ms_dir.py`

 * *Files identical despite different names*

### Comparing `fixms-0.0.0/pyproject.toml` & `fixms-0.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixms"
-version = "0.0.0"
+version = "0.0.1"
 description = ""
 authors = ["Alec Thomson (S&A, Kensington WA) <alec.thomson@csiro.au>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "*"
```

### Comparing `fixms-0.0.0/PKG-INFO` & `fixms-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixms
-Version: 0.0.0
+Version: 0.0.1
 Summary: 
 Author: Alec Thomson (S&A, Kensington WA)
 Author-email: alec.thomson@csiro.au
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,26 +13,28 @@
 Provides-Extra: dev
 Requires-Dist: astropy (>=5,<6)
 Requires-Dist: numpy
 Requires-Dist: python-casacore
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest)
+![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest) [![Python package](https://github.com/AlecThomson/FixMS/actions/workflows/main.yml/badge.svg)](https://github.com/AlecThomson/FixMS/actions/workflows/main.yml)
 
 # FixMS
 
 ASKAP utilities for updating MeasurementSets for external imagers.
 
 ASKAP MSs are produced in a way that breaks compatibility with most other imagers (e.g. CASA, WSclean). Here we provide two modules (with CLI hooks) that fix the two stages that need to be applied to produce astronomically correct imagers with non-YandaSoft imagers:
 
 1. `fix_ms_dir` : ASKAP MeasurementSets are phased towards the centre of field, but not the centre of its given beam. This utility reads the appropriate offsets to the beam centre from the `BEAM_OFFSET` and updates the `FIELD` table, as well as the phase and delay reference columns.
 
 2. `fix_ms_corrs` : ASKAP MeasurementSets, as calibrated by the obervatory, provide correlations in the instrument frame. ASKAP has a unique 'roll' axis which means, in principle, the instrument frame can be at any arbitrary rotation on the sky. This utility applies the appropriate rotation matrix to the visibilities such the 'X' is aligned North-South and 'Y' is aligned East-West (IAU convention). Further, ASKAPsoft defines Stokes I as $I=XX+YY$, whereas most other telescopes use $I=\frac{1}{2}(XX+YY)$ (note this also applies to all other Stokes paramters). This factor is also corrected for here at the same time as the rotation.
 
+Full documentation on [Read The Docs](https://fixms.readthedocs.io/en/latest/).
+
 ## Installation
 
 Obtain and install Python 3 (I recommend [Miniforge](https://github.com/conda-forge/miniforge) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)).
 
 Install the Python scripts:
 
 Latest:
```


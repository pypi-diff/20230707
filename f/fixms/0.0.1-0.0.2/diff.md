# Comparing `tmp/fixms-0.0.1.tar.gz` & `tmp/fixms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixms-0.0.1.tar", max compression
+gzip compressed data, was "fixms-0.0.2.tar", max compression
```

## Comparing `fixms-0.0.1.tar` & `fixms-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3216 2023-07-07 07:58:45.133732 fixms-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-07 07:58:45.133732 fixms-0.0.1/fixms/__init__.py
--rw-r--r--   0        0        0    12138 2023-07-07 07:58:45.133732 fixms-0.0.1/fixms/fix_ms_corrs.py
--rw-r--r--   0        0        0    12457 2023-07-07 07:58:45.133732 fixms-0.0.1/fixms/fix_ms_dir.py
--rw-r--r--   0        0        0      713 2023-07-07 07:58:45.133732 fixms-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 fixms-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-07 08:10:30.113801 fixms-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3097 2023-07-07 08:10:30.113801 fixms-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 08:10:30.113801 fixms-0.0.2/fixms/__init__.py
+-rw-r--r--   0        0        0    12138 2023-07-07 08:10:30.113801 fixms-0.0.2/fixms/fix_ms_corrs.py
+-rw-r--r--   0        0        0    12457 2023-07-07 08:10:30.113801 fixms-0.0.2/fixms/fix_ms_dir.py
+-rw-r--r--   0        0        0      729 2023-07-07 08:10:30.113801 fixms-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3742 1970-01-01 00:00:00.000000 fixms-0.0.2/PKG-INFO
```

### Comparing `fixms-0.0.1/README.md` & `fixms-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest) [![Python package](https://github.com/AlecThomson/FixMS/actions/workflows/main.yml/badge.svg)](https://github.com/AlecThomson/FixMS/actions/workflows/main.yml)
+[![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest)](https://fixms.readthedocs.io/)
 
 # FixMS
 
 ASKAP utilities for updating MeasurementSets for external imagers.
 
-ASKAP MSs are produced in a way that breaks compatibility with most other imagers (e.g. CASA, WSclean). Here we provide two modules (with CLI hooks) that fix the two stages that need to be applied to produce astronomically correct imagers with non-YandaSoft imagers:
+ASKAP MSs are produced in a way that breaks compatibility with most other imagers (e.g. CASA, WSclean). Here we provide two modules (with CLI hooks) that perform the fixes that need to be applied in order to produce astronomically correct imagers with non-YandaSoft imagers:
 
 1. `fix_ms_dir` : ASKAP MeasurementSets are phased towards the centre of field, but not the centre of its given beam. This utility reads the appropriate offsets to the beam centre from the `BEAM_OFFSET` and updates the `FIELD` table, as well as the phase and delay reference columns.
 
 2. `fix_ms_corrs` : ASKAP MeasurementSets, as calibrated by the obervatory, provide correlations in the instrument frame. ASKAP has a unique 'roll' axis which means, in principle, the instrument frame can be at any arbitrary rotation on the sky. This utility applies the appropriate rotation matrix to the visibilities such the 'X' is aligned North-South and 'Y' is aligned East-West (IAU convention). Further, ASKAPsoft defines Stokes I as $I=XX+YY$, whereas most other telescopes use $I=\frac{1}{2}(XX+YY)$ (note this also applies to all other Stokes paramters). This factor is also corrected for here at the same time as the rotation.
 
 Full documentation on [Read The Docs](https://fixms.readthedocs.io/en/latest/).
```

### Comparing `fixms-0.0.1/fixms/fix_ms_corrs.py` & `fixms-0.0.2/fixms/fix_ms_corrs.py`

 * *Files identical despite different names*

### Comparing `fixms-0.0.1/fixms/fix_ms_dir.py` & `fixms-0.0.2/fixms/fix_ms_dir.py`

 * *Files identical despite different names*

### Comparing `fixms-0.0.1/pyproject.toml` & `fixms-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "fixms"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Alec Thomson (S&A, Kensington WA) <alec.thomson@csiro.au>"]
 readme = "README.md"
+license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "*"
 astropy = "^5"
 python-casacore = "*"
 tqdm = "*"
```

### Comparing `fixms-0.0.1/PKG-INFO` & `fixms-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: fixms
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
+License: MIT
 Author: Alec Thomson (S&A, Kensington WA)
 Author-email: alec.thomson@csiro.au
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Requires-Dist: astropy (>=5,<6)
 Requires-Dist: numpy
 Requires-Dist: python-casacore
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest) [![Python package](https://github.com/AlecThomson/FixMS/actions/workflows/main.yml/badge.svg)](https://github.com/AlecThomson/FixMS/actions/workflows/main.yml)
+[![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest)](https://fixms.readthedocs.io/)
 
 # FixMS
 
 ASKAP utilities for updating MeasurementSets for external imagers.
 
-ASKAP MSs are produced in a way that breaks compatibility with most other imagers (e.g. CASA, WSclean). Here we provide two modules (with CLI hooks) that fix the two stages that need to be applied to produce astronomically correct imagers with non-YandaSoft imagers:
+ASKAP MSs are produced in a way that breaks compatibility with most other imagers (e.g. CASA, WSclean). Here we provide two modules (with CLI hooks) that perform the fixes that need to be applied in order to produce astronomically correct imagers with non-YandaSoft imagers:
 
 1. `fix_ms_dir` : ASKAP MeasurementSets are phased towards the centre of field, but not the centre of its given beam. This utility reads the appropriate offsets to the beam centre from the `BEAM_OFFSET` and updates the `FIELD` table, as well as the phase and delay reference columns.
 
 2. `fix_ms_corrs` : ASKAP MeasurementSets, as calibrated by the obervatory, provide correlations in the instrument frame. ASKAP has a unique 'roll' axis which means, in principle, the instrument frame can be at any arbitrary rotation on the sky. This utility applies the appropriate rotation matrix to the visibilities such the 'X' is aligned North-South and 'Y' is aligned East-West (IAU convention). Further, ASKAPsoft defines Stokes I as $I=XX+YY$, whereas most other telescopes use $I=\frac{1}{2}(XX+YY)$ (note this also applies to all other Stokes paramters). This factor is also corrected for here at the same time as the rotation.
 
 Full documentation on [Read The Docs](https://fixms.readthedocs.io/en/latest/).
```


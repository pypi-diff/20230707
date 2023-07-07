# Comparing `tmp/dfm_tools-0.11.0.tar.gz` & `tmp/dfm_tools-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfm_tools-0.11.0.tar", last modified: Sun Apr 23 22:49:21 2023, max compression
+gzip compressed data, was "dfm_tools-0.12.0.tar", last modified: Fri Jul  7 15:39:56 2023, max compression
```

## Comparing `dfm_tools-0.11.0.tar` & `dfm_tools-0.12.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3492 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/dfm_tools/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/bathymetry.py
--rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    17127 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/energy_dissipation.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    28771 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/get_nc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9793 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/get_nc_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    18353 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/hydrolib_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    32206 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/interpolate_grid2bnd.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/linebuilder.py
--rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/meshkernel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13218 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/modelbuilder.py
--rw-r--r--   0 runner    (1001) docker     (122)    23929 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/modplot.py
--rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/regulargrid.py
--rw-r--r--   0 runner    (1001) docker     (122)    27467 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/dfm_tools/xarray_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/dfm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4181 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-23 22:49:21.000000 dfm_tools-0.11.0/dfm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1728 2023-04-23 22:49:21.437927 dfm_tools-0.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-23 22:49:21.433927 dfm_tools-0.11.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19768 2023-04-23 22:49:08.000000 dfm_tools-0.11.0/tests/test_dfm_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2353 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/dfm_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/bathymetry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/coastlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4227 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17494 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/energy_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28537 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/get_nc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9793 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/get_nc_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21311 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/hydrolib_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35184 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/interpolate_grid2bnd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/linebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12273 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/meshkernel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/modelbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23929 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/modplot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19385 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/xarray_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17957 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/dfm_tools/xugrid_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/dfm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-07 15:39:56.000000 dfm_tools-0.12.0/dfm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:39:56.692954 dfm_tools-0.12.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15155 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/test_dfm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/test_external_packages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/test_meshkernel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-07 15:39:42.000000 dfm_tools-0.12.0/tests/utils.py
```

### Comparing `dfm_tools-0.11.0/PKG-INFO` & `dfm_tools-0.12.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 Metadata-Version: 2.1
 Name: dfm_tools
-Version: 0.11.0
+Version: 0.12.0
 Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
 Home-page: https://github.com/Deltares/dfm_tools
 Author: Jelmer Veenstra
 Author-email: Jelmer.Veenstra@Deltares.nl
 License: GNU General Public License v3 (GPLv3)
 Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: complete
 
 [![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
 [![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
 [![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
+[![pytest-py311](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml)
 [![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
-[![generate-documentation](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
+[![Available on pypi](https://img.shields.io/pypi/v/dfm_tools.svg)](https://pypi.python.org/pypi/dfm_tools)
+[![Supported versions](https://img.shields.io/pypi/pyversions/dfm_tools.svg)](https://pypi.org/project/dfm_tools)
+[![Downloads](https://img.shields.io/pypi/dm/dfm_tools.svg)](https://pypistats.org/packages/dfm_tools)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7857393.svg)](https://doi.org/10.5281/zenodo.7857393)
 
-dfm_tools
-=========
+# dfm_tools
 
 A Python package for pre- and postprocessing D-FlowFM model input and output files. Contains convenience functions built on top of other packages like [xarray](https://github.com/pydata/xarray), [xugrid](https://github.com/Deltares/xugrid), [hydrolib-core](https://github.com/Deltares/HYDROLIB-core) and many more.
 
-Information and examples
---------
-- [pdf](https://nbviewer.org/github/Deltares/dfm_tools/raw/pptx/docs/dfm_tools.pdf?flush_cache=true) with dfm_tools information, features and examples
-- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/dfm_tools/blob/main/docs/dfm_tools/index.html) generated from docstrings
-- [jupyter notebooks](https://github.com/Deltares/dfm_tools/blob/main/notebooks) with example code
-- [use binder](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD) to run these notebooks interactively (loading takes a while)
-- [github folder](https://github.com/Deltares/dfm_tools/tree/main/tests/examples) with more example scripts
+## Information
 
-Installation basics
---------
-- latest release: ``pip install dfm_tools`` (excludes ``cartopy`` since it is only installable via conda)
-
-Installation recommendation
---------
-- download and install Anaconda 64 bit (with Python 3.8 or later) from https://www.anaconda.com/distribution/#download-section
-- open Anaconda prompt
-- ``conda create --name dfm_tools_env -c conda-forge python=3.8 spyder -y`` (you can also install a newer python version)
-- ``conda activate dfm_tools_env``
-- ``conda install -c conda-forge git shapely cartopy pyepsg geopandas contextily xarray dask netcdf4 bottleneck xugrid cdsapi pydap -y`` (installs conda-forge requirements)
-- ``python -m pip install git+https://github.com/Deltares/dfm_tools`` (this command installs dfm_tools and all required non-conda packages, also use to update)
-- long paths error? Check [this Github issue](https://github.com/Deltares/HYDROLIB-core/issues/327#issuecomment-1266534032)
-- OpenSSL error? Fix your conda base env by doing [this](https://github.com/conda/conda/issues/11795#issuecomment-1335666474) or maybe [this](https://github.com/conda/conda/issues/11795#issuecomment-1382661765). Let us know if you encounter this issue.
-- to remove environment when necessary: ``conda remove -n dfm_tools_env --all``
+- install with ``pip install dfm_tools -U`` (or [installation guide](https://deltares.github.io/dfm_tools/installation))
+- [online documentation](https://deltares.github.io/dfm_tools) with installation guide, contributing guide, tutorials/examples, API reference and a convenient search box.
+- Bug or feature request? Create a [GitHub issue](https://github.com/Deltares/dfm_tools/issues)
```

### Comparing `dfm_tools-0.11.0/README.md` & `dfm_tools-0.12.0/dfm_tools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,46 @@
+Metadata-Version: 2.1
+Name: dfm-tools
+Version: 0.12.0
+Summary: dfm_tools are pre- and post-processing tools for Delft3D FM
+Home-page: https://github.com/Deltares/dfm_tools
+Author: Jelmer Veenstra
+Author-email: Jelmer.Veenstra@Deltares.nl
+License: GNU General Public License v3 (GPLv3)
+Keywords: dfm_tools,D-FlowFM,D-HYDRO,post-processing,pre-processing,mapfiles,hisfiles
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: complete
+
 [![pytest-py38](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py38.yml)
 [![pytest-py39](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py39.yml)
 [![pytest-py310](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py310.yml)
+[![pytest-py311](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml/badge.svg?branch=main)](https://github.com/Deltares/dfm_tools/actions/workflows/pytest-py311.yml)
 [![codecov](https://img.shields.io/codecov/c/github/deltares/dfm_tools.svg?style=flat-square)](https://app.codecov.io/gh/deltares/dfm_tools?displayType=list)
-[![generate-documentation](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml/badge.svg)](https://github.com/Deltares/dfm_tools/actions/workflows/generate-documentation.yml)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Deltares_dfm_tools&metric=alert_status)](https://sonarcloud.io/summary/overall?id=Deltares_dfm_tools)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD)
+[![Available on pypi](https://img.shields.io/pypi/v/dfm_tools.svg)](https://pypi.python.org/pypi/dfm_tools)
+[![Supported versions](https://img.shields.io/pypi/pyversions/dfm_tools.svg)](https://pypi.org/project/dfm_tools)
+[![Downloads](https://img.shields.io/pypi/dm/dfm_tools.svg)](https://pypistats.org/packages/dfm_tools)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7857393.svg)](https://doi.org/10.5281/zenodo.7857393)
 
-dfm_tools
-=========
+# dfm_tools
 
 A Python package for pre- and postprocessing D-FlowFM model input and output files. Contains convenience functions built on top of other packages like [xarray](https://github.com/pydata/xarray), [xugrid](https://github.com/Deltares/xugrid), [hydrolib-core](https://github.com/Deltares/HYDROLIB-core) and many more.
 
-Information and examples
---------
-- [pdf](https://nbviewer.org/github/Deltares/dfm_tools/raw/pptx/docs/dfm_tools.pdf?flush_cache=true) with dfm_tools information, features and examples
-- [online documentation](https://htmlpreview.github.io/?https://github.com/Deltares/dfm_tools/blob/main/docs/dfm_tools/index.html) generated from docstrings
-- [jupyter notebooks](https://github.com/Deltares/dfm_tools/blob/main/notebooks) with example code
-- [use binder](https://mybinder.org/v2/gh/Deltares/dfm_tools/HEAD) to run these notebooks interactively (loading takes a while)
-- [github folder](https://github.com/Deltares/dfm_tools/tree/main/tests/examples) with more example scripts
-
-Installation basics
---------
-- latest release: ``pip install dfm_tools`` (excludes ``cartopy`` since it is only installable via conda)
+## Information
 
-Installation recommendation
---------
-- download and install Anaconda 64 bit (with Python 3.8 or later) from https://www.anaconda.com/distribution/#download-section
-- open Anaconda prompt
-- ``conda create --name dfm_tools_env -c conda-forge python=3.8 spyder -y`` (you can also install a newer python version)
-- ``conda activate dfm_tools_env``
-- ``conda install -c conda-forge git shapely cartopy pyepsg geopandas contextily xarray dask netcdf4 bottleneck xugrid cdsapi pydap -y`` (installs conda-forge requirements)
-- ``python -m pip install git+https://github.com/Deltares/dfm_tools`` (this command installs dfm_tools and all required non-conda packages, also use to update)
-- long paths error? Check [this Github issue](https://github.com/Deltares/HYDROLIB-core/issues/327#issuecomment-1266534032)
-- OpenSSL error? Fix your conda base env by doing [this](https://github.com/conda/conda/issues/11795#issuecomment-1335666474) or maybe [this](https://github.com/conda/conda/issues/11795#issuecomment-1382661765). Let us know if you encounter this issue.
-- to remove environment when necessary: ``conda remove -n dfm_tools_env --all``
+- install with ``pip install dfm_tools -U`` (or [installation guide](https://deltares.github.io/dfm_tools/installation))
+- [online documentation](https://deltares.github.io/dfm_tools) with installation guide, contributing guide, tutorials/examples, API reference and a convenient search box.
+- Bug or feature request? Create a [GitHub issue](https://github.com/Deltares/dfm_tools/issues)
```

### Comparing `dfm_tools-0.11.0/dfm_tools/__init__.py` & `dfm_tools-0.12.0/dfm_tools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 .. include:: ../README.md
 """
 
 __author__ = """Jelmer Veenstra"""
 __email__ = 'jelmer.veenstra@deltares.nl'
-__version__ = '0.11.0'
+__version__ = '0.12.0'
 
 from dfm_tools.deprecated import *
 from dfm_tools.errors import *
 from dfm_tools.download import *
 from dfm_tools.get_nc import *
 from dfm_tools.get_nc_helpers import *
 from dfm_tools.hydrolib_helpers import *
 from dfm_tools.meshkernel_helpers import *
 from dfm_tools.interpolate_grid2bnd import *
 from dfm_tools.linebuilder import *
 from dfm_tools.modplot import *
-from dfm_tools.regulargrid import *
 from dfm_tools.xarray_helpers import *
+from dfm_tools.xugrid_helpers import *
 from dfm_tools.energy_dissipation import *
 from dfm_tools.bathymetry import *
+from dfm_tools.coastlines import *
 #from dfm_tools.modelbuilder import * #commented since we do not want to expose these functions with hardcoded parameters
 
 import warnings
 warnings.filterwarnings('always',category=DeprecationWarning)
```

### Comparing `dfm_tools-0.11.0/dfm_tools/bathymetry.py` & `dfm_tools-0.12.0/dfm_tools/bathymetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 @author: veenstra
 """
 
 import numpy as np
 
 
 def write_bathy_toasc(filename_asc,lon_sel_ext,lat_sel_ext,elev_sel_ext,asc_fmt='%9.2f',nodata_val=32767):
+    """
+    empty docstring
+    """
 
     print('writing to asc file')
     if elev_sel_ext.shape != (lat_sel_ext.shape[0], lon_sel_ext.shape[0]):
         raise ValueError('resulting shape of elev_sel_ext %s is not consistent with lat_sel_ext/lon_sel_ext vars %s'%(elev_sel_ext.shape,(lat_sel_ext.shape[0], lon_sel_ext.shape[0])))
     if isinstance(elev_sel_ext,np.ma.core.MaskedArray): #masked has to be filled in order for the nans to be visible
         elev_sel_ext = elev_sel_ext.filled(np.nan)
     if np.isnan(elev_sel_ext).sum()>0:
```

### Comparing `dfm_tools-0.11.0/dfm_tools/download.py` & `dfm_tools-0.12.0/dfm_tools/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 
 import os
 import pandas as pd
 from pathlib import Path
 import xarray as xr
 from pydap.client import open_url
 from pydap.cas.get_cookies import setup_session
-import warnings
 from dfm_tools.errors import OutOfRangeError
 import cdsapi
 import cftime
 
 
 def download_ERA5(varkey,
                   longitude_min, longitude_max, latitude_min, latitude_max, 
                   date_min, date_max,
                   dir_output='.', overwrite=False):
+    """
+    empty docstring
+    """
     
     #TODO: describe something about the .cdsapirc file
     #TODO: make this function cdsapi generic, instead of ERA5 hardcoded (make flexible for product_type/name/name_output) (variables_dict is not used actively anymore, so this is possible)
     
     c = cdsapi.Client() # import cdsapi and create a Client instance # https://cds.climate.copernicus.eu/api-how-to
     
     #dictionary with ERA5 variables #this is not actively used
@@ -41,21 +43,28 @@
                       'msl':'mean_sea_level_pressure',
                       'u10':'10m_u_component_of_wind',
                       'u10n':'10m_u_component_of_neutral_wind',
                       'v10':'10m_v_component_of_wind',
                       'v10n':'10m_v_component_of_neutral_wind',
                       'mer':'mean_evaporation_rate',
                       'mtpr':'mean_total_precipitation_rate',
+                      'p140209':'air_density_over_the_oceans',
                       }
     if varkey not in variables_dict.keys(): #TODO: how to get list of available vars? mean_sea_level_pressure and msl both return a dataset with msl varkey, but standard_name air_pressure_at_mean_sea_level returns an error
         raise KeyError(f'"{varkey}" not available, choose from: {list(variables_dict.keys())}')
     
     period_range = pd.period_range(date_min,date_max,freq='M')
     print(f'retrieving data from {period_range[0]} to {period_range[-1]} (freq={period_range.freq})')
     
+    #make sure the data fully covers the desired spatial extent. Download 1 additional grid cell (resolution is 1/4 degrees) in both directions
+    longitude_min -= 1/4
+    longitude_max += 1/4
+    latitude_min  -= 1/4
+    latitude_max  += 1/4
+    
     for date in period_range:
         name_output = f'era5_{varkey}_{date.strftime("%Y-%m")}.nc'
         file_out = Path(dir_output,name_output)
         if file_out.is_file() and not overwrite:
             print(f'"{name_output}" found and overwrite=False, continuing.')
             continue
         print (f'retrieving ERA5 data for variable "{varkey}" and month {date.strftime("%Y-%m")} (YYYY-MM)')
@@ -75,84 +84,86 @@
 
 
 def download_CMEMS(varkey,
                    longitude_min, longitude_max, latitude_min, latitude_max, 
                    date_min, date_max, freq='D',
                    dir_output='.', file_prefix='', overwrite=False,
                    credentials=None):
+    """
+    empty docstring
+    """
 
-    date_min = pd.Timestamp(date_min)-pd.Timedelta(days=1) #CMEMS has daily noon values (not midnight), so subtract one day from date_min to cover desired time extent
+    date_min, date_max = round_timestamp_to_outer_noon(date_min,date_max)
     
-    if 'my_datemax' not in globals(): #set multiyear date_max (my_datemax) as global variable, so it only has to be retreived once per download run (otherwise once per variable)
-        print('retrieving enddate of multiyear CMEMS dataset')
-        dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m' #assuming here that physchem and bio reanalyisus/multiyear datasets have the same enddate, this seems safe
-        ds = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
-        my_times = ds.time.to_series()
-        global my_datemax
-        my_datemax = my_times.iloc[-1]
-
-    if pd.Timestamp(date_max) <= my_datemax:
-        product = 'reanalysis'
-    elif pd.Timestamp(date_min) > my_datemax:
-        product = 'analysisforecast'
-    else:
-        raise ValueError(f'Requested timerange is {date_min} to {date_max}. Currently, it is only possible to query periods before OR after the multiyear/reanalysis enddate ({my_datemax}).')
+    global product #set product as global variable, so it only has to be retreived once per download run (otherwise once per variable)
+    if 'product' not in globals():
+        print('retrieving time range of CMEMS reanalysis and forecast products') #assuming here that physchem and bio reanalyisus/multiyear datasets have the same enddate, this seems safe
+        reanalysis_tstart, reanalysis_tstop = get_OPeNDAP_xr_ds_timerange(dataset_url='https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m', credentials=credentials)
+        forecast_tstart, forecast_tstop = get_OPeNDAP_xr_ds_timerange(dataset_url='https://nrt.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_anfc_0.083deg_P1D-m', credentials=credentials)
+        if (date_min >= reanalysis_tstart) & (date_max <= reanalysis_tstop):
+            product = 'reanalysis'
+            print(f"The CMEMS '{product}' product will be used.")
+        elif (date_min >= forecast_tstart) & (date_max <= forecast_tstop):
+            product = 'analysisforecast'
+            print(f"The CMEMS '{product}' product will be used.")
+        else:
+            raise ValueError(f'Requested timerange ({date_min} to {date_max}) is not fully within timerange of reanalysis product ({reanalysis_tstart} to {reanalysis_tstop}) or forecast product ({forecast_tstart} to {forecast_tstop}).')
     
     Path(dir_output).mkdir(parents=True, exist_ok=True)
     if varkey in ['bottomT','tob','mlotst','siconc','sithick','so','thetao','uo','vo','usi','vsi','zos']: #for physchem
         if product == 'analysisforecast': #forecast: https://data.marine.copernicus.eu/product/GLOBAL_ANALYSISFORECAST_PHY_001_024/description
-            if varkey=='bottomT': #rename old to new anfc varname (still called bottomT in reanalysis)
-                varkey = 'tob'
-            if varkey in ['uo','vo']:
+            if varkey in ['uo','vo']: #anfc datset is splitted over multiple urls, construct the correct one here.
                 varkey_name = 'phy-cur'
             elif varkey in ['so','thetao']:
                 varkey_name = 'phy-'+varkey
             else:
                 varkey_name = 'phy'
             dataset_url = f'https://nrt.cmems-du.eu/thredds/dodsC/cmems_mod_glo_{varkey_name}_anfc_0.083deg_P1D-m'#.html' #TODO: also PT6H-i timeresolution available but not for all variables and not for reanalysis
         else: #reanalysis: https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/description
             dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m'
     else: #for bio
         if product == 'analysisforecast': #forecast: https://data.marine.copernicus.eu/product/GLOBAL_ANALYSISFORECAST_PHY_001_024/description
             dataset_url = 'https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-bio-001-028-daily' #contains ['chl','fe','no3','nppv','o2','ph','phyc','po4','si','spco2']
         else: #https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_BGC_001_029/description
             dataset_url = 'https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_bgc_my_0.25_P1D-m' #contains ['chl','no3','nppv','o2','po4','si']
     
+    #make sure the data fully covers the desired spatial extent. Download 2 additional grid cells (resolution is 1/12 degrees, but a bit more/less in alternating cells) in each direction
+    longitude_min -= 2/12
+    longitude_max += 2/12
+    latitude_min  -= 2/12
+    latitude_max  += 2/12
+    
     download_OPeNDAP(dataset_url=dataset_url,
                      credentials=credentials, #credentials=['username','password'], or create "%USERPROFILE%/CMEMS_credentials.txt" with username on line 1 and password on line 2. Register at: https://resources.marine.copernicus.eu/registration-form'
                      varkey=varkey,
                      longitude_min=longitude_min, longitude_max=longitude_max, latitude_min=latitude_min, latitude_max=latitude_max,
                      date_min=date_min, date_max=date_max,
                      dir_output=dir_output, file_prefix=file_prefix, overwrite=overwrite)
 
 
+def get_CMEMS_credentials():
+    """
+    parse file with CMEMS credentials to username/password
+    """
+    file_credentials = f'{os.path.expanduser("~")}/CMEMS_credentials.txt'
+    if not os.path.exists(file_credentials):
+        raise FileNotFoundError(f'credentials argument not supplied and file_credentials not available ({file_credentials})')
+    with open(file_credentials) as fc:
+        username = fc.readline().strip()
+        password = fc.readline().strip()
+    return username, password
+
+
 def open_OPeNDAP_xr(dataset_url, credentials=None):
     """
     How to get the opendap dataset_url (CMEMS example):
         - https://data.marine.copernicus.eu/products
         - go to the data access tab of a product, e.g.: https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/services
         - click the opendap link of the dataset of your choice
         - copy the dataset_url from the adress bar (excl .html), e.g.: https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m
-        
-        Example multiyear phys/chem:
-            https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/services
-            https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_phy_my_0.083_P1D-m
-            ['bottomT','mlotst','siconc','sithick','so','thetao','uo','usi','vo','vsi','zos']
-        Example multiyear bio:
-            https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_BGC_001_029/services
-            https://my.cmems-du.eu/thredds/dodsC/cmems_mod_glo_bgc_my_0.25_P1D-m
-            ['chl','no3','nppv','o2','po4','si']
-        Example forecast phys/chem:
-            https://data.marine.copernicus.eu/product/GLOBAL_ANALYSIS_FORECAST_PHY_001_024/services
-            https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-phy-001-024
-            ['bottomT','mlotst','siconc','sithick','so','thetao','uo','usi','vo','vsi','zos']
-        Example forecast bio:
-            https://data.marine.copernicus.eu/product/GLOBAL_ANALYSIS_FORECAST_BIO_001_028/services
-            https://nrt.cmems-du.eu/thredds/dodsC/global-analysis-forecast-bio-001-028-daily
-            ['chl','fe','no3','nppv','o2','ph','phyc','po4','si','spco2']
     
     How to get the opendap dataset_url (HYCOM example):
         - https://www.hycom.org/dataserver
         - Select a product and search for THREDDS, e.g.: https://www.hycom.org/dataserver/gofs-3pt1/analysis
         - find an opendap dataset_url, it depends per product/run where to find it.
         Some examples:
             https://tds.hycom.org/thredds/dodsC/GLBu0.08/expt_19.1/2010
@@ -165,41 +176,34 @@
         cas_url = 'https://cmems-cas.cls.fr/cas/login'
         session = setup_session(cas_url, username, password)
         cookies_dict = session.cookies.get_dict()
         if 'CASTGC' not in cookies_dict.keys():
             raise KeyError('CASTGC key missing from session cookies_dict, probably authentication failure')
         session.cookies.set("CASTGC", cookies_dict['CASTGC'])
         #TODO: add check for wrong dataset_id (now always "AttributeError: You cannot set the charset when no content-type is defined")
-        DAP_dataset = open_url(dataset_url, session=session)#, user_charset='utf-8') # TODO: user_charset needs PyDAP >= v3.3.0 see https://github.com/pydap/pydap/pull/223/commits 
-        data_store = xr.backends.PydapDataStore(DAP_dataset)
+        dap_dataset = open_url(dataset_url, session=session, user_charset='utf-8')
+        data_store = xr.backends.PydapDataStore(dap_dataset)
         return data_store
     
     if isinstance(dataset_url,list):
         dataset_url_one = dataset_url[0]
     else:
         dataset_url_one = dataset_url
     
     if 'cmems-du.eu' in dataset_url_one:
         if isinstance(dataset_url,list):
             raise TypeError('list not supported by opendap method used for cmems')
         
-        #parse credentials to username/password #TODO: now CMEMS specific, make more generic
         if credentials is None:
-            file_credentials = f'{os.path.expanduser("~")}/CMEMS_credentials.txt'
-            if not os.path.exists(file_credentials):
-                raise FileNotFoundError(f'credentials argument not supplied and file_credentials not available ({file_credentials})')
-            with open(file_credentials) as fc:
-                username = fc.readline().strip()
-                password = fc.readline().strip()
+            username, password = get_CMEMS_credentials() #parse file with CMEMS credentials to username/password
         else:
-            username,password = credentials
+            username, password = credentials
 
-        print(f'opening pydap connection to opendap dataset: {dataset_url}.html')
+        print(f'opening pydap connection to opendap dataset and opening with xarray: {dataset_url}.html')
         data_store = copernicusmarine_datastore(dataset_url=dataset_url, username=username, password=password)
-        print('xarray opening opendap dataset')
         data_xr = xr.open_dataset(data_store)
     elif 'hycom.org' in dataset_url_one:
         if isinstance(dataset_url,list):
             print(f'xarray opening opendap dataset like: {dataset_url[0]}.html ({len(dataset_url)} urls/years)')
             data_xr = xr.open_mfdataset(dataset_url,decode_times=False) #TODO: for some reason decode_times does not work: "ValueError: unable to decode time units 'hours since analysis' with 'the default calendar'."
         else:
             print(f'xarray opening opendap dataset: {dataset_url}.html')
@@ -305,7 +309,27 @@
         
         print(f'xarray subsetting data per {period_range.freq}: {date_str}')
         data_xr_var_seltime = data_xr_var.sel(time=slice(date_str,date_str)) #+' 12:00:00', 
         
         print(f'xarray writing netcdf file: {name_output}')
         data_xr_var_seltime.to_netcdf(os.path.join(dir_output,name_output)) #TODO: add chunks={'time':1} or only possible with opening?
         data_xr_var_seltime.close()
+
+
+def get_OPeNDAP_xr_ds_timerange(dataset_url, credentials):
+    ds = open_OPeNDAP_xr(dataset_url=dataset_url, credentials=credentials)
+    ds_times = ds.time.to_series()
+    ds_tstart, ds_tstop = ds_times.iloc[0], ds_times.iloc[-1]
+    return ds_tstart, ds_tstop
+
+
+def round_timestamp_to_outer_noon(date_min, date_max):
+    """
+    Since the CMEMS dataset only contains noon-values, we often need to round to the previous or next noon timestep to download enough data.
+    
+    """
+    
+    td_12h = pd.Timedelta(hours=12)
+    date_min = (pd.Timestamp(date_min) + td_12h).floor('1d') - td_12h
+    date_max = (pd.Timestamp(date_max) - td_12h).ceil('1d') + td_12h
+    return date_min, date_max
+
```

### Comparing `dfm_tools-0.11.0/dfm_tools/energy_dissipation.py` & `dfm_tools-0.12.0/dfm_tools/energy_dissipation.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.11.0/dfm_tools/get_nc.py` & `dfm_tools-0.12.0/dfm_tools/get_nc.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,28 @@
 
 import numpy as np
 import datetime as dt
 import re
 import xugrid as xu
 import xarray as xr
 import matplotlib.pyplot as plt
-from dfm_tools.xarray_helpers import get_vertical_dimensions, Dataset_varswithdim
+from dfm_tools.xarray_helpers import Dataset_varswithdim
+from dfm_tools.xugrid_helpers import get_vertical_dimensions
 import netCDF4
 
 
 def calc_dist_pythagoras(x1,x2,y1,y2):
     distance = np.sqrt((x2 - x1)**2 + (y2 - y1)**2)
     return distance
 
 
 def calc_dist_haversine(lon1,lon2,lat1,lat2):
-    """
-    calculates distance between lat/lon coordinates in meters
-    https://community.esri.com/t5/coordinate-reference-systems-blog/distance-on-a-sphere-the-haversine-formula/ba-p/902128
-    """
+    #calculates distance between lat/lon coordinates in meters
+    #https://community.esri.com/t5/coordinate-reference-systems-blog/distance-on-a-sphere-the-haversine-formula/ba-p/902128
+    
     # convert to radians
     lon1_rad = np.deg2rad(lon1)
     lon2_rad = np.deg2rad(lon2)
     lat1_rad = np.deg2rad(lat1)
     lat2_rad = np.deg2rad(lat2)
     
     # apply formulae
@@ -241,18 +241,18 @@
     uds = uds.set_coords(['mesh2d_flowelem_zw','mesh2d_flowelem_zcc'])
     return uds
 
 
 def reconstruct_zw_zcc_fromz(data_xr_map):
     """
     reconstruct full grid output (time/face-varying z-values) for zvalue model. Necessary when extracting values with zdepth w.r.t. waterlevel/bedlevel
+    """
     #TODO: gives spotty result for 0/0.1m w.r.t. bedlevel for Grevelingen zmodel
     #TODO: remove hardcoding of varnames (assuming wl/bl variables are available)
     #TODO: center values are clipped to waterlevel+bedlevel, so the center values of the top+bottom layer are currently incorrect
-    """
     
     dimn_layer, dimn_interfaces = get_vertical_dimensions(data_xr_map)
     
     data_frommap_wl_sel = data_xr_map['mesh2d_s1']
     data_frommap_z0_sel = data_frommap_wl_sel*0
     data_frommap_bl_sel = data_xr_map['mesh2d_flowelem_bl']
     
@@ -269,17 +269,16 @@
     return data_xr_map
 
 
 def reconstruct_zw_zcc_fromzsigma(uds):
     """
     reconstruct full grid output (time/face-varying z-values) for zsigmavalue model without full grid output. Implemented in https://issuetracker.deltares.nl/browse/UNST-5477
     based on https://cfconventions.org/cf-conventions/cf-conventions.html#_ocean_sigma_over_z_coordinate
-    #TODO: center values are clipped to bedlevel, so the center values of the bottom layer are currently incorrect
     """
-    
+    #TODO: center values are clipped to bedlevel, so the center values of the bottom layer are currently incorrect
     #TODO: default fillvalues are not automatically parsed to nan, so doing it manually: https://github.com/pydata/xarray/issues/2742
     fillvals = netCDF4.default_fillvals
     
     osz_formulaterms_int_dict = get_formula_terms(uds,varn_contains='interface')
     osz_formulaterms_lay_dict = get_formula_terms(uds,varn_contains='layer')
     
     uds_eta = uds[osz_formulaterms_int_dict['eta']] #mesh2d_s1
@@ -306,14 +305,17 @@
     uds['mesh2d_flowelem_zcc'] = zcc_sigmapart.fillna(zcc_zpart)
     
     uds = uds.set_coords(['mesh2d_flowelem_zw','mesh2d_flowelem_zcc'])
     return uds
 
 
 def reconstruct_zw_zcc(ds):
+    """
+    reconstruct full grid output (time/face-varying z-values) for all layertypes, passes on to respective reconstruction function
+    """
     dimn_layer, dimn_interfaces = get_vertical_dimensions(ds)
     
     if dimn_layer is not None: #D-FlowFM mapfile
         gridname = ds.grid.name
         varname_zint = f'{gridname}_flowelem_zw'
     elif 'laydim' in ds.dims: #D-FlowFM hisfile
         varname_zint = 'zcoordinate_w'
@@ -446,16 +448,15 @@
     return ds_atdepths
 
 
 def rasterize_ugrid(uds:xu.UgridDataset, ds_like:xr.Dataset = None, resolution:float = None):
     """
     Rasterizing ugrid dataset to regular dataset. ds_like has higher priority than `resolution`. If both are not passed, a raster is generated of at least 200x200
     inspired by xugrid.plot.imshow and xugrid.ugrid.ugrid2d.rasterize/rasterize_like.
-
-
+    
     Parameters
     ----------
     uds : xu.UgridDataset
         DESCRIPTION.
     ds_like : xr.Dataset, optional
         xr.Dataset with ed x and y variables to interpolate uds to. The default is None.
     resolution : float, optional
@@ -468,45 +469,38 @@
 
     Returns
     -------
     ds : TYPE
         DESCRIPTION.
 
     """
-    #TODO: maybe put part of code in xugrid (https://github.com/Deltares/xugrid/issues/31)
-    #TODO: vars can also be rasterized with uds_facevars[var].ugrid.rasterize(resolution), but is not efficient. Wait for uds.rasterize() method: https://github.com/Deltares/xugrid/issues/61
-    if not isinstance(uds,xu.core.wrap.UgridDataset):
-        raise TypeError(f'rasterize_ugrid expected xu.core.wrap.UgridDataset, got {type(uds)} instead')
     
-    grid = uds.grid
-    xu_facedim = uds.grid.face_dimension
-    uds_facevars = Dataset_varswithdim(uds,xu_facedim)
-    
-    if ds_like is not None:
-        regx = ds_like.x
-        regy = ds_like.y
+    if isinstance(uds,xu.core.wrap.UgridDataset):
+        xu_facedim = uds.grid.face_dimension
+        uds_facevars = Dataset_varswithdim(uds,xu_facedim)
+        face_str = f'Dataset with {len(uds_facevars.data_vars)} face variables'
+    elif isinstance(uds,xu.core.wrap.UgridDataArray):
+        face_str = 'DataArray'
     else:
-        xmin, ymin, xmax, ymax = grid.bounds
+        raise TypeError(f'rasterize_ugrid expected xu.core.wrap.UgridDataset or xu.core.wrap.UgridDataArray, got {type(uds)} instead')
+    
+    if ds_like is None:
+        xmin, ymin, xmax, ymax = uds.grid.bounds
         dx = xmax - xmin
         dy = ymax - ymin
         if resolution is None: # check if a rasterization resolution is passed, otherwise default to 200 raster cells otherwise for the smallest axis.
             resolution = min(dx, dy) / 200
         d = abs(resolution)
         regx = np.arange(xmin + 0.5 * d, xmax, d)
         regy = np.arange(ymin + 0.5 * d, ymax, d)
+        ds_like = xr.DataArray(np.empty((len(regy), len(regx))), {"y": regy, "x": regx}, ["y", "x"])
     
-    regx, regy, index = grid.rasterize_like(x=regx,y=regy) #TODO: this can be used to steer rasterization, eg with xstart/ystart/xres/yres
-    index_da = xr.DataArray(index,dims=('y','x'))
-    
-    print(f'>> rasterizing ugrid dataset with {len(uds_facevars.data_vars)} face variables to shape={index_da.shape}: ',end='')
+    print(f'>> rasterizing ugrid {face_str} to shape=({len(ds_like.y)},{len(ds_like.y)}): ',end='')
     dtstart = dt.datetime.now()
-    ds = uds_facevars.isel({xu_facedim:index_da})
-    ds = ds.where(index_da != grid.fill_value)
-    ds['x'] = xr.DataArray(regx,dims='x')
-    ds['y'] = xr.DataArray(regy,dims='y')
+    ds = uds.ugrid.rasterize_like(other=ds_like)
     print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
     
     return ds
 
 
 def plot_ztdata(data_xr_sel, varname, ax=None, only_contour=False, **kwargs):
     """
```

### Comparing `dfm_tools-0.11.0/dfm_tools/get_nc_helpers.py` & `dfm_tools-0.12.0/dfm_tools/get_nc_helpers.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.11.0/dfm_tools/hydrolib_helpers.py` & `dfm_tools-0.12.0/dfm_tools/hydrolib_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 import pandas as pd
 import cftime
 import numpy as np
 import xarray as xr
 from cftime import date2num
 import hydrolib.core.dflowfm as hcdfm
-import warnings
 import datetime as dt
+import geopandas
+from shapely.geometry import LineString
 
 
 def Dataset_to_T3D(datablock_xr):
     """
     convert an xarray.DataArray (is one data_var) or an xarray.Dataset (with one or two data_vars) with time and depth dimension to a hydrolib T3D object
     """
     
@@ -302,23 +303,14 @@
         
     if drop_emptycols:
         pointlike_pd = pointlike_pd.dropna(axis=1).copy()
         
     return pointlike_pd
 
 
-def parse_xy_to_datetime(pointlike_pd):
-    datatimevals_pdstr = (pointlike_pd['x'].astype(int).apply(lambda x:f'{x:08d}') +
-                          pointlike_pd['y'].astype(int).apply(lambda x:f'{x:06d}'))
-    pointlike_pd.index = pd.to_datetime(datatimevals_pdstr)
-    pointlike_pd_timeidx = pointlike_pd.drop(['x','y'],axis=1)
-    
-    return pointlike_pd_timeidx
-
-
 def TimModel_to_DataFrame(data_tim:hcdfm.TimModel, parse_column_labels:bool = True, refdate:(dt.datetime, pd.Timestamp, str) = None):
     """
     
 
     Parameters
     ----------
     data_tim : hcdfm.TimModel
@@ -362,7 +354,93 @@
     
     if refdate:
         refdate_pd = pd.Timestamp(refdate)
         tim_pd.index = refdate_pd + pd.to_timedelta(tim_pd.index,unit='minutes')
     
     return tim_pd
 
+
+def pointlike_to_geodataframe_points(polyline_object, crs='EPSG:4326', add_pointnames=True, only_xy=False):
+    """
+    empty docstring
+    """
+    #conversion to dataframe
+    #polyobject_pd = dfmt.pointnames(polyline_object)
+    polyobject_pd = pd.DataFrame([dict(p) for p in polyline_object.points])
+    
+    if only_xy:
+        df = pd.DataFrame()
+    else:
+        df = polyobject_pd.drop(['x','y'],axis=1) #also includes n/z and maybe data column
+    
+    if add_pointnames and hasattr(polyline_object,'metadata'): #optionally add names
+        df['plipoint_name'] = pd.Series(polyobject_pd.index).apply(lambda x: f'{polyline_object.metadata.name}_{x+1:04d}')
+    
+    #make gdf of points (1 point per row)
+    gdf = geopandas.GeoDataFrame(data=df, geometry=geopandas.points_from_xy(polyobject_pd['x'],polyobject_pd['y']), crs=crs)
+    
+    return gdf
+
+
+def PolyFile_to_geodataframe_points(polyfile_object:hcdfm.PolyFile, crs:str='EPSG:4326', add_pointnames:bool=True):
+    """
+    
+
+    Parameters
+    ----------
+    polyfile_object : hcdfm.PolyFile
+        get this object with hcdfm.PolyFile(path_to_plifile).
+    crs : str, optional
+        DESCRIPTION. The default is 'EPSG:4326'.
+    add_pointnames : bool, optional
+        DESCRIPTION. The default is True.
+
+    Returns
+    -------
+    gdf : TYPE
+        gdf of all the pli files with columns: location, geometry (Points). Crs = 4326 (decimal degrees).
+
+    """
+    
+    gdf_list = []
+    for polyobj in polyfile_object.objects:
+        gdf_one = pointlike_to_geodataframe_points(polyobj,crs=crs, add_pointnames=add_pointnames)
+        gdf_list.append(gdf_one)
+    gdf = pd.concat(gdf_list, ignore_index=True)
+    return gdf
+
+
+def PolyFile_to_geodataframe_linestrings(polyfile_object, crs='EPSG:4326'):
+    """
+    empty docstring
+    """
+    plilines_list = []
+    plinames_list = []
+    for iPO, polyline_object in enumerate(polyfile_object.objects):
+        polyobject_pd = pd.DataFrame([dict(p) for p in polyline_object.points]) #TODO: getting only x/y might be faster, but maybe we also need the other columns like z/n/data?
+        polygon_geom = LineString(zip(polyobject_pd['x'],polyobject_pd['y']))
+        
+        #make gdf of points (1 point per row)
+        plilines_list.append(polygon_geom)
+        plinames_list.append(polyline_object.metadata.name)
+    gdf_polyfile = geopandas.GeoDataFrame({'name': plinames_list, 'geometry': plilines_list}, crs=crs)
+    return gdf_polyfile
+
+
+def parse_xy_to_datetime(pointlike_pd):
+    datatimevals_pdstr = (pointlike_pd['x'].astype(int).apply(lambda x:f'{x:08d}') +
+                          pointlike_pd['y'].astype(int).apply(lambda x:f'{x:06d}'))
+    pointlike_pd.index = pd.to_datetime(datatimevals_pdstr)
+    pointlike_pd_timeidx = pointlike_pd.drop(['x','y'],axis=1)
+    
+    return pointlike_pd_timeidx
+
+
+def tekalobject_to_DataFrame(polyobject):
+    #conversion to dataframe
+    polyobject_pd = pointlike_to_DataFrame(polyobject)
+    
+    #conversion of xy to datetime
+    polyobject_pd = parse_xy_to_datetime(polyobject_pd) #TODO: not suported the other way round, necessary to add?
+    polyobject_pd.columns = polyobject.description.content.split('\n')[2:] #to fix legend labels
+    polyobject_pd.index.name = polyobject.metadata.name
+    return polyobject_pd
```

### Comparing `dfm_tools-0.11.0/dfm_tools/interpolate_grid2bnd.py` & `dfm_tools-0.12.0/dfm_tools/interpolate_grid2bnd.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 import os
 import glob
 import datetime as dt
 import numpy as np
 import pandas as pd
 import xarray as xr
+import xugrid as xu
 from pathlib import Path
 from scipy.spatial import KDTree
 import warnings
 import hydrolib.core.dflowfm as hcdfm
+import geopandas
 
-from dfm_tools.hydrolib_helpers import Dataset_to_TimeSeries, Dataset_to_T3D, Dataset_to_Astronomic, pointlike_to_DataFrame
+from dfm_tools.hydrolib_helpers import Dataset_to_TimeSeries, Dataset_to_T3D, Dataset_to_Astronomic, pointlike_to_DataFrame, PolyFile_to_geodataframe_points
 from dfm_tools.errors import OutOfRangeError
 
 
 def get_conversion_dict(ncvarname_updates={}):
     
     """
     get the conversion_dict, optionally with updated ncvarnames
@@ -72,14 +74,15 @@
     for k,v in ncvarname_updates.items():
         conversion_dict[k]['ncvarname'] = v
     return conversion_dict
 
 
 def interpolate_tide_to_bc(tidemodel, file_pli, component_list=None, nPoints=None):
     """
+    empty docstring
     """
     # translate dict from .\hydro_tools\FES\PreProcessing_FES_TideModel_imaginary.m
     #component_list = ['2N2','LABDA2','MF','MFM','P1','SSA','EPSILON2','M2','MKS2','MU2','Q1','T2','J1','M3','MM','N2','R2','K1','M4','MN4','N4','S1','K2','M6','MS4','NU2','S2','L2','M8','MSF','O1','S4','MSQM','SA']
     translate_dict = {'LA2':'LABDA2', #TODO: use value instead of key in bc file? Support using value instead of key in const_list also (like line above)
                       'EPS2':'EPSILON2', 
                       'Z0':'A0',
                       'MTM':'MFM', #Needs to be verified
@@ -91,14 +94,21 @@
                         'GTSM4.1preliminary': Path(r'p:\1230882-emodnet_hrsm\GTSMv3.0EMODnet\EMOD_MichaelTUM_yearcomponents\GTSMv4.1_yeartide_2014_2.20.06\compare_fouhis_fouxyz_v3','gtsmv4.1_2014_*_withfu_v3_rasterized.nc'),
                         #TODO: add tpxo8 (tpxo9 is also available), catalog: https://opendap.deltares.nl/thredds/catalog/opendap/deltares/delftdashboard/tidemodels/tpxo80/catalog.html
                         }
     if tidemodel not in dir_pattern_dict.keys():
         raise KeyError(f'invalid tidemodel "{tidemodel}", options are: {list(dir_pattern_dict.keys())}')
     if tidemodel == 'GTSM4.1preliminary':
         warnings.warn(UserWarning(f'you are using tidemodel "{tidemodel}", beware that the dataset is preliminary so it is still quite coarse and may contain errors. Check your results carefully'))
+    
+    #Check whether the polyfile contains multiple polyline, in that case show a warning
+    pli = hcdfm.PolyFile(file_pli)
+    if len(pli.objects) > 1:
+        warnings.warn(UserWarning(f"The polyfile {file_pli} contains multiple polylines. Only the first one will be used by DFLOW-FM for the boundary conditions."))
+        #TODO when issue UNST-7012 is solved, remove this warning or add it in more places)
+    
     dir_pattern = dir_pattern_dict[tidemodel]
     
     if component_list is None:
         file_list_nc = glob.glob(str(dir_pattern))
         dir_pattern_basename = os.path.basename(dir_pattern)
         replace = dir_pattern_basename.split('*')
         component_list = [os.path.basename(x).replace(replace[0],'').replace(replace[1],'') for x in file_list_nc] #TODO: make this less hard-coded
@@ -152,19 +162,22 @@
     
     ForcingModel_object = plipointsDataset_to_ForcingModel(plipointsDataset=data_interp)
     
     return ForcingModel_object
 
 
 def open_dataset_extra(dir_pattern, quantity, tstart, tstop, conversion_dict=None, refdate_str=None, reverse_depth=False, chunks=None):
+    """
+    empty docstring
+    """
     
     if conversion_dict is None:
         conversion_dict = get_conversion_dict()
     
-    if quantity=='uxuy': #T3Dvector
+    if quantity=='uxuyadvectionvelocitybnd': #T3Dvector
         quantity_list = ['ux','uy']
     else:
         quantity_list = [quantity]
     ncvarname_list = [conversion_dict[quan]['ncvarname'] for quan in quantity_list]
     
     #convert tstart/tstop from str/dt.datetime/pd.Timestamp to pd.Timestamp. WARNING: when supplying '05-04-2016', monthfirst is assumed, so 2016-05-04 will be the result (may instead of april).
     tstart = pd.Timestamp(tstart)
@@ -283,16 +296,16 @@
     
     return data_xr_vars
 
 
 def interp_regularnc_to_plipoints(data_xr_reg, file_pli, nPoints=None, load=True):
     """
     load: interpolation errors are only raised upon loading, so do this per default
-    #TODO: make format of this dataset more in line with existing bnd-nc format and hisfile: https://issuetracker.deltares.nl/browse/UNST-6549
     """
+    #TODO: make format of this dataset more in line with existing bnd-nc format and hisfile: https://issuetracker.deltares.nl/browse/UNST-6549
     data_xr_var = data_xr_reg #TODO: rename in script
     
     #load boundary file
     polyfile_object = hcdfm.PolyFile(file_pli)
     
     #check if polyobj names in plifile are unique
     polynames_pd = pd.Series([polyobj.metadata.name for polyobj in polyfile_object.objects])
@@ -380,14 +393,66 @@
         raise ValueError(f'{len(reqlatlon_pd_outbounds)} of requested pli points are out of bounds (valid longitude range {lonvar_vals.min()} to {lonvar_vals.max()}, valid latitude range {latvar_vals.min()} to {latvar_vals.max()}):\n{reqlatlon_pd_outbounds}')
     time_passed = (dt.datetime.now()-dtstart).total_seconds()
     print(f'>>time passed: {time_passed:.2f} sec')
 
     return data_interp_loaded
 
 
+def interp_uds_to_plipoints(uds:xu.UgridDataset, gdf:geopandas.GeoDataFrame, nPoints:int=None) -> xr.Dataset:
+    """
+    To interpolate an unstructured dataset (like a *_map.nc file) read with xugrid to plipoint locations
+    
+    Parameters
+    ----------
+    uds : xu.UgridDataset
+        dfm model output read using dfm_tools. Dims: mesh2d_nLayers, mesh2d_nInterfaces, time, mesh2d_nNodes, mesh2d_nFaces, mesh2d_nMax_face_nodes, mesh2d_nEdges.
+    gdf : geopandas.GeoDataFrame (str/path is also supported)
+        gdf with location, geometry (Point) and crs corresponding to model crs.
+    nPoints : int, optional
+        amount of points (None gives all). The default is None.
+
+    Raises
+    ------
+    Exception
+        DESCRIPTION.
+
+    Returns
+    -------
+    ds : TYPE
+        xr.Dataset with dims: plipoints, time, depth.
+
+    """
+    facedim = uds.grid.face_dimension
+    
+    if isinstance(gdf,(str,Path)): #TODO: align plipoints/gdf with other functions, now three input types are supported, but the interp_regularnc_to_plipoints requires paths to plifiles (and others also)
+        gdf = PolyFile_to_geodataframe_points(hcdfm.PolyFile(gdf))
+    
+    gdf = gdf.iloc[:nPoints]
+    ds = uds.ugrid.sel_points(x=gdf.geometry.x, y=gdf.geometry.y)
+    #TODO: drop mesh2d_face_x and mesh2d_face_y variables
+    
+    if len(gdf)!=ds.dims[facedim]: #TODO: check this until https://github.com/Deltares/xugrid/issues/100 is solved, after that, make a testcase that checks only this if-statement
+        ds_points = geopandas.points_from_xy(ds.x,ds.y)
+        gdfpoint_inds_bool = pd.Series(index=range(len(gdf)))
+        gdfpoint_inds_bool[:] = True
+        for iR, gdf_row in gdf.iterrows():
+            gdf_point = gdf_row.geometry
+            if gdf_point in ds_points:
+                gdfpoint_inds_bool.iloc[iR] = False
+        gdf_stats = gdf.copy()
+        gdf_stats['missing'] = gdfpoint_inds_bool
+        raise ValueError(f'requested {len(gdf)} points but resulted in ds with {ds.dims[facedim]} points, missing points are probably outside of the uds model domain:\n{gdf_stats}')
+
+    ds = ds.rename({facedim:'plipoints'}) # rename mesh2d_nFaces to plipoints
+    
+    ds['plipoint_name'] = xr.DataArray(gdf['plipoint_name'].tolist(), dims='plipoints') # change name of plipoint (node to gdf name)
+    ds = ds.set_index({'plipoints':'plipoint_name'})
+    return ds
+
+
 def interp_hisnc_to_plipoints(data_xr_his, file_pli, kdtree_k=3, load=True):
     """
     interpolate stations in hisfile to points of polyfile
     """
     #KDTree, finds minimal eucledian distance between points (haversine would be better). Alternatively sklearn.neighbors.BallTree: tree = BallTree(data_lonlat_pd)
     
     datavars_list = list(data_xr_his.data_vars)
@@ -432,14 +497,17 @@
     data_interp = data_interp.load()
     print('done')
 
     return data_interp
     
 
 def plipointsDataset_to_ForcingModel(plipointsDataset):
+    """
+    empty docstring
+    """
     quantity_list = list(plipointsDataset.data_vars)
     npoints = len(plipointsDataset.plipoints)
     
     #start conversion to Forcingmodel object
     print(f'Converting {npoints} plipoints to hcdfm.ForcingModel():',end='')
     dtstart = dt.datetime.now()
     ForcingModel_object = hcdfm.ForcingModel()
```

### Comparing `dfm_tools-0.11.0/dfm_tools/linebuilder.py` & `dfm_tools-0.12.0/dfm_tools/linebuilder.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.11.0/dfm_tools/meshkernel_helpers.py` & `dfm_tools-0.12.0/dfm_tools/meshkernel_helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,17 +11,49 @@
 import datetime as dt
 import hydrolib.core.dflowfm as hcdfm
 import pandas as pd
 from dfm_tools.hydrolib_helpers import pointlike_to_DataFrame
 from dfm_tools import __version__
 import getpass
 import numpy as np
+from dfm_tools.coastlines import get_coastlines_gdb
+from netCDF4 import default_fillvals
+import geopandas
+
+
+def meshkernel_delete_withcoastlines(mk, res:str='f', min_area:float = 0, crs=None):
+    """
+    empty docstring
+    """
+    mesh_bnds = mk.mesh2d_get_mesh_boundaries_as_polygons()
+    mesh_bnds.x_coordinates
+    bbox = (mesh_bnds.x_coordinates.min(), mesh_bnds.y_coordinates.min(), mesh_bnds.x_coordinates.max(), mesh_bnds.y_coordinates.max())
+    
+    print('>> reading coastlines: ',end='')
+    dtstart = dt.datetime.now()
+    coastlines_gdb = get_coastlines_gdb(bbox=bbox, res=res, min_area=min_area, crs=crs)
+    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
+    
+    for coastline_geom in coastlines_gdb['geometry']: #TODO: also possible without loop? >> geometry_separator=-999.9 so that value can be used to concat polygons. >> use hydrolib poly as input? https://github.com/Deltares/MeshKernelPy/issues/35
+        xx, yy = coastline_geom.exterior.coords.xy
+        xx = np.array(xx)
+        yy = np.array(yy)
+        
+        delete_pol_geom = meshkernel.GeometryList(x_coordinates=xx, y_coordinates=yy) #TODO: .copy()/to_numpy() makes the array contiguous in memory, which is necessary for meshkernel.mesh2d_delete()
+        mk.mesh2d_delete(geometry_list=delete_pol_geom, 
+                         delete_option=meshkernel.DeleteMeshOption(2), #ALL_COMPLETE_FACES/2: Delete all faces of which the complete face is inside the polygon
+                         invert_deletion=False) #TODO: cuts away link that is neccesary, so results in non-orthogonal grid (probably usecase of english channel?)
 
 
 def meshkernel_delete_withpol(mk, file_ldb, minpoints=None):
+    """
+    empty docstring
+    """
+    #TODO: read file_ldb as geodataframe (convert pointlike to geodataframe) and merge code with meshkernel_delete_withcoastlines: https://github.com/Deltares/dfm_tools/issues/427
+    
     print('>> reading+converting ldb: ',end='')
     dtstart = dt.datetime.now()
     pol_ldb = hcdfm.PolyFile(file_ldb)
     pol_ldb_list = [pointlike_to_DataFrame(x) for x in pol_ldb.objects] #TODO: this is quite slow, speed up possible?
     if minpoints is not None:
         pol_ldb_list = [x for x in pol_ldb_list if len(x)>minpoints] #filter only large polygons for performance
     for iP, pol_ldb in enumerate(pol_ldb_list):
@@ -32,18 +64,35 @@
     for iP, pol_del in enumerate(pol_ldb_list): #TODO: also possible without loop? >> geometry_separator=-999.9 so that value can be used to concat polygons. >> use hydrolib poly as input? https://github.com/Deltares/MeshKernelPy/issues/35
         delete_pol_geom = meshkernel.GeometryList(x_coordinates=pol_del['x'].to_numpy(), y_coordinates=pol_del['y'].to_numpy()) #TODO: .copy()/to_numpy() makes the array contiguous in memory, which is necessary for meshkernel.mesh2d_delete()
         mk.mesh2d_delete(geometry_list=delete_pol_geom, 
                          delete_option=meshkernel.DeleteMeshOption(2), #ALL_COMPLETE_FACES/2: Delete all faces of which the complete face is inside the polygon
                          invert_deletion=False) #TODO: cuts away link that is neccesary, so results in non-orthogonal grid (probably usecase of english channel?)
 
 
-def meshkernel_to_UgridDataset(mk:meshkernel.meshkernel.MeshKernel, remove_noncontiguous:bool = False) -> xr.Dataset:
-    mesh2d_grid3 = mk.mesh2d_get()
-
-    xu_grid = xu.Ugrid2d.from_meshkernel(mesh2d_grid3)
+def meshkernel_check_geographic(mk):
+    """
+    get projection from meshkernel instance
+    """
+    if mk.get_projection()==meshkernel.ProjectionType.SPHERICAL:
+        is_geographic = True
+    else:
+        is_geographic = False
+    return is_geographic
+
+
+def meshkernel_to_UgridDataset(mk:meshkernel.MeshKernel, crs=None, remove_noncontiguous:bool = False) -> xu.UgridDataset:
+    """
+    empty docstring
+    """
+    
+    is_geographic = meshkernel_check_geographic(mk)
+    
+    mesh2d_grid = mk.mesh2d_get()
+    
+    xu_grid = xu.Ugrid2d.from_meshkernel(mesh2d_grid)
     
     #remove non-contiguous grid parts
     def xugrid_remove_noncontiguous(grid):
         #based on https://deltares.github.io/xugrid/examples/connectivity.html#connected-components
         #uses https://docs.scipy.org/doc/scipy/reference/sparse.csgraph.html
         #TODO: maybe replace with meshkernel?
         uda = xu.UgridDataArray(
@@ -64,89 +113,133 @@
     #convert 0-based to 1-based grid for connectivity variables like face_node_connectivity #TODO: FM kernel needs 1-based grid, but it should read the attributes instead. Report this (#ug_get_meshgeom, #12, ierr=0. ** WARNING: Could not read mesh face x-coordinates)
     ds_idx = xu_grid_ds.filter_by_attrs(start_index=0)
     for varn_conn in ds_idx.data_vars:
         xu_grid_ds[varn_conn] += 1
         xu_grid_ds[varn_conn].attrs["_FillValue"] += 1
         xu_grid_ds[varn_conn].attrs["start_index"] += 1
     
-    xu_grid_ds = xu_grid_ds.assign_attrs({#'Conventions': 'CF-1.8 UGRID-1.0 Deltares-0.10', #add Deltares convention (was CF-1.8 UGRID-1.0)
+    xu_grid_ds = xu_grid_ds.assign_attrs({#'Conventions': 'CF-1.8 UGRID-1.0 Deltares-0.10', #TODO: conventions come from xugrid, so this line is not necessary
                                           'institution': 'Deltares',
                                           'references': 'https://www.deltares.nl',
                                           'source': f'Created with meshkernel {meshkernel.__version__}, xugrid {xu.__version__} and dfm_tools {__version__}',
                                           'history': 'Created on %s, %s'%(dt.datetime.now().strftime('%Y-%m-%dT%H:%M:%S%z'),getpass.getuser()), #TODO: add timezone
                                           })
-    
-    # add attrs (to projected_coordinate_system/wgs84 empty int variable): #TODO: should depend on is_geographic flag in make_basegrid()
-    # attribute_dict = {
-    #     'name': 'WGS84',
-    #     'epsg': np.array([4326], dtype=int),
-    #     'grid_mapping_name': 'Unknown projected',
-    #     'longitude_of_prime_meridian': np.array([0.0], dtype=float),
-    #     'semi_major_axis': np.array([6378137.0], dtype=float),
-    #     'semi_minor_axis': np.array([6356752.314245], dtype=float),
-    #     'inverse_flattening': np.array([6356752.314245], dtype=float),
-    #     'EPSG_code': 'EPSG:4326',
-    #     'value': 'value is equal to EPSG code'}
-    # xu_grid_ds['wgs84'] = xr.DataArray(np.array(0,dtype=int),dims=(),attrs=attribute_dict)
+    #TODO: xugrid overwrites this upon saving the network file: https://github.com/Deltares/xugrid/issues/111
     
     xu_grid_uds = xu.UgridDataset(xu_grid_ds)
+    add_crs_to_dataset(uds=xu_grid_uds,is_geographic=is_geographic,crs=crs)
+    
     return xu_grid_uds
 
 
-def make_basegrid(lon_min,lon_max,lat_min,lat_max,dx=0.05,dy=0.05,angle=0):
-    print('modelbuilder.make_basegrid()')
-    # create base grid
-    num_columns = int(np.round((lon_max-lon_min)/dx))
-    num_rows = int(np.round((lat_max-lat_min)/dy))
+def add_crs_to_dataset(uds:(xu.UgridDataset,xr.Dataset),is_geographic:bool,crs:(str,int)):
+    """
     
-    make_grid_parameters = meshkernel.MakeGridParameters(num_columns=num_columns,
-                                                         num_rows=num_rows,
-                                                         angle=angle,
+
+    Parameters
+    ----------
+    uds : (xu.UgridDataset,xr.Dataset)
+        DESCRIPTION.
+    is_geographic : bool
+        whether it is a spherical (True) or cartesian (False), property comes from meshkernel instance.
+    crs : (str,int)
+        epsg, e.g. 'EPSG:4326' or 4326.
+
+    Raises
+    ------
+    ValueError
+        DESCRIPTION.
+
+    Returns
+    -------
+    None.
+
+    """
+    #get crs information (name/num)
+    if crs is None:
+        crs_num = 0
+        crs_name = ''
+    else:
+        crs_info = geopandas.GeoSeries(crs=crs).crs #also contains area-of-use (name/bounds), datum (ellipsoid/prime-meridian)
+        crs_num = crs_info.to_epsg()
+        crs_name = crs_info.name
+    crs_str = f'EPSG:{crs_num}'
+    
+    #check if combination of is_geographic and crs makes sense
+    if is_geographic and crs_num!=4326:
+        raise ValueError(f'provided grid is sperical (is_geographic=True) but crs="{crs}" while only "EPSG:4326" (WGS84) is supported for spherical grids') #TODO: is this true?
+    if not is_geographic and crs_num==4326:
+        raise ValueError('provided grid is cartesian (is_geographic=False) but crs="EPSG:4326" (WGS84), this combination is not supported')
+    
+    if is_geographic:
+        grid_mapping_name = 'latitude_longitude'
+        crs_varn = 'wgs84'
+    else:
+        grid_mapping_name = 'Unknown projected'
+        crs_varn = 'projected_coordinate_system'
+    
+    attribute_dict = {
+        'name': crs_name, # not required, but convenient for the user
+        'epsg': np.array(crs_num, dtype=int), # epsg or EPSG_code should be present for the interacter to load the grid and by QGIS to recognize the epsg.
+        'EPSG_code': crs_str, # epsg or EPSG_code should be present for the interacter to load the grid and by QGIS to recognize the epsg.
+        'grid_mapping_name': grid_mapping_name, # without grid_mapping_name='latitude_longitude', interacter sees the grid as cartesian
+        }
+    
+    uds[crs_varn] = xr.DataArray(np.array(default_fillvals['i4'],dtype=int),dims=(),attrs=attribute_dict)
+
+
+def make_basegrid(lon_min,lon_max,lat_min,lat_max,dx,dy,angle=0,is_geographic=True):
+    """
+    empty docstring
+    """
+    # create base grid
+    make_grid_parameters = meshkernel.MakeGridParameters(angle=angle,
                                                          origin_x=lon_min,
                                                          origin_y=lat_min,
+                                                         upper_right_x=lon_max,
+                                                         upper_right_y=lat_max,
                                                          block_size_x=dx,
                                                          block_size_y=dy)
     
-    geometry_list = meshkernel.GeometryList(np.empty(0, dtype=np.double), np.empty(0, dtype=np.double)) # A polygon must to be provided. If empty it will not be used. If a polygon is provided it will be used in the generation of the curvilinear grid. The polygon must be closed
-    mk = meshkernel.MeshKernel() #TODO: is_geographic=True was used in modelbuilder, but refinement super slow and raises "MeshKernelError: MeshRefinement::connect_hanging_nodes: The number of non-hanging nodes is neither 3 nor 4."
-    mk.curvilinear_make_uniform(make_grid_parameters, geometry_list) #TODO: make geometry_list argument optional: https://github.com/Deltares/MeshKernelPy/issues/30
+    mk = meshkernel.MeshKernel(is_geographic=is_geographic)
+    mk.curvilinear_make_uniform_on_extension(make_grid_parameters)
     mk.curvilinear_convert_to_mesh2d() #convert to ugrid/mesh2d
     
     return mk
 
 
-def refine_basegrid(mk, data_bathy_sel,min_face_size=0.1):
-    print('modelbuilder.refine_basegrid()')
-    samp_x,samp_y = np.meshgrid(data_bathy_sel.lon.to_numpy(),data_bathy_sel.lat.to_numpy())
-    samp_z = data_bathy_sel.elevation.to_numpy().astype(float) #TODO: without .astype(float), meshkernelpy generates "TypeError: incompatible types, c_short_Array_27120 instance instead of LP_c_double instance": https://github.com/Deltares/MeshKernelPy/issues/31
-    samp_x = samp_x.ravel()
-    samp_y = samp_y.ravel()
-    samp_z = samp_z.ravel()
-    geomlist = meshkernel.GeometryList(x_coordinates=samp_x, y_coordinates=samp_y, values=samp_z) #TODO: does not check if lenghts of input array is equal (samp_z[1:]) https://github.com/Deltares/MeshKernelPy/issues/32
-    
+def refine_basegrid(mk, data_bathy_sel, min_edge_size):
+    """
+    empty docstring
+    """
+    
+    lon_np = data_bathy_sel.lon.to_numpy()
+    lat_np = data_bathy_sel.lat.to_numpy()
+    values_np = data_bathy_sel.elevation.to_numpy().flatten().astype('float') #TODO: astype to avoid "TypeError: incompatible types, c_short_Array_74880 instance instead of LP_c_double instance"
+    gridded_samples = meshkernel.GriddedSamples(x_coordinates=lon_np,y_coordinates=lat_np,values=values_np)
+
+
     #refinement
-    mesh_refinement_parameters = meshkernel.MeshRefinementParameters(refine_intersected=False, #TODO: provide defaults for several arguments, so less arguments are required
-                                                                     use_mass_center_when_refining=False, #TODO: what does this do?
-                                                                     min_face_size=min_face_size, #TODO: size in meters would be more convenient: https://github.com/Deltares/MeshKernelPy/issues/33
+    mesh_refinement_parameters = meshkernel.MeshRefinementParameters(min_edge_size=min_edge_size, #always in meters
                                                                      refinement_type=meshkernel.RefinementType(1), #Wavecourant/1,
                                                                      connect_hanging_nodes=True, #set to False to do multiple refinement steps (e.g. for multiple regions)
-                                                                     account_for_samples_outside_face=True, #outsidecell argument for --refine?
-                                                                     max_refinement_iterations=5,
-                                                                     ) #TODO: missing the arguments dtmax (necessary?), hmin (min_face_size but then in meters instead of degrees), smoothiters (currently refinement is patchy along coastlines, goes good in dflowfm exec after additional implementation of HK), spherical 1/0 (necessary?)
-    
-    mk.mesh2d_refine_based_on_samples(samples=geomlist,
-                                       relative_search_radius=0.5, #TODO: bilin interp is preferred, but this is currently not supported (samples have to be ravelled): https://github.com/Deltares/MeshKernelPy/issues/34
-                                       minimum_num_samples=3,
-                                       mesh_refinement_params=mesh_refinement_parameters,
-                                       )
+                                                                     smoothing_iterations=2,
+                                                                     max_courant_time=120)
+    
+    mk.mesh2d_refine_based_on_gridded_samples(gridded_samples=gridded_samples,
+                                               mesh_refinement_params=mesh_refinement_parameters,
+                                               use_nodal_refinement=True) #TODO: what does this do?
     
     return mk
 
 
 def generate_bndpli(lon_min, lon_max, lat_min, lat_max, dlon, dlat, name='bnd'): #TODO: maybe generate with meshkernel?
+    """
+    empty docstring
+    """
 
     vals_lon_ar = np.arange(lon_min, lon_max, dlon)
     vals_lon = np.linspace(lon_min, lon_max,len(vals_lon_ar))
     vals_lat_ar = np.arange(lat_min, lat_max, dlat)
     vals_lat = np.linspace(lat_min, lat_max,len(vals_lat_ar))
     pli_p1 = np.c_[np.repeat(lon_min,len(vals_lat)),vals_lat]
     pli_p2 = np.c_[vals_lon,np.repeat(lat_max,len(vals_lon))]
```

### Comparing `dfm_tools-0.11.0/dfm_tools/modelbuilder.py` & `dfm_tools-0.12.0/dfm_tools/modelbuilder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,59 @@
 """
 Created on Tue Apr  4 16:12:56 2023
 
 @author: groenenb, sclaan
-edited by: veenstra
+edited by: veenstra, zijlker
 
 This is a proof of concept that will be properly coded in the near future and probably end up under hydromt-delft3dfm
 Since the functions in this script contain hardcoded parameters, it is not exposed to public and you need to import like dfmt.modelbuilder.[function]
 """
 
 import os
 import xarray as xr
 import pandas as pd
 import dfm_tools as dfmt
 import hydrolib.core.dflowfm as hcdfm
 import datetime as dt
 import glob
 
 
-def preprocess_interpolate_nc_to_bc(ext_bnd,
-                                    list_quantities,#quantities should be in conversion_dict.keys(). waterlevelbnd is steric/zos, tide is tidal components from FES/EOT
-                                    tstart,
-                                    tstop,
-                                    list_plifiles,
-                                    dir_pattern,
-                                    dir_output='.',
-                                    refdate_str=None,
-                                    conversion_dict=dfmt.get_conversion_dict(),
-                                    tidemodel='FES2014'): #FES2014, FES2012, EOT20, GTSM4.1preliminary
+def cmems_nc_to_bc(ext_bnd, list_quantities, tstart, tstop, file_pli, dir_pattern, dir_output, refdate_str):
     #input examples in https://github.com/Deltares/dfm_tools/blob/main/tests/examples/preprocess_interpolate_nc_to_bc.py
-    model = 'CMEMS'
     
-    for file_pli in list_plifiles:
-        file_bc_basename = os.path.basename(file_pli).replace('.pli','')
-        for quantity in list_quantities:
-            print(f'processing quantity: {quantity}')
-            if quantity=='tide': 
-                if tidemodel == 'FES2014': #for comparing to older FES bc-files
-                    component_list = ['2n2','mf','p1','m2','mks2','mu2','q1','t2','j1','m3','mm','n2','r2','k1','m4','mn4','s1','k2','m6','ms4','nu2','s2','l2','m8','msf','o1','s4']
-                else:
-                    component_list = None #None results in all tidemodel components
-                ForcingModel_object = dfmt.interpolate_tide_to_bc(tidemodel=tidemodel, file_pli=file_pli, component_list=component_list, nPoints=None)
-            else:
-                #open regulargridDataset and do some basic stuff (time selection, renaming depth/lat/lon/varname, converting units, etc)
-                data_xr_vars = dfmt.open_dataset_extra(dir_pattern=dir_pattern, quantity=quantity,
-                                                       tstart=tstart, tstop=tstop,
-                                                       conversion_dict=conversion_dict,
-                                                       refdate_str=refdate_str)
-                #interpolate regulargridDataset to plipointsDataset
-                data_interp = dfmt.interp_regularnc_to_plipoints(data_xr_reg=data_xr_vars, file_pli=file_pli)
-                
-                #convert plipointsDataset to hydrolib ForcingModel
-                ForcingModel_object = dfmt.plipointsDataset_to_ForcingModel(plipointsDataset=data_interp)
-                        
-            if quantity=='tide':
-                file_bc_out = os.path.join(dir_output,f'{quantity}_{file_bc_basename}_{tidemodel}.bc')
-            else:
-                file_bc_out = os.path.join(dir_output,f'{quantity}_{file_bc_basename}_{model}.bc')
-            
-            ForcingModel_object.save(filepath=file_bc_out)
-            
-            #generate boundary object for the ext file (quantity, pli-filename, bc-filename)
-            boundary_object = hcdfm.Boundary(quantity=quantity.replace('tide','waterlevelbnd'), #the FM quantity for tide is also waterlevelbnd
-                                             locationfile=file_pli,
-                                             forcingfile=ForcingModel_object)
-            ext_bnd.boundary.append(boundary_object)
+    file_bc_basename = os.path.basename(file_pli).replace('.pli','')
+    for quantity in list_quantities:
+        print(f'processing quantity: {quantity}')
+        
+        tstart, tstop = dfmt.round_timestamp_to_outer_noon(tstart,tstop)
+        #open regulargridDataset and do some basic stuff (time selection, renaming depth/lat/lon/varname, converting units, etc)
+        data_xr_vars = dfmt.open_dataset_extra(dir_pattern=dir_pattern, quantity=quantity,
+                                               tstart=tstart, tstop=tstop,
+                                               conversion_dict=dfmt.get_conversion_dict(),
+                                               refdate_str=refdate_str)
+        #interpolate regulargridDataset to plipointsDataset
+        data_interp = dfmt.interp_regularnc_to_plipoints(data_xr_reg=data_xr_vars, file_pli=file_pli)
+        
+        #convert plipointsDataset to hydrolib ForcingModel
+        ForcingModel_object = dfmt.plipointsDataset_to_ForcingModel(plipointsDataset=data_interp)
+                    
+        file_bc_out = os.path.join(dir_output,f'{quantity}_{file_bc_basename}_CMEMS.bc')
+        
+        ForcingModel_object.save(filepath=file_bc_out)
+        
+        #generate boundary object for the ext file (quantity, pli-filename, bc-filename)
+        boundary_object = hcdfm.Boundary(quantity=quantity.replace('tide','waterlevelbnd'), #the FM quantity for tide is also waterlevelbnd
+                                         locationfile=file_pli,
+                                         forcingfile=ForcingModel_object)
+        ext_bnd.boundary.append(boundary_object)
     
     return ext_bnd
 
     
-def preprocess_ini_cmems_to_nc(ext_old, tstart='1998-01-01',
-        dir_data  = r'p:\i1000668-tcoms\03_newModel\01_input\02_bnd\data_opendap', #folder containing CMEMS so and thetao netcdf files
-        dir_out = '.'):
+def preprocess_ini_cmems_to_nc(ext_old, tstart, dir_data, dir_out):
     
     file_nc_list_so = glob.glob(f'{dir_data}\\cmems_so_*.nc')
     file_nc_list_thetao = glob.glob(f'{dir_data}\\cmems_thetao_*.nc')
     file_nc_list = file_nc_list_so + file_nc_list_thetao
     
     print(f'opening {len(file_nc_list)} datasets')
     data_xr = xr.open_mfdataset(file_nc_list)
@@ -95,78 +74,43 @@
                                          operand=hcdfm.Operand.override, #O
                                          )
     ext_old.forcing.append(forcing_saltem)
     
     return ext_old
     
     
-def preprocess_merge_meteofiles(ext_old,
-        mode = 'HYCOM', # 'HIRLAM_meteo' 'HIRLAM_meteo-heatflux' 'HARMONIE' 'HYCOM' 'ERA5_wind_pressure' 'ERA5_heat_model' 'ERA5_radiation' 'ERA5_rainfall' 'WOA'
-        varkey_list = [],
-        dir_data = [],
-        dir_output = '.',
-        time_slice = slice('2013-12-30','2014-01-01')):
+def preprocess_merge_meteofiles_era5(ext_old, varkey_list, dir_data, dir_output, time_slice):
 
     if isinstance(varkey_list[0], list):
         varkey_lists = varkey_list
     else:
         varkey_lists = [varkey_list]
     
     for varkey_list in varkey_lists:
-        if 'HIRLAM' in mode:
-            if mode == 'HIRLAM_meteo': #1year voor meteo crasht (HIRLAM72_*\\h72_*) door conflicting dimension sizes, sourcefolders opruimen? meteo_heatflux folders zijn schoner dus daar werkt het wel
-                dir_data = 'P:\\1204257-dcsmzuno\\2014\\data\\meteo\\HIRLAM72_*' #files contain: ['air_pressure_fixed_height','northward_wind','eastward_wind']
-            elif mode == 'HIRLAM_meteo-heatflux':
-                dir_data = 'P:\\1204257-dcsmzuno\\2014\\data\\meteo-heatflux\\HIRLAM72_*' # files contain: ['dew_point_temperature','air_temperature','cloud_area_fraction']
-            fn_match_pattern = 'h72_20131*.nc'
-            file_out_prefix = 'h72_'
-            preprocess = dfmt.preprocess_hirlam #temporary(?) fix for >1D-vars with same name as its dim
-        elif mode == 'HARMONIE':
-            dir_data = 'p:\\1204257-dcsmzuno\\data\\meteo\\HARMONIE\\nc\\air_*' #many invalid files, so subsetting here
-            fn_match_pattern = 'HARMONIE_*_2020_*.nc'
-            file_out_prefix = 'HARMONIE_'
-            preprocess = None
-        elif mode == 'HYCOM':
-            dir_data = 'c:\\DATA\\dfm_tools_testdata\\GLBu0.08_expt_91.2'
-            fn_match_pattern = 'HYCOM_ST_GoO_*.nc'
-            file_out_prefix = 'HYCOM_ST_GoO_'
-            preprocess = None
-            #rename_variables = {'salinity':'so', 'water_temp':'thetao'}
-        elif 'ERA5' in mode:
-            fn_match_pattern = f'era5_.*({"|".join(varkey_list)})_.*.nc' #simpler but selects more files: 'era5_*.nc'
-            file_out_prefix = f'era5_{"_".join(varkey_list)}_'
-            preprocess = dfmt.preprocess_ERA5 #reduce expver dimension if present
-        elif mode == 'WOA':
-            dir_data = r'p:\1204257-dcsmzuno\data\WOA13'
-            fn_match_pattern = 'woa13_decav_s*.nc'
-            file_out_prefix = 'woa13_decav_s_'
-            preprocess = dfmt.preprocess_woa #add 360-day calendar unit to time attrs before decode_cf
-        else:
-            raise Exception('ERROR: wrong mode %s'%(mode))
+        fn_match_pattern = f'era5_.*({"|".join(varkey_list)})_.*.nc' #simpler but selects more files: 'era5_*.nc'
+        file_out_prefix = f'era5_{"_".join(varkey_list)}_'
+        preprocess = dfmt.preprocess_ERA5 #reduce expver dimension if present
         
         if not os.path.exists(dir_output):
             os.makedirs(dir_output)
         
         file_nc = os.path.join(dir_data,fn_match_pattern)
         
         data_xr_tsel = dfmt.merge_meteofiles(file_nc=file_nc, time_slice=time_slice, 
                                              preprocess=preprocess,
                                              add_global_overlap=False, #GTSM specific: extend data beyond -180 to 180 longitude
                                              zerostart=False) #GTSM specific: extend data with 0-value fields 1 and 2 days before all_tstart
         
         #write to netcdf file
         print('>> writing file (can take a while): ',end='')
         dtstart = dt.datetime.now()
-        try:
-            times_np = data_xr_tsel['time'].to_series()
-        except:
-            times_np = data_xr_tsel['time'].to_numpy() #.to_series() does not work for woa 360_day data. .to_numpy() results in numpy.datetime64 for other datasets, which has no attribute strftime
+        times_np = data_xr_tsel['time'].to_series()
         time_start_str = times_np[0].strftime("%Y%m%d")
         time_stop_str = times_np[-1].strftime("%Y%m%d")
-        file_out = os.path.join(dir_output, f'{file_out_prefix}{time_start_str}to{time_stop_str}_{mode}.nc')
+        file_out = os.path.join(dir_output, f'{file_out_prefix}{time_start_str}to{time_stop_str}_ERA5.nc')
         data_xr_tsel.to_netcdf(file_out)
         print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
         
         #append to ext model
         if varkey_list == ['msl','u10n','v10n','chnk']:
             forcing_meteo = hcdfm.ExtOldForcing(quantity='airpressure_windx_windy_charnock',
                                                 filename=file_out,
```

### Comparing `dfm_tools-0.11.0/dfm_tools/modplot.py` & `dfm_tools-0.12.0/dfm_tools/modplot.py`

 * *Files identical despite different names*

### Comparing `dfm_tools-0.11.0/dfm_tools/xarray_helpers.py` & `dfm_tools-0.12.0/dfm_tools/xarray_helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 @author: veenstra
 """
 
 import os
 import re
 from netCDF4 import Dataset
 import xarray as xr
-import xugrid as xu
 import datetime as dt
 import glob
 import pandas as pd
 import warnings
 import numpy as np
 from dfm_tools.errors import OutOfRangeError
 
@@ -130,17 +129,17 @@
     return ds
 
 
 def prevent_dtype_int(ds): #TODO: this is not used, maybe phase out?
     """
     Prevent writing to int, since it might mess up dataset (https://github.com/Deltares/dfm_tools/issues/239 and https://github.com/pydata/xarray/issues/7039)
     Since floats are used instead of ints, the disksize of the dataset will be larger
-    TODO: alternatively remove scale_factor key from attrs, so it can be recomputed (seems to also work): ds[var].encoding.pop('scale_factor')
-    TODO: maybe add to preprocess_ERA5 (preferrably popping scale_factor attribute to keep file size small)
     """
+    #TODO: alternatively remove scale_factor key from attrs, so it can be recomputed (seems to also work): ds[var].encoding.pop('scale_factor')
+    #TODO: maybe add to preprocess_ERA5 (preferrably popping scale_factor attribute to keep file size small)
     for var in ds.data_vars:
         var_encoding = ds[var].encoding
         if 'dtype' in var_encoding.keys():
             if 'int' in str(var_encoding['dtype']):
                 ds[var].encoding.pop('dtype') #remove dtype key from attrs
     return ds
 
@@ -245,15 +244,15 @@
         decode_cf = True        
 
     file_nc_list = file_to_list(file_nc)
 
     print(f'>> opening multifile dataset of {len(file_nc_list)} files (can take a while with lots of files): ',end='')
     dtstart = dt.datetime.now()
     data_xr = xr.open_mfdataset(file_nc_list,
-                                parallel=True, #speeds up the process
+                                #parallel=True, #TODO: speeds up the process, but often "OSError: [Errno -51] NetCDF: Unknown file format" on WCF
                                 preprocess=preprocess,
                                 chunks=chunks,
                                 drop_variables=drop_variables, #necessary since dims/vars with equal names are not allowed by xarray, add again later and requested matroos to adjust netcdf format.
                                 decode_cf=decode_cf)
     print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
     
     #rename variables
@@ -261,274 +260,142 @@
         if 'lon' in data_xr.variables:
             data_xr = data_xr.rename({'lon':'longitude', 'lat':'latitude'})
         elif 'x' in data_xr.variables:
             data_xr = data_xr.rename({'x':'longitude', 'y':'latitude'})
         else:
             raise KeyError('no longitude/latitude, lon/lat or x/y variables found in dataset')
 
-    varkeys = data_xr.variables.mapping.keys()
     #data_xr.attrs['comment'] = 'merged with dfm_tools from https://github.com/Deltares/dfm_tools' #TODO: add something like this or other attributes? (some might also be dropped now)
     
     #select time and do checks #TODO: check if calendar is standard/gregorian
-    data_xr_tsel = data_xr.sel(time=time_slice)
-    if data_xr_tsel.get_index('time').duplicated().any():
+    data_xr = data_xr.sel(time=time_slice)
+    if data_xr.get_index('time').duplicated().any():
         print('dropping duplicate timesteps')
-        data_xr_tsel = data_xr_tsel.sel(time=~data_xr_tsel.get_index('time').duplicated()) #drop duplicate timesteps
+        data_xr = data_xr.sel(time=~data_xr.get_index('time').duplicated()) #drop duplicate timesteps
     
     #check if there are times selected
-    if len(data_xr_tsel.time)==0:
+    if len(data_xr.time)==0:
         raise OutOfRangeError(f'ERROR: no times selected, ds_text={data_xr.time[[0,-1]].to_numpy()} and time_slice={time_slice}')
     
     #check if there are no gaps (more than one unique timestep)
-    times_pd = data_xr_tsel['time'].to_series()
+    times_pd = data_xr['time'].to_series()
     timesteps_uniq = times_pd.diff().iloc[1:].unique()
     if len(timesteps_uniq)>1:
         raise Exception(f'ERROR: gaps found in selected dataset (are there sourcefiles missing?), unique timesteps (hour): {timesteps_uniq/1e9/3600}')
     
     #check if requested times are available in selected files (in times_pd)
     if time_slice.start not in times_pd.index:
         raise OutOfRangeError(f'ERROR: time_slice_start="{time_slice.start}" not in selected files, timerange: "{times_pd.index[0]}" to "{times_pd.index[-1]}"')
     if time_slice.stop not in times_pd.index:
         raise OutOfRangeError(f'ERROR: time_slice_stop="{time_slice.stop}" not in selected files, timerange: "{times_pd.index[0]}" to "{times_pd.index[-1]}"')
     
-    #TODO: check conversion implementation with hydro_tools\ERA5\ERA52DFM.py. Also move to separate function?
+    data_xr = convert_meteo_units(data_xr)
+    
+    #convert 0to360 sourcedata to -180to+180
+    convert_360to180 = (data_xr['longitude'].to_numpy()>180).any()
+    if convert_360to180: #TODO: make more flexible for models that eg pass -180/+180 crossing (add overlap at lon edges).
+        lon_newvar = (data_xr.coords['longitude'] + 180) % 360 - 180
+        data_xr.coords['longitude'] = lon_newvar.assign_attrs(data_xr['longitude'].attrs) #this re-adds original attrs
+        data_xr = data_xr.sortby(data_xr['longitude'])
+    
+    #GTSM specific addition for longitude overlap
+    if add_global_overlap: # assumes -180 to ~+179.75 (full global extent, but no overlap). Does not seem to mess up results for local models.
+        if len(data_xr.longitude.values) != len(np.unique(data_xr.longitude.values%360)):
+            raise Exception(f'add_global_overlap=True, but there are already overlapping longitude values: {data_xr.longitude}')
+        overlap_ltor = data_xr.sel(longitude=data_xr.longitude<=-179)
+        overlap_ltor['longitude'] = overlap_ltor['longitude'] + 360
+        overlap_rtol = data_xr.sel(longitude=data_xr.longitude>=179)
+        overlap_rtol['longitude'] = overlap_rtol['longitude'] - 360
+        data_xr = xr.concat([data_xr,overlap_ltor,overlap_rtol],dim='longitude').sortby('longitude')
+    
+    #GTSM specific addition for zerovalues during spinup
+    #TODO: doing this drops all encoding from variables, causing them to be converted into floats. Also makes sense since 0 pressure does not fit into int16 range as defined by scalefac and offset
+    #'scale_factor': 0.17408786412952254, 'add_offset': 99637.53795606793
+    #99637.53795606793 - 0.17408786412952254*32768
+    #99637.53795606793 + 0.17408786412952254*32767
+    if zerostart:
+        field_zerostart = data_xr.isel(time=[0,0])*0 #two times first field, set values to 0
+        field_zerostart['time'] = [times_pd.index[0]-dt.timedelta(days=2),times_pd.index[0]-dt.timedelta(days=1)] #TODO: is one zero field not enough? (is replacing first field not also ok? (results in 1hr transition period)
+        data_xr = xr.concat([field_zerostart,data_xr],dim='time',combine_attrs='no_conflicts') #combine_attrs argument prevents attrs from being dropped
+    
+    # converting from int16 to float32 (by removing dtype from encoding) or recompute scale_factor/add_offset is necessary for ERA5 dataset
+    #data_xr = prevent_dtype_int(data_xr)
+    data_xr = recompute_scaling_and_offset(data_xr)
+    
+    return data_xr
+
+
+def convert_meteo_units(data_xr):
+    
+    #TODO: check conversion implementation with hydro_tools\ERA5\ERA52DFM.py
+    #TODO: keep/update attrs
+    #TODO: reduce code complexity
+    
     def get_unit(data_xr_var):
         if 'units' in data_xr_var.attrs.keys():
             unit = data_xr_var.attrs["units"]
         else:
             unit = '-'
         return unit
+    
+    varkeys = data_xr.variables.mapping.keys()
+    
     #convert Kelvin to Celcius
     for varkey_sel in ['air_temperature','dew_point_temperature','d2m','t2m']: # 2 meter dewpoint temparature / 2 meter temperature
-        if varkey_sel in varkeys:
-            current_unit = get_unit(data_xr_tsel[varkey_sel])
-            new_unit = 'C'
-            print(f'converting {varkey_sel} unit from Kelvin to Celcius: [{current_unit}] to [{new_unit}]')
-            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
-            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] - 273.15
+        if varkey_sel not in varkeys:
+            continue
+        current_unit = get_unit(data_xr[varkey_sel])
+        new_unit = 'C'
+        print(f'converting {varkey_sel} unit from Kelvin to Celcius: [{current_unit}] to [{new_unit}]')
+        data_xr[varkey_sel] = data_xr[varkey_sel] - 273.15
+        data_xr[varkey_sel].attrs['units'] = new_unit
     #convert fraction to percentage
     for varkey_sel in ['cloud_area_fraction','tcc']: #total cloud cover
-        if varkey_sel in varkeys:
-            current_unit = get_unit(data_xr_tsel[varkey_sel])
-            new_unit = '%' #unit is soms al %
-            print(f'converting {varkey_sel} unit from fraction to percentage: [{current_unit}] to [{new_unit}]')
-            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
-            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] * 100
+        if varkey_sel not in varkeys:
+            continue
+        current_unit = get_unit(data_xr[varkey_sel])
+        new_unit = '%' #unit is soms al %
+        print(f'converting {varkey_sel} unit from fraction to percentage: [{current_unit}] to [{new_unit}]')
+        data_xr[varkey_sel] = data_xr[varkey_sel] * 100
+        data_xr[varkey_sel].attrs['units'] = new_unit
     #convert kg/m2/s to mm/day
     for varkey_sel in ['mer','mtpr']: #mean evaporation rate / mean total precipitation rate
-        if varkey_sel in varkeys:
-            current_unit = get_unit(data_xr_tsel[varkey_sel])
-            new_unit = 'mm/day'
-            print(f'converting {varkey_sel} unit from kg/m2/s to mm/day: [{current_unit}] to [{new_unit}]')
-            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
-            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] * 86400 # kg/m2/s to mm/day (assuming rho_water=1000)
+        if varkey_sel not in varkeys:
+            continue
+        current_unit = get_unit(data_xr[varkey_sel])
+        new_unit = 'mm/day'
+        print(f'converting {varkey_sel} unit from kg/m2/s to mm/day: [{current_unit}] to [{new_unit}]')
+        data_xr[varkey_sel] = data_xr[varkey_sel] * 86400 # kg/m2/s to mm/day (assuming rho_water=1000)
+        data_xr[varkey_sel].attrs['units'] = new_unit
     #convert J/m2 to W/m2
     for varkey_sel in ['ssr','strd']: #solar influx (surface_net_solar_radiation) / surface_thermal_radiation_downwards
-        if varkey_sel in varkeys:
-            current_unit = get_unit(data_xr_tsel[varkey_sel])
-            new_unit = 'W m**-2'
-            print(f'converting {varkey_sel} unit from J/m2 to W/m2: [{current_unit}] to [{new_unit}]')
-            data_xr_tsel[varkey_sel].attrs['units'] = new_unit
-            data_xr_tsel[varkey_sel] = data_xr_tsel[varkey_sel] / 3600 # 3600s/h #TODO: 1W = 1J/s, so does not make sense?
+        if varkey_sel not in varkeys:
+            continue
+        current_unit = get_unit(data_xr[varkey_sel])
+        new_unit = 'W m**-2'
+        print(f'converting {varkey_sel} unit from J/m2 to W/m2: [{current_unit}] to [{new_unit}]')
+        data_xr[varkey_sel] = data_xr[varkey_sel] / 3600 # 3600s/h #TODO: 1W = 1J/s, so does not make sense?
+        data_xr[varkey_sel].attrs['units'] = new_unit
     #solar influx increase for beta=6%
     if 'ssr' in varkeys:
         print('ssr (solar influx) increase for beta=6%')
-        data_xr_tsel['ssr'] = data_xr_tsel['ssr'] *.94
-    
-    #convert 0to360 sourcedata to -180to+180
-    convert_360to180 = (data_xr['longitude'].to_numpy()>180).any()
-    if convert_360to180:
-        data_xr.coords['longitude'] = (data_xr.coords['longitude'] + 180) % 360 - 180
-        data_xr = data_xr.sortby(data_xr['longitude'])
+        data_xr['ssr'] = data_xr['ssr'] *.94
     
-    #GTSM specific addition for longitude overlap
-    if add_global_overlap: # assumes -180 to ~+179.75 (full global extent, but no overlap). Does not seem to mess up results for local models.
-        if len(data_xr_tsel.longitude.values) != len(np.unique(data_xr_tsel.longitude.values%360)):
-            raise Exception(f'add_global_overlap=True, but there are already overlapping longitude values: {data_xr_tsel.longitude}')
-        overlap_ltor = data_xr_tsel.sel(longitude=data_xr_tsel.longitude<=-179)
-        overlap_ltor['longitude'] = overlap_ltor['longitude'] + 360
-        overlap_rtol = data_xr_tsel.sel(longitude=data_xr_tsel.longitude>=179)
-        overlap_rtol['longitude'] = overlap_rtol['longitude'] - 360
-        data_xr_tsel = xr.concat([data_xr_tsel,overlap_ltor,overlap_rtol],dim='longitude').sortby('longitude')
-    
-    #GTSM specific addition for zerovalues during spinup
-    if zerostart:
-        field_zerostart = data_xr_tsel.isel(time=[0,0])*0 #two times first field, set values to 0
-        field_zerostart['time'] = [times_pd.index[0]-dt.timedelta(days=2),times_pd.index[0]-dt.timedelta(days=1)] #TODO: is one zero field not enough? (is replacing first field not also ok? (results in 1hr transition period)
-        data_xr_tsel = xr.concat([field_zerostart,data_xr_tsel],dim='time')#.sortby('time')
-    
-    # converting from int16 to float32 (by removing dtype from encoding) or recompute scale_factor/add_offset is necessary for ERA5 dataset
-    #data_xr_tsel = prevent_dtype_int(data_xr_tsel)
-    data_xr_tsel = recompute_scaling_and_offset(data_xr_tsel)
-    
-    #data_xr_tsel.time.encoding['units'] = 'hours since 1900-01-01 00:00:00' #TODO: maybe add different reftime?
-    
-    return data_xr_tsel
+    return data_xr
 
 
 def Dataset_varswithdim(ds,dimname): #TODO: dit zit ook in xugrid, wordt nu gebruikt in hisfile voorbeeldscript en kan handig zijn, maar misschien die uit xugrid gebruiken?
+    """
+    empty docstring
+    """
     if dimname not in ds.dims:
         raise KeyError(f'dimension {dimname} not in dataset, available are: {list(ds.dims)}')
     
     varlist_keep = []
     for varname in ds.variables.keys():
         if dimname in ds[varname].dims:
             varlist_keep.append(varname)
     ds = ds[varlist_keep]
     
     return ds
 
 
-def get_vertical_dimensions(uds): #TODO: maybe add layer_dimension and interface_dimension properties to xugrid?
-    """
-    get vertical_dimensions from grid_info of ugrid mapfile (this will fail for hisfiles). The info is stored in the layer_dimension and interface_dimension attribute of the mesh2d variable of the dataset (stored in uds.grid after reading with xugrid)
-    
-    processing cb_3d_map.nc
-        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
-    processing Grevelingen-FM_0*_map.nc
-        >> found layer/interface dimensions in file: nmesh2d_layer nmesh2d_interface (these are updated in open_partitioned_dataset)
-    processing DCSM-FM_0_5nm_0*_map.nc
-        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
-    processing MB_02_0*_map.nc
-        >> found layer/interface dimensions in file: mesh2d_nLayers mesh2d_nInterfaces
-    """
-    
-    if not hasattr(uds,'grid'): #early return in case of e.g. hisfile
-        return None, None
-        
-    gridname = uds.grid.name
-    grid_info = uds.grid.to_dataset()[gridname]
-    if hasattr(grid_info,'layer_dimension'):
-        return grid_info.layer_dimension, grid_info.interface_dimension
-    else:
-        return None, None
-
-
-def remove_ghostcells(uds): #TODO: create JIRA issue: add domainno attribute to partitioned mapfiles or remove ghostcells from output (or make values in ghostcells the same as not-ghostcells)
-    """
-    Dropping ghostcells if there is a domainno variable present and there is a domainno in the filename.
-    Not using most-occurring domainno in var, since this is not a valid assumption for merged datasets and might be invalid for a very small partition.
-    
-    """
-    gridname = uds.grid.name
-    varn_domain = f'{gridname}_flowelem_domain'
-    
-    #check if dataset has domainno variable, return uds if not present
-    if varn_domain not in uds.data_vars:
-        print('[nodomainvar] ',end='')
-        return uds
-    
-    #derive domainno from filename, return uds if not present
-    fname = uds.encoding['source']
-    if '_' not in fname: #safety escape in case there is no _ in the filename
-        print('[nodomainfname] ',end='')
-        return uds
-    fname_splitted = fname.split('_')
-    part_domainno_fromfname = fname_splitted[-2] #this is not valid for rstfiles (date follows after partnumber), but they cannot be read with xugrid anyway since they are mapformat=1
-    if not part_domainno_fromfname.isnumeric() or len(part_domainno_fromfname)!=4:
-        print('[nodomainfname] ',end='')
-        return uds
-    
-    #drop ghostcells
-    part_domainno_fromfname = int(part_domainno_fromfname)
-    da_domainno = uds[varn_domain]
-    idx = np.flatnonzero(da_domainno == part_domainno_fromfname)
-    uds = uds.isel({uds.grid.face_dimension:idx})
-    return uds
-
-
-def remove_periodic_cells(uds): #TODO: implement proper fix: https://github.com/Deltares/xugrid/issues/63
-    """
-    For global models with grids that go "around the back". Temporary fix to drop all faces that are larger than grid_extent/2 (eg 360/2=180 degrees in case of GTSM)
-    
-    """
-    #print('>> remove_periodic_cells() on dataset: ',end='')
-    #dtstart = dt.datetime.now()
-    face_node_x = uds.grid.face_node_coordinates[:,:,0]
-    grid_extent = uds.grid.bounds[2] - uds.grid.bounds[0]
-    face_node_maxdx = np.nanmax(face_node_x,axis=1) - np.nanmin(face_node_x,axis=1)
-    bool_face = face_node_maxdx < grid_extent/2
-    if bool_face.all(): #early return for when no cells have to be removed (might increase performance)
-        return uds
-    uds = uds.sel({uds.grid.face_dimension:bool_face})
-    #print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    return uds
-
-
-def open_partitioned_dataset(file_nc, chunks={'time':1}, remove_ghost=True, remove_periodic=False, **kwargs): 
-    """
-    using xugrid to read and merge partitions, with some additional features (remaning old layerdim, timings, set zcc/zw as data_vars)
-
-    Parameters
-    ----------
-    file_nc : TYPE
-        DESCRIPTION.
-    chunks : TYPE, optional
-        chunks={'time':1} increases performance significantly upon reading, but causes memory overloads when performing sum/mean/etc actions over time dimension (in that case 100/200 is better). The default is {'time':1}.
-
-    Raises
-    ------
-    Exception
-        DESCRIPTION.
-
-    Returns
-    -------
-    ds_merged_xu : TYPE
-        DESCRIPTION.
-    
-    file_nc = 'p:\\1204257-dcsmzuno\\2006-2012\\3D-DCSM-FM\\A18b_ntsu1\\DFM_OUTPUT_DCSM-FM_0_5nm\\DCSM-FM_0_5nm_0*_map.nc' #3D DCSM
-    file_nc = 'p:\\archivedprojects\\11206813-006-kpp2021_rmm-2d\\C_Work\\31_RMM_FMmodel\\computations\\model_setup\\run_207\\results\\RMM_dflowfm_0*_map.nc' #RMM 2D
-    file_nc = 'p:\\1230882-emodnet_hrsm\\GTSMv5.0\\runs\\reference_GTSMv4.1_wiCA_2.20.06_mapformat4\\output\\gtsm_model_0*_map.nc' #GTSM 2D
-    file_nc = 'p:\\11208053-005-kpp2022-rmm3d\\C_Work\\01_saltiMarlein\\RMM_2019_computations_02\\computations\\theo_03\\DFM_OUTPUT_RMM_dflowfm_2019\\RMM_dflowfm_2019_0*_map.nc' #RMM 3D
-    file_nc = 'p:\\archivedprojects\\11203379-005-mwra-updated-bem\\03_model\\02_final\\A72_ntsu0_kzlb2\\DFM_OUTPUT_MB_02\\MB_02_0*_map.nc'
-    Timings (xu.open_dataset/xu.merge_partitions):
-        - DCSM 3D 20 partitions  367 timesteps: 231.5/ 4.5 sec (decode_times=False: 229.0 sec)
-        - RMM  2D  8 partitions  421 timesteps:  55.4/ 4.4 sec (decode_times=False:  56.6 sec)
-        - GTSM 2D  8 partitions  746 timesteps:  71.8/30.0 sec (decode_times=False: 204.8 sec)
-        - RMM  3D 40 partitions  146 timesteps: 168.8/ 6.3 sec (decode_times=False: 158.4 sec)
-        - MWRA 3D 20 partitions 2551 timesteps:  74.4/ 3.4 sec (decode_times=False:  79.0 sec)
-    
-    """
-    #TODO: FM-mapfiles contain wgs84/projected_coordinate_system variables. xugrid has .crs property, projected_coordinate_system/wgs84 should be updated to be crs so it will be automatically handled? >> make dflowfm issue (and https://github.com/Deltares/xugrid/issues/42)
-    #TODO: add support for multiple grids via keyword? GTSM+riv grid also only contains only one grid, so no testcase available
-    #TODO: speed up open_dataset https://github.com/Deltares/dfm_tools/issues/225 (also remove_ghost and remove_periodic)
-    
-    dtstart_all = dt.datetime.now()
-    file_nc_list = file_to_list(file_nc)
-    
-    print(f'>> xu.open_dataset() with {len(file_nc_list)} partition(s): ',end='')
-    dtstart = dt.datetime.now()
-    partitions = []
-    for iF, file_nc_one in enumerate(file_nc_list):
-        print(iF+1,end=' ')
-        ds = xr.open_dataset(file_nc_one, chunks=chunks, **kwargs)
-        if 'nFlowElem' in ds.dims and 'nNetElem' in ds.dims: #for mapformat1 mapfiles: merge different face dimensions (rename nFlowElem to nNetElem) to make sure the dataset topology is correct
-            print('[mapformat1] ',end='')
-            ds = ds.rename({'nFlowElem':'nNetElem'})
-        uds = xu.core.wrap.UgridDataset(ds)
-        if remove_ghost: #TODO: this makes it way slower (at least for GTSM), but is necessary since values on overlapping cells are not always identical (eg in case of Venice ucmag)
-            uds = remove_ghostcells(uds)
-        if remove_periodic: #TODO: makes it also slower, check if bool/idx makes difference in performance?
-            uds = remove_periodic_cells(uds)
-        partitions.append(uds)
-    print(': ',end='')
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    if len(partitions) == 1: #do not merge in case of 1 partition
-        return partitions[0]
-    
-    print(f'>> xu.merge_partitions() with {len(file_nc_list)} partition(s): ',end='')
-    dtstart = dt.datetime.now()
-    ds_merged_xu = xu.merge_partitions(partitions)
-    print(f'{(dt.datetime.now()-dtstart).total_seconds():.2f} sec')
-    
-    #print variables that are dropped in merging procedure. Often only ['mesh2d_face_x_bnd', 'mesh2d_face_y_bnd'], which can be derived by combining node_coordinates (mesh2d_node_x mesh2d_node_y) and face_node_connectivity (mesh2d_face_nodes). >> can be removed from FM-mapfiles (email of 16-1-2023)
-    varlist_onepart = list(partitions[0].variables.keys())
-    varlist_merged = list(ds_merged_xu.variables.keys())
-    varlist_dropped_bool = ~pd.Series(varlist_onepart).isin(varlist_merged)
-    varlist_dropped = pd.Series(varlist_onepart).loc[varlist_dropped_bool]
-    if varlist_dropped_bool.any():
-        print(f'>> some variables dropped with merging of partitions: {varlist_dropped.tolist()}')
-    
-    print(f'>> dfmt.open_partitioned_dataset() total: {(dt.datetime.now()-dtstart_all).total_seconds():.2f} sec')
-    return ds_merged_xu
-
```

### Comparing `dfm_tools-0.11.0/dfm_tools.egg-info/SOURCES.txt` & `dfm_tools-0.12.0/dfm_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 README.md
 setup.cfg
 setup.py
 dfm_tools/__init__.py
 dfm_tools/bathymetry.py
+dfm_tools/coastlines.py
 dfm_tools/deprecated.py
 dfm_tools/download.py
 dfm_tools/energy_dissipation.py
 dfm_tools/errors.py
 dfm_tools/get_nc.py
 dfm_tools/get_nc_helpers.py
 dfm_tools/hydrolib_helpers.py
 dfm_tools/interpolate_grid2bnd.py
 dfm_tools/linebuilder.py
 dfm_tools/meshkernel_helpers.py
 dfm_tools/modelbuilder.py
 dfm_tools/modplot.py
-dfm_tools/regulargrid.py
 dfm_tools/xarray_helpers.py
+dfm_tools/xugrid_helpers.py
 dfm_tools.egg-info/PKG-INFO
 dfm_tools.egg-info/SOURCES.txt
 dfm_tools.egg-info/dependency_links.txt
 dfm_tools.egg-info/not-zip-safe
 dfm_tools.egg-info/requires.txt
 dfm_tools.egg-info/top_level.txt
 tests/__init__.py
-tests/test_dfm_tools.py
+tests/test_dfm_tools.py
+tests/test_download.py
+tests/test_external_packages.py
+tests/test_meshkernel_helpers.py
+tests/utils.py
```

### Comparing `dfm_tools-0.11.0/setup.cfg` & `dfm_tools-0.12.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 [metadata]
 name = dfm_tools
-version = 0.11.0
+version = 0.12.0
 author = Jelmer Veenstra
 author_email = Jelmer.Veenstra@Deltares.nl
 description = dfm_tools are pre- and post-processing tools for Delft3D FM
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Deltares/dfm_tools
 keywords = dfm_tools, D-FlowFM, D-HYDRO, post-processing, pre-processing, mapfiles, hisfiles
 license = GNU General Public License v3 (GPLv3)
 license_files = ('LICENSE')
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering :: Information Analysis
+	License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+	Programming Language :: Python
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 python_requires = >=3.8
 install_requires = 
 	scipy<1.10.0
 	numpy
 	matplotlib
-	pandas
+	pandas<2.0.0
 	shapely>=1.7.0
-	pyepsg
 	geopandas
 	contextily
-	xarray<2023.3.0
+	xarray
 	dask
 	netcdf4>=1.5.3
 	bottleneck
-	xugrid>=0.2.1
+	xugrid>=0.6.1
 	cdsapi
-	pydap
+	pydap>=3.3.0
 	hydrolib-core>=0.5.1
-	meshkernel>=2.0.2
+	meshkernel>=2.1.0
 packages = find:
 include_package_data = True
 zip_safe = False
 
 [options.extras_require]
 test = 
 	bump2version>=0.5.11
-	pdoc3
 	flake8
 	pytest
 	pytest-cov
 	twine
 	jupyter
 	notebook
+	mkdocs
+	mkdocs-material
+	mkdocs-jupyter
+	mkdocstrings-python
+	mkdocs-exclude
 complete = 
 	%(test)s
 
 [tool:pytest]
 python_files = test_*.py
 console_output_style = count
 norecursedirs = tests/*
```

### Comparing `dfm_tools-0.11.0/tests/test_dfm_tools.py` & `dfm_tools-0.12.0/tests/test_dfm_tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,59 +5,27 @@
 import pytest
 import os
 import glob
 import dfm_tools as dfmt
 import numpy as np
 import hydrolib.core.dflowfm as hcdfm
 import pandas as pd
-import requests
-import pathlib
-import xarray as xr
-
-
-def download_testdata():
-    #TODO: work with pooch instead, like: https://github.com/Deltares/xugrid/blob/main/xugrid/data/sample_data.py
-    #TODO: make opendap folder structure the same as local testdata folder
-    
-    fname_list = []
-    fname_list += ['DFM_curvedbend_3D/cb_3d_map.nc']
-    fname_list += ['DFM_curvedbend_3D/cb_3d_his.nc']
-    fname_list += [f'DFM_grevelingen_3D/Grevelingen-FM_{i:04d}_map.nc' for i in range(8)]
-    fname_list += ['DFM_grevelingen_3D/Grevelingen-FM_0000_his.nc']
-    fname_list += ['DFM_grevelingen_3D/Grevelingen_FM_grid_20190603_net.nc']
-    # fname_list += ['westernscheldt_sph_map.nc']
-
-    for fname in fname_list:
-        file_nc = os.path.join(dir_testinput,fname)
-        file_dirname = os.path.dirname(file_nc)
-        if os.path.exists(file_nc): #skip if file exists
-            continue
-        pathlib.Path(file_dirname).mkdir(parents=True, exist_ok=True) #make subdir if needed
-        
-        file_url = f'https://opendap.deltares.nl/thredds/fileServer/opendap/deltares/Delft3D/netcdf_example_files/{fname}'
-        print(f'downloading {file_url} to {file_nc}')
-        r = requests.get(file_url, allow_redirects=True)
-        r.raise_for_status() #raise HTTPError if url not exists
-        with open(file_nc, 'wb') as f:
-            f.write(r.content)
-
-dir_testinput = os.path.join(r'c:\DATA','dfm_tools_testdata') #on WCF
-if not os.path.exists(dir_testinput): #for instance when running on github or 
-    dir_testinput = './dfm_tools_testdata'
-    download_testdata()
+
+from tests.utils import maybe_download_testdata
+
+dir_testinput = maybe_download_testdata()
 
 
 # ACCEPTANCE TESTS VIA EXAMPLE SCRIPTS, these are the ones who are only meant to generate output files
 
 dir_tests = os.path.dirname(__file__) #F9 doesnt work, only F5 (F5 also only method to reload external definition scripts)
 list_configfiles = glob.glob(os.path.join(dir_tests,'examples','*.py')) + glob.glob(os.path.join(dir_tests,'examples_workinprogress','*.py'))
 list_configfiles = [x for x in list_configfiles if 'workinprogress_xarray_performance' not in x] #ignore this slow script
 dir_output_general = os.path.join(dir_tests,'examples_output')
-if not os.path.exists(dir_output_general):
-    os.mkdir(dir_output_general)
+os.makedirs(dir_output_general, exist_ok=True)
 
 @pytest.mark.requireslocaldata
 @pytest.mark.acceptance
 @pytest.mark.parametrize("file_config", [pytest.param(file_config, id=os.path.basename(file_config).replace('.py','')) for file_config in list_configfiles])
 def test_run_examples(file_config):
     # 1. Set up test data
     dir_output = os.path.join(dir_output_general,os.path.basename(file_config).replace('.py',''))
@@ -68,24 +36,14 @@
     
     if test:
         raise OSError('execution did not finish properly')
 
 
 ##### UNITTESTS AND SYSTEMTESTS
 
-@pytest.mark.unittest
-def test_import_shapely():
-    """
-    tests whether shapely can be imported successfully, this is a problem in some environments
-    in that case 'import shapely' works, but import 'shapely.geometry' fails
-    """
-    import shapely
-    import shapely.geometry
-    
-
 @pytest.mark.parametrize("file_nc, expected_size", [pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen-FM_0000_map.nc'), (5599,3,2), id='from 1 map partion Grevelingen'),
                                                     pytest.param(os.path.join(dir_testinput,'DFM_grevelingen_3D','Grevelingen_FM_grid_20190603_net.nc'), (44804,4,2), id='fromnet Grevelingen')])
 @pytest.mark.systemtest
 def test_facenodecoordinates_shape(file_nc, expected_size):
     
     uds = dfmt.open_partitioned_dataset(file_nc)
     facenodecoordinates = uds.grid.face_node_coordinates
@@ -331,57 +289,7 @@
     refdate = '2016-01-01'
     tim_pd = dfmt.TimModel_to_DataFrame(data_tim, parse_column_labels=True, refdate=refdate)
     
     assert tim_pd.index[0] == pd.Timestamp('2016-01-01 00:00:00')
     assert len(tim_pd) == 91
     assert tim_pd.columns[-1] == 'Phaeocystis_P (g/m3)'
 
-
-@pytest.mark.systemtest
-def test_opendataset_ugridplot(): #this one fails with xarray>=2023.3.0: https://github.com/Deltares/xugrid/issues/78
-    file_nc = os.path.join(dir_testinput,'DFM_curvedbend_3D/cb_3d_map.nc')
-    
-    uds = dfmt.open_partitioned_dataset(file_nc,chunks={'time':1})
-
-    uds['mesh2d_flowelem_bl'].ugrid.plot(edgecolors='face', cmap='jet')
-    
-    
-@pytest.mark.unittest
-def test_xr_interp_to_newdim(): #this one fails with scipy>=1.10.0: https://github.com/pydata/xarray/issues/7701
-    ds = xr.Dataset()
-    so_np = np.array([[[35.819576, 35.82568 , 35.82873 ],
-                       [35.819576, 35.824154, 35.831783],
-                       [35.822628, 35.824154, 35.82873 ]],
-                      
-                      [[35.802788, 35.80584 , 35.815   ],
-                       [35.815   , 35.810417, 35.821102],
-                       [35.824154, 35.813473, 35.81805 ]],
-                      
-                      [[35.786003, 35.789055,       np.nan],
-                       [35.807365, 35.796684,       np.nan],
-                       [35.824154, 35.80584 ,       np.nan]],
-                      
-                      [[35.776848,       np.nan,       np.nan],
-                       [35.792107,       np.nan,       np.nan],
-                       [35.822628,       np.nan,       np.nan]],
-                      
-                      [[35.781425,       np.nan,       np.nan],
-                       [35.792107,       np.nan,       np.nan],
-                       [35.789055,       np.nan,       np.nan]]])
-    ds['so'] = xr.DataArray(so_np,dims=('depth','latitude','longitude'))
-    ds['longitude'] = xr.DataArray([-9.6, -9.5, -9.4], dims=('longitude'))
-    ds['latitude'] = xr.DataArray([42.9, 43.0, 43.1], dims=('latitude'))
-    
-    x_xr = xr.DataArray([-9.5],dims=('plipoints'))
-    y_xr = xr.DataArray([43],dims=('plipoints'))
-    
-    
-    interp_with_floats = ds.interp(longitude=x_xr[0], latitude=y_xr[0], method='linear').so #selecting one value from the da drops the new plipoints dimension
-    interp_with_da_existing = ds.interp(longitude=x_xr.values, latitude=y_xr.values, method='linear').so.isel(longitude=0,latitude=0) #using the DataArray values keeps lat/lon dimenions, gives the same interp result
-    interp_with_da_newdim = ds.interp(longitude=x_xr, latitude=y_xr, method='linear').so.isel(plipoints=0) #using the DataArray introduces a plipoints dimension, which gives different interp result
-    print(interp_with_floats.to_numpy())
-    print(interp_with_da_existing.to_numpy())
-    print(interp_with_da_newdim.to_numpy())
-    print(xr.__version__)
-    
-    assert (interp_with_floats.isnull()==interp_with_da_existing.isnull()).all() #success
-    assert (interp_with_floats.isnull()==interp_with_da_newdim.isnull()).all() #fails with scipy>=1.10.0
```

